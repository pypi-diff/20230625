# Comparing `tmp/aissist-0.0.5.tar.gz` & `tmp/aissist-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.5.tar` & `aissist-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.5/LICENSE
--rw-r--r--   0        0        0      212 2023-06-25 03:44:03.985612 aissist-0.0.5/Pipfile
--rw-r--r--   0        0        0    41743 2023-06-25 03:44:08.209610 aissist-0.0.5/Pipfile.lock
--rw-r--r--   0        0        0     1181 2023-06-25 03:04:17.106277 aissist-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.5/aissist/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-25 03:38:07.089502 aissist-0.0.5/aissist/aissistant.py
--rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.5/aissist/spinner.py
--rw-r--r--   0        0        0       22 2023-06-25 03:45:49.137565 aissist-0.0.5/aissist/version.py
--rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.5/images/screenshot.png
--rw-r--r--   0        0        0      899 2023-06-25 03:45:53.397563 aissist-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 aissist-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.6/LICENSE
+-rw-r--r--   0        0        0      212 2023-06-25 03:44:03.985612 aissist-0.0.6/Pipfile
+-rw-r--r--   0        0        0    41743 2023-06-25 03:44:08.209610 aissist-0.0.6/Pipfile.lock
+-rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.6/aissist/__init__.py
+-rw-r--r--   0        0        0     3391 2023-06-25 03:38:07.089502 aissist-0.0.6/aissist/aissistant.py
+-rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.6/aissist/spinner.py
+-rw-r--r--   0        0        0       22 2023-06-25 03:53:01.265161 aissist-0.0.6/aissist/version.py
+-rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.6/images/screenshot.png
+-rw-r--r--   0        0        0      899 2023-06-25 03:52:49.025175 aissist-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.6/PKG-INFO
```

### Comparing `aissist-0.0.5/LICENSE` & `aissist-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.5/Pipfile.lock` & `aissist-0.0.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aissist-0.0.5/README.md` & `aissist-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # AI Assistant
 
 This library was written to scratch a personal itch.  I have found GPT 3.5 to be incredibly useful in my day-to-day coding activities, but also found that having to go to a web browser and interact there was tedious.  What I really wanted was a tool that would:
 
 1. Be accessible from a simple command line prompt (`ai`)
-1. Open up a shell to talk to ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
+1. That single command should open up a shell to interact with ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
 1. Have chat history accessible with the up arrow
 1. Have syntax highlighting on ChatGPT responses
 1. Have multi-line editing capabilities on multi-line prompts
 
 This library is precisely that, and no more.
 
 ## Installation
 
-Via pypi
+Install using pypi with
 
 ```bash
 pip install aissistant
 ```
 
-There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key.
+There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key. `aissist` will prompt you if the key is not set or is invalid.
 
 ## Usage
 
 Invoke the program with `ai`.  There are few controls. Simply enter a prompt, and hit Escape THEN Enter to submit the prompt.
 
 Inside of each session there is a history, and you can use the up arrow to revisit and edit previous prompts.
 
 Here is a simple example
 
-![An example of using aissist to write Python](images/screenshot.png)
+![An example of using aissist to write Python](https://github.com/craigmbooth/aissist/raw/master/images/screenshot.png)
```

### Comparing `aissist-0.0.5/aissist/aissistant.py` & `aissist-0.0.6/aissist/aissistant.py`

 * *Files identical despite different names*

### Comparing `aissist-0.0.5/aissist/spinner.py` & `aissist-0.0.6/aissist/spinner.py`

 * *Files identical despite different names*

### Comparing `aissist-0.0.5/images/screenshot.png` & `aissist-0.0.6/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `aissist-0.0.5/pyproject.toml` & `aissist-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aissist"
-version = "0.0.5"
+version = "0.0.6"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
```

### Comparing `aissist-0.0.5/PKG-INFO` & `aissist-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissist
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple GPT command line interface
 Author-email: Craig Booth <craigmbooth@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,35 +19,35 @@
 Project-URL: Homepage, https://github.com/craigmbooth/aissist
 
 # AI Assistant
 
 This library was written to scratch a personal itch.  I have found GPT 3.5 to be incredibly useful in my day-to-day coding activities, but also found that having to go to a web browser and interact there was tedious.  What I really wanted was a tool that would:
 
 1. Be accessible from a simple command line prompt (`ai`)
-1. Open up a shell to talk to ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
+1. That single command should open up a shell to interact with ChatGPT, with the system already prompted to respond tersely but helpfully to coding questions
 1. Have chat history accessible with the up arrow
 1. Have syntax highlighting on ChatGPT responses
 1. Have multi-line editing capabilities on multi-line prompts
 
 This library is precisely that, and no more.
 
 ## Installation
 
-Via pypi
+Install using pypi with
 
 ```bash
 pip install aissistant
 ```
 
-There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key.
+There is one required environment variable, `OPENAI_API_KEY`, which should contain an OpenAI API key. `aissist` will prompt you if the key is not set or is invalid.
 
 ## Usage
 
 Invoke the program with `ai`.  There are few controls. Simply enter a prompt, and hit Escape THEN Enter to submit the prompt.
 
 Inside of each session there is a history, and you can use the up arrow to revisit and edit previous prompts.
 
 Here is a simple example
 
-![An example of using aissist to write Python](images/screenshot.png)
+![An example of using aissist to write Python](https://github.com/craigmbooth/aissist/raw/master/images/screenshot.png)
```

