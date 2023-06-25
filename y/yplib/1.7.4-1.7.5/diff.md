# Comparing `tmp/yplib-1.7.4.tar.gz` & `tmp/yplib-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.4.tar", last modified: Sun Jun 25 08:07:21 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.5.tar", last modified: Sun Jun 25 08:09:42 2023, max compression
```

## Comparing `yplib-1.7.4.tar` & `yplib-1.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:07:21.327007 yplib-1.7.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 08:07:21.326504 yplib-1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 08:07:21.327007 yplib-1.7.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 08:07:17.000000 yplib-1.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:07:21.323927 yplib-1.7.4/yplib/
--rw-rw-rw-   0        0        0      411 2023-06-25 07:55:58.000000 yplib-1.7.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.4/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.4/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.4/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:07:21.326264 yplib-1.7.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 08:07:21.000000 yplib-1.7.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-25 08:07:21.000000 yplib-1.7.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:07:21.000000 yplib-1.7.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 08:07:21.000000 yplib-1.7.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.342840 yplib-1.7.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:09:42.342662 yplib-1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:09:42.343290 yplib-1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 08:09:25.000000 yplib-1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.339069 yplib-1.7.5/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.5/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.5/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.5/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.341588 yplib-1.7.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.4/LICENSE` & `yplib-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/setup.py` & `yplib-1.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.4",
+  version="1.7.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.4/yplib/chart.py` & `yplib-1.7.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/yplib/chart_html.py` & `yplib-1.7.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/yplib/db.py` & `yplib-1.7.5/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/yplib/file.py` & `yplib-1.7.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/yplib/http_util.py` & `yplib-1.7.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.4/yplib/index.py` & `yplib-1.7.5/yplib/index.py`

 * *Files identical despite different names*

