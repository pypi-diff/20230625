# Comparing `tmp/aissist-0.0.3.tar.gz` & `tmp/aissist-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.3.tar` & `aissist-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.3/LICENSE
--rw-r--r--   0        0        0      198 2023-06-25 02:16:37.284114 aissist-0.0.3/Pipfile
--rw-r--r--   0        0        0    41428 2023-06-25 02:35:33.773116 aissist-0.0.3/Pipfile.lock
--rw-r--r--   0        0        0     1064 2023-06-25 02:48:46.081052 aissist-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.3/aissist/__init__.py
--rw-r--r--   0        0        0     3760 2023-06-24 04:15:37.054524 aissist-0.0.3/aissist/aissistant.py
--rw-r--r--   0        0        0       22 2023-06-25 03:00:10.618799 aissist-0.0.3/aissist/version.py
--rw-r--r--   0        0        0      885 2023-06-25 03:00:02.358977 aissist-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 aissist-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.4/LICENSE
+-rw-r--r--   0        0        0      198 2023-06-25 02:16:37.284114 aissist-0.0.4/Pipfile
+-rw-r--r--   0        0        0    41428 2023-06-25 02:35:33.773116 aissist-0.0.4/Pipfile.lock
+-rw-r--r--   0        0        0     1181 2023-06-25 03:04:17.106277 aissist-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.4/aissist/__init__.py
+-rw-r--r--   0        0        0     3271 2023-06-25 03:18:46.124935 aissist-0.0.4/aissist/aissistant.py
+-rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.4/aissist/spinner.py
+-rw-r--r--   0        0        0       22 2023-06-25 03:25:49.962157 aissist-0.0.4/aissist/version.py
+-rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.4/images/screenshot.png
+-rw-r--r--   0        0        0      885 2023-06-25 03:25:48.354141 aissist-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 aissist-0.0.4/PKG-INFO
```

### Comparing `aissist-0.0.3/LICENSE` & `aissist-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.3/Pipfile.lock` & `aissist-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aissist-0.0.3/README.md` & `aissist-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 1. Be accessible from a simple command line prompt (`ai`)
 1. Open up a shell to talk to ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
 1. Have chat history accessible with the up arrow
 1. Have syntax highlighting on ChatGPT responses
 1. Have multi-line editing capabilities on multi-line prompts
 
-THis library is just that.
+This library is precisely that, and no more.
 
 ## Installation
 
 Via pypi
 
 ```bash
 pip install aissistant
@@ -20,8 +20,13 @@
 
 There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key.
 
 ## Usage
 
 Invoke the program with `ai`.  There are few controls. Simply enter a prompt, and hit Escape THEN Enter to submit the prompt.
 
-Inside of each session there is a history, and you can use the up arrow to revisit and edit previous prompts.
+Inside of each session there is a history, and you can use the up arrow to revisit and edit previous prompts.
+
+Here is a simple example
+
+![An example of using aissist to write Python](images/screenshot.png)
+
```

### Comparing `aissist-0.0.3/aissist/aissistant.py` & `aissist-0.0.4/aissist/aissistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,29 @@
 import os
 import sys
-from prompt_toolkit import PromptSession
-import threading
-import time
+
 import openai
+from prompt_toolkit import PromptSession
 from pygments import highlight
-from pygments.lexers import get_lexer_by_name, guess_lexer
+from pygments.lexers import guess_lexer
 from pygments.formatters import TerminalFormatter
 
+from spinner import Spinner
+
 try:
     openai.api_key = os.environ["OPENAI_API_KEY"]
 except KeyError:
     print("Please put your API key in the OPENAI_API_KEY environment variable.")
     sys.exit(1)
 
 prompt = """You are a helpful but succinct chatbot that assists an impatient programmer by directly answering questions. You understand that the programmer is advanced enough to understand succinct phrases and prefers direct answers with little boilerplate.
 """
 
 session = PromptSession()
 
-spinner_flag = True  # Flag to control the spinner
-
-def spinner():
-    while spinner_flag:
-        for char in '|/-\\':
-            sys.stdout.write('\r' + char)
-            sys.stdout.flush()
-            time.sleep(0.1)
-    sys.stdout.write("\r")
-
-def stop_spinner():
-    global spinner_flag
-    spinner_flag = False
-
-def start_spinner():
-    global spinner_flag
-    spinner_flag = True
 
 def prompt_continuation(width: int,
                         line_number,
                         is_soft_wrap):
     return '.' * (width-1) + " "
 
 
@@ -99,25 +83,23 @@
     result = session.prompt(">>> ", multiline=True,
                 prompt_continuation=prompt_continuation)
 
     messages.append(
         {"role": "user", "content": result}
     )
 
-    start_spinner()
-    spinner_thread = threading.Thread(target=spinner)
-    spinner_thread.start()
+    spinner = Spinner()
+    spinner.start()
 
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=messages,
     )
     message = response["choices"][0]["message"]
-    stop_spinner()
-    spinner_thread.join()
+    spinner.stop()
 
     messages.append(message)
     print(" ")
     highlight_codeblocks(message["content"])
     print(" ")
 
     return messages
```

### Comparing `aissist-0.0.3/pyproject.toml` & `aissist-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aissist"
-version = "0.0.3"
+version = "0.0.4"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
```

### Comparing `aissist-0.0.3/PKG-INFO` & `aissist-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissist
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple GPT command line interface
 Author-email: Craig Booth <craigmbooth@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 
 1. Be accessible from a simple command line prompt (`ai`)
 1. Open up a shell to talk to ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
 1. Have chat history accessible with the up arrow
 1. Have syntax highlighting on ChatGPT responses
 1. Have multi-line editing capabilities on multi-line prompts
 
-THis library is just that.
+This library is precisely that, and no more.
 
 ## Installation
 
 Via pypi
 
 ```bash
 pip install aissistant
@@ -40,7 +40,13 @@
 There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key.
 
 ## Usage
 
 Invoke the program with `ai`.  There are few controls. Simply enter a prompt, and hit Escape THEN Enter to submit the prompt.
 
 Inside of each session there is a history, and you can use the up arrow to revisit and edit previous prompts.
+
+Here is a simple example
+
+![An example of using aissist to write Python](images/screenshot.png)
+
+
```

