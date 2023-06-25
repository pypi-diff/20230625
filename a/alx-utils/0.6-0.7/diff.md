# Comparing `tmp/alx-utils-0.6.tar.gz` & `tmp/alx-utils-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alx-utils-0.6.tar", last modified: Sat Jun 24 22:45:37 2023, max compression
+gzip compressed data, was "alx-utils-0.7.tar", last modified: Sun Jun 25 10:17:13 2023, max compression
```

## Comparing `alx-utils-0.6.tar` & `alx-utils-0.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.547699 alx-utils-0.6/
--rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.6/MANIFEST.in
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 22:45:37.546699 alx-utils-0.6/PKG-INFO
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.543699 alx-utils-0.6/alx_utils.egg-info/
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 22:45:36.000000 alx-utils-0.6/alx_utils.egg-info/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)      399 2023-06-24 22:45:37.000000 alx-utils-0.6/alx_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-24 22:45:36.000000 alx-utils-0.6/alx_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-24 22:45:36.000000 alx-utils-0.6/alx_utils.egg-info/entry_points.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-24 22:45:37.000000 alx-utils-0.6/alx_utils.egg-info/requires.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-24 22:45:37.000000 alx-utils-0.6/alx_utils.egg-info/top_level.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-24 22:45:37.547699 alx-utils-0.6/setup.cfg
--rw-r--r--   0 bio       (1000) bio       (1000)      525 2023-06-24 22:45:17.000000 alx-utils-0.6/setup.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.543699 alx-utils-0.6/src/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.6/src/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      534 2023-06-24 18:15:27.000000 alx-utils-0.6/src/alx_utils.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.544699 alx-utils-0.6/tools/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.6/tools/__init__.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.544699 alx-utils-0.6/tools/checker/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.6/tools/checker/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      577 2023-06-24 18:30:50.000000 alx-utils-0.6/tools/checker/index.py
--rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.6/tools/checker/test.bash
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 22:45:37.545699 alx-utils-0.6/tools/init_task/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.6/tools/init_task/__init__.py
--rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.6/tools/init_task/scraper.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.667721 alx-utils-0.7/
+-rw-r--r--   0 bio       (1000) bio       (1000)     1064 2023-06-25 09:05:59.000000 alx-utils-0.7/LICENSE
+-rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.7/MANIFEST.in
+-rw-r--r--   0 bio       (1000) bio       (1000)     1723 2023-06-25 10:17:13.667721 alx-utils-0.7/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)     1501 2023-06-25 09:57:04.000000 alx-utils-0.7/README.md
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.664721 alx-utils-0.7/alx_utils.egg-info/
+-rw-r--r--   0 bio       (1000) bio       (1000)     1723 2023-06-25 10:17:12.000000 alx-utils-0.7/alx_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)      417 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-25 10:17:12.000000 alx-utils-0.7/alx_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/entry_points.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/requires.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/top_level.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-25 10:17:13.668721 alx-utils-0.7/setup.cfg
+-rw-r--r--   0 bio       (1000) bio       (1000)      739 2023-06-25 10:16:58.000000 alx-utils-0.7/setup.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.665721 alx-utils-0.7/src/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.7/src/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      534 2023-06-24 18:15:27.000000 alx-utils-0.7/src/alx_utils.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.665721 alx-utils-0.7/tools/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.7/tools/__init__.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.666721 alx-utils-0.7/tools/checker/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.7/tools/checker/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      577 2023-06-24 18:30:50.000000 alx-utils-0.7/tools/checker/index.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.7/tools/checker/test.bash
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.666721 alx-utils-0.7/tools/init_task/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.7/tools/init_task/__init__.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.7/tools/init_task/scraper.py
```

### Comparing `alx-utils-0.6/src/alx_utils.py` & `alx-utils-0.7/src/alx_utils.py`

 * *Files identical despite different names*

### Comparing `alx-utils-0.6/tools/checker/index.py` & `alx-utils-0.7/tools/checker/index.py`

 * *Files identical despite different names*

### Comparing `alx-utils-0.6/tools/checker/test.bash` & `alx-utils-0.7/tools/checker/test.bash`

 * *Files identical despite different names*

### Comparing `alx-utils-0.6/tools/init_task/scraper.py` & `alx-utils-0.7/tools/init_task/scraper.py`

 * *Files identical despite different names*

