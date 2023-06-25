# Comparing `tmp/chatlab-0.14.0.tar.gz` & `tmp/chatlab-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-0.14.0.tar", max compression
+gzip compressed data, was "chatlab-0.14.1.tar", max compression
```

## Comparing `chatlab-0.14.0.tar` & `chatlab-0.14.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 chatlab-0.14.0/LICENSE
--rw-r--r--   0        0        0     7121 2023-06-24 20:10:32.954739 chatlab-0.14.0/README.md
--rw-r--r--   0        0        0     1863 2023-06-25 17:54:33.824854 chatlab-0.14.0/chatlab/__init__.py
--rw-r--r--   0        0        0       23 2023-06-25 17:58:11.386691 chatlab-0.14.0/chatlab/_version.py
--rw-r--r--   0        0        0      897 2023-06-24 22:32:44.193741 chatlab-0.14.0/chatlab/builtins.py
--rw-r--r--   0        0        0     9684 2023-06-25 05:54:27.338669 chatlab-0.14.0/chatlab/conversation.py
--rw-r--r--   0        0        0     2382 2023-06-25 17:43:22.956069 chatlab-0.14.0/chatlab/decorators.py
--rw-r--r--   0        0        0     7698 2023-06-25 17:43:22.956463 chatlab-0.14.0/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-06-25 04:13:12.062499 chatlab-0.14.0/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-06-25 02:50:41.266379 chatlab-0.14.0/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-06-24 22:32:44.194023 chatlab-0.14.0/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-06-25 04:54:08.204496 chatlab-0.14.0/chatlab/models.py
--rw-r--r--   0        0        0     7212 2023-06-25 17:43:22.956810 chatlab-0.14.0/chatlab/registry.py
--rw-r--r--   0        0        0     2023 2023-06-25 17:58:11.386497 chatlab-0.14.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-23 17:12:00.817039 chatlab-0.14.0/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-06-25 17:54:33.826902 chatlab-0.14.0/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-06-25 17:43:22.957117 chatlab-0.14.0/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-06-24 22:32:44.195986 chatlab-0.14.0/tests/test_messaging.py
--rw-r--r--   0        0        0     6792 2023-06-25 02:49:49.084533 chatlab-0.14.0/tests/test_registry.py
--rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 chatlab-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-06-25 18:11:28.688504 chatlab-0.14.1/LICENSE
+-rw-r--r--   0        0        0     7121 2023-06-25 18:11:28.688504 chatlab-0.14.1/README.md
+-rw-r--r--   0        0        0     1863 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/_version.py
+-rw-r--r--   0        0        0      897 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/builtins.py
+-rw-r--r--   0        0        0     9684 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/conversation.py
+-rw-r--r--   0        0        0     2382 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/decorators.py
+-rw-r--r--   0        0        0     7698 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/models.py
+-rw-r--r--   0        0        0     7212 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/registry.py
+-rw-r--r--   0        0        0     2023 2023-06-25 18:11:28.688504 chatlab-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_messaging.py
+-rw-r--r--   0        0        0     6792 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_registry.py
+-rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 chatlab-0.14.1/PKG-INFO
```

### Comparing `chatlab-0.14.0/LICENSE` & `chatlab-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/README.md` & `chatlab-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/__init__.py` & `chatlab-0.14.1/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/builtins.py` & `chatlab-0.14.1/chatlab/builtins.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/conversation.py` & `chatlab-0.14.1/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/decorators.py` & `chatlab-0.14.1/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/display.py` & `chatlab-0.14.1/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/markdown.py` & `chatlab-0.14.1/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/messaging.py` & `chatlab-0.14.1/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/models.py` & `chatlab-0.14.1/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/chatlab/registry.py` & `chatlab-0.14.1/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/pyproject.toml` & `chatlab-0.14.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "0.14.0"
+version = "0.14.1"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Markdown for LLMs."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `chatlab-0.14.0/tests/test_decorators.py` & `chatlab-0.14.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/tests/test_messaging.py` & `chatlab-0.14.1/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/tests/test_registry.py` & `chatlab-0.14.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.0/PKG-INFO` & `chatlab-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 0.14.0
+Version: 0.14.1
 Summary: Markdown for LLMs.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

