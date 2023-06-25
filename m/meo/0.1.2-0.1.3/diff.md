# Comparing `tmp/meo-0.1.2.tar.gz` & `tmp/meo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.2.tar", last modified: Sun Jun 25 14:11:38 2023, max compression
+gzip compressed data, was "meo-0.1.3.tar", last modified: Sun Jun 25 15:25:30 2023, max compression
```

## Comparing `meo-0.1.2.tar` & `meo-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.2/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 14:11:38.034730 meo-0.1.2/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.2/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.031396 meo-0.1.2/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      114 2023-06-24 12:18:03.000000 meo-0.1.2/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-25 14:11:34.000000 meo-0.1.2/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)      253 2023-06-24 12:22:10.000000 meo-0.1.2/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      459 2023-06-24 12:43:12.000000 meo-0.1.2/meo/crack/pdf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4881 2023-06-24 14:53:11.000000 meo-0.1.2/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.2/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2212 2023-06-24 12:29:18.000000 meo-0.1.2/meo/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.2/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.2/meo/screen.py
--rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.2/meo/utils.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.031396 meo-0.1.2/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      343 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-25 14:11:38.034730 meo-0.1.2/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1341 2023-06-25 14:06:12.000000 meo-0.1.2/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/test/
--rw-r--r--   0 meo       (1000) meo       (1000)      101 2023-06-24 13:02:17.000000 meo-0.1.2/test/test-read.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.2/test/test.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 15:25:30.262524 meo-0.1.3/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.3/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 15:25:30.262524 meo-0.1.3/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.3/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 15:25:30.262524 meo-0.1.3/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      114 2023-06-24 12:18:03.000000 meo-0.1.3/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-25 14:31:28.000000 meo-0.1.3/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 15:25:30.262524 meo-0.1.3/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)      253 2023-06-24 12:22:10.000000 meo-0.1.3/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      459 2023-06-24 12:43:12.000000 meo-0.1.3/meo/crack/pdf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     7235 2023-06-25 15:18:49.000000 meo-0.1.3/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.3/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2428 2023-06-25 15:23:35.000000 meo-0.1.3/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.3/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.3/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.3/meo/utils.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 15:25:30.262524 meo-0.1.3/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 15:25:30.000000 meo-0.1.3/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      343 2023-06-25 15:25:30.000000 meo-0.1.3/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-25 15:25:30.000000 meo-0.1.3/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-25 15:25:30.000000 meo-0.1.3/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-25 15:25:30.000000 meo-0.1.3/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-25 15:25:30.262524 meo-0.1.3/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1341 2023-06-25 14:06:12.000000 meo-0.1.3/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 15:25:30.262524 meo-0.1.3/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)      101 2023-06-24 13:02:17.000000 meo-0.1.3/test/test-read.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.3/test/test.py
```

### Comparing `meo-0.1.2/LICENSE` & `meo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.2/PKG-INFO` & `meo-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.2
+Version: 0.1.3
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.2/meo/flask.py` & `meo-0.1.3/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.2/meo/io.py` & `meo-0.1.3/meo/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,14 +59,22 @@
     assert isinstance(_bytes, bytes)
     for encoding in ["utf8", 'gbk', 'utf16', 'utf32']:
         try:
             return _bytes.decode(encoding)
         except: pass
     raise ValueError("bytes must be {utf8, gbk, utf16, utf32}")
 
+def cat(*path):
+    file_bytes = bytes()
+    for p in path:
+        if os.path.isfile(p):
+            file_bytes += load_file(p)
+        else:
+            raise ValueError(f"{p} is not a file")
+    return file_bytes
 
 if __name__ == '__main__':
     data = {
         "test": 111
     }
     to_json(data, "./test/output.json")
     to_json5(data, "./test/output.json5")
```

### Comparing `meo-0.1.2/meo/net.py` & `meo-0.1.3/meo/net.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.2/meo/screen.py` & `meo-0.1.3/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.2/meo.egg-info/PKG-INFO` & `meo-0.1.3/meo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.2
+Version: 0.1.3
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.2/setup.py` & `meo-0.1.3/setup.py`

 * *Files identical despite different names*

