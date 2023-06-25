# Comparing `tmp/aissist-0.0.4.tar.gz` & `tmp/aissist-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.4.tar` & `aissist-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.4/LICENSE
--rw-r--r--   0        0        0      198 2023-06-25 02:16:37.284114 aissist-0.0.4/Pipfile
--rw-r--r--   0        0        0    41428 2023-06-25 02:35:33.773116 aissist-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0     1181 2023-06-25 03:04:17.106277 aissist-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.4/aissist/__init__.py
--rw-r--r--   0        0        0     3271 2023-06-25 03:18:46.124935 aissist-0.0.4/aissist/aissistant.py
--rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.4/aissist/spinner.py
--rw-r--r--   0        0        0       22 2023-06-25 03:25:49.962157 aissist-0.0.4/aissist/version.py
--rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.4/images/screenshot.png
--rw-r--r--   0        0        0      885 2023-06-25 03:25:48.354141 aissist-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 aissist-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.5/LICENSE
+-rw-r--r--   0        0        0      212 2023-06-25 03:44:03.985612 aissist-0.0.5/Pipfile
+-rw-r--r--   0        0        0    41743 2023-06-25 03:44:08.209610 aissist-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0     1181 2023-06-25 03:04:17.106277 aissist-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.5/aissist/__init__.py
+-rw-r--r--   0        0        0     3391 2023-06-25 03:38:07.089502 aissist-0.0.5/aissist/aissistant.py
+-rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.5/aissist/spinner.py
+-rw-r--r--   0        0        0       22 2023-06-25 03:45:49.137565 aissist-0.0.5/aissist/version.py
+-rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.5/images/screenshot.png
+-rw-r--r--   0        0        0      899 2023-06-25 03:45:53.397563 aissist-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 aissist-0.0.5/PKG-INFO
```

### Comparing `aissist-0.0.4/LICENSE` & `aissist-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.4/Pipfile.lock` & `aissist-0.0.5/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820075757575758%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'223032408d592f83d55d7787c53d4d3f74ca6001d00ebd23d0f891137c3c05f0'}}",*

 * * "'default'": "{'tomlkit': OrderedDict([('hashes', "*

 * *              "['sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171', "*

 * *              "'sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3']), "*

 * *              "('index', 'pypi'), ('version', '==0.11.8')])}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "350829552f4c5127ff1a1f0d018bb2b11f4c69e2b0e63cfda0a0aca98e4d26e2"
+            "sha256": "223032408d592f83d55d7787c53d4d3f74ca6001d00ebd23d0f891137c3c05f0"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.8"
         },
         "sources": [
             {
@@ -450,14 +450,22 @@
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
+        "tomlkit": {
+            "hashes": [
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
+            ],
+            "index": "pypi",
+            "version": "==0.11.8"
+        },
         "tqdm": {
             "hashes": [
                 "sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5",
                 "sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.65.0"
```

### Comparing `aissist-0.0.4/README.md` & `aissist-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aissist-0.0.4/aissist/aissistant.py` & `aissist-0.0.5/aissist/aissistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import textwrap
 
 import openai
 from prompt_toolkit import PromptSession
 from pygments import highlight
 from pygments.lexers import guess_lexer
 from pygments.formatters import TerminalFormatter
 
@@ -47,15 +48,15 @@
 
     if in_backticks:
         result += '\033[0m'  # Reset text formatting
 
     return result
 
 
-def highlight_codeblocks(markdown):
+def highlight_codeblocks(markdown, columns: int):
     """Highlights code blocks in a markdown string and prints them to the console
     using pygments library.
     """
 
     inside_block = False
     current_block = ""
     for line in markdown.split("\n"):
@@ -71,15 +72,15 @@
                 current_block = ""
             inside_block = not inside_block
 
         elif inside_block is True:
             current_block += line + "\n"
         else:
             line = bold_single_backticks(line)
-            print(line)
+            sys.stdout.write(line)
 
 def loop(messages):
     """Main loop for the program"""
     
     result = session.prompt(">>> ", multiline=True,
                 prompt_continuation=prompt_continuation)
 
@@ -91,19 +92,23 @@
     spinner.start()
 
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=messages,
     )
     message = response["choices"][0]["message"]
+
     spinner.stop()
 
     messages.append(message)
+
+
     print(" ")
-    highlight_codeblocks(message["content"])
+    terminal_width = os.get_terminal_size().columns
+    highlight_codeblocks(message["content"], columns=terminal_width)
     print(" ")
 
     return messages
 
 def main():
 
     print("ESCAPE followed by ENTER to send. Ctrl-C to quit")
```

### Comparing `aissist-0.0.4/aissist/spinner.py` & `aissist-0.0.5/aissist/spinner.py`

 * *Files identical despite different names*

### Comparing `aissist-0.0.4/images/screenshot.png` & `aissist-0.0.5/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `aissist-0.0.4/pyproject.toml` & `aissist-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aissist"
-version = "0.0.4"
+version = "0.0.5"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
@@ -20,14 +20,15 @@
 requires-python = ">=3.7"
 
 dependencies = [
   "openai<0.28",
   "prompt_toolkit<4",
   "pygments<3",
   "requests<3",
+  "tomlkit<1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/craigmbooth/aissist"
 "Bug Tracker" = "https://github.com/craigmbooth/aissist/issues"
 
 [build-system]
```

### Comparing `aissist-0.0.4/PKG-INFO` & `aissist-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aissist
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple GPT command line interface
 Author-email: Craig Booth <craigmbooth@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: openai<0.28
 Requires-Dist: prompt_toolkit<4
 Requires-Dist: pygments<3
 Requires-Dist: requests<3
+Requires-Dist: tomlkit<1
 Project-URL: Bug Tracker, https://github.com/craigmbooth/aissist/issues
 Project-URL: Homepage, https://github.com/craigmbooth/aissist
 
 # AI Assistant
 
 This library was written to scratch a personal itch.  I have found GPT 3.5 to be incredibly useful in my day-to-day coding activities, but also found that having to go to a web browser and interact there was tedious.  What I really wanted was a tool that would:
```

