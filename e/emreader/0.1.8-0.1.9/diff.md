# Comparing `tmp/emreader-0.1.8.tar.gz` & `tmp/emreader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emreader-0.1.8.tar", max compression
+gzip compressed data, was "emreader-0.1.9.tar", max compression
```

## Comparing `emreader-0.1.8.tar` & `emreader-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.8/README.md
--rw-r--r--   0        0        0      898 2023-06-25 17:26:45.673016 emreader-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.8/src/__init__.py
--rw-r--r--   0        0        0     3828 2023-06-25 17:15:52.721516 emreader-0.1.8/src/app.py
--rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.8/src/core/__init__.py
--rw-r--r--   0        0        0      143 2023-06-22 19:52:00.056298 emreader-0.1.8/src/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.8/src/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4388 2023-06-25 17:24:33.737509 emreader-0.1.8/src/core/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     8710 2023-06-22 20:20:06.352156 emreader-0.1.8/src/core/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2771 2023-06-25 17:25:23.728843 emreader-0.1.8/src/core/__pycache__/eml.cpython-310.pyc
--rw-r--r--   0        0        0     6300 2023-06-22 20:18:38.256286 emreader-0.1.8/src/core/__pycache__/eml.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2023-06-22 19:52:01.169455 emreader-0.1.8/src/core/__pycache__/parse_tab.cpython-310.pyc
--rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.8/src/core/__pycache__/parse_tab.cpython-311.pyc
--rw-r--r--   0        0        0      830 2023-06-25 17:07:44.040581 emreader-0.1.8/src/core/__pycache__/store.cpython-310.pyc
--rw-r--r--   0        0        0     3538 2023-06-22 19:52:01.170857 emreader-0.1.8/src/core/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.8/src/core/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0     6204 2023-06-25 17:24:18.772026 emreader-0.1.8/src/core/base.py
--rw-r--r--   0        0        0     3228 2023-06-25 17:25:20.263466 emreader-0.1.8/src/core/eml.py
--rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.8/src/core/parse_tab.py
--rw-r--r--   0        0        0      597 2023-06-25 17:02:25.950652 emreader-0.1.8/src/core/store.py
--rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.8/src/core/util.py
--rw-r--r--   0        0        0        0 2023-06-22 19:55:56.070115 emreader-0.1.8/src/db/.gitkeep
--rw-r--r--   0        0        0      189 2023-06-22 19:51:55.311457 emreader-0.1.8/src/runner.py
--rw-r--r--   0        0        0        0 2023-06-22 19:55:56.070115 emreader-0.1.8/src/storage/output/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-22 19:56:09.592388 emreader-0.1.8/src/storage/source/emails/.gitkeep
--rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 emreader-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.9/README.md
+-rw-r--r--   0        0        0      911 2023-06-25 17:33:59.637419 emreader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.9/src/__init__.py
+-rw-r--r--   0        0        0     3828 2023-06-25 17:15:52.721516 emreader-0.1.9/src/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.9/src/core/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-22 19:52:00.056298 emreader-0.1.9/src/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.9/src/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4388 2023-06-25 17:24:33.737509 emreader-0.1.9/src/core/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     8710 2023-06-22 20:20:06.352156 emreader-0.1.9/src/core/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2771 2023-06-25 17:25:23.728843 emreader-0.1.9/src/core/__pycache__/eml.cpython-310.pyc
+-rw-r--r--   0        0        0     6300 2023-06-22 20:18:38.256286 emreader-0.1.9/src/core/__pycache__/eml.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2023-06-22 19:52:01.169455 emreader-0.1.9/src/core/__pycache__/parse_tab.cpython-310.pyc
+-rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.9/src/core/__pycache__/parse_tab.cpython-311.pyc
+-rw-r--r--   0        0        0      830 2023-06-25 17:07:44.040581 emreader-0.1.9/src/core/__pycache__/store.cpython-310.pyc
+-rw-r--r--   0        0        0     3538 2023-06-22 19:52:01.170857 emreader-0.1.9/src/core/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.9/src/core/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     6204 2023-06-25 17:24:18.772026 emreader-0.1.9/src/core/base.py
+-rw-r--r--   0        0        0     3228 2023-06-25 17:25:20.263466 emreader-0.1.9/src/core/eml.py
+-rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.9/src/core/parse_tab.py
+-rw-r--r--   0        0        0      597 2023-06-25 17:02:25.950652 emreader-0.1.9/src/core/store.py
+-rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.9/src/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:55:56.070115 emreader-0.1.9/src/db/.gitkeep
+-rw-r--r--   0        0        0      189 2023-06-22 19:51:55.311457 emreader-0.1.9/src/runner.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:55:56.070115 emreader-0.1.9/src/storage/output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 19:56:09.592388 emreader-0.1.9/src/storage/source/emails/.gitkeep
+-rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 emreader-0.1.9/PKG-INFO
```

### Comparing `emreader-0.1.8/pyproject.toml` & `emreader-0.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "emreader"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["themba <themba@advantch.com>"]
 readme = "README.md"
 license = "Commercial"
-packages = [{include = "src"}]
+packages = [{include = "src", from = "." }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 cffi = "^1.15.1"
 chardet = "^5.1.0"
 charset-normalizer = "^3.1.0"
 click = "^8.1.3"
```

### Comparing `emreader-0.1.8/src/app.py` & `emreader-0.1.9/src/app.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/base.cpython-310.pyc` & `emreader-0.1.9/src/core/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/base.cpython-311.pyc` & `emreader-0.1.9/src/core/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/eml.cpython-310.pyc` & `emreader-0.1.9/src/core/__pycache__/eml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/eml.cpython-311.pyc` & `emreader-0.1.9/src/core/__pycache__/eml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/parse_tab.cpython-310.pyc` & `emreader-0.1.9/src/core/__pycache__/parse_tab.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/parse_tab.cpython-311.pyc` & `emreader-0.1.9/src/core/__pycache__/parse_tab.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/store.cpython-310.pyc` & `emreader-0.1.9/src/core/__pycache__/store.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/util.cpython-310.pyc` & `emreader-0.1.9/src/core/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/__pycache__/util.cpython-311.pyc` & `emreader-0.1.9/src/core/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/base.py` & `emreader-0.1.9/src/core/base.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/eml.py` & `emreader-0.1.9/src/core/eml.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/parse_tab.py` & `emreader-0.1.9/src/core/parse_tab.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/store.py` & `emreader-0.1.9/src/core/store.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/src/core/util.py` & `emreader-0.1.9/src/core/util.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.8/PKG-INFO` & `emreader-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emreader
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: Commercial
 Author: themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

