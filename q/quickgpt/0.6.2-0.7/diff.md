# Comparing `tmp/quickgpt-0.6.2.tar.gz` & `tmp/quickgpt-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgpt-0.6.2.tar", last modified: Mon Apr 24 15:35:03 2023, max compression
+gzip compressed data, was "quickgpt-0.7.tar", last modified: Sun Jun 25 04:32:49 2023, max compression
```

## Comparing `quickgpt-0.6.2.tar` & `quickgpt-0.7.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-24 15:35:03.884707 quickgpt-0.6.2/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-17 02:41:32.000000 quickgpt-0.6.2/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/bin/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6.2/bin/quickgpt
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-24 15:28:50.000000 quickgpt-0.6.2/quickgpt/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt/thread/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     6593 2023-04-24 15:30:08.000000 quickgpt-0.6.2/quickgpt/thread/__init__.py
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      935 2023-04-24 15:32:21.000000 quickgpt-0.6.2/quickgpt/thread/messagetypes.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2772 2023-04-24 15:32:27.000000 quickgpt-0.6.2/quickgpt/thread/response.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/top_level.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-24 15:35:03.884707 quickgpt-0.6.2/setup.cfg
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-04-24 15:24:28.000000 quickgpt-0.6.2/setup.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4350 2023-06-25 04:32:49.967853 quickgpt-0.7/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-24 15:35:03.000000 quickgpt-0.7/README.rst
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/bin/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.7/bin/quickgpt
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1663 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     8339 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/function/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      593 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/function/__init__.py
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      285 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/function/parameter.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt/thread/messagetypes/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1815 2023-06-25 04:32:45.000000 quickgpt-0.7/quickgpt/thread/messagetypes/__init__.py
+-rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2772 2023-04-24 15:32:27.000000 quickgpt-0.7/quickgpt/thread/response.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-06-25 04:32:49.967853 quickgpt-0.7/quickgpt.egg-info/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4350 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      384 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/requires.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-06-25 04:32:49.000000 quickgpt-0.7/quickgpt.egg-info/top_level.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-06-25 04:32:49.967853 quickgpt-0.7/setup.cfg
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      803 2023-06-25 04:32:45.000000 quickgpt-0.7/setup.py
```

### Comparing `quickgpt-0.6.2/PKG-INFO` & `quickgpt-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6.2
+Version: 0.7
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.6.2/README.rst` & `quickgpt-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6.2/bin/quickgpt` & `quickgpt-0.7/bin/quickgpt`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6.2/quickgpt/__init__.py` & `quickgpt-0.7/quickgpt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from quickgpt.thread import Thread
 
-__version__ = "0.6.2"
+__version__ = "0.7"
 
 import os
 
 class QuickGPT:
     def __init__(self, api_key=None, retry_count=3):
         """ Main QuickGPT object
 
@@ -18,15 +18,15 @@
             api_key = os.environ.get("OPENAI_API_KEY")
 
         self.api_key = api_key
         self.retry_count = retry_count
 
         self.threads = []
 
-    def new_thread(self, model="gpt-3.5-turbo"):
+    def new_thread(self, model="gpt-3.5-turbo-0613"):
         """ Creates a brand new Thread.
 
         Args:
             model (str):
 
         Returns:
             Thread: A new Thread for managing a conversation
```

### Comparing `quickgpt-0.6.2/quickgpt/thread/__init__.py` & `quickgpt-0.7/quickgpt/thread/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     def __init__(self, quickgpt, model):
         self.quickgpt = quickgpt
         self.model = model
 
         openai.api_key = quickgpt.api_key
 
         self.thread = []
+        self.functions = {}
+        self.usage = {
+            "prompt_tokens": 0,
+            "completion_tokens": 0,
+            "total_tokens": 0
+        }
+
         self.id = str(uuid4())
 
         self.tokenizer = None
 
     def __len__(self):
         """ Returns the length of the Thread, by message count
 
@@ -68,15 +75,16 @@
             dict: A JSON-safe representation of this thread, to be restored
                 later using thread.restore()
         """
 
         return {
             "__quickgpt-thread__": {
                 "id": self.id,
-                "thread": self.messages
+                "thread": self.messages,
+                "usage": self.usage
             }
         }
 
     def restore(self, obj):
         """ Restores a serialized Thread object,
         provided by thread.serialize()
 
@@ -86,14 +94,17 @@
         Returns:
             None
         """
 
         thread_dict = obj["__quickgpt-thread__"]
         self.id = thread_dict["id"]
 
+        if "usage" in obj:
+            self.usage = obj["usage"]
+
         self.feed(thread_dict["thread"])
 
     def clear(self, include_sticky=False):
         """ Resets the thread, preserving only messages that were
         marked as sticky - unless include_sticky is set to True."""
 
         for message in self.thread:
@@ -107,28 +118,31 @@
             # Check if the first argument is a list, and then make it the parent
             iter(messages[0])
             messages = messages[0]
         except TypeError:
             pass
 
         for msg in messages:
-            assert type(msg) in (System, Assistant, User, Response, dict), \
-                "Must be of type System, Assistant, User, Response, or dict"
+            assert type(msg) in (System, Assistant, User, Function, Response, dict), \
+                "Must be of type System, Assistant, User, Function, Response, or dict"
 
             # Convert a boring old dict message to a pretty object message
             if type(msg) == dict:
                 role = msg["role"]
                 content = msg["content"]
 
                 if role == "system":
                     msg = System(content)
                 elif role == "assistant":
                     msg = Assistant(content)
                 elif role == "user":
                     msg = User(content)
+                elif role == "function":
+                    name = msg["name"]
+                    msg = Function(name, content)
                 else:
                     raise TypeError("Unknown role '%s'" % role)
 
             if insert:
                 self.thread.insert(insert, msg)
             else:
                 self.thread.append(msg)
@@ -150,62 +164,105 @@
 
         Returns:
             list: JSON-safe list of all messages
         """
 
         return [ msg.obj for msg in self.thread ]
 
-    def run(self, *append_messages, feed=True, stream=False):
+    def add_function(self, method):
+        """ Add a function that ChatGPT can call back.
+
+        *name
+        *method
+
+        Returns:
+            Response:
+        """
+
+        self.functions[method.__name__] = method
+
+    def run(self, *append_messages, feed=True, stream=False, functions=None):
         """ Executes the current Thread and get a response. If ``feed`` is
         True, it will automatically save the response to the Thread.
 
         You can provide *append_messages that will only apply to this run(),
         and won't be permanently stored in the Thread.
 
+        *functions allows you to define functions.
+
         Returns:
             Response: The resulting Response object from OpenAI
         """
 
         messages = self.messages
         append_messages = [ msg.obj for msg in append_messages ]
 
         for i in range(self.quickgpt.retry_count):
             try:
-                response_obj = openai.ChatCompletion.create(
-                    model=self.model,
-                    messages=messages + append_messages,
-                    stream=stream
-                )
+                if functions:
+                    response_obj = openai.ChatCompletion.create(
+                        model=self.model,
+                        messages=messages + append_messages,
+                        stream=stream,
+                        functions=functions,
+                        function_call="auto"
+                    )
+                else:
+                    response_obj = openai.ChatCompletion.create(
+                        model=self.model,
+                        messages=messages + append_messages,
+                        stream=stream
+                    )
 
                 break
             except openai.error.RateLimitError as e:
                 if self.quickgpt.retry_count == i - 1:
                     print("Failed after %s tries" % self.quickgpt.retry_count)
                     raise e
 
                 print("OpenAI returned RateLimitError, trying again after 10 sec...")
+
                 time.sleep(10)
             except openai.error.InvalidRequestError as e:
                 print(
                     json.dumps({
                         "messages": messages + append_messages,
                         "model": self.model
                     }, indent=2)
                 )
 
                 print("Please see failed request encoded as JSON above.")
 
                 raise e
 
-        response = Response(response_obj, stream=stream)
+        self.usage = response_obj["usage"]
+
+        message = response_obj["choices"][0]["message"]
+
+        if "function_call" in message:
+            function_call = message["function_call"]
+            name = function_call["name"]
+            arguments = json.loads(function_call["arguments"])
+
+            content = self.functions[name](**arguments)
+
+            function = Function(name, content)
+
+            if feed:
+                self.feed(Assistant(None, function_call=function_call))
+                self.feed(function)
+
+            return function
+        else:
+            response = Response(response_obj, stream=stream)
 
-        if feed:
-            self.feed(response)
+            if feed:
+                self.feed(response)
 
-        return response
+            return response
 
     def moderate(self, prompt):
         """ Validate a prompt to ensure it's safe for OpenAI's policies
 
         Args:
             prompt (str): The user's query to validate
```

### Comparing `quickgpt-0.6.2/quickgpt/thread/messagetypes.py` & `quickgpt-0.7/quickgpt/thread/messagetypes/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tiktoken
 
-class Message:
+class Message(object):
     def __init__(self, content, sticky=False):
         self.content = content
         self.sticky = sticky
 
     @property
     def role(self):
         return self.__class__.__name__.lower()
@@ -31,8 +31,40 @@
         """ Returns the length of the content, in tokens """
         tokenizer = tiktoken.get_encoding("cl100k_base")
 
         return len(tokenizer.encode(self.message))
 
 class System(Message): pass
 class User(Message): pass
-class Assistant(Message): pass
+class Assistant(Message):
+    def __init__(self, content, function_call=None, sticky=False):
+        self.content = content
+        self.function_call = function_call
+        self.sticky = sticky
+
+    @property
+    def obj(self):
+        if self.function_call:
+            return {
+                "role": self.role,
+                "function_call": self.function_call,
+                "content": self.content
+            }
+        else:
+            return {
+                "role": self.role,
+                "content": self.content
+            }
+
+class Function(Message):
+    def __init__(self, name, content, sticky=False):
+        self.name = name
+        self.content = content
+        self.sticky = sticky
+
+    @property
+    def obj(self):
+        return {
+            "role": self.role,
+            "name": self.name,
+            "content": self.content
+        }
```

### Comparing `quickgpt-0.6.2/quickgpt/thread/response.py` & `quickgpt-0.7/quickgpt/thread/response.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6.2/quickgpt.egg-info/PKG-INFO` & `quickgpt-0.7/quickgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6.2
+Version: 0.7
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.6.2/setup.py` & `quickgpt-0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='quickgpt',
-    version='0.6.2',
+    version='0.7',
     description='A barebones library to make interacting with OpenAI\'s ChatGPT API much simpler.',
     long_description=open("README.rst", "r").read(),
     author='Ben Baptist',
     author_email='me@benbaptist.com',
     url='https://github.com/benbaptist/quickgpt',
     packages=find_packages(),
     scripts=['bin/quickgpt'],
```

