# Comparing `tmp/proJSON-1.2.3.tar.gz` & `tmp/proJSON-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proJSON-1.2.3.tar", last modified: Sat Jun 24 14:41:30 2023, max compression
+gzip compressed data, was "proJSON-1.2.4.tar", last modified: Sun Jun 25 13:34:35 2023, max compression
```

## Comparing `proJSON-1.2.3.tar` & `proJSON-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:41:30.078972 proJSON-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-24 14:41:15.000000 proJSON-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-24 14:41:30.078972 proJSON-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-24 14:41:15.000000 proJSON-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-24 14:41:15.000000 proJSON-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:41:30.078972 proJSON-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:41:30.074972 proJSON-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:41:30.078972 proJSON-1.2.3/src/proJSON/
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-24 14:41:15.000000 proJSON-1.2.3/src/proJSON/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:41:30.078972 proJSON-1.2.3/src/proJSON.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-24 14:41:30.000000 proJSON-1.2.3/src/proJSON.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-24 14:41:30.000000 proJSON-1.2.3/src/proJSON.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:41:30.000000 proJSON-1.2.3/src/proJSON.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:41:30.000000 proJSON-1.2.3/src/proJSON.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 14:41:30.000000 proJSON-1.2.3/src/proJSON.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:41:30.078972 proJSON-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-24 14:41:15.000000 proJSON-1.2.3/tests/test_projson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:34:35.472360 proJSON-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-25 13:34:20.000000 proJSON-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-25 13:34:35.472360 proJSON-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-25 13:34:20.000000 proJSON-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-25 13:34:20.000000 proJSON-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:34:35.472360 proJSON-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:34:35.468360 proJSON-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:34:35.468360 proJSON-1.2.4/src/proJSON/
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-06-25 13:34:20.000000 proJSON-1.2.4/src/proJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:34:35.472360 proJSON-1.2.4/src/proJSON.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-25 13:34:35.000000 proJSON-1.2.4/src/proJSON.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-25 13:34:35.000000 proJSON-1.2.4/src/proJSON.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:34:35.000000 proJSON-1.2.4/src/proJSON.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 13:34:35.000000 proJSON-1.2.4/src/proJSON.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 13:34:35.000000 proJSON-1.2.4/src/proJSON.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:34:35.472360 proJSON-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-25 13:34:20.000000 proJSON-1.2.4/tests/test_projson.py
```

### Comparing `proJSON-1.2.3/LICENSE` & `proJSON-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proJSON-1.2.3/PKG-INFO` & `proJSON-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.2.3
+Version: 1.2.4
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,15 +75,15 @@
 
 ### Init
 
 ``` python
 
 from proJSON import Crafter
 
-template = {
+schema = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
     "stringExample" : {
         "type": "string",
@@ -104,15 +104,15 @@
                 "type": "string",
                 "maxlen": 1
             },
         }
     } 
 }
 
-crafter = Crafter(template)
+crafter = Crafter(schema)
 
 ```
 
 ### Encoding data
 
 ``` python
```

### Comparing `proJSON-1.2.3/README.md` & `proJSON-1.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 ### Init
 
 ``` python
 
 from proJSON import Crafter
 
-template = {
+schema = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
     "stringExample" : {
         "type": "string",
@@ -90,15 +90,15 @@
                 "type": "string",
                 "maxlen": 1
             },
         }
     } 
 }
 
-crafter = Crafter(template)
+crafter = Crafter(schema)
 
 ```
 
 ### Encoding data
 
 ``` python
```

### Comparing `proJSON-1.2.3/pyproject.toml` & `proJSON-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proJSON"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="JKinc", email="communications@jkinc.co.uk" },
 ]
 description = "A python library to compress a dict into a bytearray."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `proJSON-1.2.3/src/proJSON/__init__.py` & `proJSON-1.2.4/src/proJSON/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def decode(self, data: bytes):
 
         if self.compression == "zlib":
             data = decompress(data)
         elif self.compression == "lz4":
             if len(data) > 256:
                 context = frame.create_decompression_context()
-                decompressed = frame.compress_begin(context)
+                decompressed = b""
                 for i in floor(len(data) / 256):
                     decompressed += frame.decompress_chunk(context, data[i*256:(i+1)*256])
                 decompressed += frame.decompress_chunk(context, data[floor(len(data) / 256):floor(len(data) / 256)+(len(data) % 256)])
             else:
                 decompressed = frame.decompress(data)
                 
             data = decompressed
```

### Comparing `proJSON-1.2.3/src/proJSON.egg-info/PKG-INFO` & `proJSON-1.2.4/src/proJSON.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.2.3
+Version: 1.2.4
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,15 +75,15 @@
 
 ### Init
 
 ``` python
 
 from proJSON import Crafter
 
-template = {
+schema = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
     "stringExample" : {
         "type": "string",
@@ -104,15 +104,15 @@
                 "type": "string",
                 "maxlen": 1
             },
         }
     } 
 }
 
-crafter = Crafter(template)
+crafter = Crafter(schema)
 
 ```
 
 ### Encoding data
 
 ``` python
```

### Comparing `proJSON-1.2.3/tests/test_projson.py` & `proJSON-1.2.4/tests/test_projson.py`

 * *Files identical despite different names*

