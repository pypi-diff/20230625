# Comparing `tmp/pyezviz-0.2.1.2.tar.gz` & `tmp/pyezviz-0.2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.2.tar", last modified: Sun Jun 18 17:17:33 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.3.tar", last modified: Sun Jun 25 09:29:05 2023, max compression
```

## Comparing `pyezviz-0.2.1.2.tar` & `pyezviz-0.2.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.994405 pyezviz-0.2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    53961 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:17:33.994405 pyezviz-0.2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58799 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/setup.py
```

### Comparing `pyezviz-0.2.1.2/LICENSE.md` & `pyezviz-0.2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/README.md` & `pyezviz-0.2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/__init__.py` & `pyezviz-0.2.1.3/pyezviz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .cas import EzvizCAS
 from .client import EzvizClient
 from .constants import (
     BatteryCameraWorkMode,
     DefenseModeType,
     DeviceCatagories,
     DeviceSwitchType,
+    DisplayMode,
     IntelligentDetectionMode,
     MessageFilterType,
     NightVisionMode,
     SoundMode,
     SupportExt,
 )
 from .exceptions import (
@@ -36,14 +37,15 @@
     "EzvizAuthTokenExpired",
     "EzvizAuthVerificationCode",
     "EzvizCAS",
     "MQTTClient",
     "DefenseModeType",
     "IntelligentDetectionMode",
     "BatteryCameraWorkMode",
+    "DisplayMode",
     "NightVisionMode",
     "MessageFilterType",
     "DeviceCatagories",
     "DeviceSwitchType",
     "SupportExt",
     "SoundMode",
     "TestRTSPAuth",
```

### Comparing `pyezviz-0.2.1.2/pyezviz/__main__.py` & `pyezviz-0.2.1.3/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.3/pyezviz/api_endpoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 API_ENDPOINT_SWITCH_DEFENCE_MODE = "/v3/userdevices/v1/group/switchDefenceMode"
 
 API_ENDPOINT_DETECTION_SENSIBILITY = "/api/device/configAlgorithm"
 API_ENDPOINT_DETECTION_SENSIBILITY_GET = "/api/device/queryAlgorithmConfig"
 API_ENDPOINT_SET_DEFENCE_SCHEDULE = "/api/device/defence/plan2"
 API_ENDPOINT_CAM_ENCRYPTKEY = "/api/device/query/encryptkey"
 API_ENDPOINT_CANCEL_ALARM = "/api/device/cancelAlarm"
-
+API_ENDPOINT_DEVICE_SYS_OPERATION = "/api/device/v2/sysOper/"
 API_ENDPOINT_DEVCONFIG_BY_KEY = "/v3/devconfig/v1/keyValue/"
 
 # Videogo DeviceApi
 API_ENDPOINT_DEVICES = "/v3/devices/"
 API_ENDPOINT_SWITCH_STATUS = "/switchStatus"
+API_ENDPOINT_SWITCH_OTHER = "/switch"
 API_ENDPOINT_PTZCONTROL = "/ptzControl"
 API_ENDPOINT_ALARM_SOUND = "/alarm/sound"
 API_ENDPOINT_SWITCH_SOUND_ALARM = "/sendAlarm"
 API_ENDPOINT_DO_NOT_DISTURB = "/nodisturb"
 API_ENDPOINT_VIDEO_ENCRYPT = "encryptedInfo/risk"
+API_ENDPOINT_CHANGE_DEFENCE_STATUS = "changeDefenceStatusReq"
 
 API_ENDPOINT_CREATE_PANORAMIC = "/api/panoramic/devices/pics/collect"
 API_ENDPOINT_RETURN_PANORAMIC = "/api/panoramic/devices/pics"
 
 # MQTT
 API_ENDPOINT_REGISTER_MQTT = "/v1/getClientId"
 API_ENDPOINT_START_MQTT = "/api/push/start"
```

### Comparing `pyezviz-0.2.1.2/pyezviz/camera.py` & `pyezviz-0.2.1.3/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/cas.py` & `pyezviz-0.2.1.3/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/client.py` & `pyezviz-0.2.1.3/pyezviz/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 import requests
 
 from .api_endpoints import (
     API_ENDPOINT_ALARM_SOUND,
     API_ENDPOINT_ALARMINFO_GET,
     API_ENDPOINT_CAM_ENCRYPTKEY,
     API_ENDPOINT_CANCEL_ALARM,
+    API_ENDPOINT_CHANGE_DEFENCE_STATUS,
     API_ENDPOINT_CREATE_PANORAMIC,
     API_ENDPOINT_DETECTION_SENSIBILITY,
     API_ENDPOINT_DETECTION_SENSIBILITY_GET,
     API_ENDPOINT_DEVCONFIG_BY_KEY,
+    API_ENDPOINT_DEVICE_SYS_OPERATION,
     API_ENDPOINT_DEVICES,
     API_ENDPOINT_DO_NOT_DISTURB,
     API_ENDPOINT_GROUP_DEFENCE_MODE,
     API_ENDPOINT_LOGIN,
     API_ENDPOINT_LOGOUT,
     API_ENDPOINT_PAGELIST,
     API_ENDPOINT_PANORAMIC_DEVICES_OPERATION,
@@ -31,14 +33,15 @@
     API_ENDPOINT_REFRESH_SESSION_ID,
     API_ENDPOINT_RETURN_PANORAMIC,
     API_ENDPOINT_SEND_CODE,
     API_ENDPOINT_SERVER_INFO,
     API_ENDPOINT_SET_DEFENCE_SCHEDULE,
     API_ENDPOINT_SET_LUMINANCE,
     API_ENDPOINT_SWITCH_DEFENCE_MODE,
+    API_ENDPOINT_SWITCH_OTHER,
     API_ENDPOINT_SWITCH_SOUND_ALARM,
     API_ENDPOINT_SWITCH_STATUS,
     API_ENDPOINT_UNIFIEDMSG_LIST_GET,
     API_ENDPOINT_UPGRADE_DEVICE,
     API_ENDPOINT_USER_ID,
     API_ENDPOINT_V3_ALARMS,
     API_ENDPOINT_VIDEO_ENCRYPT,
@@ -202,17 +205,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not request MFA code: Got {req.status_code} : {req.text})"
+                f'Could not request MFA code: Got {json_output["meta"]})'
             )
 
         return True
 
     def get_service_urls(self) -> Any:
         """Get Ezviz service urls."""
 
@@ -242,15 +245,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(f"Error getting Service URLs: {json_output['meta']}")
 
         service_urls = json_output["systemConfigInfo"]
         service_urls["sysConf"] = service_urls["sysConf"].split("|")
 
         return service_urls
 
@@ -292,31 +295,33 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             # session is wrong, need to relogin
             self.login()
-            logging.info(
-                "Json request error, relogging (max retries: %s)", str(max_retries)
+            _LOGGER.warning(
+                "Could not get pagelist, relogging (max retries: %s), got: %s",
+                str(max_retries),
+                json_output["meta"],
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
         if json_key is None:
             json_result = json_output
         else:
             json_result = json_output[json_key]
 
         if not json_result:
             # session is wrong, need to relogin
             self.login()
-            logging.info(
+            _LOGGER.warning(
                 "Impossible to load the devices, here is the returned response: %s",
                 str(req.text),
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
         return json_result
 
@@ -359,16 +364,16 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
-            if json_output["meta"].get("code") == 500:
+        if json_output["meta"]["code"] != 200:
+            if json_output["meta"]["code"] == 500:
                 _LOGGER.debug(
                     "Retry getting alarm info, server returned busy: %s",
                     json_output["meta"],
                 )
                 return self.get_alarminfo(serial, limit, max_retries + 1)
 
             raise PyEzvizError(
@@ -429,69 +434,166 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f"Could not get unified message list: Got {json_output['meta']})"
             )
 
         return json_output
 
-    def _switch_status(
+    def switch_status(
         self, serial: str, status_type: int, enable: int, max_retries: int = 0
     ) -> bool:
-        """Switch status on a device."""
+        """Camera features are represented as switches. Switch them on or off."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
+        channel_no = 0
+
         try:
             req = self._session.put(
-                "https://"
-                + self._token["api_url"]
-                + API_ENDPOINT_DEVICES
-                + serial
-                + "/1/1/"
-                + str(status_type)
-                + API_ENDPOINT_SWITCH_STATUS,
-                data={
+                url=f"https://{self._token['api_url']}{API_ENDPOINT_DEVICES}{serial}/{channel_no}/{enable}/{status_type}{API_ENDPOINT_SWITCH_STATUS}",
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.switch_status(serial, status_type, enable, max_retries + 1)
+
+            raise HTTPError from err
+
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
+        if json_output["meta"]["code"] != 200:
+            raise PyEzvizError(f'Could not set the switch: Got {json_output["meta"]})')
+
+        return True
+
+    def switch_status_other(
+        self,
+        serial: str,
+        status_type: int,
+        enable: int,
+        channel_number: int = 1,
+        max_retries: int = 0,
+    ) -> bool:
+        """Features are represented as switches. This api is for alternative switch types to turn them on or off.
+
+        All day recording is a good example.
+        """
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.put(
+                url=f"https://{self._token['api_url']}{API_ENDPOINT_DEVICES}{serial}{API_ENDPOINT_SWITCH_OTHER}",
+                timeout=self._timeout,
+                params={
+                    "channelNo": channel_number,
                     "enable": enable,
-                    "serial": serial,
-                    "channelNo": "1",
-                    "type": status_type,
+                    "switchType": status_type,
                 },
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.switch_status_other(
+                    serial, status_type, enable, channel_number, max_retries + 1
+                )
+
+            raise HTTPError from err
+
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
+        if json_output["meta"]["code"] != 200:
+            raise PyEzvizError(f'Could not set the switch: Got {json_output["meta"]})')
+
+        return True
+
+    def set_camera_defence(
+        self,
+        serial: str,
+        enable: int,
+        channel_no: int = 1,
+        arm_type: str = "Global",
+        actor: str = "V",
+        max_retries: int = 0,
+    ) -> bool:
+        """Enable/Disable motion detection on camera."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.put(
+                url=f"https://{self._token['api_url']}{API_ENDPOINT_DEVICES}{serial}/{channel_no}/{API_ENDPOINT_CHANGE_DEFENCE_STATUS}",
                 timeout=self._timeout,
+                data={
+                    "type": arm_type,
+                    "status": enable,
+                    "actor": actor,
+                },
             )
 
             req.raise_for_status()
 
         except requests.HTTPError as err:
             if err.response.status_code == 401:
                 # session is wrong, need to relogin
                 self.login()
-                return self._switch_status(serial, status_type, enable, max_retries + 1)
+                return self.set_camera_defence(serial, enable, max_retries + 1)
 
             raise HTTPError from err
 
         try:
             json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
-            raise PyEzvizError(f"Could not set the switch: Got {json_output})")
+        if json_output["meta"]["code"] != 200:
+            raise PyEzvizError(
+                f'Could not arm or disarm Camera: Got {json_output["meta"]})'
+            )
 
         return True
 
     def set_battery_camera_work_mode(self, serial: str, value: int) -> bool:
         """Set battery camera work mode."""
         return self.set_device_config_by_key(serial, value, key="batteryCameraWorkMode")
 
@@ -507,14 +609,20 @@
         """Set night vision mode."""
         return self.set_device_config_by_key(
             serial,
             value=f'{{"graphicType":{mode},"luminance":{luminance}}}',
             key="NightVision_Model",
         )
 
+    def set_display_mode(self, serial: str, mode: int) -> bool:
+        """Change video color and saturation mode."""
+        return self.set_device_config_by_key(
+            serial, value=f'{{"mode":{mode}}}', key="display_mode"
+        )
+
     def set_device_config_by_key(
         self,
         serial: str,
         value: Any,
         key: str = "batteryCameraWorkMode",
         max_retries: int = 0,
     ) -> bool:
@@ -561,15 +669,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f"Could not set camera work mode: Got {json_output['meta']})"
             )
 
         return True
 
     def upgrade_device(self, serial: str, max_retries: int = 0) -> bool:
@@ -604,17 +712,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not initiate firmare upgrade: Got {req.status_code} : {req.text})"
+                f'Could not initiate firmare upgrade: Got {json_output["meta"]})'
             )
 
         return True
 
     def sound_alarm(self, serial: str, enable: int = 1, max_retries: int = 0) -> bool:
         """Sound alarm on a device."""
         if max_retries > MAX_RETRIES:
@@ -651,17 +759,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not set the alarm sound: Got {req.status_code} : {req.text})"
+                f'Could not set the alarm sound: Got {json_output["meta"]})'
             )
 
         return True
 
     def get_user_id(self, max_retries: int = 0) -> Any:
         """Get Ezviz userid, used by restricted api endpoints."""
 
@@ -690,15 +798,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f"Could not set video encryption: Got {json_output['meta']})"
             )
 
         return json_output["deviceTokenInfo"]
 
     def set_video_enc(
@@ -767,21 +875,74 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f"Could not set video encryption: Got {json_output['meta']})"
             )
 
         return True
 
+    def reboot_camera(
+        self,
+        serial: str,
+        delay: int = 1,
+        operation: int = 1,
+        max_retries: int = 0,
+    ) -> bool:
+        """Reboot camera."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                url=f'https://{self._token["api_url"]}{API_ENDPOINT_DEVICE_SYS_OPERATION}{serial}',
+                data={
+                    "oper": operation,
+                    "deviceSerial": serial,
+                    "delay": delay,
+                },
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.reboot_camera(
+                    serial,
+                    delay,
+                    operation,
+                    max_retries + 1,
+                )
+
+            raise HTTPError from err
+
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
+        if json_output["resultCode"] != "0":
+            raise PyEzvizError(f"Could not reboot device {json_output})")
+
+        return True
+
     def get_group_defence_mode(self, max_retries: int = 0) -> Any:
         """Get group arm status. The alarm arm/disarm concept on 1st page of app."""
 
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
@@ -810,15 +971,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f"Could not get group defence status: Got {json_output['meta']})"
             )
 
         return json_output["mode"]
 
     # Not tested
@@ -851,17 +1012,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not cancel alarm siren: Got {req.status_code} : {req.text})"
+                f'Could not cancel alarm siren: Got {json_output["meta"]})'
             )
 
         return True
 
     def load_cameras(self) -> dict[Any, Any]:
         """Load and return all cameras objects."""
 
@@ -1176,29 +1337,29 @@
                 raise PyEzvizError(
                     "Impossible to decode response: "
                     + str(err)
                     + "\nResponse was: "
                     + str(req.text)
                 ) from err
 
-            if json_result["meta"].get("code") == 200:
+            if json_result["meta"]["code"] == 200:
                 self._session.headers["sessionId"] = json_result["sessionInfo"][
                     "sessionId"
                 ]
                 self._token["session_id"] = str(json_result["sessionInfo"]["sessionId"])
                 self._token["rf_session_id"] = str(
                     json_result["sessionInfo"]["refreshSessionId"]
                 )
 
                 if not self._token.get("service_urls"):
                     self._token["service_urls"] = self.get_service_urls()
 
                 return self._token
 
-            if json_result["meta"].get("code") == 403:
+            if json_result["meta"]["code"] == 403:
                 if self.account and self.password:
                     self._token = {
                         "session_id": None,
                         "rf_session_id": None,
                         "username": None,
                         "api_url": self._token["api_url"],
                     }
@@ -1239,17 +1400,17 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         self.close_session()
 
-        return bool(json_result["meta"].get("code") == 200)
+        return bool(json_result["meta"]["code"] == 200)
 
-    def set_camera_defence(self, serial: str, enable: int) -> bool:
+    def set_camera_defence_old(self, serial: str, enable: int) -> bool:
         """Enable/Disable motion detection on camera."""
         cas_client = EzvizCAS(self._token)
         cas_client.set_camera_defence_state(serial, enable)
 
         return True
 
     def api_set_defence_schedule(
@@ -1304,15 +1465,15 @@
             raise PyEzvizError(
                 f"Could not set the schedule: Got {req.status_code} : {req.text})"
             )
 
         return True
 
     def api_set_defence_mode(self, mode: DefenseModeType, max_retries: int = 0) -> bool:
-        """Set defence mode."""
+        """Set defence mode for all devices. The alarm panel from main page is used."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.post(
                 "https://" + self._token["api_url"] + API_ENDPOINT_SWITCH_DEFENCE_MODE,
                 data={
@@ -1339,17 +1500,17 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not set defence mode: Got {req.status_code} : {req.text})"
+                f'Could not set defence mode: Got {json_output["meta"]})'
             )
 
         return True
 
     def do_not_disturb(
         self,
         serial: str,
@@ -1385,17 +1546,17 @@
 
         try:
             json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
-        if json_output["meta"].get("code") != 200:
+        if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
-                f"Could not set defence mode: Got {req.status_code} : {req.text})"
+                f'Could not set defence mode: Got {json_output["meta"]})'
             )
 
         return True
 
     def set_floodlight_brightness(
         self,
         serial: str,
@@ -1442,15 +1603,15 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["meta"]["code"] != 200:
-            _LOGGER.error(response_json)
+            _LOGGER.error("Unable to set brightness, got: %s", response_json["meta"])
             return False
 
         return True
 
     def detection_sensibility(
         self,
         serial: str,
@@ -1587,18 +1748,14 @@
                 self.login()
                 return self.alarm_sound(serial, sound_type, enable, max_retries + 1)
 
             raise HTTPError from err
 
         return True
 
-    def switch_status(self, serial: str, status_type: int, enable: int = 0) -> bool:
-        """Switch status of a device."""
-        return self._switch_status(serial, status_type, enable)
-
     def _get_page_list(self) -> Any:
         """Get ezviz device info broken down in sections."""
         return self._api_get_pagelist(
             page_filter="CLOUD, TIME_PLAN, CONNECTION, SWITCH,"
             "STATUS, WIFI, NODISTURB, KMS,"
             "P2P, TIME_PLAN, CHANNEL, VTM, DETECTOR,"
             "FEATURE, CUSTOM_TAG, UPGRADE, VIDEO_QUALITY,"
```

### Comparing `pyezviz-0.2.1.2/pyezviz/constants.py` & `pyezviz-0.2.1.3/pyezviz/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,14 +344,23 @@
 
     NIGHT_VISION_COLOUR = 1
     NIGHT_VISION_B_W = 0
     NIGHT_VISION_SMART = 2
 
 
 @unique
+class DisplayMode(Enum):
+    """Display modes or image styles."""
+
+    DISPLAY_MODE_ORIGINAL = 1
+    DISPLAY_MODE_SOFT = 2
+    DISPLAY_MODE_VIVID = 3
+
+
+@unique
 class BatteryCameraWorkMode(Enum):
     """Battery camera work modes."""
 
     BATTERY_WORK_MODE_PLUGGED_IN = 2
     BATTERY_WORK_MODE_HIGH_PERFORM = 1
     BATTERY_WORK_MODE_POWER_SAVING = 0
     BATTERY_WORK_MODE_SUPER_POWER_SAVE = 3
```

### Comparing `pyezviz-0.2.1.2/pyezviz/exceptions.py` & `pyezviz-0.2.1.3/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/mqtt.py` & `pyezviz-0.2.1.3/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.3/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/pyezviz/utils.py` & `pyezviz-0.2.1.3/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.2/setup.py` & `pyezviz-0.2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.2",
+    version="0.2.1.3",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

