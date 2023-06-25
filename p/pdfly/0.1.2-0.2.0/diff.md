# Comparing `tmp/pdfly-0.1.2.tar.gz` & `tmp/pdfly-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.1.2.tar", last modified: Thu Jun  8 14:12:38 2023, max compression
+gzip compressed data, was "pdfly-0.2.0.tar", last modified: Sun Jun 25 07:58:30 2023, max compression
```

## Comparing `pdfly-0.1.2.tar` & `pdfly-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/
--rw-rw-r--   0 moose     (1000) moose     (1000)     1514 2023-03-18 14:12:20.000000 pdfly-0.1.2/LICENSE
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-08 14:12:38.962738 pdfly-0.1.2/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)     3938 2023-03-19 13:01:13.000000 pdfly-0.1.2/README.md
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/pdfly/
--rw-rw-r--   0 moose     (1000) moose     (1000)      164 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/__init__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      114 2023-03-18 14:12:20.000000 pdfly-0.1.2/pdfly/__main__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       87 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/_utils.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       22 2023-06-08 14:12:35.000000 pdfly-0.1.2/pdfly/_version.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2765 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/cat.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2891 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/cli.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      594 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/compress.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      846 2023-06-08 14:12:26.000000 pdfly-0.1.2/pdfly/extract_images.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     6269 2023-06-08 14:12:26.000000 pdfly-0.1.2/pdfly/metadata.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2384 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/pagemeta.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      724 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/up2.py
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/pdfly.egg-info/
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)      414 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/SOURCES.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        1 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/dependency_links.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       49 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/entry_points.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       40 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/requires.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        6 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/top_level.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)     3627 2023-03-19 13:01:13.000000 pdfly-0.1.2/pyproject.toml
--rw-rw-r--   0 moose     (1000) moose     (1000)     1784 2023-06-08 14:12:38.962738 pdfly-0.1.2/setup.cfg
--rw-rw-r--   0 moose     (1000) moose     (1000)      463 2023-03-19 13:01:13.000000 pdfly-0.1.2/setup.py
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/
+-rw-rw-r--   0 moose     (1000) moose     (1000)     1514 2023-03-18 14:12:20.000000 pdfly-0.2.0/LICENSE
+-rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-25 07:58:30.675734 pdfly-0.2.0/PKG-INFO
+-rw-rw-r--   0 moose     (1000) moose     (1000)     3938 2023-03-19 13:01:13.000000 pdfly-0.2.0/README.md
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/pdfly/
+-rw-rw-r--   0 moose     (1000) moose     (1000)      164 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/__init__.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      114 2023-03-18 14:12:20.000000 pdfly-0.2.0/pdfly/__main__.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)       87 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/_utils.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)       22 2023-06-25 07:58:27.000000 pdfly-0.2.0/pdfly/_version.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     2765 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/cat.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     4409 2023-06-25 07:58:04.000000 pdfly-0.2.0/pdfly/cli.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      594 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/compress.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      846 2023-06-08 14:12:26.000000 pdfly-0.2.0/pdfly/extract_images.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     6269 2023-06-08 14:12:26.000000 pdfly-0.2.0/pdfly/metadata.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     2384 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/pagemeta.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      724 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/up2.py
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/pdfly.egg-info/
+-rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/PKG-INFO
+-rw-rw-r--   0 moose     (1000) moose     (1000)      414 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/SOURCES.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)        1 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/dependency_links.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)       49 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/entry_points.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)       47 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/requires.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)        6 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/top_level.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)     3627 2023-03-19 13:01:13.000000 pdfly-0.2.0/pyproject.toml
+-rw-rw-r--   0 moose     (1000) moose     (1000)     1791 2023-06-25 07:58:30.675734 pdfly-0.2.0/setup.cfg
+-rw-rw-r--   0 moose     (1000) moose     (1000)      463 2023-03-19 13:01:13.000000 pdfly-0.2.0/setup.py
```

### Comparing `pdfly-0.1.2/LICENSE` & `pdfly-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/PKG-INFO` & `pdfly-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.1.2
+Version: 0.2.0
 Summary: A pure-python CLI application to manipulate PDF files
 Home-page: https://github.com/py-pdf/pdfly
 Author: Martin Thoma
 Author-email: info@martin-thoma.de
 Maintainer: Martin Thoma
 Maintainer-email: info@martin-thoma.de
 License: BSD-3-Clause
```

### Comparing `pdfly-0.1.2/README.md` & `pdfly-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/cat.py` & `pdfly-0.2.0/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/compress.py` & `pdfly-0.2.0/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/extract_images.py` & `pdfly-0.2.0/pdfly/extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/metadata.py` & `pdfly-0.2.0/pdfly/metadata.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/pagemeta.py` & `pdfly-0.2.0/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly/up2.py` & `pdfly-0.2.0/pdfly/up2.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/pdfly.egg-info/PKG-INFO` & `pdfly-0.2.0/pdfly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.1.2
+Version: 0.2.0
 Summary: A pure-python CLI application to manipulate PDF files
 Home-page: https://github.com/py-pdf/pdfly
 Author: Martin Thoma
 Author-email: info@martin-thoma.de
 Maintainer: Martin Thoma
 Maintainer-email: info@martin-thoma.de
 License: BSD-3-Clause
```

### Comparing `pdfly-0.1.2/pyproject.toml` & `pdfly-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.2/setup.cfg` & `pdfly-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 python_requires = >=3.6.1
 install_requires = 
 	pypdf>=3.8.2
-	typer
+	typer>=0.9.0
 	pillow
 	pydantic
 	rich
 
 [options.entry_points]
 console_scripts = 
 	pdfly = pdfly.cli:entry_point
```

