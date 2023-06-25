# Comparing `tmp/logix-1.0.3.tar.gz` & `tmp/logix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logix-1.0.3.tar", last modified: Thu Jun 22 18:19:26 2023, max compression
+gzip compressed data, was "logix-1.0.4.tar", last modified: Sun Jun 25 07:57:15 2023, max compression
```

## Comparing `logix-1.0.3.tar` & `logix-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:19:26.107097 logix-1.0.3/
--rw-rw-rw-   0        0        0     1066 2023-06-22 15:13:24.000000 logix-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      558 2023-06-22 18:19:26.101174 logix-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-06-22 15:13:24.000000 logix-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 18:19:26.099549 logix-1.0.3/logix.egg-info/
--rw-rw-rw-   0        0        0      558 2023-06-22 18:19:25.000000 logix-1.0.3/logix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-06-22 18:19:25.000000 logix-1.0.3/logix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:19:25.000000 logix-1.0.3/logix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:19:25.000000 logix-1.0.3/logix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1671 2023-06-22 18:17:54.000000 logix-1.0.3/logix.py
--rw-rw-rw-   0        0        0       42 2023-06-22 18:19:26.107097 logix-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-06-22 18:19:06.000000 logix-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:57:14.989245 logix-1.0.4/
+-rw-rw-rw-   0        0        0     1066 2023-06-22 15:13:24.000000 logix-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      558 2023-06-25 07:57:14.987493 logix-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-06-22 15:13:24.000000 logix-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 07:57:14.977118 logix-1.0.4/logix.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-06-25 07:57:14.000000 logix-1.0.4/logix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-06-25 07:57:14.000000 logix-1.0.4/logix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:57:14.000000 logix-1.0.4/logix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:57:14.000000 logix-1.0.4/logix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1519 2023-06-25 07:56:02.000000 logix-1.0.4/logix.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:57:14.989245 logix-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-06-25 07:55:58.000000 logix-1.0.4/setup.py
```

### Comparing `logix-1.0.3/LICENSE` & `logix-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logix-1.0.3/PKG-INFO` & `logix-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logix
-Version: 1.0.3
+Version: 1.0.4
 Summary: A lightweight logging utility library
 Author: Шахзодбек
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `logix-1.0.3/README.md` & `logix-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `logix-1.0.3/logix.egg-info/PKG-INFO` & `logix-1.0.4/logix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logix
-Version: 1.0.3
+Version: 1.0.4
 Summary: A lightweight logging utility library
 Author: Шахзодбек
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `logix-1.0.3/setup.py` & `logix-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='logix',
-    version='1.0.3',
+    version='1.0.4',
     author='Шахзодбек',
     description='A lightweight logging utility library',
     packages=[''],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

