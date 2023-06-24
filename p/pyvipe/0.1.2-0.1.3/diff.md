# Comparing `tmp/pyvipe-0.1.2.tar.gz` & `tmp/pyvipe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvipe-0.1.2.tar", last modified: Sat Jun 24 21:15:16 2023, max compression
+gzip compressed data, was "pyvipe-0.1.3.tar", last modified: Sat Jun 24 21:58:03 2023, max compression
```

## Comparing `pyvipe-0.1.2.tar` & `pyvipe-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.796939 pyvipe-0.1.2/
--rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.1.2/LICENSE
--rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:15:16.796370 pyvipe-0.1.2/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      955 2023-06-24 20:24:36.000000 pyvipe-0.1.2/README.md
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.787878 pyvipe-0.1.2/completion/
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.790266 pyvipe-0.1.2/completion/bash/
--rw-r--r--   0 constantinhong   (501) staff       (20)      243 2023-06-24 20:31:10.000000 pyvipe-0.1.2/completion/bash/pyvipe
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.791051 pyvipe-0.1.2/completion/zsh/
--rw-r--r--   0 constantinhong   (501) staff       (20)      311 2023-06-24 11:30:47.000000 pyvipe-0.1.2/completion/zsh/_pyvipe
--rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-06-24 20:49:12.000000 pyvipe-0.1.2/pyproject.toml
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.792532 pyvipe-0.1.2/pyvipe/
--rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-23 20:03:21.000000 pyvipe-0.1.2/pyvipe/__init__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.1.2/pyvipe/__main__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     2556 2023-06-24 20:49:12.000000 pyvipe-0.1.2/pyvipe/pyvipe.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:15:16.795435 pyvipe-0.1.2/pyvipe.egg-info/
--rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:15:16.000000 pyvipe-0.1.2/pyvipe.egg-info/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      295 2023-06-24 21:15:16.000000 pyvipe-0.1.2/pyvipe.egg-info/SOURCES.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-24 21:15:16.000000 pyvipe-0.1.2/pyvipe.egg-info/dependency_links.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-06-24 21:15:16.000000 pyvipe-0.1.2/pyvipe.egg-info/entry_points.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-06-24 21:15:16.000000 pyvipe-0.1.2/pyvipe.egg-info/top_level.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-24 21:15:16.797085 pyvipe-0.1.2/setup.cfg
--rw-r--r--   0 constantinhong   (501) staff       (20)     1460 2023-06-24 20:49:12.000000 pyvipe-0.1.2/setup.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.029747 pyvipe-0.1.3/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.1.3/LICENSE
+-rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:58:03.029345 pyvipe-0.1.3/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      955 2023-06-24 20:24:36.000000 pyvipe-0.1.3/README.md
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.021132 pyvipe-0.1.3/completion/
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.024185 pyvipe-0.1.3/completion/bash/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      243 2023-06-24 21:19:54.000000 pyvipe-0.1.3/completion/bash/vipe
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.024733 pyvipe-0.1.3/completion/zsh/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      310 2023-06-24 21:25:34.000000 pyvipe-0.1.3/completion/zsh/_vipe
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-06-24 21:54:08.000000 pyvipe-0.1.3/pyproject.toml
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.025905 pyvipe-0.1.3/pyvipe/
+-rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-23 20:03:21.000000 pyvipe-0.1.3/pyvipe/__init__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.1.3/pyvipe/__main__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     2556 2023-06-24 21:51:29.000000 pyvipe-0.1.3/pyvipe/pyvipe.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.028756 pyvipe-0.1.3/pyvipe.egg-info/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      291 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/SOURCES.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/dependency_links.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/entry_points.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/top_level.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-24 21:58:03.029843 pyvipe-0.1.3/setup.cfg
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1456 2023-06-24 21:54:17.000000 pyvipe-0.1.3/setup.py
```

### Comparing `pyvipe-0.1.2/LICENSE` & `pyvipe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvipe-0.1.2/PKG-INFO` & `pyvipe-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.1.2
+Version: 0.1.3
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
```

### Comparing `pyvipe-0.1.2/README.md` & `pyvipe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyvipe-0.1.2/pyproject.toml` & `pyvipe-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyvipe"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 maintainers = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 license = {file = "LICENSE"}
```

### Comparing `pyvipe-0.1.2/pyvipe/pyvipe.py` & `pyvipe-0.1.3/pyvipe/pyvipe.py`

 * *Files identical despite different names*

### Comparing `pyvipe-0.1.2/pyvipe.egg-info/PKG-INFO` & `pyvipe-0.1.3/pyvipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.1.2
+Version: 0.1.3
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
```

### Comparing `pyvipe-0.1.2/setup.py` & `pyvipe-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name = 'pyvipe',
-    version = '0.1.2',
+    version = '0.1.3',
     description='edit pipe with your editor.',
     author='Constantin Hong',
     author_email='hongconstantin@gmail.com',
     url='https://github.com/Constantin1489/pyvipe',
     maintainer='Constantin Hong',
     maintainer_email='hongconstantin@gmail.com',
     readme = "README.md",
     packages = ['pyvipe'],
     data_files = [
-        ('share/bash-completion/completions', ['completion/bash/pyvipe']),
-        ('share/zsh/site-functions', ['completion/zsh/_pyvipe'])
+        ('share/bash-completion/completions', ['completion/bash/vipe']),
+        ('share/zsh/site-functions', ['completion/zsh/_vipe'])
         ],
     python_requires='>=3.9',
     project_urls = {
         'Documentation': 'https://github.com/Constantin1489/pyvipe#readme',
         'Source': 'https://github.com/Constantin1489/pyvipe',
         'Tracker': 'https://github.com/Constantin1489/pyvipe/issues',
         },
```

