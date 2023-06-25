# Comparing `tmp/FlightRadarAPI-1.3.0.tar.gz` & `tmp/FlightRadarAPI-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.0.tar", last modified: Sat Jun 24 16:18:36 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.1.tar", last modified: Sat Jun 24 19:43:04 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.0.tar` & `FlightRadarAPI-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.674620 FlightRadarAPI-1.3.0/
-drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.644915 FlightRadarAPI-1.3.0/FlightRadar24/
--rw-rw-rw-   0        0        0      469 2023-06-24 16:16:53.000000 FlightRadarAPI-1.3.0/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     6731 2023-06-24 16:06:24.000000 FlightRadarAPI-1.3.0/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2048 2023-05-28 15:31:59.000000 FlightRadarAPI-1.3.0/FlightRadar24/core.py
--rw-rw-rw-   0        0        0     9199 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     1753 2023-05-28 15:37:24.000000 FlightRadarAPI-1.3.0/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.672711 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3138 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     3138 2023-06-24 16:18:36.673620 FlightRadarAPI-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2467 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 16:18:36.674620 FlightRadarAPI-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:43:04.823797 FlightRadarAPI-1.3.1/
+drwxrwxrwx   0        0        0        0 2023-06-24 19:43:04.794357 FlightRadarAPI-1.3.1/FlightRadar24/
+-rw-rw-rw-   0        0        0      469 2023-06-24 19:41:59.000000 FlightRadarAPI-1.3.1/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     8357 2023-06-24 19:38:40.000000 FlightRadarAPI-1.3.1/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.1/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0       38 2023-06-24 17:52:59.000000 FlightRadarAPI-1.3.1/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0     9199 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.1/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     1839 2023-06-24 19:04:31.000000 FlightRadarAPI-1.3.1/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:43:04.821357 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3138 2023-06-24 19:43:04.000000 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-24 19:43:04.000000 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:43:04.000000 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-24 19:43:04.000000 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 19:43:04.000000 FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3138 2023-06-24 19:43:04.822785 FlightRadarAPI-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2467 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:43:04.823797 FlightRadarAPI-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.1/setup.py
```

### Comparing `FlightRadarAPI-1.3.0/FlightRadar24/api.py` & `FlightRadarAPI-1.3.1/FlightRadar24/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 # -*- coding: utf-8 -*-
+from typing import Any, Dict, List, Optional, Tuple
 
 from .core import Core
+from .errors import LoginError
 from .flight import Flight
 from .request import APIRequest
 
-from deprecated import deprecated
-from typing import Any, Dict, List, Optional, Tuple
-
 
 class FlightRadar24API(object):
     """
-    Flight Radar 24 API
+    Main class of the FlightRadarAPI
     """
 
-    __real_time_flight_tracker_config = {
-        "faa": "1",
-        "satellite": "1",
-        "mlat": "1",
-        "flarm": "1",
-        "adsb": "1",
-        "gnd": "1",
-        "air": "1",
-        "vehicles": "1",
-        "estimated": "1",
-        "maxage": "14400",
-        "gliders": "1",
-        "stats": "1",
-        "limit": "5000"
-        }
-
-    def login(self, user: str, password: str) -> Dict:
-        # Log in with Flightradar24 Premium user credentials
-        data = {
-            "email": user,
-            "password": password,
-            "remember": "true",
-            "type": "web"
+    def __init__(self, user: Optional[str] = None, password: Optional[str] = None):
+        self.__real_time_flight_tracker_config = {
+            "faa": "1",
+            "satellite": "1",
+            "mlat": "1",
+            "flarm": "1",
+            "adsb": "1",
+            "gnd": "1",
+            "air": "1",
+            "vehicles": "1",
+            "estimated": "1",
+            "maxage": "14400",
+            "gliders": "1",
+            "stats": "1",
+            "limit": "5000"
         }
+        self.__login_data: Optional[Dict] = None
 
-        request = APIRequest(Core.user_login_url, headers = Core.json_headers, data = data)
-        self.__real_time_flight_tracker_config["enc"] = request.get_cookie("_frPl")
-
-        return request.get_content()
+        if user is not None and password is not None:
+            self.login(user, password)
 
     def get_airlines(self) -> List[Dict]:
         """
         Return a list with all airlines.
         """
-        request = APIRequest(Core.airlines_data_url, headers = Core.json_headers)
-        return request.get_content()["rows"]
+        response = APIRequest(Core.airlines_data_url, headers = Core.json_headers)
+        return response.get_content()["rows"]
 
     def get_airline_logo(self, iata: str, icao: str) -> Optional[Tuple[bytes, str]]:
         """
         Download the logo of an airline from FlightRadar24 and return it as bytes.
         """
         first_logo_url = Core.airline_logo_url.format(iata, icao)
 
@@ -74,31 +64,31 @@
 
     def get_airport(self, code: str) -> Dict:
         """
         Return detailed information about an airport.
 
         :param code: ICAO or IATA of the airport.
         """
-        request = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
-        return request.get_content()["details"]
+        response = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
+        return response.get_content()["details"]
 
     def get_airports(self) -> List[Dict]:
         """
         Return a list with all airports.
         """
-        request = APIRequest(Core.airports_data_url, headers = Core.json_headers)
-        return request.get_content()["rows"]
+        response = APIRequest(Core.airports_data_url, headers = Core.json_headers)
+        return response.get_content()["rows"]
 
     def get_bounds(self, zone: Dict[str, float]) -> str:
         """
         Convert coordinate dictionary to a string "y1, y2, x1, x2".
 
         :param zone: Dictionary containing the following keys: tl_y, tl_x, br_y, br_x
         """
-        return "{},{},{},{}".format(zone["tl_y"], zone["br_y"] , zone["tl_x"], zone["br_x"])
+        return "{},{},{},{}".format(zone["tl_y"], zone["br_y"], zone["tl_x"], zone["br_x"])
 
     def get_country_flag(self, country: str) -> Optional[Tuple[bytes, str]]:
         """
         Download the flag of a country from FlightRadar24 and return it as bytes.
 
         :param country: Country name
         """
@@ -114,67 +104,121 @@
         if not str(status_code).startswith("4"):
             return response.get_content(), flag_url.split(".")[-1]
 
     def get_flight_details(self, flight_id: str) -> Dict[Any, Any]:
         """
         Return the flight details from Data Live Flightradar24.
         """
-        request = APIRequest(Core.flight_data_url.format(flight_id), headers = Core.json_headers)
-        return request.get_content()
+        response = APIRequest(Core.flight_data_url.format(flight_id), headers = Core.json_headers)
+        return response.get_content()
 
     def get_flights(self, airline: str = None, bounds: str = None, registration: str = None, aircraft_type: str = None) -> List[Flight]:
         """
         Return a list of flights. See more options at set_real_time_flight_tracker_config() method.
 
         :param airline: the airline ICAO. Ex: "DAL"
         :param bounds: coordinates (y1, y2 ,x1, x2). Ex: "75.78,-75.78,-427.56,427.56"
         :param registration: aircraft registration
         :param aircraft_type: aircraft model code. Ex: "B737"
         """
-
         request_params = self.__real_time_flight_tracker_config.copy()
 
         # Insert the parameters "airline", "bounds", "reg",and "type" in the dictionary for the request.
         if airline: request_params["airline"] = airline
         if bounds: request_params["bounds"] = bounds.replace(",", "%2C")
         if registration: request_params["reg"] = registration
         if aircraft_type: request_params["type"] = aircraft_type
 
         # Get all flights from Data Live Flightradar24.
-        request = APIRequest(Core.real_time_flight_tracker_data_url, request_params, Core.json_headers)
-        response = request.get_content()
+        response = APIRequest(Core.real_time_flight_tracker_data_url, request_params, Core.json_headers)
+        response = response.get_content()
 
         flights = []
 
         for flight_id, flight_info in response.items():
 
             # Get flights only.
             if flight_id[0].isnumeric():
                 flights.append(Flight(flight_id, flight_info))
 
         return flights
 
+    def get_login_data(self) -> Dict[Any, Any]:
+        """
+        Return the user data.
+        """
+        if not self.is_logged_in():
+            raise LoginError("You must log in to your account.")
+
+        return self.__login_data["userData"].copy()
+
     def get_real_time_flight_tracker_config(self) -> Dict[str, str]:
         """
         Return the current config of the real time flight tracker, used by get_flights() method.
         """
         return self.__real_time_flight_tracker_config.copy()
 
     def get_zones(self) -> Dict[str, Dict]:
         """
         Returns all major zones on the globe.
         """
-        request = APIRequest(Core.zones_data_url, headers = Core.json_headers)
-        zones = request.get_content()
+        response = APIRequest(Core.zones_data_url, headers = Core.json_headers)
+        zones = response.get_content()
 
         if "version" in zones:
             zones.pop("version")
 
         return zones
 
+    def is_logged_in(self) -> bool:
+        """
+        Check if the user is logged into the FlightRadar24 account.
+        """
+        return self.__login_data is not None
+
+    def login(self, user: str, password: str) -> None:
+        """
+        Log in to a FlightRadar24 account.
+
+        :param user: Your email.
+        :param password: Your password.
+        """
+        data = {
+            "email": user,
+            "password": password,
+            "remember": "true",
+            "type": "web"
+        }
+
+        response = APIRequest(Core.user_login_url, headers = Core.json_headers, data = data)
+        status_code = response.get_status_code()
+        content = response.get_content()
+
+        if not str(status_code).startswith("2") or not content.get("success"):
+            if isinstance(content, dict): raise LoginError(content["message"])
+            else: raise LoginError("Your email or password is incorrect")
+
+        self.__real_time_flight_tracker_config["enc"] = response.get_cookie("_frPl")
+
+        self.__login_data = {
+            "userData": content["userData"],
+            "cookies": response.get_cookies()
+        }
+
+    def logout(self) -> None:
+        """
+        Log out of the Flightradar24 account.
+        """
+        if not self.__login_data: return
+
+        APIRequest(Core.user_login_url, headers = Core.json_headers, cookies = self.__login_data["cookies"])
+
+        self.__real_time_flight_tracker_config.pop("enc")
+        self.__login_data = None
+
     def set_real_time_flight_tracker_config(self, **config: str) -> None:
         """
         Set config for the real time flight tracker, used by get_flights() method.
         """
         for key, value in config.items():
 
             # Check if the parameter exists and if the value is numeric.
```

### Comparing `FlightRadarAPI-1.3.0/FlightRadar24/core.py` & `FlightRadarAPI-1.3.1/FlightRadar24/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     cdn_flightradar_base_url = "https://cdn.flightradar24.com"
     flightradar_base_url = "https://www.flightradar24.com"
     data_live_base_url = "https://data-live.flightradar24.com"
     data_cloud_base_url = "https://data-cloud.flightradar24.com"
 
     # User login URL.
     user_login_url = flightradar_base_url + "/user/login"
+    user_logout_url = flightradar_base_url + "/user/logout"
 
     # Flights data URLs.
     real_time_flight_tracker_data_url = data_cloud_base_url + "/zones/fcgi/feed.js"
     flight_data_url = data_live_base_url + "/clickhandler/?flight={}"
 
     # Airports data URLs.
     airport_data_url = flightradar_base_url + "/airports/traffic-stats/?airport={}"
```

### Comparing `FlightRadarAPI-1.3.0/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.1/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.0/FlightRadar24/request.py` & `FlightRadarAPI-1.3.1/FlightRadar24/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
     __content_encodings = {
         "": lambda x: x,
         "br": brotli.decompress,
         "gzip": gzip.decompress
     }
 
-    def __init__(self, url, params = {}, headers = {}, data = None):
+    def __init__(self, url, params = {}, headers = {}, data = None, cookies = None):
 
         self.url = url
         self.params = params
         self.headers = headers
         self.data = data
+        self.cookies = cookies
 
         if data is None:
             if params: url += "?" + "&".join(["{}={}".format(k, v) for k, v in params.items()])
-            self.__response = requests.get(url, headers = headers)
+            self.__response = requests.get(url, headers = headers, cookies = cookies)
         else:
-            self.__response = requests.post(url, data = data, headers = headers)
+            self.__response = requests.post(url, headers = headers, cookies = cookies, data = data)
 
     def get_content(self) -> Union[Dict, bytes]:
         content = self.__response.content
         content_encoding = self.get_content_encoding()
         content_type = self.get_content_type()
 
         # Try to decode the content.
```

### Comparing `FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.1/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.0
+Version: 1.3.1
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.0/LICENSE` & `FlightRadarAPI-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.0/PKG-INFO` & `FlightRadarAPI-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.0
+Version: 1.3.1
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.0/README.md` & `FlightRadarAPI-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.0/setup.py` & `FlightRadarAPI-1.3.1/setup.py`

 * *Files identical despite different names*

