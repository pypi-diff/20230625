# Comparing `tmp/purpleair_api-1.0.2a1.tar.gz` & `tmp/purpleair_api-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpleair_api-1.0.2a1.tar", last modified: Thu May 18 04:42:14 2023, max compression
+gzip compressed data, was "purpleair_api-1.1.0a1.tar", last modified: Sun Jun 25 14:36:30 2023, max compression
```

## Comparing `purpleair_api-1.0.2a1.tar` & `purpleair_api-1.1.0a1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/purpleair_api/
--rw-r--r--   0 runner    (1001) docker     (123)    43928 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPIConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/purpleair_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 04:42:14.403680 purpleair_api-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:36:30.683745 purpleair_api-1.1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-25 14:36:30.683745 purpleair_api-1.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:36:30.683745 purpleair_api-1.1.0a1/purpleair_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirAPIConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirAPIError.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirAPIHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirLocalAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27865 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirReadAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/PurpleAirWriteAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/purpleair_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:36:30.683745 purpleair_api-1.1.0a1/purpleair_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-25 14:36:30.000000 purpleair_api-1.1.0a1/purpleair_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-25 14:36:30.000000 purpleair_api-1.1.0a1/purpleair_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 14:36:30.000000 purpleair_api-1.1.0a1/purpleair_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 14:36:30.000000 purpleair_api-1.1.0a1/purpleair_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 14:36:30.000000 purpleair_api-1.1.0a1/purpleair_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-25 14:36:30.687745 purpleair_api-1.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-25 14:36:19.000000 purpleair_api-1.1.0a1/setup.py
```

### Comparing `purpleair_api-1.0.2a1/LICENSE` & `purpleair_api-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `purpleair_api-1.0.2a1/PKG-INFO` & `purpleair_api-1.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpleair_api
-Version: 1.0.2a1
+Version: 1.1.0a1
 Home-page: https://github.com/carlkidcrypto/purpleair_api
 Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_api,purple air api,purple_air,purple air
 Platform: Windows 32/64
 Platform: Linux 32/64
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: purpleair_api Version: 1.0.2a1 Home-page: https://
+Metadata-Version: 2.1 Name: purpleair_api Version: 1.1.0a1 Home-page: https://
 github.com/carlkidcrypto/purpleair_api Author: Carlos Santos Author-email:
 dose.lucky.sake@cloak.id License: MIT Keywords: purpleair_api,purple air
 api,purple_air,purple air Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE # purple_air_api (PAA) This is a python3 wrapper
 for the new PurpleAirAPI (PAA). Details of the API can be found using this
 link:
```

### Comparing `purpleair_api-1.0.2a1/README.md` & `purpleair_api-1.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPI.py` & `purpleair_api-1.1.0a1/purpleair_api/PurpleAirReadAPI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,165 +1,28 @@
 #!/usr/bin/env python3
 
 """
     Copyright 2023 carlkidcrypto, All rights reserved.
     A python3 class designed to fetch data from Purple Air's new API.
+    This class will handle all `read` requests
     https://api.purpleair.com/#api-welcome
 """
 
-import requests
-import json
-from purpleair_api.PurpleAirAPIConstants import (
-    ACCEPTED_FIELD_NAMES_DICT,
-    PRINT_DEBUG_MSGS,
-    SUCCESS_CODE_LIST,
-    ERROR_CODES_LIST,
-)
+from purpleair_api.PurpleAirAPIHelpers import send_url_get_request
 
 
-class PurpleAirAPIError(Exception):
+class PurpleAirReadAPI:
     """
-    Custom Exception for our PurpleAirAPI class.
+    The PurpleAirReadAPI class designed to send valid
+    read requests.
     """
 
-    def __init__(self, message_string):
-        self.message = message_string
-        super().__init__(self.message)
-
-
-def debug_log(debug_msg_string):
-    """
-    A helper function to print out
-    debug messages only if DEBUG is defined as True in
-    'PurpleAirAPIConstants.py'. Messages will be the color
-    red.
-
-    :param str debug_msg_string: The debug message string
-    """
-
-    if PRINT_DEBUG_MSGS:
-        # Make debug messages red using ANSI escape code.
-        print("\033[1;31m" + str(debug_msg_string) + "\x1b[0m")
-
-
-class PurpleAirAPI:
-    """
-    The PurpleAirAPI class designed to send valid
-    PurpleAirAPI requests.
-    """
-
-    def __init__(self, your_api_read_key=None, your_api_write_key=None):
-        """
-        :param str your_api_read_key: A valid PurpleAirAPI Read key
-        :param str your_api_write_key: A valid PurpleAirAPI Write key
-        """
-
-        if your_api_read_key is None and your_api_write_key is None:
-            raise PurpleAirAPIError(
-                "Ensure one or both of 'your_api_read_key'/'your_api_write_key' key(s) are provided"
-            )
-
+    def __init__(self, api_read_key=None):
         # Save off the API key for internal usage
-        self._your_api_read_key = your_api_read_key
-        self._your_api_write_key = your_api_write_key
-
-        # Create the base API request string. Must be HTTPS.
-        self._base_api_v1_request_string = "https://api.purpleair.com/v1/"
-
-        # Place holders for information we care about
-        self._api_versions = {}
-        self._api_keys_last_checked = {}
-        self._api_key_types = {}
-
-        retval_api_read_key = None
-        retval_api_write_key = None
-
-        if your_api_read_key is not None:
-            retval_api_read_key = self._check_an_api_key(your_api_read_key)
-
-        if your_api_write_key is not None:
-            retval_api_write_key = self._check_an_api_key(your_api_write_key)
-
-        debug_log(self._api_versions)
-        debug_log(self._api_keys_last_checked)
-        debug_log(self._api_key_types)
-
-        if retval_api_read_key is not None:
-            if self._api_key_types[your_api_read_key] == "READ":
-                print("PurpleAirAPI: Successfully authenticated read key")
-
-            else:
-                raise PurpleAirAPIError("Ensure 'your_api_read_key' is a read key.")
-
-        if retval_api_write_key is not None:
-            if self._api_key_types[your_api_write_key] == "WRITE":
-                print("PurpleAirAPI: Successfully authenticated write key")
-
-            else:
-                raise PurpleAirAPIError("Ensure 'your_api_write_key' is a write key")
-
-    def _check_an_api_key(self, str_api_key_to_check):
-        """
-        An internal class helper method to check if an API key is valid.
-
-        :param str str_api_key_to_check: A valid PurpleAirAPI key to check
-
-        :return True, if an API key can be successfully verified.
-        """
-        request_url = self._base_api_v1_request_string + "keys"
-        my_request = requests.get(
-            request_url, headers={"X-API-Key": str(str_api_key_to_check)}
-        )
-
-        the_request_text_as_json = json.loads(my_request.text)
-        debug_log(the_request_text_as_json)
-
-        if my_request.status_code in SUCCESS_CODE_LIST:
-            # We good :) get the request text
-            self._api_versions[str_api_key_to_check] = the_request_text_as_json[
-                "api_version"
-            ]
-            self._api_keys_last_checked[
-                str_api_key_to_check
-            ] = the_request_text_as_json["time_stamp"]
-            self._api_key_types[str_api_key_to_check] = the_request_text_as_json[
-                "api_key_type"
-            ]
-            my_request.close()
-            del my_request
-            return True
-
-        else:
-            raise PurpleAirAPIError(
-                f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
-            )
-
-    @property
-    def get_api_versions(self):
-        """
-        A method to return the API versions being used for both read/write keys.
-        """
-
-        return self._api_versions
-
-    @property
-    def get_api_key_last_checked(self):
-        """
-        A method to return the timestamp of when the API read/write keys were last checked.
-        """
-
-        return self._api_keys_last_checked
-
-    @property
-    def get_api_key_type(self):
-        """
-        A method to return the API key types being used.
-        """
-
-        return self._api_key_types
+        self._your_api_read_key = api_read_key
 
     def request_sensor_data(self, sensor_index, read_key=None, fields=None):
         """
         A method to retrieve sensor data from one sensor. Will return the
         response payload as a python dictionary.
 
         :param int sensor_index: The sensor_index as found in the JSON for
@@ -185,15 +48,15 @@
         """
 
         request_url = self._base_api_v1_request_string + "sensors/" + f"{sensor_index}"
 
         optional_parameters_dict = {"read_key": read_key, "fields": fields}
 
         first_optional_parameter_separator = "?"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
 
     def request_multiple_sensors_data(
@@ -291,15 +154,15 @@
             "nwlng": nwlng,
             "nwlat": nwlat,
             "selng": selng,
             "selat": selat,
         }
 
         first_optional_parameter_separator = "&"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
 
     def request_sensor_historic_data(
@@ -374,38 +237,38 @@
             "start_timestamp": start_timestamp,
             "end_timestamp": end_timestamp,
             "modified_since": end_timestamp,
             "average": average,
         }
 
         first_optional_parameter_separator = "&"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
 
     def request_group_detail_data(self, group_id):
         """
         A method to retrieve a list of all members of a specified group.
 
         :param int group_id: The group_id of the requested group. This group must be owned by the api_key.
         """
 
         request_url = self._base_api_v1_request_string + f"groups/{group_id}"
-        return self._send_url_get_request(request_url, self._your_api_read_key)
+        return send_url_get_request(request_url, self._your_api_read_key)
 
     def request_group_list_data(self):
         """
         A method to retrieve a list of all groups owned by the provided api_key.
         """
 
         request_url = self._base_api_v1_request_string + f"groups/"
-        return self._send_url_get_request(request_url, self._your_api_read_key)
+        return send_url_get_request(request_url, self._your_api_read_key)
 
     def request_member_data(self, group_id, member_id, fields=None):
         """
         A method to get a members' data from a group to which said member belongs.
 
         :param int group_id: Groups unique ID.
 
@@ -448,15 +311,15 @@
         )
 
         # Add to the request_url string depending on what optional parameters are
         # passed in. Turn them into a dict of optional parameters
         optional_parameters_dict = {"fields": fields}
 
         first_optional_parameter_separator = "?"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
 
     def request_member_historic_data(
@@ -526,15 +389,15 @@
         optional_parameters_dict = {
             "start_timestamp": start_timestamp,
             "end_timestamp": end_timestamp,
             "average": average,
         }
 
         first_optional_parameter_separator = "&"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
 
     def request_members_data(
@@ -629,315 +492,13 @@
             "nwlng": nwlng,
             "nwlat": nwlat,
             "selng": selng,
             "selat": selat,
         }
 
         first_optional_parameter_separator = "&"
-        return self._send_url_get_request(
+        return send_url_get_request(
             request_url,
             self._your_api_read_key,
             first_optional_parameter_separator,
             optional_parameters_dict,
         )
-
-    def post_create_group_data(self, name):
-        """
-        A method to create a group for sensors.
-
-        :param str name: The name of the group to create.
-        """
-
-        post_url = self._base_api_v1_request_string + f"groups"
-
-        return self._send_url_post_request(
-            post_url, self._your_api_write_key, {"name": name}
-        )
-
-    def post_create_member(
-        self,
-        group_id,
-        sensor_index=None,
-        sensor_id=None,
-        owner_email=None,
-        location_type=None,
-    ):
-        """
-        Using a sensor_id (Parameters Option 1)
-        The sensor_id should be exactly as printed on the label on the sensor. When no owner_email is provided, the sensor has to be marked as public.
-
-        :param int group_id: The group_id of the group to add a member to. This group must be owned by the api_key.
-
-        :param str sensor_id: The sensor_id of the new member sensor. This must be AS PRINTED on the sensor’s label.
-
-        Using a sensor_index (Parameters Option 2)
-        The sensor_index can be found in lists for example from a /sensors api call. When no owner_email is provided, the sensor has to be marked as public.
-
-        :param int group_id: The group_id of the group to add a member to. This group must be owned by the api_key.
-
-        :param int sensor_index: The sensor_index of the new member as found in the JSON for this specific sensor.
-
-        Using sensor_id with a private sensor by specifying owner_email and optionally location_type. (Parameters Option 3)
-        This example will produce an error if any provided value does not match the current configuration of the sensor. Note, too many incorrect attempts may disable your API key, so do not try guessing the email!!
-
-        :param int group_id: The group_id of the group to add a member to. This group must be owned by the api_key.
-
-        :param str sensor_id: The sensor_id of the new member sensor. This must be AS PRINTED on the sensor’s label.
-
-        :param str owner_email: An email address that matches the Owner email as set by previously completing the PurpleAir registration form at www.purpleair.com/register.
-
-        :param (optional) int location_type: The expected location_type of the new member.
-                                             Possible values are: 0 = Outside or 1 = Inside.
-                                             If the target member is not of this type, an error will result.
-                                             NOTE: This value is required if the sensor in question is marked as ‘private’ on the registration form.
-        """
-
-        post_url = self._base_api_v1_request_string + f"groups/{group_id}/members"
-
-        if (
-            sensor_index is None
-            and sensor_id is not None
-            and owner_email is None
-            and location_type is None
-        ):
-            # We good, use the sensor id
-            debug_log("post_create_member - option 1")
-            return self._send_url_post_request(
-                post_url, self._your_api_write_key, {"sensor_id": str(sensor_id)}
-            )
-
-        elif (
-            sensor_index is not None
-            and sensor_id is None
-            and owner_email is None
-            and location_type is None
-        ):
-            # We good, use the sensor index
-            debug_log("post_create_member - option 2")
-            return self._send_url_post_request(
-                post_url, self._your_api_write_key, {"sensor_index": sensor_index}
-            )
-
-        elif sensor_index is None and sensor_id is not None and owner_email is not None:
-            # We good, use the private sensor id.
-            debug_log("post_create_member - option 3")
-            return self._send_url_post_request(
-                post_url,
-                self._your_api_write_key,
-                {
-                    "sensor_id": str(sensor_id),
-                    "owner_email": owner_email,
-                    "location_type": location_type,
-                },
-            )
-
-        else:
-            raise PurpleAirAPIError("Invalid configuration of method parameters!")
-
-    def post_delete_group(self, group_id):
-        """
-        A method to delete a group for sensors.
-
-        :param int group_id: The group_id of the group to delete
-        """
-
-        post_url = self._base_api_v1_request_string + f"groups/{group_id}"
-
-        return self._send_url_delete_request(post_url, self._your_api_write_key)
-
-    def post_delete_member(self, group_id, member_id):
-        """
-        :param int group_id: The group_id of the group in which member_id is in.
-        :param int member_id: The member_id to delete.
-        """
-
-        post_url = (
-            self._base_api_v1_request_string + f"groups/{group_id}/members/{member_id}"
-        )
-
-        return self._send_url_delete_request(post_url, self._your_api_write_key)
-
-    def _send_url_get_request(
-        self,
-        request_url,
-        api_key_to_use,
-        first_optional_parameter_separator=None,
-        optional_parameters_dict=None,
-    ):
-        """
-        A class helper to send the url request. It can also add onto the
-        'request_url' string if 'optional_parameters_dict' are provided.
-
-        :param str request_url: The constructed string url request string.
-        :param str first_optional_parameter_separator: The separator between first parameter
-                                                       in optional_parameters_dict. i.e '?' or '&'.
-        :param dict optional_parameters_dict: Optional parameters that can be added onto the
-                                              request_url.
-        """
-
-        if optional_parameters_dict is not None:
-            if first_optional_parameter_separator not in ["?", "&"]:
-                raise PurpleAirAPIError(
-                    f"Invalid `first_optional_parameter_separator: {first_optional_parameter_separator}` passed into `_send_url_get_request`!"
-                )
-
-            opt_param_count = 0
-            for opt_param, val in optional_parameters_dict.items():
-                if val is not None:
-                    opt_param_count = opt_param_count + 1
-
-                    if opt_param_count == 1:
-                        request_url = (
-                            request_url
-                            + f"{first_optional_parameter_separator}{opt_param}={str(val)}"
-                        )
-
-                    elif opt_param_count >= 2:
-                        request_url = request_url + f"&{opt_param}={str(val)}"
-
-        # Strip any quotes that might persist
-        request_url = request_url.replace('"', "")
-        # Strip away any whitespace that might persist
-        request_url = request_url.replace(" ", "")
-        debug_log(request_url)
-        my_request = None
-        my_request = requests.get(
-            request_url, headers={"X-API-Key": str(api_key_to_use)}
-        )
-
-        the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
-
-        if self._verify_request_status_codes(my_request.status_code):
-            my_request.close()
-            del my_request
-            return the_request_text_as_json
-
-        else:
-            raise PurpleAirAPIError(
-                f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
-            )
-
-    def _send_url_post_request(
-        self, request_url, api_key_to_use, json_post_parameters={}
-    ):
-        """
-        A class helper to send the url request. It can also add onto the
-        'request_url' string if 'optional_parameters_dict' are provided.
-
-        :param str request_url: The constructed string url request string.
-        """
-
-        debug_log(request_url)
-        my_request = None
-        if json_post_parameters:
-            debug_log(json_post_parameters)
-            my_request = requests.post(
-                request_url,
-                headers={"X-API-Key": str(api_key_to_use)},
-                json=json_post_parameters,
-            )
-
-        else:
-            debug_log(json_post_parameters)
-            my_request = requests.post(
-                request_url, headers={"X-API-Key": str(api_key_to_use)}
-            )
-
-        the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
-
-        if self._verify_request_status_codes(my_request.status_code):
-            my_request.close()
-            del my_request
-            return the_request_text_as_json
-
-        else:
-            raise PurpleAirAPIError(
-                f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
-            )
-
-    def _send_url_delete_request(
-        self, request_url, api_key_to_use, json_post_parameters={}
-    ):
-        """
-        A class helper to send the url request. It can also add onto the
-        'request_url' string if 'optional_parameters_dict' are provided.
-
-        :param str request_url: The constructed string url request string.
-        """
-
-        debug_log(request_url)
-        my_request = None
-        if json_post_parameters:
-            my_request = requests.delete(
-                request_url,
-                headers={"X-API-Key": str(api_key_to_use)},
-                json=json_post_parameters,
-            )
-
-        else:
-            my_request = requests.delete(
-                request_url, headers={"X-API-Key": str(api_key_to_use)}
-            )
-
-        the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
-
-        if self._verify_request_status_codes(my_request.status_code):
-            my_request.close()
-            del my_request
-            return the_request_text_as_json
-
-        else:
-            raise PurpleAirAPIError(
-                f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
-            )
-
-    @staticmethod
-    def _verify_request_status_codes(status_code) -> bool:
-        """
-        A helper to check those status codes.
-        True if in SUCCESS_CODE_LIST
-        False if in ERROR_CODES_LIST
-        """
-
-        if status_code in SUCCESS_CODE_LIST:
-            return True
-
-        elif status_code in ERROR_CODES_LIST:
-            return False
-
-    @staticmethod
-    def _convert_requests_text_to_json(text=None) -> dict:
-        """
-        A helper to convert request.text to json.
-
-        :param str text: The request.txt to convert to json
-
-        :return dict
-        """
-
-        the_request_text_as_json = None
-        if text:
-            debug_log(f"_convert_requests_text_to_json - text: {text}")
-            the_request_text_as_json = json.loads(text)
-            debug_log(
-                f"_convert_requests_text_to_json - json: {the_request_text_as_json}"
-            )
-
-        return the_request_text_as_json
-
-    @staticmethod
-    def _sanitize_sensor_data_from_paa(paa_return_data) -> dict:
-        """
-        A helper method.
-        Since not all sensors support all field names we check that the keys exist
-        in the sensor data. If they do not exist we add it in with a NULL
-        equivalent. i.e 0.0, 0, "", etc.
-        We access the "sensor" key inside this method.
-
-        :param dict paa_return_data: A dictionary with paa return data
-        """
-
-        for key_str in ACCEPTED_FIELD_NAMES_DICT.keys():
-            if key_str not in paa_return_data["sensor"].keys():
-                paa_return_data["sensor"][key_str] = ACCEPTED_FIELD_NAMES_DICT[key_str]
-
-        return paa_return_data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPIConstants.py` & `purpleair_api-1.1.0a1/purpleair_api/PurpleAirAPIConstants.py`

 * *Files identical despite different names*

### Comparing `purpleair_api-1.0.2a1/purpleair_api.egg-info/PKG-INFO` & `purpleair_api-1.1.0a1/purpleair_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpleair-api
-Version: 1.0.2a1
+Version: 1.1.0a1
 Home-page: https://github.com/carlkidcrypto/purpleair_api
 Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_api,purple air api,purple_air,purple air
 Platform: Windows 32/64
 Platform: Linux 32/64
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: purpleair-api Version: 1.0.2a1 Home-page: https://
+Metadata-Version: 2.1 Name: purpleair-api Version: 1.1.0a1 Home-page: https://
 github.com/carlkidcrypto/purpleair_api Author: Carlos Santos Author-email:
 dose.lucky.sake@cloak.id License: MIT Keywords: purpleair_api,purple air
 api,purple_air,purple air Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE # purple_air_api (PAA) This is a python3 wrapper
 for the new PurpleAirAPI (PAA). Details of the API can be found using this
 link:
```

### Comparing `purpleair_api-1.0.2a1/setup.py` & `purpleair_api-1.1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         os.path.join(os.path.dirname(__file__), filename), encoding="utf-8"
     ) as file:
         return file.read()
 
 
 setup(
     name="purpleair_api",
-    version="1.0.2a1",
+    version="1.1.0a1",
     license="MIT",
     author="Carlos Santos",
     author_email="dose.lucky.sake@cloak.id",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     packages=["purpleair_api"],
     url="https://github.com/carlkidcrypto/purpleair_api",
```

