# Comparing `tmp/aissistant-0.0.1.tar.gz` & `tmp/aissistant-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissistant-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissistant-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissistant-0.0.1.tar` & `aissistant-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissistant-0.0.1/LICENSE
--rw-r--r--   0        0        0      198 2023-06-25 02:16:37.284114 aissistant-0.0.1/Pipfile
--rw-r--r--   0        0        0    41428 2023-06-25 02:35:33.773116 aissistant-0.0.1/Pipfile.lock
--rw-r--r--   0        0        0       12 2023-06-22 03:54:21.530635 aissistant-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissistant-0.0.1/aissistant/__init__.py
--rw-r--r--   0        0        0     3760 2023-06-24 04:15:37.054524 aissistant-0.0.1/aissistant/assistant.py
--rw-r--r--   0        0        0       22 2023-06-24 03:27:53.780926 aissistant-0.0.1/aissistant/version.py
--rw-r--r--   0        0        0      870 2023-06-25 02:21:44.761475 aissistant-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1158 2023-06-24 03:38:56.048390 aissistant-0.0.1/setup.cfg
--rw-r--r--   0        0        0      103 2023-06-24 03:39:36.847937 aissistant-0.0.1/setup.py
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 aissistant-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissistant-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissistant-0.0.2/LICENSE
+-rw-r--r--   0        0        0      198 2023-06-25 02:16:37.284114 aissistant-0.0.2/Pipfile
+-rw-r--r--   0        0        0    41428 2023-06-25 02:35:33.773116 aissistant-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0     1064 2023-06-25 02:48:46.081052 aissistant-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissistant-0.0.2/aissistant/__init__.py
+-rw-r--r--   0        0        0     3760 2023-06-24 04:15:37.054524 aissistant-0.0.2/aissistant/assistant.py
+-rw-r--r--   0        0        0       22 2023-06-25 02:51:11.940746 aissistant-0.0.2/aissistant/version.py
+-rw-r--r--   0        0        0      896 2023-06-25 02:51:19.292380 aissistant-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 aissistant-0.0.2/PKG-INFO
```

### Comparing `aissistant-0.0.1/LICENSE` & `aissistant-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aissistant-0.0.1/Pipfile.lock` & `aissistant-0.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aissistant-0.0.1/aissistant/assistant.py` & `aissistant-0.0.2/aissistant/assistant.py`

 * *Files identical despite different names*

### Comparing `aissistant-0.0.1/pyproject.toml` & `aissistant-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [project]
 name = "aissistant"
-version = "0.0.1"
+version = "0.0.2"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
+
 readme = "README.md"
+
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 
 requires-python = ">=3.7"
+
 dependencies = [
-  "requests<3",
+  "openai<0.28",
+  "prompt_toolkit<4",
   "pygments<3",
-  "openai<0.28"
+  "requests<3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/craigmbooth/aissistant"
 "Bug Tracker" = "https://github.com/craigmbooth/aissistant/issues"
 
 [build-system]
```

