# Comparing `tmp/ercotutils-1.0.0.tar.gz` & `tmp/ercotutils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/matthew/PycharmProjects/ercot_mis_pylib/dist/.tmp-fy1zzjvh/ercotutils-1.0.0.tar", last modified: Sat May 20 12:40:34 2023, max compression
+gzip compressed data, was "/home/matthew/PycharmProjects/ercot_mis_pylib/dist/.tmp-u297wrzd/ercotutils-1.1.0.tar", last modified: Sun Jun 25 13:06:37 2023, max compression
```

## Comparing `ercotutils-1.0.0.tar` & `ercotutils-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:40:34.000000 ercotutils-1.0.0/
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1064 2023-05-20 04:21:06.000000 ercotutils-1.0.0/LICENSE.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)      936 2023-05-20 12:40:34.000000 ercotutils-1.0.0/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)      410 2023-05-20 12:24:19.000000 ercotutils-1.0.0/README.md
--rw-r--r--   0 matthew   (1000) matthew   (1000)       84 2023-05-20 12:20:07.000000 ercotutils-1.0.0/pyproject.toml
--rw-r--r--   0 matthew   (1000) matthew   (1000)      718 2023-05-20 12:40:34.000000 ercotutils-1.0.0/setup.cfg
--rw-r--r--   0 matthew   (1000) matthew   (1000)      583 2023-05-20 12:32:52.000000 ercotutils-1.0.0/setup.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils/
--rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:28:14.000000 ercotutils-1.0.0/src/ercotutils/__init__.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1734 2023-05-20 12:19:06.000000 ercotutils-1.0.0/src/ercotutils/misutil.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      936 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)      297 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/SOURCES.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/dependency_links.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       16 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/requires.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       11 2023-05-20 12:40:34.000000 ercotutils-1.0.0/src/ercotutils.egg-info/top_level.txt
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-25 13:06:37.000000 ercotutils-1.1.0/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1064 2023-05-20 04:21:06.000000 ercotutils-1.1.0/LICENSE.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      968 2023-06-25 13:06:37.000000 ercotutils-1.1.0/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      442 2023-06-25 12:55:12.000000 ercotutils-1.1.0/README.md
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       84 2023-05-20 12:20:07.000000 ercotutils-1.1.0/pyproject.toml
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      718 2023-06-25 13:06:37.000000 ercotutils-1.1.0/setup.cfg
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      583 2023-06-25 12:58:33.000000 ercotutils-1.1.0/setup.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2023-05-20 12:28:14.000000 ercotutils-1.1.0/src/ercotutils/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2674 2023-06-25 13:01:49.000000 ercotutils-1.1.0/src/ercotutils/misutil.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      968 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      297 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       16 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/requires.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       11 2023-06-25 13:06:37.000000 ercotutils-1.1.0/src/ercotutils.egg-info/top_level.txt
```

### Comparing `ercotutils-1.0.0/LICENSE.txt` & `ercotutils-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ercotutils-1.0.0/PKG-INFO` & `ercotutils-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ercotutils
-Version: 1.0.0
+Version: 1.1.0
 Summary: ERCOT utils for Python
 Home-page: https://github.com/mmccollom/ercot_mis_pylib
 Author: Matthew McCollom
 Author-email: matthewmccollom1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmccollom/ercot_mis_pylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,22 +12,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ERCOT Python Utility
 This library aims to ease the use of the ERCOT MIS system.
 
+### How to install
+    pip install ercotutils
+
 ### How to use
-    from ercotutils import misutil
-    
-    # Get a list of all the ICE documents for a given report type
-    ice_doc_list = misutil.get_ice_doc_list('13499')
+```python
+from ercotutils import misutil
 
-    ....
+# Get a list of all the ICE documents for a given report type
+ice_doc_list = misutil.get_ice_doc_list('13499')
 
+....
 
-    # Get the file contents of a zipped csv document
-    byte_content = misutil.get_zipped_file_contents('4433444')
 
+# Get the file contents of a zipped csv document
+byte_content = misutil.get_zipped_file_contents('4433444')
+```
 
 ### License
 MIT License
```

### Comparing `ercotutils-1.0.0/setup.cfg` & `ercotutils-1.1.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ercotutils
-version = 1.0.0
+version = 1.1.0
 author = Matthew McCollom
 author_email = matthewmccollom1989@gmail.com
 description = ERCOT utils for Python
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mmccollom/ercot_mis_pylib
 project_urls =
```

### Comparing `ercotutils-1.0.0/setup.py` & `ercotutils-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ercotutils',
-    version='1.0.0',
+    version='1.1.0',
     author='Matthew McCollom',
     author_email='matthewmccollom1989@gmail.com',
     description="ERCOT utils for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mmccollom/ercot_mis_pylib',
     project_urls={
```

### Comparing `ercotutils-1.0.0/src/ercotutils/misutil.py` & `ercotutils-1.1.0/src/ercotutils/misutil.py`

 * *Files 23% similar despite different names*

```diff
@@ -56,8 +56,42 @@
         f.extract(target, '/tmp')
         with open(file_path, 'rb') as f:
             b = f.read()
 
     # delete temporary file
     os.remove(filename)
 
-    return b
+    return b
+
+
+def get_file_contents(document_id: str) -> bytes:
+    """
+    Get the contents of a file from a url
+
+    Parameters:
+    ----------
+        url (str): The url to get the file from
+
+    Returns:
+    ----------
+        bytes: The contents of the file
+    """
+    url = f'https://www.ercot.com/misdownload/servlets/mirDownload?doclookupId={document_id}'
+
+    filename = '/tmp/' + next(tempfile._get_candidate_names())
+    # NOTE the stream=True parameter below
+    with requests.get(url, stream=True) as r:
+        r.raise_for_status()
+        with open(filename, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                # If you have chunk encoded response uncomment if
+                # and set chunk_size parameter to None.
+                # if chunk:
+                f.write(chunk)
+
+    with open(filename, 'rb') as f:
+        b = f.read()
+
+    # delete temporary file
+    os.remove(filename)
+
+    return b
```

### Comparing `ercotutils-1.0.0/src/ercotutils.egg-info/PKG-INFO` & `ercotutils-1.1.0/src/ercotutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ercotutils
-Version: 1.0.0
+Version: 1.1.0
 Summary: ERCOT utils for Python
 Home-page: https://github.com/mmccollom/ercot_mis_pylib
 Author: Matthew McCollom
 Author-email: matthewmccollom1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmccollom/ercot_mis_pylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,22 +12,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ERCOT Python Utility
 This library aims to ease the use of the ERCOT MIS system.
 
+### How to install
+    pip install ercotutils
+
 ### How to use
-    from ercotutils import misutil
-    
-    # Get a list of all the ICE documents for a given report type
-    ice_doc_list = misutil.get_ice_doc_list('13499')
+```python
+from ercotutils import misutil
 
-    ....
+# Get a list of all the ICE documents for a given report type
+ice_doc_list = misutil.get_ice_doc_list('13499')
 
+....
 
-    # Get the file contents of a zipped csv document
-    byte_content = misutil.get_zipped_file_contents('4433444')
 
+# Get the file contents of a zipped csv document
+byte_content = misutil.get_zipped_file_contents('4433444')
+```
 
 ### License
 MIT License
```

