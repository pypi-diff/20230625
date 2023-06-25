# Comparing `tmp/FlightRadarAPI-1.3.3.tar.gz` & `tmp/FlightRadarAPI-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.3.tar", last modified: Sun Jun 25 05:05:01 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.4.tar", last modified: Sun Jun 25 05:19:18 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.3.tar` & `FlightRadarAPI-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.013511 FlightRadarAPI-1.3.3/FlightRadar24/
--rw-rw-rw-   0        0        0      553 2023-06-25 05:04:16.000000 FlightRadarAPI-1.3.3/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     9606 2023-06-25 05:04:32.000000 FlightRadarAPI-1.3.3/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.3/FlightRadar24/core.py
--rw-rw-rw-   0        0        0       40 2023-06-25 02:41:44.000000 FlightRadarAPI-1.3.3/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.3/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     2834 2023-06-25 04:39:09.000000 FlightRadarAPI-1.3.3/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.036642 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.248874 FlightRadarAPI-1.3.4/
+drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.237869 FlightRadarAPI-1.3.4/FlightRadar24/
+-rw-rw-rw-   0        0        0      553 2023-06-25 05:19:13.000000 FlightRadarAPI-1.3.4/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     9606 2023-06-25 05:04:32.000000 FlightRadarAPI-1.3.4/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.4/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0       40 2023-06-25 02:41:44.000000 FlightRadarAPI-1.3.4/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.4/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     2809 2023-06-25 05:19:03.000000 FlightRadarAPI-1.3.4/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.246863 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0     3181 2023-06-25 05:19:18.247875 FlightRadarAPI-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 05:19:18.248874 FlightRadarAPI-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.4/setup.py
```

### Comparing `FlightRadarAPI-1.3.3/FlightRadar24/__init__.py` & `FlightRadarAPI-1.3.4/FlightRadar24/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 
 from .api import FlightRadar24API, FlightTrackerConfig
 from .flight import Flight
```

### Comparing `FlightRadarAPI-1.3.3/FlightRadar24/api.py` & `FlightRadarAPI-1.3.4/FlightRadar24/api.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.3/FlightRadar24/core.py` & `FlightRadarAPI-1.3.4/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.3/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.4/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.3/FlightRadar24/request.py` & `FlightRadarAPI-1.3.4/FlightRadar24/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
-from requests.models import Response
-from requests.structures import CaseInsensitiveDict
 from typing import Dict, Optional, Union
 
 import brotli
 import json
 import gzip
+
 import requests
+import requests.structures
 
 
 class APIRequest(object):
     """
     Class to make requests to the FlightRadar24.
     """
     __content_encodings = {
@@ -72,21 +72,21 @@
 
     def get_cookies(self) -> Dict:
         """
         Return the received cookies from the request.
         """
         return self.__response.cookies.get_dict()
 
-    def get_headers(self) -> CaseInsensitiveDict:
+    def get_headers(self) -> requests.structures.CaseInsensitiveDict:
         """
         Return the headers of the response.
         """
         return self.__response.headers
 
-    def get_response_object(self) -> Response:
+    def get_response_object(self) -> requests.models.Response:
         """
         Return the received response object.
         """
         return self.__response
 
     def get_status_code(self) -> int:
         """
```

### Comparing `FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.3/LICENSE` & `FlightRadarAPI-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.3/PKG-INFO` & `FlightRadarAPI-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.3/README.md` & `FlightRadarAPI-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.3/setup.py` & `FlightRadarAPI-1.3.4/setup.py`

 * *Files identical despite different names*

