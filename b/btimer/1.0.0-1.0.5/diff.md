# Comparing `tmp/btimer-1.0.0.tar.gz` & `tmp/btimer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btimer-1.0.0.tar", last modified: Sun Jun 25 12:31:43 2023, max compression
+gzip compressed data, was "btimer-1.0.5.tar", last modified: Sun Jun 25 12:24:26 2023, max compression
```

## Comparing `btimer-1.0.0.tar` & `btimer-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:31:43.457056 btimer-1.0.0/
--rw-r--r--   0 dylan      (501) staff       (20)     1075 2023-06-25 03:17:01.000000 btimer-1.0.0/LICENSE.txt
--rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:31:43.456953 btimer-1.0.0/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      658 2023-06-25 11:59:20.000000 btimer-1.0.0/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:31:43.456826 btimer-1.0.0/btimer.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      227 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (501) staff       (20)       13 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        6 2023-06-25 12:31:43.000000 btimer-1.0.0/btimer.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)      641 2023-06-25 12:31:32.000000 btimer-1.0.0/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:31:43.457089 btimer-1.0.0/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1508 2023-06-25 11:53:46.000000 btimer-1.0.0/timer.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:24:26.765778 btimer-1.0.5/
+-rw-r--r--   0 dylan      (501) staff       (20)     1075 2023-06-25 03:17:01.000000 btimer-1.0.5/LICENSE.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:24:26.765667 btimer-1.0.5/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      658 2023-06-25 11:59:20.000000 btimer-1.0.5/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:24:26.765532 btimer-1.0.5/btimer.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      227 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       13 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        6 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      641 2023-06-25 12:24:21.000000 btimer-1.0.5/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:24:26.765817 btimer-1.0.5/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1508 2023-06-25 11:53:46.000000 btimer-1.0.5/timer.py
```

### Comparing `btimer-1.0.0/LICENSE.txt` & `btimer-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btimer-1.0.0/PKG-INFO` & `btimer-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.0
+Version: 1.0.5
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.0/README.md` & `btimer-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `btimer-1.0.0/btimer.egg-info/PKG-INFO` & `btimer-1.0.5/btimer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.0
+Version: 1.0.5
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.0/pyproject.toml` & `btimer-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btimer"
-version = "1.0.0"
+version = "1.0.5"
 authors = [
   { name="Dylan Ngo", email="it.tinhngo@gmail.com" },
 ]
 description = "Help people get away from the computer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `btimer-1.0.0/timer.py` & `btimer-1.0.5/timer.py`

 * *Files identical despite different names*

