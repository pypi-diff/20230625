# Comparing `tmp/pyezviz-0.2.1.4.tar.gz` & `tmp/pyezviz-0.2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.4.tar", last modified: Sun Jun 25 11:59:05 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.5.tar", last modified: Sun Jun 25 18:27:08 2023, max compression
```

## Comparing `pyezviz-0.2.1.4.tar` & `pyezviz-0.2.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.733543 pyezviz-0.2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    59673 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:59:05.733543 pyezviz-0.2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.119688 pyezviz-0.2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:27:08.119688 pyezviz-0.2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/setup.py
```

### Comparing `pyezviz-0.2.1.4/LICENSE.md` & `pyezviz-0.2.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/README.md` & `pyezviz-0.2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/__init__.py` & `pyezviz-0.2.1.5/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/__main__.py` & `pyezviz-0.2.1.5/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.5/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/camera.py` & `pyezviz-0.2.1.5/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/cas.py` & `pyezviz-0.2.1.5/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/client.py` & `pyezviz-0.2.1.5/pyezviz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 data=payload,
                 timeout=self._timeout,
             )
 
             req.raise_for_status()
 
         except requests.ConnectionError as err:
-            raise InvalidURL("A Invalid URL or Proxy error occured") from err
+            raise InvalidURL("A Invalid URL or Proxy error occurred") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
         try:
             json_result = req.json()
 
@@ -207,17 +207,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not request MFA code: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not request MFA code: Got {json_output})")
 
         return True
 
     def get_service_urls(self) -> Any:
         """Get Ezviz service urls."""
 
         if not self._token["session_id"]:
@@ -227,35 +225,32 @@
             req = self._session.get(
                 f"https://{self._token['api_url']}{API_ENDPOINT_SERVER_INFO}",
                 timeout=self._timeout,
             )
             req.raise_for_status()
 
         except requests.ConnectionError as err:
-            raise InvalidURL("A Invalid URL or Proxy error occured") from err
+            raise InvalidURL("A Invalid URL or Proxy error occurred") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
-        if not req.text:
-            raise PyEzvizError("No data")
-
         try:
             json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(f"Error getting Service URLs: {json_output['meta']}")
+            raise PyEzvizError(f"Error getting Service URLs: {json_output}")
 
         service_urls = json_output["systemConfigInfo"]
         service_urls["sysConf"] = service_urls["sysConf"].split("|")
 
         return service_urls
 
     def _api_get_pagelist(
@@ -299,15 +294,15 @@
 
         if json_output["meta"]["code"] != 200:
             # session is wrong, need to relogin
             self.login()
             _LOGGER.warning(
                 "Could not get pagelist, relogging (max retries: %s), got: %s",
                 str(max_retries),
-                json_output["meta"],
+                json_output,
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
         json_result = json_output if not json_key else json_output[json_key]
 
         return json_result
 
@@ -336,17 +331,14 @@
             if err.response.status_code == 401:
                 # session is wrong, need to relogin
                 self.login()
                 return self.get_alarminfo(serial, limit, max_retries + 1)
 
             raise HTTPError from err
 
-        if req.text == "":
-            raise PyEzvizError("No data")
-
         try:
             json_output: dict = req.json()
 
         except ValueError as err:
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
@@ -354,21 +346,19 @@
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
             if json_output["meta"]["code"] == 500:
                 _LOGGER.debug(
                     "Retry getting alarm info, server returned busy: %s",
-                    json_output["meta"],
+                    json_output,
                 )
                 return self.get_alarminfo(serial, limit, max_retries + 1)
 
-            raise PyEzvizError(
-                f"Could not get data from alarm api: Got {json_output['meta']})"
-            )
+            raise PyEzvizError(f"Could not get data from alarm api: Got {json_output})")
 
         return json_output
 
     def get_device_messages_list(
         self,
         serials: str | None = None,
         s_type: int = MessageFilterType.FILTER_TYPE_ALL_ALARM.value,
@@ -406,31 +396,28 @@
                 self.login()
                 return self.get_device_messages_list(
                     serials, s_type, limit, date, end_time, tags, max_retries + 1
                 )
 
             raise HTTPError from err
 
-        if req.text == "":
-            raise PyEzvizError("No data")
-
         try:
             json_output: dict = req.json()
 
         except ValueError as err:
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not get unified message list: Got {json_output['meta']})"
+                f"Could not get unified message list: Got {json_output})"
             )
 
         return json_output
 
     def switch_status(
         self, serial: str, status_type: int, enable: int, max_retries: int = 0
     ) -> bool:
@@ -464,15 +451,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(f'Could not set the switch: Got {json_output["meta"]})')
+            raise PyEzvizError(f"Could not set the switch: Got {json_output})")
 
         return True
 
     def switch_status_other(
         self,
         serial: str,
         status_type: int,
@@ -518,15 +505,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(f'Could not set the switch: Got {json_output["meta"]})')
+            raise PyEzvizError(f"Could not set the switch: Got {json_output})")
 
         return True
 
     def set_camera_defence(
         self,
         serial: str,
         enable: int,
@@ -569,17 +556,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not arm or disarm Camera: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not arm or disarm Camera: Got {json_output})")
 
         return True
 
     def set_battery_camera_work_mode(self, serial: str, value: int) -> bool:
         """Set battery camera work mode."""
         return self.set_device_config_by_key(serial, value, key="batteryCameraWorkMode")
 
@@ -656,17 +641,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f"Could not set camera work mode: Got {json_output['meta']})"
-            )
+            raise PyEzvizError(f"Could not set camera work mode: Got {json_output})")
 
         return True
 
     def upgrade_device(self, serial: str, max_retries: int = 0) -> bool:
         """Upgrade device firmware."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
@@ -700,15 +683,15 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f'Could not initiate firmare upgrade: Got {json_output["meta"]})'
+                f"Could not initiate firmware upgrade: Got {json_output})"
             )
 
         return True
 
     def get_storage_status(self, serial: str, max_retries: int = 0) -> Any:
         """Get device storage status."""
         if max_retries > MAX_RETRIES:
@@ -786,17 +769,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not set the alarm sound: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not set the alarm sound: Got {json_output})")
 
         return True
 
     def get_user_id(self, max_retries: int = 0) -> Any:
         """Get Ezviz userid, used by restricted api endpoints."""
 
         if max_retries > MAX_RETRIES:
@@ -825,17 +806,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f"Could not set video encryption: Got {json_output['meta']})"
-            )
+            raise PyEzvizError(f"Could get user id, Got: {json_output})")
 
         return json_output["deviceTokenInfo"]
 
     def set_video_enc(
         self,
         serial: str,
         enable: int = 1,
@@ -902,17 +881,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f"Could not set video encryption: Got {json_output['meta']})"
-            )
+            raise PyEzvizError(f"Could not set video encryption: Got {json_output})")
 
         return True
 
     def reboot_camera(
         self,
         serial: str,
         delay: int = 1,
@@ -999,15 +976,15 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not get group defence status: Got {json_output['meta']})"
+                f"Could not get group defence status: Got {json_output})"
             )
 
         return json_output["mode"]
 
     # Not tested
     def cancel_alarm_device(self, serial: str, max_retries: int = 0) -> bool:
         """Cacnel alarm on an Alarm device."""
@@ -1039,17 +1016,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not cancel alarm siren: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not cancel alarm siren: Got {json_output})")
 
         return True
 
     def load_cameras(self) -> dict[Any, Any]:
         """Load and return all cameras objects."""
 
         devices = self.get_device_infos()
@@ -1159,15 +1134,28 @@
             )
 
             req.raise_for_status()
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
-        return req.text
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        _LOGGER.debug("PTZ Control: %s", json_output)
+
+        return True
 
     def get_cam_key(
         self, serial: str, smscode: int | None = None, max_retries: int = 0
     ) -> Any:
         """Get Camera encryption key."""
 
         if max_retries > MAX_RETRIES:
@@ -1205,22 +1193,20 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("resultCode") == "20002":
-            raise PyEzvizError(
-                f"MFA code required: Got {req.status_code} : {req.text})"
-            )
+        if json_output["resultCode"] == "20002":
+            raise EzvizAuthVerificationCode(f"MFA code required: Got {json_output})")
 
-        if json_output.get("resultCode") != "0":
+        if json_output["resultCode"] != "0":
             raise PyEzvizError(
-                f"Could not get camera encryption key: Got {req.status_code} : {req.text})"
+                f"Could not get camera encryption key: Got {json_output})"
             )
 
         return json_output
 
     def create_panoramic(self, serial: str, max_retries: int = 0) -> Any:
         """Create panoramic image."""
 
@@ -1251,17 +1237,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("resultCode") != "0":
+        if json_output["resultCode"] != "0":
             raise PyEzvizError(
-                f"Could not send command to create panoramic photo: Got {req.status_code} : {req.text})"
+                f"Could not send command to create panoramic photo: Got {json_output})"
             )
 
         return json_output
 
     def return_panoramic(self, serial: str, max_retries: int = 0) -> Any:
         """Return panoramic image url list."""
 
@@ -1292,18 +1278,16 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("resultCode") != "0":
-            raise PyEzvizError(
-                f"Could retrieve panoramic photo: Got {req.status_code} : {req.text})"
-            )
+        if json_output["resultCode"] != "0":
+            raise PyEzvizError(f"Could retrieve panoramic photo: Got {json_output})")
 
         return json_output
 
     def ptz_control_coordinates(
         self, serial: str, x_axis: float, y_axis: float
     ) -> bool:
         """PTZ Coordinate Move."""
@@ -1331,14 +1315,27 @@
             )
 
             req.raise_for_status()
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
+        try:
+            json_result = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        _LOGGER.debug("PTZ control coordinates: %s", json_result)
+
         return True
 
     def login(self, sms_code: int | None = None) -> dict[Any, Any]:
         """Get or refresh ezviz login token."""
         if self._token["session_id"] and self._token["rf_session_id"]:
             try:
                 req = self._session.put(
@@ -1483,18 +1480,16 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("resultCode") != 0:
-            raise PyEzvizError(
-                f"Could not set the schedule: Got {req.status_code} : {req.text})"
-            )
+        if json_output["resultCode"] != "0":
+            raise PyEzvizError(f"Could not set the schedule: Got {json_output})")
 
         return True
 
     def api_set_defence_mode(self, mode: DefenseModeType, max_retries: int = 0) -> bool:
         """Set defence mode for all devices. The alarm panel from main page is used."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
@@ -1527,28 +1522,26 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not set defence mode: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not set defence mode: Got {json_output})")
 
         return True
 
     def do_not_disturb(
         self,
         serial: str,
         enable: int = 1,
         channelno: int = 1,
         max_retries: int = 0,
     ) -> bool | str:
-        """Set do not disturb on camera with spesified serial."""
+        """Set do not disturb on camera with specified serial."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.put(
                 "https://"
                 + self._token["api_url"]
@@ -1573,17 +1566,15 @@
         try:
             json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(
-                f'Could not set defence mode: Got {json_output["meta"]})'
-            )
+            raise PyEzvizError(f"Could not set defence mode: Got {json_output})")
 
         return True
 
     def set_floodlight_brightness(
         self,
         serial: str,
         luminance: int = 50,
@@ -1629,16 +1620,15 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["meta"]["code"] != 200:
-            _LOGGER.error("Unable to set brightness, got: %s", response_json["meta"])
-            return False
+            raise PyEzvizError(f"Unable to set brightness, got: {response_json}")
 
         return True
 
     def detection_sensibility(
         self,
         serial: str,
         sensibility: int = 3,
@@ -1682,16 +1672,18 @@
 
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
-        if response_json["resultCode"] and response_json["resultCode"] != "0":
-            return "Unknown value"
+        if response_json["resultCode"] != "0":
+            raise PyEzvizError(
+                f"Unable to set detection sensibility. Got: {response_json}"
+            )
 
         return True
 
     def get_detection_sensibility(
         self, serial: str, type_value: str = "0", max_retries: int = 0
     ) -> Any:
         """Get detection sensibility notifications."""
@@ -1724,15 +1716,17 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
-            return None
+            raise PyEzvizError(
+                f"Unable to get detection sensibility. Got: {response_json}"
+            )
 
         if response_json["algorithmConfig"]["algorithmList"]:
             for idx in response_json["algorithmConfig"]["algorithmList"]:
                 if idx["type"] == type_value:
                     return idx["value"]
 
         return None
@@ -1772,14 +1766,22 @@
             if err.response.status_code == 401:
                 # session is wrong, need to re-log-in
                 self.login()
                 return self.alarm_sound(serial, sound_type, enable, max_retries + 1)
 
             raise HTTPError from err
 
+        try:
+            response_json = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError("Could not decode response:" + str(err)) from err
+
+        _LOGGER.debug("Response: %s", response_json)
+
         return True
 
     def _get_page_list(self) -> Any:
         """Get ezviz device info broken down in sections."""
         return self._api_get_pagelist(
             page_filter="CLOUD, TIME_PLAN, CONNECTION, SWITCH,"
             "STATUS, WIFI, NODISTURB, KMS,"
```

### Comparing `pyezviz-0.2.1.4/pyezviz/constants.py` & `pyezviz-0.2.1.5/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/exceptions.py` & `pyezviz-0.2.1.5/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/mqtt.py` & `pyezviz-0.2.1.5/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.5/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/pyezviz/utils.py` & `pyezviz-0.2.1.5/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.4/setup.py` & `pyezviz-0.2.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.4",
+    version="0.2.1.5",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

