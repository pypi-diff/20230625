# Comparing `tmp/perke-0.4.3.tar.gz` & `tmp/perke-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perke-0.4.3.tar", last modified: Sat Jun 24 10:09:01 2023, max compression
+gzip compressed data, was "perke-0.4.4.tar", last modified: Sun Jun 25 09:51:48 2023, max compression
```

## Comparing `perke-0.4.3.tar` & `perke-0.4.4.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-24 10:08:27.000000 perke-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 10:08:27.000000 perke-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-24 10:09:01.285089 perke-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-24 10:08:27.000000 perke-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.281088 perke-0.4.3/perke/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 10:08:27.000000 perke-0.4.3/perke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 10:08:27.000000 perke-0.4.3/perke/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.281088 perke-0.4.3/perke/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:08:27.000000 perke-0.4.3/perke/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-24 10:08:27.000000 perke-0.4.3/perke/base/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-06-24 10:08:27.000000 perke-0.4.3/perke/base/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-24 10:08:27.000000 perke-0.4.3/perke/base/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-24 10:08:27.000000 perke-0.4.3/perke/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/perke/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-24 10:08:27.000000 perke-0.4.3/perke/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-24 10:08:27.000000 perke-0.4.3/perke/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-24 10:08:27.000000 perke-0.4.3/perke/cli/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-24 10:08:27.000000 perke-0.4.3/perke/cli/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/perke/unsupervised/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/perke/unsupervised/graph_based/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/multipartite_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/position_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/single_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/text_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-24 10:08:27.000000 perke-0.4.3/perke/unsupervised/graph_based/topic_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/perke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:08:27.000000 perke-0.4.3/perke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-24 10:08:27.000000 perke-0.4.3/perke/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-24 10:08:27.000000 perke-0.4.3/perke/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 10:08:51.000000 perke-0.4.3/perke/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.281088 perke-0.4.3/perke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 10:09:01.000000 perke-0.4.3/perke.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:09:01.285089 perke-0.4.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 10:08:27.000000 perke-0.4.3/requirements/develop.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 10:08:27.000000 perke-0.4.3/requirements/documentation.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-24 10:08:27.000000 perke-0.4.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 10:08:27.000000 perke-0.4.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:09:01.285089 perke-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-24 10:08:27.000000 perke-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.208378 perke-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-25 09:51:15.000000 perke-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 09:51:15.000000 perke-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-25 09:51:48.208378 perke-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-25 09:51:15.000000 perke-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-25 09:51:15.000000 perke-0.4.4/perke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 09:51:15.000000 perke-0.4.4/perke/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:15.000000 perke-0.4.4/perke/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-25 09:51:15.000000 perke-0.4.4/perke/base/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-06-25 09:51:15.000000 perke-0.4.4/perke/base/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-25 09:51:15.000000 perke-0.4.4/perke/base/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-25 09:51:15.000000 perke-0.4.4/perke/base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-25 09:51:15.000000 perke-0.4.4/perke/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-25 09:51:15.000000 perke-0.4.4/perke/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-25 09:51:15.000000 perke-0.4.4/perke/cli/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-25 09:51:15.000000 perke-0.4.4/perke/cli/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 09:51:15.000000 perke-0.4.4/perke/resources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke/unsupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.208378 perke-0.4.4/perke/unsupervised/graph_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/multipartite_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/position_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/single_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/text_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-25 09:51:15.000000 perke-0.4.4/perke/unsupervised/graph_based/topic_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.208378 perke-0.4.4/perke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:15.000000 perke-0.4.4/perke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 09:51:15.000000 perke-0.4.4/perke/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-25 09:51:15.000000 perke-0.4.4/perke/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 09:51:38.000000 perke-0.4.4/perke/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.204378 perke-0.4.4/perke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 09:51:48.000000 perke-0.4.4/perke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:51:48.208378 perke-0.4.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 09:51:15.000000 perke-0.4.4/requirements/develop.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 09:51:15.000000 perke-0.4.4/requirements/documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-25 09:51:15.000000 perke-0.4.4/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 09:51:15.000000 perke-0.4.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:51:48.208378 perke-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-25 09:51:15.000000 perke-0.4.4/setup.py
```

### Comparing `perke-0.4.3/LICENSE` & `perke-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/PKG-INFO` & `perke-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perke
-Version: 0.4.3
+Version: 0.4.4
 Summary: A keyphrase extractor for Persian
 Home-page: https://github.com/alirezatheh/perke
 Author: Alireza Hosseini
 Author-email: alirezatheh@gmail.com
 Project-URL: Bug Tracker, https://github.com/alirezatheh/perke/issues
 Project-URL: Documentation, https://perke.readthedocs.io
 Project-URL: Source Code, https://github.com/alirezatheh/perke
```

### Comparing `perke-0.4.3/README.md` & `perke-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/base/data_structures.py` & `perke-0.4.4/perke/base/data_structures.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/base/extractor.py` & `perke-0.4.4/perke/base/extractor.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/base/readers.py` & `perke-0.4.4/perke/base/readers.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/cli/base.py` & `perke-0.4.4/perke/cli/base.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/cli/clear.py` & `perke-0.4.4/perke/cli/clear.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/cli/download.py` & `perke-0.4.4/perke/cli/download.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/__init__.py` & `perke-0.4.4/perke/unsupervised/graph_based/__init__.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/multipartite_rank.py` & `perke-0.4.4/perke/unsupervised/graph_based/multipartite_rank.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/position_rank.py` & `perke-0.4.4/perke/unsupervised/graph_based/position_rank.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/single_rank.py` & `perke-0.4.4/perke/unsupervised/graph_based/single_rank.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/text_rank.py` & `perke-0.4.4/perke/unsupervised/graph_based/text_rank.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/unsupervised/graph_based/topic_rank.py` & `perke-0.4.4/perke/unsupervised/graph_based/topic_rank.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke/utils/functions.py` & `perke-0.4.4/perke/utils/functions.py`

 * *Files identical despite different names*

### Comparing `perke-0.4.3/perke.egg-info/PKG-INFO` & `perke-0.4.4/perke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perke
-Version: 0.4.3
+Version: 0.4.4
 Summary: A keyphrase extractor for Persian
 Home-page: https://github.com/alirezatheh/perke
 Author: Alireza Hosseini
 Author-email: alirezatheh@gmail.com
 Project-URL: Bug Tracker, https://github.com/alirezatheh/perke/issues
 Project-URL: Documentation, https://perke.readthedocs.io
 Project-URL: Source Code, https://github.com/alirezatheh/perke
```

### Comparing `perke-0.4.3/perke.egg-info/SOURCES.txt` & `perke-0.4.4/perke.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 perke/base/extractor.py
 perke/base/readers.py
 perke/base/types.py
 perke/cli/__init__.py
 perke/cli/base.py
 perke/cli/clear.py
 perke/cli/download.py
+perke/resources/README.md
 perke/unsupervised/__init__.py
 perke/unsupervised/graph_based/__init__.py
 perke/unsupervised/graph_based/multipartite_rank.py
 perke/unsupervised/graph_based/position_rank.py
 perke/unsupervised/graph_based/single_rank.py
 perke/unsupervised/graph_based/text_rank.py
 perke/unsupervised/graph_based/topic_rank.py
```

### Comparing `perke-0.4.3/setup.py` & `perke-0.4.4/setup.py`

 * *Files identical despite different names*

