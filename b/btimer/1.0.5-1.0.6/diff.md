# Comparing `tmp/btimer-1.0.5.tar.gz` & `tmp/btimer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btimer-1.0.5.tar", last modified: Sun Jun 25 12:24:26 2023, max compression
+gzip compressed data, was "btimer-1.0.6.tar", last modified: Sun Jun 25 13:39:37 2023, max compression
```

## Comparing `btimer-1.0.5.tar` & `btimer-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:24:26.765778 btimer-1.0.5/
--rw-r--r--   0 dylan      (501) staff       (20)     1075 2023-06-25 03:17:01.000000 btimer-1.0.5/LICENSE.txt
--rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:24:26.765667 btimer-1.0.5/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      658 2023-06-25 11:59:20.000000 btimer-1.0.5/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 12:24:26.765532 btimer-1.0.5/btimer.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1168 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      227 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (501) staff       (20)       13 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        6 2023-06-25 12:24:26.000000 btimer-1.0.5/btimer.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)      641 2023-06-25 12:24:21.000000 btimer-1.0.5/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 12:24:26.765817 btimer-1.0.5/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1508 2023-06-25 11:53:46.000000 btimer-1.0.5/timer.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 13:39:37.856128 btimer-1.0.6/
+-rw-r--r--   0 dylan      (501) staff       (20)     1075 2023-06-25 03:17:01.000000 btimer-1.0.6/LICENSE.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     1240 2023-06-25 13:39:37.856013 btimer-1.0.6/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      730 2023-06-25 13:37:38.000000 btimer-1.0.6/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 13:39:37.855874 btimer-1.0.6/btimer.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1240 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      227 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       13 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        6 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      641 2023-06-25 13:38:33.000000 btimer-1.0.6/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 13:39:37.856164 btimer-1.0.6/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1508 2023-06-25 11:53:46.000000 btimer-1.0.6/timer.py
```

### Comparing `btimer-1.0.5/LICENSE.txt` & `btimer-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btimer-1.0.5/PKG-INFO` & `btimer-1.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.5
+Version: 1.0.6
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Buddhist Timer
 Timer tool help people get away from the computer.
 
+[BTimer documentation in the https://pypi.org](https://pypi.org/project/btimer/)
+
 ## How to set up?
 ```bash
 # Make sure your computer installed python3 and pip3
 
 pip install btimer
+
+#or
+
+pip3 install btimer
 ```
 
 ## How to use?
 ```bash
 # Open a new command line
 
 btimer
 
 # Enter number of minutes
 ```
 
-![BTimer](https://github.com/dylanngo95/timer/blob/e7fa05a90b6f27e5590ae389f0aaf4e43bd70156/doc/img01.png?raw=true)
+![BTimer](https://github.com/dylanngo95/timer/blob/main/doc/img01.png?raw=true)
 
 ## How to build?
 
 ```bash
 # setup env
 python -m venv env
 source ./env/bin/activate
```

### Comparing `btimer-1.0.5/README.md` & `btimer-1.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # Buddhist Timer
 Timer tool help people get away from the computer.
 
+[BTimer documentation in the https://pypi.org](https://pypi.org/project/btimer/)
+
 ## How to set up?
 ```bash
 # Make sure your computer installed python3 and pip3
 
 pip install btimer
+
+#or
+
+pip3 install btimer
 ```
 
 ## How to use?
 ```bash
 # Open a new command line
 
 btimer
 
 # Enter number of minutes
 ```
 
-![BTimer](https://github.com/dylanngo95/timer/blob/e7fa05a90b6f27e5590ae389f0aaf4e43bd70156/doc/img01.png?raw=true)
+![BTimer](https://github.com/dylanngo95/timer/blob/main/doc/img01.png?raw=true)
 
 ## How to build?
 
 ```bash
 # setup env
 python -m venv env
 source ./env/bin/activate
```

### Comparing `btimer-1.0.5/btimer.egg-info/PKG-INFO` & `btimer-1.0.6/btimer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.5
+Version: 1.0.6
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Buddhist Timer
 Timer tool help people get away from the computer.
 
+[BTimer documentation in the https://pypi.org](https://pypi.org/project/btimer/)
+
 ## How to set up?
 ```bash
 # Make sure your computer installed python3 and pip3
 
 pip install btimer
+
+#or
+
+pip3 install btimer
 ```
 
 ## How to use?
 ```bash
 # Open a new command line
 
 btimer
 
 # Enter number of minutes
 ```
 
-![BTimer](https://github.com/dylanngo95/timer/blob/e7fa05a90b6f27e5590ae389f0aaf4e43bd70156/doc/img01.png?raw=true)
+![BTimer](https://github.com/dylanngo95/timer/blob/main/doc/img01.png?raw=true)
 
 ## How to build?
 
 ```bash
 # setup env
 python -m venv env
 source ./env/bin/activate
```

### Comparing `btimer-1.0.5/pyproject.toml` & `btimer-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btimer"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Dylan Ngo", email="it.tinhngo@gmail.com" },
 ]
 description = "Help people get away from the computer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `btimer-1.0.5/timer.py` & `btimer-1.0.6/timer.py`

 * *Files identical despite different names*

