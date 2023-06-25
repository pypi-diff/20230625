# Comparing `tmp/quickgpt-0.7.tar.gz` & `tmp/quickgpt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgpt-0.7.tar", last modified: Sun Jun 25 04:32:49 2023, max compression
+gzip compressed data, was "quickgpt-0.7.1.tar", last modified: Sun Jun 25 04:53:57 2023, max compression
```

## Comparing `quickgpt-0.7.tar` & `quickgpt-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4350 2023-06-25 04:32:49.967853 quickgpt-0.7/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-24 15:35:03.000000 quickgpt-0.7/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/bin/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.7/bin/quickgpt
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1663 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     8339 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/function/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      593 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/function/__init__.py
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      285 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/function/parameter.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/messagetypes/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1815 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/messagetypes/__init__.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2772 2023-04-24 15:32:27.000000 quickgpt-0.7/quickgpt/thread/response.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4350 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      384 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/top_level.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-06-25 04:32:49.967853 quickgpt-0.7/setup.cfg
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      803 2023-06-25 04:32:45.000000 quickgpt-0.7/setup.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-06-25 04:53:57.621637 quickgpt-0.7.1/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-06-25 04:39:22.000000 quickgpt-0.7.1/README.rst
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/bin/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.7.1/bin/quickgpt
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/quickgpt/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1665 2023-06-25 04:53:35.000000 quickgpt-0.7.1/quickgpt/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/quickgpt/thread/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     9402 2023-06-25 04:52:07.000000 quickgpt-0.7.1/quickgpt/thread/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/quickgpt/thread/function/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      593 2023-06-25 04:32:45.000000 quickgpt-0.7.1/quickgpt/thread/function/__init__.py
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      285 2023-06-25 04:32:45.000000 quickgpt-0.7.1/quickgpt/thread/function/parameter.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/quickgpt/thread/messagetypes/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1815 2023-06-25 04:32:45.000000 quickgpt-0.7.1/quickgpt/thread/messagetypes/__init__.py
+-rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2772 2023-04-24 15:32:27.000000 quickgpt-0.7.1/quickgpt/thread/response.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:53:57.621637 quickgpt-0.7.1/quickgpt.egg-info/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-06-25 04:53:57.000000 quickgpt-0.7.1/quickgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      384 2023-06-25 04:53:57.000000 quickgpt-0.7.1/quickgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-06-25 04:53:57.000000 quickgpt-0.7.1/quickgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-06-25 04:53:57.000000 quickgpt-0.7.1/quickgpt.egg-info/requires.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-06-25 04:53:57.000000 quickgpt-0.7.1/quickgpt.egg-info/top_level.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-06-25 04:53:57.621637 quickgpt-0.7.1/setup.cfg
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-06-25 04:53:41.000000 quickgpt-0.7.1/setup.py
```

### Comparing `quickgpt-0.7/PKG-INFO` & `quickgpt-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.7
+Version: 0.7.1
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.7/README.rst` & `quickgpt-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `quickgpt-0.7/bin/quickgpt` & `quickgpt-0.7.1/bin/quickgpt`

 * *Files identical despite different names*

### Comparing `quickgpt-0.7/quickgpt/__init__.py` & `quickgpt-0.7.1/quickgpt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from quickgpt.thread import Thread
 
-__version__ = "0.7"
+__version__ = "0.7.1"
 
 import os
 
 class QuickGPT:
     def __init__(self, api_key=None, retry_count=3):
         """ Main QuickGPT object
```

### Comparing `quickgpt-0.7/quickgpt/thread/__init__.py` & `quickgpt-0.7.1/quickgpt/thread/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -164,39 +164,72 @@
 
         Returns:
             list: JSON-safe list of all messages
         """
 
         return [ msg.obj for msg in self.thread ]
 
-    def add_function(self, method):
+    def add_function(self, method, description, properties, required=[]):
         """ Add a function that ChatGPT can call back.
 
         *name
         *method
 
         Returns:
             Response:
         """
 
-        self.functions[method.__name__] = method
+        self.functions[method.__name__] = {
+            "method": method,
+            "description": description,
+            "properties": properties,
+            "required": required
+        }
 
-    def run(self, *append_messages, feed=True, stream=False, functions=None):
+    def remove_function(self, name):
+        del self.functions[name]
+
+    def run(self, *append_messages, feed=True, stream=False):
         """ Executes the current Thread and get a response. If ``feed`` is
         True, it will automatically save the response to the Thread.
 
         You can provide *append_messages that will only apply to this run(),
         and won't be permanently stored in the Thread.
 
         *functions allows you to define functions.
 
         Returns:
             Response: The resulting Response object from OpenAI
         """
 
+        functions = None
+
+        if len(self.functions) > 0:
+            functions = []
+
+            for name in self.functions:
+                function = self.functions[name]
+
+                method = function["method"]
+                description = function["description"]
+                properties = function["properties"]
+                required = function["required"]
+
+                _function = {
+                        "name": name,
+                        "description": description,
+                        "parameters": {
+                            "type": "object",
+                            "properties": properties,
+                            "required": required
+                        }
+                    }
+
+                functions.append(_function)
+
         messages = self.messages
         append_messages = [ msg.obj for msg in append_messages ]
 
         for i in range(self.quickgpt.retry_count):
             try:
                 if functions:
                     response_obj = openai.ChatCompletion.create(
@@ -239,15 +272,15 @@
         message = response_obj["choices"][0]["message"]
 
         if "function_call" in message:
             function_call = message["function_call"]
             name = function_call["name"]
             arguments = json.loads(function_call["arguments"])
 
-            content = self.functions[name](**arguments)
+            content = self.functions[name]["method"](**arguments)
 
             function = Function(name, content)
 
             if feed:
                 self.feed(Assistant(None, function_call=function_call))
                 self.feed(function)
```

### Comparing `quickgpt-0.7/quickgpt/thread/function/__init__.py` & `quickgpt-0.7.1/quickgpt/thread/function/__init__.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.7/quickgpt/thread/messagetypes/__init__.py` & `quickgpt-0.7.1/quickgpt/thread/messagetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.7/quickgpt/thread/response.py` & `quickgpt-0.7.1/quickgpt/thread/response.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.7/quickgpt.egg-info/PKG-INFO` & `quickgpt-0.7.1/quickgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.7
+Version: 0.7.1
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.7/setup.py` & `quickgpt-0.7.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='quickgpt',
-    version='0.7',
+    version='0.7.1',
     description='A barebones library to make interacting with OpenAI\'s ChatGPT API much simpler.',
     long_description=open("README.rst", "r").read(),
     author='Ben Baptist',
     author_email='me@benbaptist.com',
     url='https://github.com/benbaptist/quickgpt',
     packages=find_packages(),
     scripts=['bin/quickgpt'],
```

