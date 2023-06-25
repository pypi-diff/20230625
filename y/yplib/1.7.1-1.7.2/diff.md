# Comparing `tmp/yplib-1.7.1.tar.gz` & `tmp/yplib-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.1.tar", last modified: Sun Jun 25 07:46:56 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.2.tar", last modified: Sun Jun 25 07:54:54 2023, max compression
```

## Comparing `yplib-1.7.1.tar` & `yplib-1.7.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.383916 yplib-1.7.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 07:46:56.383857 yplib-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 07:46:56.383916 yplib-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 07:46:07.000000 yplib-1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.380982 yplib-1.7.1/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.7.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.1/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.382890 yplib-1.7.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 07:54:54.569821 yplib-1.7.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 07:54:54.569181 yplib-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:54:54.569821 yplib-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 07:54:51.000000 yplib-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:54:54.566472 yplib-1.7.2/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.7.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.2/yplib/index.py
+-rw-rw-rw-   0        0        0      316 2023-06-25 07:54:29.000000 yplib-1.7.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:54:54.568529 yplib-1.7.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 07:54:54.000000 yplib-1.7.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-25 07:54:54.000000 yplib-1.7.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:54:54.000000 yplib-1.7.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 07:54:54.000000 yplib-1.7.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.1/LICENSE` & `yplib-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.1/setup.py` & `yplib-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.1",
+  version="1.7.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.1/yplib/chart.py` & `yplib-1.7.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.1/yplib/chart_html.py` & `yplib-1.7.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.1/yplib/file.py` & `yplib-1.7.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.1/yplib/http_util.py` & `yplib-1.7.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.1/yplib/index.py` & `yplib-1.7.2/yplib/index.py`

 * *Files identical despite different names*

