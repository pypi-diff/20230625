# Comparing `tmp/yplib-1.7.7.tar.gz` & `tmp/yplib-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.7.tar", last modified: Sun Jun 25 08:44:58 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.8.tar", last modified: Sun Jun 25 08:50:42 2023, max compression
```

## Comparing `yplib-1.7.7.tar` & `yplib-1.7.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:44:58.226581 yplib-1.7.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 08:44:58.225218 yplib-1.7.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 08:44:58.226646 yplib-1.7.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 08:44:39.000000 yplib-1.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:44:58.222833 yplib-1.7.7/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    11634 2023-06-25 08:43:58.000000 yplib-1.7.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8270 2023-06-25 08:40:25.000000 yplib-1.7.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.7/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.7/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.7/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:44:58.225218 yplib-1.7.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 08:44:58.000000 yplib-1.7.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-25 08:44:58.000000 yplib-1.7.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:44:58.000000 yplib-1.7.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 08:44:58.000000 yplib-1.7.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.423374 yplib-1.7.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:50:42.423268 yplib-1.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:50:42.423958 yplib-1.7.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 08:48:36.000000 yplib-1.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.420274 yplib-1.7.8/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11634 2023-06-25 08:49:38.000000 yplib-1.7.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8270 2023-06-25 08:40:25.000000 yplib-1.7.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.8/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.8/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.8/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.422643 yplib-1.7.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.7/LICENSE` & `yplib-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/setup.py` & `yplib-1.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.7",
+  version="1.7.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.7/yplib/chart.py` & `yplib-1.7.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/yplib/chart_html.py` & `yplib-1.7.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/yplib/db.py` & `yplib-1.7.8/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/yplib/file.py` & `yplib-1.7.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/yplib/http_util.py` & `yplib-1.7.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.7/yplib/index.py` & `yplib-1.7.8/yplib/index.py`

 * *Files identical despite different names*

