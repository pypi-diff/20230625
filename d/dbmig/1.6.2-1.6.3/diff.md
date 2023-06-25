# Comparing `tmp/dbmig-1.6.2.tar.gz` & `tmp/dbmig-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbmig-1.6.2.tar", last modified: Tue Mar 14 17:59:33 2023, max compression
+gzip compressed data, was "dist/dbmig-1.6.3.tar", last modified: Sun Jun 25 12:25:27 2023, max compression
```

## Comparing `dbmig-1.6.2.tar` & `dbmig-1.6.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxr-x   0 jdemoor   (1000) jdemoor   (1000)        0 2023-03-14 17:59:33.000000 dbmig-1.6.2/
-drwxrwxr-x   0 jdemoor   (1000) jdemoor   (1000)        0 2023-03-14 17:59:33.000000 dbmig-1.6.2/dbmig/
--rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)    14027 2023-03-14 17:59:24.000000 dbmig-1.6.2/dbmig/main.py
--rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      119 2023-02-28 08:14:01.000000 dbmig-1.6.2/dbmig/__init__.py
--rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      642 2023-03-14 17:59:33.000000 dbmig-1.6.2/PKG-INFO
--rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      861 2023-03-14 17:59:24.000000 dbmig-1.6.2/setup.py
+drwxrwxr-x   0 jdemoor   (1000) jdemoor   (1000)        0 2023-06-25 12:25:27.000000 dbmig-1.6.3/
+drwxrwxr-x   0 jdemoor   (1000) jdemoor   (1000)        0 2023-06-25 12:25:27.000000 dbmig-1.6.3/dbmig/
+-rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)    14027 2023-03-14 17:59:24.000000 dbmig-1.6.3/dbmig/main.py
+-rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      119 2023-02-28 08:14:01.000000 dbmig-1.6.3/dbmig/__init__.py
+-rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      642 2023-06-25 12:25:27.000000 dbmig-1.6.3/PKG-INFO
+-rw-rw-r--   0 jdemoor   (1000) jdemoor   (1000)      867 2023-06-25 12:25:22.000000 dbmig-1.6.3/setup.py
```

### Comparing `dbmig-1.6.2/dbmig/main.py` & `dbmig-1.6.3/dbmig/main.py`

 * *Files identical despite different names*

### Comparing `dbmig-1.6.2/PKG-INFO` & `dbmig-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dbmig
-Version: 1.6.2
+Version: 1.6.3
 Summary: Simple tool to run SQL migration scripts against an RDBMS. dbmig supports PosgreSQL and should be easy to adapt to any backend supported by SQLAlchemy.
 Home-page: https://bitbucket.org/msldev/dbmig/
 Author: Julien Demoor
 Author-email: julien@jdemoor.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dbmig-1.6.2/setup.py` & `dbmig-1.6.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from distutils.core import setup
 
 setup(
 	name = 'dbmig',
-	version='1.6.2',
+	version='1.6.3',
 	author = 'Julien Demoor',
 	author_email = 'julien@jdemoor.com',
         url = 'https://bitbucket.org/msldev/dbmig/',
 	license = 'MIT',
 	description = 'Simple tool to run SQL migration scripts against an RDBMS. dbmig supports PosgreSQL and should be easy to adapt to any backend supported by SQLAlchemy.',
 	packages = ['dbmig'],
 	entry_points = {
 		'console_scripts': [
 		    'dbmig = dbmig.main:main',
 		]
     },
 	install_requires = [
-		'SQLAlchemy',
+		'SQLAlchemy<2.0.0',
 	],
 	zip_safe = False,
 	include_package_data = True,
 	classifiers=[
 	    "License :: OSI Approved :: MIT License",
 	    "Programming Language :: Python :: 2",
 	    "Programming Language :: Python :: 2.7",
```

