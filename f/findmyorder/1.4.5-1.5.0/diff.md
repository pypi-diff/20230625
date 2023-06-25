# Comparing `tmp/findmyorder-1.4.5.tar.gz` & `tmp/findmyorder-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.4.5.tar", max compression
+gzip compressed data, was "findmyorder-1.5.0.tar", max compression
```

## Comparing `findmyorder-1.4.5.tar` & `findmyorder-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-21 14:12:20.552563 findmyorder-1.4.5/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-21 14:12:20.552563 findmyorder-1.4.5/README.md
--rw-r--r--   0        0        0      113 2023-06-21 14:12:39.836780 findmyorder-1.4.5/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/main.py
--rw-r--r--   0        0        0     1921 2023-06-21 14:12:39.836780 findmyorder-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 19:44:47.031006 findmyorder-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-25 19:44:47.031006 findmyorder-1.5.0/README.md
+-rw-r--r--   0        0        0      113 2023-06-25 19:44:47.859005 findmyorder-1.5.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/config.py
+-rw-r--r--   0        0        0     2265 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-25 19:44:47.031006 findmyorder-1.5.0/findmyorder/main.py
+-rw-r--r--   0        0        0     2132 2023-06-25 19:44:47.859005 findmyorder-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.5.0/PKG-INFO
```

### Comparing `findmyorder-1.4.5/LICENSE` & `findmyorder-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.5/README.md` & `findmyorder-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.5/findmyorder/config.py` & `findmyorder-1.5.0/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.5/findmyorder/default_settings.toml` & `findmyorder-1.5.0/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.5/findmyorder/main.py` & `findmyorder-1.5.0/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.5/pyproject.toml` & `findmyorder-1.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.4.5"
+version = "1.5.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -18,49 +18,50 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 pyparsing = "^3.0.9"
 emoji = "^2.5.1"
 
-[tool.poetry.group.docs.dependencies]
-Sphinx = "7.0.1"
-furo = "2023.5.20"
-
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
     "examples/*",
-    "docs/*"
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
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
 major_emoji = "BREAKING,💥,:boom:"
 minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
-patch_emoji = "fix,Update,🎨,:art:,🐛,:bug:,🚑,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️|:arrow_up:,🩹,👷,📝,🔒,:lock:,👽,:alien:,💬,🥅,✅,:white_check_mark:,🐳,🙈,⚗️,🧐,🔇,🔊"
+patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
```

### Comparing `findmyorder-1.4.5/PKG-INFO` & `findmyorder-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.4.5
+Version: 1.5.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

