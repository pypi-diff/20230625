# Comparing `tmp/JukeAudio-0.0.2.tar.gz` & `tmp/JukeAudio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JukeAudio-0.0.2.tar", last modified: Sun Jun 25 17:45:41 2023, max compression
+gzip compressed data, was "JukeAudio-0.0.3.tar", last modified: Sun Jun 25 18:07:51 2023, max compression
```

## Comparing `JukeAudio-0.0.2.tar` & `JukeAudio-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:41.678368 JukeAudio-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 17:45:31.000000 JukeAudio-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 17:45:41.678368 JukeAudio-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-25 17:45:31.000000 JukeAudio-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:45:41.678368 JukeAudio-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:41.674368 JukeAudio-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:41.678368 JukeAudio-0.0.2/src/JukeAudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 17:45:41.000000 JukeAudio-0.0.2/src/JukeAudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-25 17:45:41.000000 JukeAudio-0.0.2/src/JukeAudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:45:41.000000 JukeAudio-0.0.2/src/JukeAudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-25 17:45:41.000000 JukeAudio-0.0.2/src/JukeAudio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:41.678368 JukeAudio-0.0.2/src/jukeaudio/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 17:45:31.000000 JukeAudio-0.0.2/src/jukeaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 17:45:31.000000 JukeAudio-0.0.2/src/jukeaudio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-25 17:45:31.000000 JukeAudio-0.0.2/src/jukeaudio/jukeaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:07:51.206884 JukeAudio-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-25 18:07:51.206884 JukeAudio-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:07:51.206884 JukeAudio-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:07:51.202884 JukeAudio-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:07:51.202884 JukeAudio-0.0.3/src/JukeAudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-25 18:07:51.000000 JukeAudio-0.0.3/src/JukeAudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-25 18:07:51.000000 JukeAudio-0.0.3/src/JukeAudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:07:51.000000 JukeAudio-0.0.3/src/JukeAudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-25 18:07:51.000000 JukeAudio-0.0.3/src/JukeAudio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:07:51.206884 JukeAudio-0.0.3/src/jukeaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/src/jukeaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/src/jukeaudio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-25 18:07:41.000000 JukeAudio-0.0.3/src/jukeaudio/jukeaudio.py
```

### Comparing `JukeAudio-0.0.2/LICENSE` & `JukeAudio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JukeAudio-0.0.2/pyproject.toml` & `JukeAudio-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JukeAudio"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Paul Karimov", email="paul_karimov@outlook.com" },
 ]
 description = "Python client for the JukeAudio API"
-readme = "README.md"
+readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `JukeAudio-0.0.2/src/jukeaudio/jukeaudio.py` & `JukeAudio-0.0.3/src/jukeaudio/jukeaudio.py`

 * *Files identical despite different names*

