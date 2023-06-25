# Comparing `tmp/jcci-0.0.1.tar.gz` & `tmp/jcci-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.1.tar", last modified: Sun Jun 25 09:40:59 2023, max compression
+gzip compressed data, was "jcci-0.0.2.tar", last modified: Sun Jun 25 10:12:33 2023, max compression
```

## Comparing `jcci-0.0.1.tar` & `jcci-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:40:59.175307 jcci-0.0.1/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:06:31.000000 jcci-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      902 2023-06-25 09:40:59.174311 jcci-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-06-25 09:39:40.000000 jcci-0.0.1/README.md
--rw-rw-rw-   0        0        0      625 2022-09-20 03:11:32.000000 jcci-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 09:40:59.175307 jcci-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 09:40:59.161306 jcci-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 09:40:59.167306 jcci-0.0.1/src/jcci/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:04:57.000000 jcci-0.0.1/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-25 09:25:01.000000 jcci-0.0.1/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    40580 2023-06-25 09:24:15.000000 jcci-0.0.1/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:40:59.172307 jcci-0.0.1/src/jcci.egg-info/
--rw-rw-rw-   0        0        0      902 2023-06-25 09:40:59.000000 jcci-0.0.1/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-25 09:40:59.000000 jcci-0.0.1/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 09:40:59.000000 jcci-0.0.1/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 09:40:59.000000 jcci-0.0.1/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 10:12:33.663928 jcci-0.0.2/
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:06:31.000000 jcci-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      900 2023-06-25 10:12:33.662927 jcci-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-06-25 09:39:40.000000 jcci-0.0.2/README.md
+-rw-rw-rw-   0        0        0      623 2023-06-25 10:11:16.000000 jcci-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 10:12:33.663928 jcci-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 10:12:33.649940 jcci-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 10:12:33.656928 jcci-0.0.2/src/jcci/
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:04:57.000000 jcci-0.0.2/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-06-25 09:25:01.000000 jcci-0.0.2/src/jcci/java_analyzer.py
+-rw-rw-rw-   0        0        0    40580 2023-06-25 09:24:15.000000 jcci-0.0.2/src/jcci/jcci.py
+drwxrwxrwx   0        0        0        0 2023-06-25 10:12:33.662927 jcci-0.0.2/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0      900 2023-06-25 10:12:33.000000 jcci-0.0.2/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-25 10:12:33.000000 jcci-0.0.2/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 10:12:33.000000 jcci-0.0.2/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 10:12:33.000000 jcci-0.0.2/src/jcci.egg-info/top_level.txt
```

### Comparing `jcci-0.0.1/PKG-INFO` & `jcci-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.1
+Version: 0.0.2
 Summary: Java code commit impact in pure Python
 Author-email: Quan Li <441640312@qq.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/baikaishuipp/jcci
+Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jcci-0.0.1/pyproject.toml` & `jcci-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Quan Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact in pure Python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://github.com/baikaishuipp/jcci"
+"Bug Tracker" = "https://github.com/baikaishuipp/jcci/issues"
```

### Comparing `jcci-0.0.1/src/jcci/java_analyzer.py` & `jcci-0.0.2/src/jcci/java_analyzer.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.1/src/jcci/jcci.py` & `jcci-0.0.2/src/jcci/jcci.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.1/src/jcci.egg-info/PKG-INFO` & `jcci-0.0.2/src/jcci.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.1
+Version: 0.0.2
 Summary: Java code commit impact in pure Python
 Author-email: Quan Li <441640312@qq.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/baikaishuipp/jcci
+Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

