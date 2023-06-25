# Comparing `tmp/tuspyserver-1.3.0.tar.gz` & `tmp/tuspyserver-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuspyserver-1.3.0.tar", last modified: Sun Jun 25 13:25:46 2023, max compression
+gzip compressed data, was "tuspyserver-1.3.1.tar", last modified: Sun Jun 25 13:30:55 2023, max compression
```

## Comparing `tuspyserver-1.3.0.tar` & `tuspyserver-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910954 tuspyserver-1.3.0/
--rw-r--r--   0 edihasaj   (501) staff       (20)     1086 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/LICENSE
--rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:25:46.910840 tuspyserver-1.3.0/PKG-INFO
--rw-r--r--   0 edihasaj   (501) staff       (20)     1393 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/README.md
--rw-r--r--   0 edihasaj   (501) staff       (20)       38 2023-06-25 13:25:46.910992 tuspyserver-1.3.0/setup.cfg
--rw-r--r--   0 edihasaj   (501) staff       (20)     1116 2023-06-25 13:24:39.000000 tuspyserver-1.3.0/setup.py
-drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910339 tuspyserver-1.3.0/tuspyserver.egg-info/
--rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/PKG-INFO
--rw-r--r--   0 edihasaj   (501) staff       (20)      261 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/SOURCES.txt
--rw-r--r--   0 edihasaj   (501) staff       (20)        1 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/dependency_links.txt
--rw-r--r--   0 edihasaj   (501) staff       (20)       51 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/requires.txt
--rw-r--r--   0 edihasaj   (501) staff       (20)       10 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/top_level.txt
-drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910673 tuspyserver-1.3.0/tusserver/
--rw-r--r--   0 edihasaj   (501) staff       (20)       22 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/tusserver/__init__.py
--rw-r--r--   0 edihasaj   (501) staff       (20)      736 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/tusserver/metadata.py
--rw-r--r--   0 edihasaj   (501) staff       (20)    11358 2023-06-25 13:20:51.000000 tuspyserver-1.3.0/tusserver/tus.py
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:30:55.921926 tuspyserver-1.3.1/
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1086 2023-06-25 12:40:59.000000 tuspyserver-1.3.1/LICENSE
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:30:55.921815 tuspyserver-1.3.1/PKG-INFO
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1393 2023-06-25 12:40:59.000000 tuspyserver-1.3.1/README.md
+-rw-r--r--   0 edihasaj   (501) staff       (20)       38 2023-06-25 13:30:55.921967 tuspyserver-1.3.1/setup.cfg
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1116 2023-06-25 13:30:52.000000 tuspyserver-1.3.1/setup.py
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:30:55.921341 tuspyserver-1.3.1/tuspyserver.egg-info/
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:30:55.000000 tuspyserver-1.3.1/tuspyserver.egg-info/PKG-INFO
+-rw-r--r--   0 edihasaj   (501) staff       (20)      261 2023-06-25 13:30:55.000000 tuspyserver-1.3.1/tuspyserver.egg-info/SOURCES.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)        1 2023-06-25 13:30:55.000000 tuspyserver-1.3.1/tuspyserver.egg-info/dependency_links.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)       51 2023-06-25 13:30:55.000000 tuspyserver-1.3.1/tuspyserver.egg-info/requires.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)       10 2023-06-25 13:30:55.000000 tuspyserver-1.3.1/tuspyserver.egg-info/top_level.txt
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:30:55.921660 tuspyserver-1.3.1/tusserver/
+-rw-r--r--   0 edihasaj   (501) staff       (20)       22 2023-06-25 12:40:59.000000 tuspyserver-1.3.1/tusserver/__init__.py
+-rw-r--r--   0 edihasaj   (501) staff       (20)      751 2023-06-25 13:29:48.000000 tuspyserver-1.3.1/tusserver/metadata.py
+-rw-r--r--   0 edihasaj   (501) staff       (20)    11358 2023-06-25 13:20:51.000000 tuspyserver-1.3.1/tusserver/tus.py
```

### Comparing `tuspyserver-1.3.0/LICENSE` & `tuspyserver-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuspyserver-1.3.0/PKG-INFO` & `tuspyserver-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuspyserver
-Version: 1.3.0
+Version: 1.3.1
 Summary: TUS py protocol implementation in FastAPI
 Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj
 Author-email: edihasaj@outlook.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.0 Summary: TUS py protocol
+Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.1 Summary: TUS py protocol
 implementation in FastAPI Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj Author-email: edihasaj@outlook.com License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown License-File: LICENSE # FastAPI Tus
```

### Comparing `tuspyserver-1.3.0/README.md` & `tuspyserver-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tuspyserver-1.3.0/setup.py` & `tuspyserver-1.3.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tuspyserver',
-    version='1.3.0',
+    version='1.3.1',
     description='TUS py protocol implementation in FastAPI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Edi Hasaj',
     license='MIT',
     author_email='edihasaj@outlook.com',
     url='https://github.com/edihasaj/tuspy-fast-api',
```

### Comparing `tuspyserver-1.3.0/tuspyserver.egg-info/PKG-INFO` & `tuspyserver-1.3.1/tuspyserver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuspyserver
-Version: 1.3.0
+Version: 1.3.1
 Summary: TUS py protocol implementation in FastAPI
 Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj
 Author-email: edihasaj@outlook.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.0 Summary: TUS py protocol
+Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.1 Summary: TUS py protocol
 implementation in FastAPI Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj Author-email: edihasaj@outlook.com License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown License-File: LICENSE # FastAPI Tus
```

### Comparing `tuspyserver-1.3.0/tusserver/metadata.py` & `tuspyserver-1.3.1/tusserver/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any
+from typing import Any, Hashable
 
 from pydantic import BaseModel
 
 
 class FileMetadata(BaseModel):
     uid: str
-    metadata: dict[Any, str]
+    metadata: dict[Hashable, str]
     size: int
     offset: int = 0
     upload_part: int = 0
     created_at: str
     defer_length: bool
     upload_chunk_size: int = 0
     expires: str | None
```

### Comparing `tuspyserver-1.3.0/tusserver/tus.py` & `tuspyserver-1.3.1/tusserver/tus.py`

 * *Files identical despite different names*

