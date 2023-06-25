# Comparing `tmp/commandeft-0.2.1.tar.gz` & `tmp/commandeft-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.2.1.tar", last modified: Mon Jun 12 20:03:57 2023, max compression
+gzip compressed data, was "commandeft-0.3.0.tar", last modified: Sun Jun 25 17:16:51 2023, max compression
```

## Comparing `commandeft-0.2.1.tar` & `commandeft-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.2.1/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-12 02:51:12.093999 commandeft-0.2.1/README.md
--rw-r--r--   0        0        0       65 2023-06-12 02:20:42.863520 commandeft-0.2.1/commandeft/.pdm-python
--rw-r--r--   0        0        0       40 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/.gitignore
--rw-r--r--   0        0        0     2201 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate
--rw-r--r--   0        0        0     1493 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.csh
--rw-r--r--   0        0        0     3078 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3397 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.nu
--rw-r--r--   0        0        0     1782 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     1211 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate_this.py
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python -> /usr/bin/python3.8
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python3.8 -> python
--rw-r--r--   0        0        0       18 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4311 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      233 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/pyvenv.cfg
--rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.2.1/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3153 2023-06-12 19:43:48.156337 commandeft-0.2.1/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/core/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-12 19:57:38.569171 commandeft-0.2.1/commandeft/core/cli.py
--rw-r--r--   0        0        0      823 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/core/decision.py
--rw-r--r--   0        0        0     1715 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/core/generation.py
--rw-r--r--   0        0        0     1132 2023-06-12 19:57:19.149060 commandeft-0.2.1/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/util/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/util/config_util.py
--rw-r--r--   0        0        0      624 2023-06-12 18:13:27.860557 commandeft-0.2.1/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2729 2023-06-12 02:42:06.423316 commandeft-0.2.1/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1644 2023-06-12 20:03:57.355324 commandeft-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 commandeft-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3541 2023-06-25 17:10:36.499026 commandeft-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2023-06-12 02:20:42.863520 commandeft-0.3.0/commandeft/.pdm-python
+-rw-r--r--   0        0        0       40 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/.gitignore
+-rw-r--r--   0        0        0     2201 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate
+-rw-r--r--   0        0        0     1493 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3078 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3397 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1782 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1211 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate_this.py
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python -> /usr/bin/python3.8
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python3.8 -> python
+-rw-r--r--   0        0        0       18 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4311 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      233 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.3.0/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3234 2023-06-25 17:15:44.889063 commandeft-0.3.0/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     3696 2023-06-25 17:15:23.200920 commandeft-0.3.0/commandeft/core/cli.py
+-rw-r--r--   0        0        0     1391 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/core/decision.py
+-rw-r--r--   0        0        0     4904 2023-06-25 17:15:48.693088 commandeft-0.3.0/commandeft/core/generation.py
+-rw-r--r--   0        0        0     2131 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/core/history_cache.py
+-rw-r--r--   0        0        0      913 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     3637 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      370 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2349 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1995 2023-06-25 17:16:51.673502 commandeft-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.3.0/PKG-INFO
```

### Comparing `commandeft-0.2.1/LICENSE` & `commandeft-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/README.md` & `commandeft-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```sh
 commandeft --configure (or -c)
 ```
 
 - You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lower temperatures perform better.
   More information about temeratures [HERE](https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api-a-few-tips-and-tricks-on-controlling-the-creativity-deterministic-output-of-prompt-responses/172683)
 - You can choose the `max_token` value.  
-  ⚠️ Keep in Mind that the guided prompt consumes ~55 tokens. The value you specify won't include these tokens.
+  ⚠️ Keep in Mind that the guided prompt(assistant role prompt + user role prompt without user's prompt) consumes ~70 tokens. The value you specify won't include these tokens.
 - You will also be asked about the action that will be performed every time when you accept a generated command when running in interactive mode.  
   The available actions are:
 
 1. Running the generated command
 2. Copying it to the clipboard
 
 Don't worry though, after this you will be asked to apply your selected action on every generation.
```

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate` & `commandeft-0.3.0/commandeft/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate.csh` & `commandeft-0.3.0/commandeft/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate.fish` & `commandeft-0.3.0/commandeft/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate.nu` & `commandeft-0.3.0/commandeft/.venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate.ps1` & `commandeft-0.3.0/commandeft/.venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/bin/activate_this.py` & `commandeft-0.3.0/commandeft/.venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py` & `commandeft-0.3.0/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.2.1/commandeft/constants/consts.py` & `commandeft-0.3.0/commandeft/constants/consts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import os
 
 
-CONFIG_FILE_PATH = os.path.expanduser("~/.commandeft/config")
+CONFIG_FILE_PATH = os.path.join(os.path.expanduser("~"), ".commandeft", "config")
+MAX_TOKENS = 4096
 
 init_messages = [
-    "What mischief are we up to now?\n Describe the command you're concocting:",
-    "Oh no, caught in another coding conundrum?\n Share the details:",
-    "Here to save the day!\n Enlighten me with the command you're grappling with:",
-    "When your coding journey hits a snag,\n Describe the task that makes you sag:",
-    "No shame in seeking guidance.\n What command do you need a helping hand with?:",
-    "Trouble seems to find you often.\ nReveal the command conundrum you're facing now:",
-    "We all need a helping hand sometimes.\n Describe the command that has you reaching out for support:",
-    "In a pickle again, I see?\n Describe the trouble you're in and let's work it out together:",
-    "Brave adventurer, share the quest for the command you seek and I shall guide you through:",
-    "When bugs run rampant, causing you despair,\n Detail the task that makes you pull out your hair:",
-    "Here to rescue you from the labyrinth of documentation!\n Unravel your challenge to me:",
-    "Seeking shell enlightenment, are we?\n Unveil the path to wisdom you're pursuing:",
-    "In the coding realm, when all is grim,\n Describe the prompt that makes you scream:",
-    "Ready to conquer the coding riddles?\n Describe the challenge you're facing, and I'll be your guide:",
-    "Stuck in the maze of complex requirements?\n Describe the twists and turns that have you feeling lost:",
-    "In the vast realm of coding, even superheroes need a sidekick!\n Tell me about the command you need assistance with:",
-    "Don't worry, I won't judge.\n We've all been there! Ask about the command that has you scratching your head:",
-    "In the vast sea of commands,\n it's okay to feel overwhelmed. Let me know which one you're struggling with, and we'll figure it out together:",
-    "Well, well, look who's in need of guidance.\n Pray tell, what has you seeking my wisdom?:",
-    "In a code abyss, dark and deep,\n Share the task that makes you weep:",
-    "In the digital realm, where all devs cry,\n A prompt for support, can't be denied!",
+    "What mischief are we up to now?\n Describe the command you're concocting:\n",
+    "Oh no, caught in another coding conundrum?\n Share the details:\n",
+    "Here to save the day!\n Enlighten me with the command you're grappling with:\n",
+    "When your coding journey hits a snag,\n Describe the task that makes you sag:\n",
+    "No shame in seeking guidance.\n What command do you need a helping hand with?:\n",
+    "Trouble seems to find you often.\n nReveal the command conundrum you're facing now:\n",
+    "We all need a helping hand sometimes.\n Describe the command that has you reaching out for support:\n",
+    "In a pickle again, I see?\n Describe the trouble you're in and let's work it out together:\n",
+    "Brave adventurer, share the quest for the command you seek and I shall guide you through:\n",
+    "When bugs run rampant, causing you despair,\n Detail the task that makes you pull out your hair:\n",
+    "Here to rescue you from the labyrinth of documentation!\n Unravel your challenge to me:\n",
+    "Seeking shell enlightenment, are we?\n Unveil the path to wisdom you're pursuing:\n",
+    "In the coding realm, when all is grim,\n Describe the prompt that makes you scream:\n",
+    "Ready to conquer the coding riddles?\n Describe the challenge you're facing, and I'll be your guide:\n",
+    "Stuck in the maze of complex requirements?\n Describe the twists and turns that have you feeling lost:\n",
+    "In the vast realm of coding, even superheroes need a sidekick!\n Tell me about the command you need assistance with:\n",
+    "Don't worry, I won't judge.\n We've all been there! Ask about the command that has you scratching your head:\n",
+    "In the vast sea of commands,\n it's okay to feel overwhelmed. Let me know which one you're struggling with, and we'll figure it out together:\n",
+    "Well, well, look who's in need of guidance.\n Pray tell, what has you seeking my wisdom?:\n",
+    "In a code abyss, dark and deep,\n Share the task that makes you weep:\n",
+    "In the digital realm, where all devs cry,\n A prompt for support, can't be denied!\n",
 ]
 
 fail_messages = [
     "Oh well, maybe next time!",
     "Better luck next time!",
     "Didn't quite get it this time huh?",
     "I guess you'll have to try again!",
```

### Comparing `commandeft-0.2.1/commandeft/main.py` & `commandeft-0.3.0/commandeft/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-import sys
 import click
 
 from commandeft.core.cli import CustomCommand, configuration_mode, print_version, prompt_in_line, interactive_mode
 
 
-def custom_exception_handler(exc_value):
-    # Handle the exception
-    click.echo(click.style(f"An error occurred:{str(exc_value),}", fg="red"))
-    sys.exit(1)
-
-
-sys.excepthook = custom_exception_handler
-
-
 @click.command(cls=CustomCommand)
 @click.help_option("-h", "--help")
 @click.option("-v", "--version", help="Show version and exit", is_flag=True)
 @click.option("-c", "--configure", help="Configure commandeft", is_flag=True)
 @click.option("-i", "--interactive", help="Run in interactive mode", is_flag=True)
 @click.option("-p", "--prompt", help="Specify your prompt inline")
 def commandeft(version, configure, interactive, prompt):
```

### Comparing `commandeft-0.2.1/PKG-INFO` & `commandeft-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.2.1
+Version: 0.3.0
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
+Keywords: commandeft cli tool shell commands prompt-based command generation natural language prompts shell commands shell scripts shell command generation intelligent code generation language-to-code conversion developer-friendly simplified scripting code efficiency streamline workflow intelligent suggestions efficient command composition gpt-3.5-turbo gpt-4 shell command suggestion interactive mode guided prompt command execution
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: Pygments==2.15.1
 Requires-Dist: aiohttp==3.8.4
@@ -14,41 +15,31 @@
 Requires-Dist: attrs==23.1.0
 Requires-Dist: cachetools==5.3.1
 Requires-Dist: certifi==2023.5.7
 Requires-Dist: cffi==1.15.1
 Requires-Dist: charset-normalizer<4.0,>=2.0
 Requires-Dist: click==8.1.3
 Requires-Dist: cryptography==41.0.1
-Requires-Dist: diskcache==5.6.1
 Requires-Dist: frozenlist==1.3.3
-Requires-Dist: gptcache==0.1.29.1
-Requires-Dist: guidance==0.0.61
 Requires-Dist: idna==3.4
-Requires-Dist: msal==1.22.0
 Requires-Dist: multidict<7.0,>=4.5
-Requires-Dist: nest-asyncio==1.5.6
-Requires-Dist: numpy==1.24.3
-Requires-Dist: openai==0.27.7
-Requires-Dist: parsimonious==0.10.0
+Requires-Dist: openai>=0.27.8
 Requires-Dist: pip-licenses==4.3.2
-Requires-Dist: platformdirs<4,>=3.2
 Requires-Dist: prettytable==3.7.0
 Requires-Dist: prompt-toolkit<4.0.0,>=3.0.1
 Requires-Dist: pycparser==2.21
-Requires-Dist: pygtrie==2.5.0
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: regex==2023.6.3
-Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
-Requires-Dist: tiktoken==0.4.0
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: urllib3==2.0.2
 Requires-Dist: wcwidth==0.2.6
 Requires-Dist: yarl<2.0,>=1.0
 Requires-Dist: InquirerPy>=0.3.4
+Requires-Dist: tiktoken>=0.4.0
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-pep8; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # CommanDeft
@@ -110,15 +101,15 @@
 ```sh
 commandeft --configure (or -c)
 ```
 
 - You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lower temperatures perform better.
   More information about temeratures [HERE](https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api-a-few-tips-and-tricks-on-controlling-the-creativity-deterministic-output-of-prompt-responses/172683)
 - You can choose the `max_token` value.  
-  ⚠️ Keep in Mind that the guided prompt consumes ~55 tokens. The value you specify won't include these tokens.
+  ⚠️ Keep in Mind that the guided prompt(assistant role prompt + user role prompt without user's prompt) consumes ~70 tokens. The value you specify won't include these tokens.
 - You will also be asked about the action that will be performed every time when you accept a generated command when running in interactive mode.  
   The available actions are:
 
 1. Running the generated command
 2. Copying it to the clipboard
 
 Don't worry though, after this you will be asked to apply your selected action on every generation.
```

