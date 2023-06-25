# Comparing `tmp/dify-client-0.1.7.tar.gz` & `tmp/dify-client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify-client-0.1.7.tar", last modified: Sun May 14 09:09:33 2023, max compression
+gzip compressed data, was "dify-client-0.1.8.tar", last modified: Sun Jun 25 08:15:23 2023, max compression
```

## Comparing `dify-client-0.1.7.tar` & `dify-client-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.859919 dify-client-0.1.7/
--rw-r--r--   0 johnwang   (501) staff       (20)     1067 2023-05-14 08:36:41.000000 dify-client-0.1.7/LICENSE
--rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-14 08:23:26.000000 dify-client-0.1.7/MANIFEST.in
--rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:09:33.859576 dify-client-0.1.7/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)     2465 2023-05-14 09:07:25.000000 dify-client-0.1.7/README.md
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.857084 dify-client-0.1.7/dify_client/
--rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-14 08:23:26.000000 dify-client-0.1.7/dify_client/__init__.py
--rw-r--r--   0 johnwang   (501) staff       (20)     2655 2023-05-14 09:09:22.000000 dify-client-0.1.7/dify_client/client.py
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.859176 dify-client-0.1.7/dify_client.egg-info/
--rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)      258 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/SOURCES.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/dependency_links.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/requires.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/top_level.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-05-14 09:09:33.860033 dify-client-0.1.7/setup.cfg
--rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-05-14 09:09:29.000000 dify-client-0.1.7/setup.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-06-25 08:15:23.572657 dify-client-0.1.8/
+-rw-rw-r--   0 johnwang   (501) staff       (20)     1067 2023-05-14 12:36:24.000000 dify-client-0.1.8/LICENSE
+-rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-15 00:17:07.000000 dify-client-0.1.8/MANIFEST.in
+-rw-r--r--   0 johnwang   (501) staff       (20)     2956 2023-06-25 08:15:23.572498 dify-client-0.1.8/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)     2466 2023-05-15 00:17:07.000000 dify-client-0.1.8/README.md
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-06-25 08:15:23.571349 dify-client-0.1.8/dify_client/
+-rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-15 00:17:07.000000 dify-client-0.1.8/dify_client/__init__.py
+-rw-r--r--   0 johnwang   (501) staff       (20)     2652 2023-06-25 08:14:57.000000 dify-client-0.1.8/dify_client/client.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-06-25 08:15:23.572148 dify-client-0.1.8/dify_client.egg-info/
+-rw-r--r--   0 johnwang   (501) staff       (20)     2956 2023-06-25 08:15:23.000000 dify-client-0.1.8/dify_client.egg-info/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)      279 2023-06-25 08:15:23.000000 dify-client-0.1.8/dify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-06-25 08:15:23.000000 dify-client-0.1.8/dify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-06-25 08:15:23.000000 dify-client-0.1.8/dify_client.egg-info/requires.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-06-25 08:15:23.000000 dify-client-0.1.8/dify_client.egg-info/top_level.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-06-25 08:15:23.572702 dify-client-0.1.8/setup.cfg
+-rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-06-25 08:14:57.000000 dify-client-0.1.8/setup.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-06-25 08:15:23.572281 dify-client-0.1.8/tests/
+-rw-r--r--   0 johnwang   (501) staff       (20)     1629 2023-05-15 00:17:07.000000 dify-client-0.1.8/tests/test_client.py
```

### Comparing `dify-client-0.1.7/LICENSE` & `dify-client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dify-client-0.1.7/PKG-INFO` & `dify-client-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dify-client
+
 A Dify App Service-API Client, using for build a webapp by request Service-API
 
 ## Usage
 
 First, install `dify-client` python sdk package:
 
 ```
```

### Comparing `dify-client-0.1.7/README.md` & `dify-client-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # dify-client
+
 A Dify App Service-API Client, using for build a webapp by request Service-API
 
 ## Usage
 
 First, install `dify-client` python sdk package:
 
 ```
```

### Comparing `dify-client-0.1.7/dify_client/client.py` & `dify-client-0.1.8/dify_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,14 @@
         if first_id:
             params["first_id"] = first_id
         if limit:
             params["limit"] = limit
 
         return self._send_request("GET", "/messages", params=params)
 
-    def get_conversations(self, user, first_id=None, limit=None, pinned=None):
-        params = {"user": user, "first_id": first_id, "limit": limit, "pinned": pinned}
+    def get_conversations(self, user, last_id=None, limit=None, pinned=None):
+        params = {"user": user, "last_id": last_id, "limit": limit, "pinned": pinned}
         return self._send_request("GET", "/conversations", params=params)
 
     def rename_conversation(self, conversation_id, name, user):
         data = {"name": name, "user": user}
         return self._send_request("POST", f"/conversations/{conversation_id}/name", data)
```

### Comparing `dify-client-0.1.7/dify_client.egg-info/PKG-INFO` & `dify-client-0.1.8/dify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dify-client
+
 A Dify App Service-API Client, using for build a webapp by request Service-API
 
 ## Usage
 
 First, install `dify-client` python sdk package:
 
 ```
```

### Comparing `dify-client-0.1.7/setup.py` & `dify-client-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dify-client",
-    version="0.1.7",
+    version="0.1.8",
     author="Dify",
     author_email="hello@dify.ai",
     description="A package for interacting with the Dify Service-API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/langgenius/dify",
     license='MIT',
```

