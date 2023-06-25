# Comparing `tmp/FlightRadarAPI-1.3.4.tar.gz` & `tmp/FlightRadarAPI-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.4.tar", last modified: Sun Jun 25 05:19:18 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.5.tar", last modified: Sun Jun 25 07:05:05 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.4.tar` & `FlightRadarAPI-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.248874 FlightRadarAPI-1.3.4/
-drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.237869 FlightRadarAPI-1.3.4/FlightRadar24/
--rw-rw-rw-   0        0        0      553 2023-06-25 05:19:13.000000 FlightRadarAPI-1.3.4/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     9606 2023-06-25 05:04:32.000000 FlightRadarAPI-1.3.4/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.4/FlightRadar24/core.py
--rw-rw-rw-   0        0        0       40 2023-06-25 02:41:44.000000 FlightRadarAPI-1.3.4/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.4/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     2809 2023-06-25 05:19:03.000000 FlightRadarAPI-1.3.4/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:19:18.246863 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 05:19:18.000000 FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.4/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-06-25 05:19:18.247875 FlightRadarAPI-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 05:19:18.248874 FlightRadarAPI-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.402528 FlightRadarAPI-1.3.5/
+drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.384741 FlightRadarAPI-1.3.5/FlightRadar24/
+-rw-rw-rw-   0        0        0      553 2023-06-25 07:00:28.000000 FlightRadarAPI-1.3.5/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     9611 2023-06-25 07:01:46.000000 FlightRadarAPI-1.3.5/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.5/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0      244 2023-06-25 06:53:16.000000 FlightRadarAPI-1.3.5/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.5/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     3091 2023-06-25 06:53:31.000000 FlightRadarAPI-1.3.5/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.400498 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0     3181 2023-06-25 07:05:05.400498 FlightRadarAPI-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:05:05.402528 FlightRadarAPI-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-06-25 06:47:19.000000 FlightRadarAPI-1.3.5/setup.py
```

### Comparing `FlightRadarAPI-1.3.4/FlightRadar24/__init__.py` & `FlightRadarAPI-1.3.5/FlightRadar24/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 from .api import FlightRadar24API, FlightTrackerConfig
 from .flight import Flight
```

### Comparing `FlightRadarAPI-1.3.4/FlightRadar24/api.py` & `FlightRadarAPI-1.3.5/FlightRadar24/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     def logout(self) -> bool:
         """
         Log out of the FlightRadar24 account.
 
         Return a boolean indicating that it successfully logged out of the server.
         """
-        if self.__login_data is None: return
+        if self.__login_data is None: return True
 
         cookies = self.__login_data["cookies"]
         self.__login_data = None
 
         response = APIRequest(Core.user_login_url, headers = Core.json_headers, cookies = cookies)
         return str(response.get_status_code()).startswith("2")
```

### Comparing `FlightRadarAPI-1.3.4/FlightRadar24/core.py` & `FlightRadarAPI-1.3.5/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.4/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.5/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.4/FlightRadar24/request.py` & `FlightRadarAPI-1.3.5/FlightRadar24/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import brotli
 import json
 import gzip
 
 import requests
 import requests.structures
 
+from .errors import CloudflareError
+
 
 class APIRequest(object):
     """
     Class to make requests to the FlightRadar24.
     """
     __content_encodings = {
         "": lambda x: x,
@@ -47,14 +49,20 @@
         }
 
         request_method = requests.get if data is None else requests.post
 
         if params: url += "?" + "&".join(["{}={}".format(k, v) for k, v in params.items()])
         self.__response = request_method(url, headers = headers, cookies = cookies, data = data)
 
+        if self.get_status_code() == 520:
+            raise CloudflareError(
+                message = "An unexpected error has occurred. Perhaps you are making too many calls?",
+                response = self.__response
+            )
+
     def get_content(self) -> Union[Dict, bytes]:
         """
         Return the received content from the request.
         """
         content = self.__response.content
 
         content_encoding = self.__response.headers.get("Content-Encoding", "")
```

### Comparing `FlightRadarAPI-1.3.4/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.4
+Version: 1.3.5
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.4/LICENSE` & `FlightRadarAPI-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.4/PKG-INFO` & `FlightRadarAPI-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.4
+Version: 1.3.5
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.4/README.md` & `FlightRadarAPI-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.4/setup.py` & `FlightRadarAPI-1.3.5/setup.py`

 * *Files identical despite different names*

