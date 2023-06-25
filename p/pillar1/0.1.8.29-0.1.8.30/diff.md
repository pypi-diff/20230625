# Comparing `tmp/pillar1-0.1.8.29.tar.gz` & `tmp/pillar1-0.1.8.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.29.tar", last modified: Sun Jun 25 00:33:48 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.30.tar", last modified: Sun Jun 25 00:35:55 2023, max compression
```

## Comparing `pillar1-0.1.8.29.tar` & `pillar1-0.1.8.30.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:33:48.140119 pillar1-0.1.8.29/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:33:48.139972 pillar1-0.1.8.29/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.29/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:33:48.139073 pillar1-0.1.8.29/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.29/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.29/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.29/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5456 2023-06-25 00:33:46.000000 pillar1-0.1.8.29/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:33:48.139744 pillar1-0.1.8.29/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:33:48.000000 pillar1-0.1.8.29/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:33:48.000000 pillar1-0.1.8.29/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:33:48.000000 pillar1-0.1.8.29/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:33:48.000000 pillar1-0.1.8.29/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:33:48.140160 pillar1-0.1.8.29/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:33:47.000000 pillar1-0.1.8.29/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:35:55.228352 pillar1-0.1.8.30/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:35:55.228228 pillar1-0.1.8.30/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.30/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:35:55.227479 pillar1-0.1.8.30/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.30/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      815 2023-06-25 00:35:52.000000 pillar1-0.1.8.30/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.30/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     5456 2023-06-25 00:33:46.000000 pillar1-0.1.8.30/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:35:55.228052 pillar1-0.1.8.30/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:35:55.000000 pillar1-0.1.8.30/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:35:55.000000 pillar1-0.1.8.30/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:35:55.000000 pillar1-0.1.8.30/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:35:55.000000 pillar1-0.1.8.30/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:35:55.228391 pillar1-0.1.8.30/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:35:54.000000 pillar1-0.1.8.30/setup.py
```

### Comparing `pillar1-0.1.8.29/PKG-INFO` & `pillar1-0.1.8.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.29
+Version: 0.1.8.30
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.29/README.md` & `pillar1-0.1.8.30/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.29/pillar1/constants_original.py` & `pillar1-0.1.8.30/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.29/pillar1/pillar1.py` & `pillar1-0.1.8.30/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.29/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.30/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.29
+Version: 0.1.8.30
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.29/setup.py` & `pillar1-0.1.8.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.29',
+    version='0.1.8.30',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

