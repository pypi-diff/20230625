# Comparing `tmp/zhon-2.0.0.tar.gz` & `tmp/zhon-2.0.1.tar.gz`

## Comparing `zhon-2.0.0.tar` & `zhon-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/__init__.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/hanzi.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/pinyin.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/zhuyin.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/cedict/__init__.py
--rw-r--r--   0        0        0    39182 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/cedict/all.py
--rw-r--r--   0        0        0    32332 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/cedict/simplified.py
--rw-r--r--   0        0        0    32327 2020-02-02 00:00:00.000000 zhon-2.0.0/src/zhon/cedict/traditional.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 zhon-2.0.0/AUTHORS.rst
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhon-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 zhon-2.0.0/README.rst
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 zhon-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 zhon-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/__init__.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/hanzi.py
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/pinyin.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/zhuyin.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/__init__.py
+-rw-r--r--   0        0        0    39182 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/all.py
+-rw-r--r--   0        0        0    32332 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/simplified.py
+-rw-r--r--   0        0        0    32327 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/traditional.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 zhon-2.0.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhon-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 zhon-2.0.1/README.rst
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 zhon-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 zhon-2.0.1/PKG-INFO
```

### Comparing `zhon-2.0.0/src/zhon/hanzi.py` & `zhon-2.0.1/src/zhon/hanzi.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/src/zhon/pinyin.py` & `zhon-2.0.1/src/zhon/pinyin.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/src/zhon/zhuyin.py` & `zhon-2.0.1/src/zhon/zhuyin.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/src/zhon/cedict/all.py` & `zhon-2.0.1/src/zhon/cedict/all.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/src/zhon/cedict/simplified.py` & `zhon-2.0.1/src/zhon/cedict/simplified.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/src/zhon/cedict/traditional.py` & `zhon-2.0.1/src/zhon/cedict/traditional.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/LICENSE.txt` & `zhon-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/README.rst` & `zhon-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `zhon-2.0.0/pyproject.toml` & `zhon-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,14 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Linguistic",
 ]
-dependencies = [
-    "appdirs",
-]
 
 [project.urls]
 Documentation = "https://tsroten.github.io/fcache"
 "Source code" = "https://github.com/tsroten/zhon"
 
 [tool.hatch.version]
 path = "src/zhon/__init__.py"
```

### Comparing `zhon-2.0.0/PKG-INFO` & `zhon-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhon
-Version: 2.0.0
+Version: 2.0.1
 Summary: Zhon provides constants used in Chinese text processing.
 Project-URL: Documentation, https://tsroten.github.io/fcache
 Project-URL: Source code, https://github.com/tsroten/zhon
 Author-email: Thomas Roten <thomas@roten.us>
 License-Expression: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE.txt
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
-Requires-Dist: appdirs
 Description-Content-Type: text/x-rst
 
 ====
 Zhon
 ====
 
 .. image:: https://badge.fury.io/py/zhon.svg
```

