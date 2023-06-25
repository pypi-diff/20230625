# Comparing `tmp/sunspot-0.4.tar.gz` & `tmp/sunspot-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunspot-0.4.tar", last modified: Sun Jun 25 19:09:35 2023, max compression
+gzip compressed data, was "sunspot-0.5.tar", last modified: Sun Jun 25 19:25:50 2023, max compression
```

## Comparing `sunspot-0.4.tar` & `sunspot-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.527535 sunspot-0.4/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12040 2023-06-25 19:09:35.527351 sunspot-0.4/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    11009 2023-06-25 19:07:59.000000 sunspot-0.4/README.md
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-25 19:09:08.000000 sunspot-0.4/pyproject.toml
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-25 19:09:35.527573 sunspot-0.4/setup.cfg
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.526608 sunspot-0.4/src/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.4/src/foobar.py
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:09:35.527166 sunspot-0.4/src/sunspot.egg-info/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12040 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/SOURCES.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/dependency_links.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-25 19:09:35.000000 sunspot-0.4/src/sunspot.egg-info/top_level.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.4/src/sunspot.py
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.4/src/test.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:25:50.921469 sunspot-0.5/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-25 19:25:50.921283 sunspot-0.5/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    10997 2023-06-25 19:24:10.000000 sunspot-0.5/README.md
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-25 19:24:30.000000 sunspot-0.5/pyproject.toml
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-25 19:25:50.921510 sunspot-0.5/setup.cfg
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:25:50.920549 sunspot-0.5/src/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.5/src/foobar.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-25 19:25:50.921095 sunspot-0.5/src/sunspot.egg-info/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-25 19:25:50.000000 sunspot-0.5/src/sunspot.egg-info/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-25 19:25:50.000000 sunspot-0.5/src/sunspot.egg-info/SOURCES.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-25 19:25:50.000000 sunspot-0.5/src/sunspot.egg-info/dependency_links.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-25 19:25:50.000000 sunspot-0.5/src/sunspot.egg-info/top_level.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.5/src/sunspot.py
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.5/src/test.py
```

### Comparing `sunspot-0.4/PKG-INFO` & `sunspot-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.4
+Version: 0.5
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 <p align="center">
   <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
-Project Description
+Sunspot
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
 
 In addition to data recovery from JPL, Sunspot provides a client tool for tracking _Observer Quantities_. For situations where a user wishes to update a web server as a function of _Target Body_ status, guide a telescope over time, orchestrate hardware control based upon the sun's position, and the like, Sunspot provides a Tracker class to execute user-defined methods with sub-second precision. A user can elect to execute methods before ("setup"), at ("test"), and/or after ("clean-up") individual ephemeris events, for the duration of that ephemeris.
 
 Create Ephemeris
 -
```

### Comparing `sunspot-0.4/README.md` & `sunspot-0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
-Project Description
+Sunspot
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
 
 In addition to data recovery from JPL, Sunspot provides a client tool for tracking _Observer Quantities_. For situations where a user wishes to update a web server as a function of _Target Body_ status, guide a telescope over time, orchestrate hardware control based upon the sun's position, and the like, Sunspot provides a Tracker class to execute user-defined methods with sub-second precision. A user can elect to execute methods before ("setup"), at ("test"), and/or after ("clean-up") individual ephemeris events, for the duration of that ephemeris.
 
 Create Ephemeris
 -
```

### Comparing `sunspot-0.4/pyproject.toml` & `sunspot-0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sunspot"
-version = "0.4"
+version = "0.5"
 description = "Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris."
 readme = "README.md"
 authors = [{ name = "Phillip Curtsmith", email = "phillip.curtsmith@gmail.com" }]
 dependencies = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `sunspot-0.4/src/foobar.py` & `sunspot-0.5/src/foobar.py`

 * *Files identical despite different names*

### Comparing `sunspot-0.4/src/sunspot.egg-info/PKG-INFO` & `sunspot-0.5/src/sunspot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.4
+Version: 0.5
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 <p align="center">
   <img src="https://github.com/phillipcurtsmith/sunspot-issues/blob/main/sunspot.png?raw=true" width="250">
 </p>
 
 Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any _Target Body_ available through the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Also provides real-time tracking of those data for the duration of an ephemeris.
 
-Project Description
+Sunspot
 -
 Sunspot recovers ephemerides using JPL's back-end HTML interface. As a result, no need to load binary SPK files (.bsp). A user must only identify a _Target Body_ and _Observer Quantities_ from the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/). Any planet, satellite, spacecraft, asteroid, or comet available in the [JPL Horizons App](https://ssd.jpl.nasa.gov/horizons/app.html#/) is available through Sunspot. Sunspot provides simple parsed lists of strings for each quantity, e.g., a list of azimuth and elevation values where a _Target Body_ can be found in the sky. Because all data are computed and furnished from JPL, Sunspot incurs very little computational overhead aside from initial parsing.
 
 In addition to data recovery from JPL, Sunspot provides a client tool for tracking _Observer Quantities_. For situations where a user wishes to update a web server as a function of _Target Body_ status, guide a telescope over time, orchestrate hardware control based upon the sun's position, and the like, Sunspot provides a Tracker class to execute user-defined methods with sub-second precision. A user can elect to execute methods before ("setup"), at ("test"), and/or after ("clean-up") individual ephemeris events, for the duration of that ephemeris.
 
 Create Ephemeris
 -
```

### Comparing `sunspot-0.4/src/sunspot.py` & `sunspot-0.5/src/sunspot.py`

 * *Files identical despite different names*

### Comparing `sunspot-0.4/src/test.py` & `sunspot-0.5/src/test.py`

 * *Files identical despite different names*

