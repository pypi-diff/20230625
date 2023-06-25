# Comparing `tmp/airtouch2-0.5b2.tar.gz` & `tmp/airtouch2-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.5b2.tar", last modified: Thu Dec 15 01:46:54 2022, max compression
+gzip compressed data, was "airtouch2-0.7.tar", last modified: Sun Jun 25 08:50:15 2023, max compression
```

## Comparing `airtouch2-0.5b2.tar` & `airtouch2-0.7.tar`

### file list

```diff
@@ -1,32 +1,58 @@
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.603846 airtouch2-0.5b2/
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     1076 2022-04-10 10:18:46.000000 airtouch2-0.5b2/LICENSE
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     2280 2022-12-15 01:46:54.603846 airtouch2-0.5b2/PKG-INFO
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      271 2022-07-19 09:39:17.000000 airtouch2-0.5b2/README.md
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      851 2022-12-14 07:20:54.000000 airtouch2-0.5b2/pyproject.toml
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)       38 2022-12-15 01:46:54.603846 airtouch2-0.5b2/setup.cfg
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.599846 airtouch2-0.5b2/src/
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.599846 airtouch2-0.5b2/src/airtouch2/
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     6950 2022-12-14 01:32:16.000000 airtouch2-0.5b2/src/airtouch2/AT2Aircon.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     6376 2022-12-14 07:19:02.000000 airtouch2-0.5b2/src/airtouch2/AT2Client.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     2940 2022-12-14 01:32:16.000000 airtouch2-0.5b2/src/airtouch2/AT2Group.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)    10223 2022-12-14 01:32:16.000000 airtouch2-0.5b2/src/airtouch2/SyncAT2Client.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      188 2022-12-12 04:49:35.000000 airtouch2-0.5b2/src/airtouch2/__init__.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      541 2022-11-28 07:36:47.000000 airtouch2-0.5b2/src/airtouch2/diff_bytes.py
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.603846 airtouch2-0.5b2/src/airtouch2/protocol/
--rw-r--r--   0 nvdh      (1000) nvdh      (1000)        0 2022-06-29 02:48:21.000000 airtouch2-0.5b2/src/airtouch2/protocol/__init__.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     2458 2022-12-07 11:36:56.000000 airtouch2-0.5b2/src/airtouch2/protocol/constants.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      647 2022-11-30 04:32:30.000000 airtouch2-0.5b2/src/airtouch2/protocol/enums.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      861 2022-11-28 07:36:47.000000 airtouch2-0.5b2/src/airtouch2/protocol/lookups.py
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.603846 airtouch2-0.5b2/src/airtouch2/protocol/messages/
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      708 2022-12-14 02:17:05.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/CommandMessage.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      578 2022-12-14 01:48:17.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/Message.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      428 2022-12-14 02:17:05.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/RequestState.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     3749 2022-12-14 01:34:52.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/ResponseMessage.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      323 2022-12-07 11:36:56.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/__init__.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     2282 2022-12-14 02:17:05.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/ac_commands.py
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     1431 2022-12-14 02:17:05.000000 airtouch2-0.5b2/src/airtouch2/protocol/messages/group_commands.py
-drwxrwxr-x   0 nvdh      (1000) nvdh      (1000)        0 2022-12-15 01:46:54.599846 airtouch2-0.5b2/src/airtouch2.egg-info/
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)     2280 2022-12-15 01:46:54.000000 airtouch2-0.5b2/src/airtouch2.egg-info/PKG-INFO
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)      815 2022-12-15 01:46:54.000000 airtouch2-0.5b2/src/airtouch2.egg-info/SOURCES.txt
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)        1 2022-12-15 01:46:54.000000 airtouch2-0.5b2/src/airtouch2.egg-info/dependency_links.txt
--rw-rw-r--   0 nvdh      (1000) nvdh      (1000)       10 2022-12-15 01:46:54.000000 airtouch2-0.5b2/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2279 2023-06-25 08:50:15.368157 airtouch2-0.7/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      850 2023-06-25 08:46:07.000000 airtouch2-0.7/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-06-25 08:50:15.368157 airtouch2-0.7/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      236 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5462 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3653 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2777 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8229 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2227 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4349 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      307 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/ResponseMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3941 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2279 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1675 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.5b2/LICENSE` & `airtouch2-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.5b2/PKG-INFO` & `airtouch2-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.5b2
+Version: 0.7
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # airtouch2_python
 In-development Python client for the Polyaire AirTouch 2 airconditioning system
 
 ## Thanks to
```

### Comparing `airtouch2-0.5b2/pyproject.toml` & `airtouch2-0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.5b2"
+version = "0.7"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Home Automation",
```

### Comparing `airtouch2-0.5b2/src/airtouch2/AT2Aircon.py` & `airtouch2-0.7/src/airtouch2/at2/At2Aircon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,47 @@
 from __future__ import annotations
+import asyncio
 import logging
 from itertools import compress
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
+from airtouch2.protocol.at2.conversions import brand_from_gateway_id, fan_speed_from_val, supported_fan_speeds, val_from_fan_speed
 if TYPE_CHECKING:
-    from airtouch2.AT2Client import AT2Client
-from airtouch2.protocol.enums import ACFanSpeedReference, ACBrand, ACMode
-from airtouch2.protocol.messages import ChangeSetTemperature, ResponseMessage, SetFanSpeed, SetMode, ToggleAC
-from airtouch2.protocol.lookups import GATEWAYID_BRAND_LOOKUP
-
-OPEN_ISSUE_TEXT = "please open an issue and detail your system to me:\n\thttps://github.com/nathanvdh/airtouch2-python/issues/new"
+    from airtouch2.at2.At2Client import At2Client
+from airtouch2.protocol.at2.enums import ACFanSpeedReference, ACBrand, ACMode
+from airtouch2.protocol.at2.messages import ChangeSetTemperature, ResponseMessage, SetFanSpeed, SetMode, ToggleAc
+from airtouch2.protocol.at2.lookups import GATEWAYID_BRAND_LOOKUP
 
 _LOGGER = logging.getLogger(__name__)
-class AT2Aircon:
-    def __init__(self, number: int, client: AT2Client, response_message: ResponseMessage):
+
+
+class At2Aircon:
+    number: int
+    on: bool
+    safety: bool
+    error: bool
+    turbo: bool
+    spill: bool
+    error_code: int
+    measured_temp: int
+    set_temp: int
+    brand: ACBrand
+    gateway_id: int
+    mode: ACMode
+    supported_fan_speeds: list[ACFanSpeedReference]
+    fan_speed: ACFanSpeedReference
+
+    def __init__(self, number: int, client: At2Client, response_message: ResponseMessage):
         self.number: int = number
-        self._client: AT2Client = client
+        self._client: At2Client = client
+        self._callbacks: list[Callable] = []
         if response_message:
             self.update(response_message)
         else:
             raise ValueError("Null response message provided")
 
-    # TODO: read through app source code more and do this more properly
-    # Currently I'm assuming:
-    #   4 speed is always LOW, MED, HIGH, POWERFUL (EXCEPT for fujitsus with 4 speeds)
-    #   3 speed is always LOW, MED, HIGH
-    #   2 speed is always LOW, HIGH
-    #   Daikins have no Auto
-    #   Gateway ID 0x14 has no Auto
-    #   Gateway IDs 0xFF with 3 speed have no Auto
-    # These are based on the app decompiled code
-    def _set_supported_fan_speeds(self, num_supported_speeds: int, gateway_id: int):
-        all_speeds:list[ACFanSpeedReference] = list(ACFanSpeedReference.__members__.values())
-        if self.brand == ACBrand.FUJITSU and num_supported_speeds == 4:
-            self.supported_fan_speeds = all_speeds[:5]
-            return
-        # Check cases that don't support Auto mode
-        if (self.brand == ACBrand.DAIKIN or (gateway_id == 0xFF and num_supported_speeds == 3) or gateway_id == 0x14):
-            self.supported_fan_speeds = []
-        else:
-            self.supported_fan_speeds = [ACFanSpeedReference.AUTO]
-
-        if num_supported_speeds > 2:
-            self.supported_fan_speeds += all_speeds[2:2+num_supported_speeds]
-        elif num_supported_speeds == 2:
-            self.supported_fan_speeds += [ACFanSpeedReference.LOW, ACFanSpeedReference.HIGH]
-        elif num_supported_speeds < 2:
-            _LOGGER.warning(f"AC{self.number} reports less than 2 supported fan speeds, this is unusual - " + OPEN_ISSUE_TEXT)
-
-    def _set_fan_speed_from_val(self, speed_val: int):
-        if speed_val < 5:
-            # Units with no Auto speed still start with low = 1
-            if ACFanSpeedReference.AUTO not in self.supported_fan_speeds:
-                speed_val -= 1
-            self.fan_speed = self.supported_fan_speeds[speed_val]
-        else:
-            self.fan_speed = ACFanSpeedReference.AUTO
-
-    def _get_speed_val_from_speed(self, fan_speed: ACFanSpeedReference):
-        speed_val = self.supported_fan_speeds.index(fan_speed)
-        # Units with no Auto speed still start with low = 1
-        if ACFanSpeedReference.AUTO not in self.supported_fan_speeds:
-            speed_val += 1
-        return speed_val
-
     def update(self, response_message: ResponseMessage) -> None:
         self.system_name = response_message.system_name
 
         # Flags
         self.on = response_message.ac_active[self.number]
         self.safety = response_message.ac_safety[self.number]
         self.error = response_message.ac_error[self.number]
@@ -81,73 +56,83 @@
         if (self.measured_temp <= 0):
             self.measured_temp = response_message.touchpad_temp
         self.set_temp = response_message.ac_set_temp[self.number]
 
         # Brand
         brand = response_message.ac_brand[self.number]
         gateway_id = response_message.ac_gateway_id[self.number]
-        # Brand based on gateway ID takes priority
-        if gateway_id:
-            if gateway_id not in GATEWAYID_BRAND_LOOKUP:
-                _LOGGER.warning(f"AC{self.number} has an unfamiliar gateway ID: {hex(gateway_id)} - " + OPEN_ISSUE_TEXT + "\nInclude the gateway ID shown above")
-                self.brand = brand
-            else:
-                self.brand = GATEWAYID_BRAND_LOOKUP[gateway_id]
+        # Brand based on gateway ID takes priority according to app smali
+        gateway_based_brand = brand_from_gateway_id(gateway_id)
+        if gateway_based_brand is not None:
+            self.brand = gateway_based_brand
         else:
             self.brand = brand
 
         # Modes
         self.mode = response_message.ac_mode[self.number]
         num_fan_speeds = response_message.ac_num_fan_speeds[self.number]
         fan_speed_val = response_message.ac_fan_speed[self.number]
-        self._set_supported_fan_speeds(num_fan_speeds, gateway_id)
-        self._set_fan_speed_from_val(fan_speed_val)
+        self.supported_fan_speeds = supported_fan_speeds(self.brand, num_fan_speeds, gateway_id)
+        self.fan_speed = fan_speed_from_val(self.supported_fan_speeds, fan_speed_val)
 
         # TODO: Handle this?
         if brand == ACBrand.NONE and gateway_id == 0:
             _LOGGER.warning(f"AC{self.number} appears disconnected from airtouch")
 
         self.name = response_message.ac_name[self.number]
 
+        for callback in self._callbacks:
+            callback()
+
+    def add_callback(self, func: Callable) -> Callable:
+        self._callbacks.append(func)
+
+        def remove_callback() -> None:
+            if func in self._callbacks:
+                self._callbacks.remove(func)
+
+        return remove_callback
+
     async def inc_dec_set_temp(self, inc: bool):
-        await self._client.send_command(ChangeSetTemperature(self.number, inc))
+        await self._client.send(ChangeSetTemperature(self.number, inc))
 
     async def set_set_temp(self, new_temp: int):
         temp_diff = new_temp - self.set_temp
         inc = temp_diff > 0
         for i in range(abs(temp_diff)):
             await self.inc_dec_set_temp(inc)
-
-    async def _turn_on_off(self, on: bool):
-        if self.on != on:
-            await self._client.send_command(ToggleAC(self.number))
+            await asyncio.sleep(0.1)  # server doesn't like being spammed, 0.1s is faster than waiting for response
 
     async def turn_off(self):
         await self._turn_on_off(False)
 
     async def turn_on(self):
         await self._turn_on_off(True)
 
     async def set_fan_speed(self, fan_speed: ACFanSpeedReference):
         if fan_speed in self.supported_fan_speeds:
-            await self._client.send_command(SetFanSpeed(self.number, self._get_speed_val_from_speed(fan_speed)))
+            await self._client.send(SetFanSpeed(self.number, val_from_fan_speed(self.supported_fan_speeds, fan_speed)))
         else:
             _LOGGER.warning(f"Cannot set fan speed to unsupported value {fan_speed}")
 
     async def set_mode(self, mode: ACMode):
-        await self._client.send_command(SetMode(self.number, mode))
+        await self._client.send(SetMode(self.number, mode))
 
     def get_status_strings(self):
         flags = [self.error, self.safety, self.spill, self.turbo]
         flag_names = ['ERROR', 'SAFETY', 'SPILL', 'TURBO']
         statuses = list(compress(flag_names, flags))
         if not statuses:
             statuses.append('NORMAL')
         return statuses
 
+    async def _turn_on_off(self, on: bool):
+        if self.on != on:
+            await self._client.send(ToggleAc(self.number))
+
     def __str__(self):
         return f"""
         System Name:\t\t{self.system_name}
         AC Number:\t\t{self.number}
         AC Name:\t\t{self.name}
         On:\t\t\t{self.on}
         Status:\t\t\t{self.get_status_strings()}
```

### Comparing `airtouch2-0.5b2/src/airtouch2/AT2Group.py` & `airtouch2-0.7/src/airtouch2/at2/At2Group.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 from itertools import compress
-from typing import TYPE_CHECKING
-from airtouch2.protocol.messages import ResponseMessage
+from typing import TYPE_CHECKING, Callable
+from airtouch2.protocol.at2.messages import ResponseMessage
 
-from airtouch2.protocol.messages import ChangeDamper, ToggleGroup
+from airtouch2.protocol.at2.messages import ChangeDamper, ToggleGroup
 if TYPE_CHECKING:
-    from airtouch2.AT2Client import AT2Client
+    from airtouch2.at2.At2Client import At2Client
 import logging
 
 
 _LOGGER = logging.getLogger(__name__)
 
-class AT2Group:
-    def __init__(self, client: AT2Client, number: int, response: ResponseMessage):
+
+class At2Group:
+    def __init__(self, client: At2Client, number: int, response: ResponseMessage):
         self._client = client
         self.number = number
+        self._callbacks: list[Callable] = []
         self.update(response)
 
     def update(self, response: ResponseMessage):
         self.name = response.group_names[self.number]
         [start_zone, num_zones] = response.group_zones[self.number]
         # 0 to 10 steps of 10%
         self.damp = response.zone_damps[start_zone]
@@ -34,16 +36,28 @@
             if (self.on != response.zone_ons[i]):
                 mismatches.add("on/offs")
             if mismatches:
                 _LOGGER.warning(f"Zones of group '{self.name}' have mismatching {', '.join(mismatches)}")
 
         self.turbo = True if response.turbo_group == self.number else False
 
+        for func in self._callbacks:
+            func()
+
+    def add_callback(self, func: Callable) -> Callable:
+        self._callbacks.append(func)
+
+        def remove_callback() -> None:
+            if func in self._callbacks:
+                self._callbacks.remove(func)
+
+        return remove_callback
+
     async def inc_dec_damp(self, inc: bool):
-        await self._client.send_command(ChangeDamper(self.number, inc))
+        await self._client.send(ChangeDamper(self.number, inc))
 
     async def set_damp(self, new_damp: int):
         if new_damp < 0 or new_damp > 10:
             raise ValueError("Dampers can only be set from 0 to 10")
         # Set to 0 is equivalent to turning off
         if new_damp == 0:
             await self.turn_off()
@@ -52,15 +66,15 @@
             damp_diff = new_damp - self.damp
             inc = damp_diff > 0
             for i in range(abs(damp_diff)):
                 await self.inc_dec_damp(inc)
 
     async def _turn_on_off(self, on: bool):
         if self.on != on:
-            await self._client.send_command(ToggleGroup(self.number))
+            await self._client.send(ToggleGroup(self.number))
 
     async def turn_off(self):
         await self._turn_on_off(False)
 
     async def turn_on(self):
         await self._turn_on_off(True)
 
@@ -75,8 +89,8 @@
     def __str__(self):
         return f"""
         Group Name:\t{self.name}
         Group Number:\t{self.number}
         On:\t\t{self.on}
         Status:\t\t{self.get_status_strings()}
         Damper:\t\t{f'{self.damp*10}%'}
-        """
+        """
```

### Comparing `airtouch2-0.5b2/src/airtouch2/diff_bytes.py` & `airtouch2-0.7/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.5b2/src/airtouch2/protocol/constants.py` & `airtouch2-0.7/src/airtouch2/protocol/at2/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,7 +72,9 @@
     #AC2_ERROR_CODE = 367
     AC1_GATEWAY_ID = 368
     #AC2_GATEWAY_ID = 369
     # AC names are 8 bytes (ResponseMessageConstants.SHORT_STRING_LENGTH)
     AC1_NAME_START = 370
     #AC2_NAME_START = 378
     HASH = 394
+
+OPEN_ISSUE_TEXT = "please open an issue and detail your system:\n\thttps://github.com/nathanvdh/airtouch2-python/issues/new"
```

### Comparing `airtouch2-0.5b2/src/airtouch2/protocol/enums.py` & `airtouch2-0.7/src/airtouch2/protocol/at2/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.5b2/src/airtouch2/protocol/lookups.py` & `airtouch2-0.7/src/airtouch2/protocol/at2/lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from airtouch2.protocol.enums import ACBrand
+from airtouch2.protocol.at2.enums import ACBrand
 
 # I cannot find documentation of what these values actually mean
 # The app prioritises this 'brand' (based on gateway id) over the other one in the message
 # GATEWAY_BRAND2_LOOKUP = {
 #     0x5  : 0x5,
 #     0xFF : 0x5,
 #     # 0x8: TETZUO (Daikin)
```

### Comparing `airtouch2-0.5b2/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7/src/airtouch2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.5b2
+Version: 0.7
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # airtouch2_python
 In-development Python client for the Polyaire AirTouch 2 airconditioning system
 
 ## Thanks to
```

