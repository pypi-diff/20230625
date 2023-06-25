# Comparing `tmp/chat-box-streamlit-0.0.5.tar.gz` & `tmp/chat-box-streamlit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.5.tar", last modified: Sun Jun 25 03:16:09 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.6.tar", last modified: Sun Jun 25 05:50:27 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.5.tar` & `chat-box-streamlit-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 03:15:57.000000 chat-box-streamlit-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:27.760755 chat-box-streamlit-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 05:50:09.000000 chat-box-streamlit-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 05:50:09.000000 chat-box-streamlit-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 05:50:27.760755 chat-box-streamlit-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-25 05:50:09.000000 chat-box-streamlit-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:27.760755 chat-box-streamlit-0.0.6/chat_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-25 05:50:09.000000 chat-box-streamlit-0.0.6/chat_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:27.760755 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 05:50:27.000000 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 05:50:27.000000 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:50:27.000000 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 05:50:27.000000 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 05:50:27.000000 chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:50:27.760755 chat-box-streamlit-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 05:50:12.000000 chat-box-streamlit-0.0.6/setup.py
```

### Comparing `chat-box-streamlit-0.0.5/LICENSE` & `chat-box-streamlit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.5/PKG-INFO` & `chat-box-streamlit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.5/README.md` & `chat-box-streamlit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.5/chat_box/__init__.py` & `chat-box-streamlit-0.0.6/chat_box/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import streamlit as st
 import streamlit.components.v1 as components
 
 
-_RELEASE = False
+_RELEASE = True
 
 if not _RELEASE:
     _chat_box = components.declare_component(
         "chat_box_streamlit",
         url="http://localhost:3001",
     )
 else:
```

### Comparing `chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.6/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.5/setup.py` & `chat-box-streamlit-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.5",
+    version="0.0.6",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

