# Comparing `tmp/iamlistening-0.1.9.tar.gz` & `tmp/iamlistening-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.9.tar", max compression
+gzip compressed data, was "iamlistening-0.2.0.tar", max compression
```

## Comparing `iamlistening-0.1.9.tar` & `iamlistening-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-05 19:08:23.478476 iamlistening-0.1.9/LICENSE
--rw-r--r--   0        0        0     1719 2023-06-05 19:08:23.478476 iamlistening-0.1.9/README.md
--rw-r--r--   0        0        0       99 2023-06-05 19:08:24.166486 iamlistening-0.1.9/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4053 2023-06-05 19:08:23.478476 iamlistening-0.1.9/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-05 19:08:24.166486 iamlistening-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 iamlistening-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 19:45:35.000738 iamlistening-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1629 2023-06-25 19:45:35.004738 iamlistening-0.2.0/README.md
+-rw-r--r--   0        0        0       99 2023-06-25 19:45:35.936797 iamlistening-0.2.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-06-25 19:45:35.004738 iamlistening-0.2.0/iamlistening/config.py
+-rw-r--r--   0        0        0      868 2023-06-25 19:45:35.004738 iamlistening-0.2.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3839 2023-06-25 19:45:35.004738 iamlistening-0.2.0/iamlistening/main.py
+-rw-r--r--   0        0        0     2163 2023-06-25 19:45:35.936797 iamlistening-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 iamlistening-0.2.0/PKG-INFO
```

### Comparing `iamlistening-0.1.9/LICENSE` & `iamlistening-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.9/README.md` & `iamlistening-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

### Comparing `iamlistening-0.1.9/iamlistening/config.py` & `iamlistening-0.2.0/iamlistening/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 settings = Dynaconf(
     envvar_prefix="TT",
     # Set the root path of the project
     root_path=os.path.dirname(ROOT),
     # Load the default settings file
     settings_files=[
         os.path.join(ROOT, "default_settings.toml"),
+        'talky_settings.toml',
         'settings.toml',
         '.secrets.toml'
     ],
     # Load the.env file
     load_dotenv=True,
     # Set the environments to True
     environments=True,
```

### Comparing `iamlistening-0.1.9/iamlistening/main.py` & `iamlistening-0.2.0/iamlistening/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,30 @@
         self.latest_message = None
         self.loop = asyncio.get_event_loop()
         self.lock = threading.Lock()
         self.stopped = False
     
     async def start(self):
         """start"""
-        if settings.discord_webhook_id:
-            # DISCORD
-            intents = discord.Intents.default()
-            intents.message_content = True
-            bot = discord.Bot(intents=intents)
 
-            @bot.event
-            async def on_ready():
-                await self.post_init()
+        if settings.telethon_api_id:
+            # TELEGRAM
+            bot = await TelegramClient(
+                        None,
+                        settings.telethon_api_id,
+                        settings.telethon_api_hash
+                        ).start(bot_token=settings.bot_token)
+            await self.post_init()
+
+            @bot.on(events.NewMessage())
+            async def telethon(event):
+                await self.handle_message(event.message.message)
+
+            await bot.run_until_disconnected()
 
-            @bot.event
-            async def on_message(message: discord.Message):
-                await self.handle_message(message.content)
-            await bot.start(settings.bot_token)
         elif settings.matrix_hostname:
             # MATRIX
             config = botlib.Config()
             config.emoji_verify = True
             config.ignore_unverified_devices = True
             config.store_path = './config/matrix/'
             creds = botlib.Creds(
@@ -67,55 +69,53 @@
             for action in bot.listener._startup_registry:
                 for room_id in bot.api.async_client.rooms:
                     await action(room_id)
             await bot.api.async_client.sync_forever(
                                                     timeout=3000,
                                                     full_state=True
                                                 )
-        elif settings.telethon_api_id:
-            # TELEGRAM
-            bot = await TelegramClient(
-                        None,
-                        settings.telethon_api_id,
-                        settings.telethon_api_hash
-                        ).start(bot_token=settings.bot_token)
-            await self.post_init()
+        elif settings.bot_token:
+            # DISCORD
+            intents = discord.Intents.default()
+            intents.message_content = True
+            bot = discord.Bot(intents=intents)
 
-            @bot.on(events.NewMessage())
-            async def telethon(event):
-                await self.handle_message(event.message.message)
+            @bot.event
+            async def on_ready():
+                await self.post_init()
+
+            @bot.event
+            async def on_message(message: discord.Message):
+                await self.handle_message(message.content)
+            await bot.start(settings.bot_token)
 
-            await bot.run_until_disconnected()
         else:
             self.logger.warning("Check settings")
             await asyncio.sleep(7200)
 
     async def get_latest_message(self):
         """Return the latest message."""
         while True:
             with self.lock:
                 if self.latest_message is not None:
                     msg = self.latest_message
                     self.latest_message = None
-                    # self.logger.debug(f"Latest message: {msg}")
                     return msg
 
             await asyncio.sleep(0.1)
 
     async def handle_message(self, message_content):
         """Handle a new message."""
-        # self.logger.debug(f"Message received: {message_content}")
         self.latest_message = message_content
-        # self.logger.debug(f"handle_message self.latest_message: {self.latest_message}")
 
 
     async def run_forever(self):
         """Run the listener forever."""
         while not self.stopped:
             await self.start()
 
     async def post_init(self):
-        return
+        return "bot is online"
 
     def stop(self):
         """Stop the listener."""
         self.stopped = True
```

### Comparing `iamlistening-0.1.9/pyproject.toml` & `iamlistening-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.9"
+version = "0.2.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
@@ -14,50 +14,54 @@
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/iamlistening/discussions"
 "Issues" =  "https://github.com/mraniki/iamlistening/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-asyncio = "*"
-dynaconf = "*"
-apprise= "*"
-telethon= "*"
-py-cord= "*"
-simplematrixbotlib= "*"
+dynaconf = "^3.1.12"
+telethon= "^1.28.5"
+py-cord= "^2.4.1"
+simplematrixbotlib= "^2.9.0"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "*"
-pytest = "*"
-pytest-cov = "*"
-pytest-asyncio = "*"
-pytest-mock = "*"
-coverage = "*"
+python-semantic-release = "^7.34.3"
+pytest = "^7.0"
+pytest-cov = "^4.1"
+pytest-asyncio = "^0.21.0"
+pytest-mock = "^3.11.1"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
 [tool.coverage.run]
 omit = [
     "tests/*",
-    "examples/*"
+    "examples/*",
+    "docs/*",
+    "*/config.py"
 ]
 
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.1"
+sphinx-autoapi = "^2.1.0"
+furo = "^2023.5.20"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","iamlistening/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-major_emoji = "💥"
-minor_emoji = "🥚,🚀,💄,✨"
-patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
+major_emoji = "BREAKING,💥,:boom:"
+minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
+patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
```

### Comparing `iamlistening-0.1.9/PKG-INFO` & `iamlistening-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.9
+Version: 0.2.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: apprise
-Requires-Dist: asyncio
-Requires-Dist: dynaconf
-Requires-Dist: py-cord
-Requires-Dist: simplematrixbotlib
-Requires-Dist: telethon
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: py-cord (>=2.4.1,<3.0.0)
+Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0)
+Requires-Dist: telethon (>=1.28.5,<2.0.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
 Description-Content-Type: text/markdown
 
 # I Am Listening
 
@@ -55,14 +53,14 @@
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

