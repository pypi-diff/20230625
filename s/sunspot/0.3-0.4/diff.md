# Comparing `tmp/sunspot-0.3.tar.gz` & `tmp/sunspot-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunspot-0.3.tar", last modified: Sun Jun 25 15:03:58 2023, max compression
+gzip compressed data, was "sunspot-0.4.tar", last modified: Sun Jun 25 19:09:35 2023, max compression
```

## Comparing `sunspot-0.3.tar` & `sunspot-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 15:03:58.283515 sunspot-0.3/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    11970 2023-06-25 15:03:58.283331 sunspot-0.3/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    10939 2023-06-25 12:24:26.000000 sunspot-0.3/README.md
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-25 15:03:16.000000 sunspot-0.3/pyproject.toml
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-25 15:03:58.283558 sunspot-0.3/setup.cfg
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 15:03:58.282595 sunspot-0.3/src/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.3/src/foobar.py
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 15:03:58.283154 sunspot-0.3/src/sunspot.egg-info/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    11970 2023-06-25 15:03:58.000000 sunspot-0.3/src/sunspot.egg-info/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-25 15:03:58.000000 sunspot-0.3/src/sunspot.egg-info/SOURCES.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-25 15:03:58.000000 sunspot-0.3/src/sunspot.egg-info/dependency_links.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-25 15:03:58.000000 sunspot-0.3/src/sunspot.egg-info/top_level.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.3/src/sunspot.py
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.3/src/test.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.527535 sunspot-0.4/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12040 2023-06-25 19:09:35.527351 sunspot-0.4/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    11009 2023-06-25 19:07:59.000000 sunspot-0.4/README.md
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-25 19:09:08.000000 sunspot-0.4/pyproject.toml
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-25 19:09:35.527573 sunspot-0.4/setup.cfg
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.526608 sunspot-0.4/src/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.4/src/foobar.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.527166 sunspot-0.4/src/sunspot.egg-info/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12040 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/SOURCES.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/dependency_links.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/top_level.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.4/src/sunspot.py
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.4/src/test.py
```

### Comparing `sunspot-0.3/PKG-INFO` & `sunspot-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.3
+Version: 0.4
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="sunspot.png" width="250">
+  <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
 Project Description
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
```

### Comparing `sunspot-0.3/README.md` & `sunspot-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="sunspot.png" width="250">
+  <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
 Project Description
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
```

### Comparing `sunspot-0.3/pyproject.toml` & `sunspot-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sunspot"
-version = "0.3"
+version = "0.4"
 description = "Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris."
 readme = "README.md"
 authors = [{ name = "Phillip Curtsmith", email = "phillip.curtsmith@gmail.com" }]
 dependencies = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `sunspot-0.3/src/foobar.py` & `sunspot-0.4/src/foobar.py`

 * *Files identical despite different names*

### Comparing `sunspot-0.3/src/sunspot.egg-info/PKG-INFO` & `sunspot-0.4/src/sunspot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.3
+Version: 0.4
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="sunspot.png" width="250">
+  <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
 Project Description
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
```

### Comparing `sunspot-0.3/src/sunspot.py` & `sunspot-0.4/src/sunspot.py`

 * *Files identical despite different names*

### Comparing `sunspot-0.3/src/test.py` & `sunspot-0.4/src/test.py`

 * *Files identical despite different names*

