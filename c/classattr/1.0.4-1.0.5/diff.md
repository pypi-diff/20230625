# Comparing `tmp/classattr-1.0.4.tar.gz` & `tmp/classattr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classattr-1.0.4.tar", last modified: Sun Jun 18 18:16:48 2023, max compression
+gzip compressed data, was "classattr-1.0.5.tar", last modified: Sun Jun 25 12:52:13 2023, max compression
```

## Comparing `classattr-1.0.4.tar` & `classattr-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.4/LICENSE
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:16:48.164215 classattr-1.0.4/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2345 2023-06-18 17:53:49.000000 classattr-1.0.4/README.md
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/classattr/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      107 2023-06-18 18:15:18.000000 classattr-1.0.4/classattr/__init__.py
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     8240 2023-06-18 18:03:56.000000 classattr-1.0.4/classattr/classattr.py
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/classattr.egg-info/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      203 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       10 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/top_level.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 18:16:48.168216 classattr-1.0.4/setup.cfg
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      609 2023-06-18 18:14:44.000000 classattr-1.0.4/setup.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-25 12:52:13.376558 classattr-1.0.5/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.5/LICENSE
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     3464 2023-06-25 12:52:13.376558 classattr-1.0.5/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     3054 2023-06-25 11:44:08.000000 classattr-1.0.5/README.md
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-25 12:52:13.376558 classattr-1.0.5/classattr/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      107 2023-06-25 12:48:44.000000 classattr-1.0.5/classattr/__init__.py
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     8240 2023-06-18 18:03:56.000000 classattr-1.0.5/classattr/classattr.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-25 12:52:13.376558 classattr-1.0.5/classattr.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     3464 2023-06-25 12:52:13.000000 classattr-1.0.5/classattr.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      203 2023-06-25 12:52:13.000000 classattr-1.0.5/classattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-25 12:52:13.000000 classattr-1.0.5/classattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       10 2023-06-25 12:52:13.000000 classattr-1.0.5/classattr.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-25 12:52:13.376558 classattr-1.0.5/setup.cfg
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      609 2023-06-18 18:14:44.000000 classattr-1.0.5/setup.py
```

### Comparing `classattr-1.0.4/LICENSE` & `classattr-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `classattr-1.0.4/classattr/classattr.py` & `classattr-1.0.5/classattr/classattr.py`

 * *Files identical despite different names*

### Comparing `classattr-1.0.4/setup.py` & `classattr-1.0.5/setup.py`

 * *Files identical despite different names*

