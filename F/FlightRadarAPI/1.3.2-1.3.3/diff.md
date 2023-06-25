# Comparing `tmp/FlightRadarAPI-1.3.2.tar.gz` & `tmp/FlightRadarAPI-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.2.tar", last modified: Sun Jun 25 05:01:58 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.3.tar", last modified: Sun Jun 25 05:05:01 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.2.tar` & `FlightRadarAPI-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 05:01:58.833416 FlightRadarAPI-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 05:01:58.813566 FlightRadarAPI-1.3.2/FlightRadar24/
--rw-rw-rw-   0        0        0      553 2023-06-25 03:12:12.000000 FlightRadarAPI-1.3.2/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     9609 2023-06-25 04:56:12.000000 FlightRadarAPI-1.3.2/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.2/FlightRadar24/core.py
--rw-rw-rw-   0        0        0       40 2023-06-25 02:41:44.000000 FlightRadarAPI-1.3.2/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.2/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     2834 2023-06-25 04:39:09.000000 FlightRadarAPI-1.3.2/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:01:58.831436 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:01:58.000000 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-25 05:01:58.000000 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 05:01:58.000000 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 05:01:58.000000 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 05:01:58.000000 FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:01:58.832417 FlightRadarAPI-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 05:01:58.833416 FlightRadarAPI-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.013511 FlightRadarAPI-1.3.3/FlightRadar24/
+-rw-rw-rw-   0        0        0      553 2023-06-25 05:04:16.000000 FlightRadarAPI-1.3.3/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     9606 2023-06-25 05:04:32.000000 FlightRadarAPI-1.3.3/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.3/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0       40 2023-06-25 02:41:44.000000 FlightRadarAPI-1.3.3/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.3/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     2834 2023-06-25 04:39:09.000000 FlightRadarAPI-1.3.3/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:05:01.036642 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 05:05:00.000000 FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     3181 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 05:05:01.038110 FlightRadarAPI-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.3/setup.py
```

### Comparing `FlightRadarAPI-1.3.2/FlightRadar24/__init__.py` & `FlightRadarAPI-1.3.3/FlightRadar24/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 from .api import FlightRadar24API, FlightTrackerConfig
 from .flight import Flight
```

### Comparing `FlightRadarAPI-1.3.2/FlightRadar24/api.py` & `FlightRadarAPI-1.3.3/FlightRadar24/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         response = APIRequest(second_logo_url, headers = Core.image_headers)
         status_code = response.get_status_code()
 
         if not str(status_code).startswith("4"):
             return response.get_content(), second_logo_url.split(".")[-1]
 
-    def get_airport(self, code: str, /) -> Dict:
+    def get_airport(self, code: str) -> Dict:
         """
         Return detailed information about an airport.
 
         :param code: ICAO or IATA of the airport
         """
         response = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
         return response.get_content()["details"]
```

### Comparing `FlightRadarAPI-1.3.2/FlightRadar24/core.py` & `FlightRadarAPI-1.3.3/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.2/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.3/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.2/FlightRadar24/request.py` & `FlightRadarAPI-1.3.3/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.2/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.3/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.2
+Version: 1.3.3
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.2/LICENSE` & `FlightRadarAPI-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.2/PKG-INFO` & `FlightRadarAPI-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.2
+Version: 1.3.3
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.2/README.md` & `FlightRadarAPI-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.2/setup.py` & `FlightRadarAPI-1.3.3/setup.py`

 * *Files identical despite different names*

