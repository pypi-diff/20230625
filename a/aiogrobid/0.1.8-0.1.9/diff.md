# Comparing `tmp/aiogrobid-0.1.8.tar.gz` & `tmp/aiogrobid-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogrobid-0.1.8.tar", last modified: Mon Jun 12 18:03:33 2023, max compression
+gzip compressed data, was "aiogrobid-0.1.9.tar", last modified: Mon Jun 12 18:15:38 2023, max compression
```

## Comparing `aiogrobid-0.1.8.tar` & `aiogrobid-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.800284 aiogrobid-0.1.8/
--rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:03:33.800583 aiogrobid-0.1.8/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.796749 aiogrobid-0.1.8/aiogrobid/
--rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/aiogrobid/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      396 2023-05-29 06:48:15.000000 aiogrobid-0.1.8/aiogrobid/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     3765 2023-06-12 17:59:03.000000 aiogrobid-0.1.8/aiogrobid/client.py
--rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/aiogrobid/exceptions.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.799919 aiogrobid-0.1.8/aiogrobid.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      325 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       50 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       59 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      613 2023-06-12 18:03:33.801494 aiogrobid-0.1.8/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:15:38.676640 aiogrobid-0.1.9/
+-rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.9/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:15:38.676803 aiogrobid-0.1.9/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.9/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:15:38.672969 aiogrobid-0.1.9/aiogrobid/
+-rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.9/aiogrobid/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      397 2023-06-12 18:15:22.000000 aiogrobid-0.1.9/aiogrobid/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3766 2023-06-12 18:15:12.000000 aiogrobid-0.1.9/aiogrobid/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.9/aiogrobid/exceptions.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:15:38.676252 aiogrobid-0.1.9/aiogrobid.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      325 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       50 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       59 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-12 18:15:38.000000 aiogrobid-0.1.9/aiogrobid.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.9/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      613 2023-06-12 18:15:38.677594 aiogrobid-0.1.9/setup.cfg
```

### Comparing `aiogrobid-0.1.8/LICENSE` & `aiogrobid-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.8/PKG-INFO` & `aiogrobid-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.8/README.md` & `aiogrobid-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.8/aiogrobid/client.py` & `aiogrobid-0.1.9/aiogrobid/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from aiobaseclient import BaseClient
 from lxml import etree
 
-from exceptions import BadRequestError
+from .exceptions import BadRequestError
 
 
 class GrobidClient(BaseClient):
     def __init__(self, base_url):
         super().__init__(base_url=base_url)
 
     def _get_text_for_one(self, root, name):
```

### Comparing `aiogrobid-0.1.8/aiogrobid.egg-info/PKG-INFO` & `aiogrobid-0.1.9/aiogrobid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.8/setup.cfg` & `aiogrobid-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = 
 	Topic :: Utilities
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = aiogrobid
 python_requires = '>=3.8',
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/izihawa/aiogrobid
 
 [options]
 packages = find:
 install_requires = 
 	aiobaseclient >= 0.2.4
 	fire >= 0.3.1
```

