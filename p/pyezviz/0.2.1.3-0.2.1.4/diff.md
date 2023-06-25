# Comparing `tmp/pyezviz-0.2.1.3.tar.gz` & `tmp/pyezviz-0.2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.3.tar", last modified: Sun Jun 25 09:29:05 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.4.tar", last modified: Sun Jun 25 11:59:05 2023, max compression
```

## Comparing `pyezviz-0.2.1.3.tar` & `pyezviz-0.2.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    58799 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:29:05.000000 pyezviz-0.2.1.3/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:29:05.633178 pyezviz-0.2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 09:28:51.000000 pyezviz-0.2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.733543 pyezviz-0.2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59673 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:59:05.729543 pyezviz-0.2.1.4/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 11:59:05.000000 pyezviz-0.2.1.4/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:59:05.733543 pyezviz-0.2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 11:58:56.000000 pyezviz-0.2.1.4/setup.py
```

### Comparing `pyezviz-0.2.1.3/LICENSE.md` & `pyezviz-0.2.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/README.md` & `pyezviz-0.2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/__init__.py` & `pyezviz-0.2.1.4/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/__main__.py` & `pyezviz-0.2.1.4/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.4/pyezviz/api_endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 API_ENDPOINT_DETECTION_SENSIBILITY = "/api/device/configAlgorithm"
 API_ENDPOINT_DETECTION_SENSIBILITY_GET = "/api/device/queryAlgorithmConfig"
 API_ENDPOINT_SET_DEFENCE_SCHEDULE = "/api/device/defence/plan2"
 API_ENDPOINT_CAM_ENCRYPTKEY = "/api/device/query/encryptkey"
 API_ENDPOINT_CANCEL_ALARM = "/api/device/cancelAlarm"
 API_ENDPOINT_DEVICE_SYS_OPERATION = "/api/device/v2/sysOper/"
+API_ENDPOINT_DEVICE_STORAGE_STATUS = "/api/device/queryStorageStatus"
 API_ENDPOINT_DEVCONFIG_BY_KEY = "/v3/devconfig/v1/keyValue/"
 
 # Videogo DeviceApi
 API_ENDPOINT_DEVICES = "/v3/devices/"
 API_ENDPOINT_SWITCH_STATUS = "/switchStatus"
 API_ENDPOINT_SWITCH_OTHER = "/switch"
 API_ENDPOINT_PTZCONTROL = "/ptzControl"
```

### Comparing `pyezviz-0.2.1.3/pyezviz/camera.py` & `pyezviz-0.2.1.4/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/cas.py` & `pyezviz-0.2.1.4/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/client.py` & `pyezviz-0.2.1.4/pyezviz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     API_ENDPOINT_CAM_ENCRYPTKEY,
     API_ENDPOINT_CANCEL_ALARM,
     API_ENDPOINT_CHANGE_DEFENCE_STATUS,
     API_ENDPOINT_CREATE_PANORAMIC,
     API_ENDPOINT_DETECTION_SENSIBILITY,
     API_ENDPOINT_DETECTION_SENSIBILITY_GET,
     API_ENDPOINT_DEVCONFIG_BY_KEY,
+    API_ENDPOINT_DEVICE_STORAGE_STATUS,
     API_ENDPOINT_DEVICE_SYS_OPERATION,
     API_ENDPOINT_DEVICES,
     API_ENDPOINT_DO_NOT_DISTURB,
     API_ENDPOINT_GROUP_DEFENCE_MODE,
     API_ENDPOINT_LOGIN,
     API_ENDPOINT_LOGOUT,
     API_ENDPOINT_PAGELIST,
@@ -281,17 +282,14 @@
             if err.response.status_code == 401:
                 # session is wrong, need to relogin
                 self.login()
                 return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
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
@@ -305,27 +303,15 @@
             _LOGGER.warning(
                 "Could not get pagelist, relogging (max retries: %s), got: %s",
                 str(max_retries),
                 json_output["meta"],
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
-        if json_key is None:
-            json_result = json_output
-        else:
-            json_result = json_output[json_key]
-
-        if not json_result:
-            # session is wrong, need to relogin
-            self.login()
-            _LOGGER.warning(
-                "Impossible to load the devices, here is the returned response: %s",
-                str(req.text),
-            )
-            return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
+        json_result = json_output if not json_key else json_output[json_key]
 
         return json_result
 
     def get_alarminfo(self, serial: str, limit: int = 1, max_retries: int = 0) -> dict:
         """Get data from alarm info API for camera serial."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
@@ -719,14 +705,54 @@
         if json_output["meta"]["code"] != 200:
             raise PyEzvizError(
                 f'Could not initiate firmare upgrade: Got {json_output["meta"]})'
             )
 
         return True
 
+    def get_storage_status(self, serial: str, max_retries: int = 0) -> Any:
+        """Get device storage status."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                url=f"https://{self._token['api_url']}{API_ENDPOINT_DEVICE_STORAGE_STATUS}",
+                data={"subSerial": serial},
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.get_storage_status(serial, max_retries + 1)
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
+            raise PyEzvizError(
+                f"Could not get device storage status: Got {json_output})"
+            )
+
+        return json_output["storageStatus"]
+
     def sound_alarm(self, serial: str, enable: int = 1, max_retries: int = 0) -> bool:
         """Sound alarm on a device."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.put(
```

### Comparing `pyezviz-0.2.1.3/pyezviz/constants.py` & `pyezviz-0.2.1.4/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/exceptions.py` & `pyezviz-0.2.1.4/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/mqtt.py` & `pyezviz-0.2.1.4/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.4/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/pyezviz/utils.py` & `pyezviz-0.2.1.4/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.3/setup.py` & `pyezviz-0.2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.3",
+    version="0.2.1.4",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

