# Comparing `tmp/solarwatt-energymanager-py-1.2.1.tar.gz` & `tmp/solarwatt-energymanager-py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarwatt-energymanager-py-1.2.1.tar", last modified: Sun Mar  5 11:48:40 2023, max compression
+gzip compressed data, was "solarwatt-energymanager-py-1.3.0.tar", last modified: Sun Jun 25 17:40:57 2023, max compression
```

## Comparing `solarwatt-energymanager-py-1.2.1.tar` & `solarwatt-energymanager-py-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 11:48:40.512857 solarwatt-energymanager-py-1.2.1/
--rw-rw-rw-   0        0        0     1092 2022-03-31 18:25:53.000000 solarwatt-energymanager-py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     1518 2023-03-05 11:48:40.512857 solarwatt-energymanager-py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-03-05 11:48:17.000000 solarwatt-energymanager-py-1.2.1/README.md
--rw-rw-rw-   0        0        0      110 2021-12-18 09:59:04.000000 solarwatt-energymanager-py-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      749 2023-03-05 11:48:40.525391 solarwatt-energymanager-py-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-05 11:48:40.448940 solarwatt-energymanager-py-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-05 11:48:40.482044 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/
--rw-rw-rw-   0        0        0      382 2023-03-04 15:31:44.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/__init__.py
--rw-rw-rw-   0        0        0     4861 2022-04-04 17:49:19.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/battery_converter_device.py
--rw-rw-rw-   0        0        0     2492 2023-03-05 11:34:55.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/device.py
--rw-rw-rw-   0        0        0     2179 2022-03-31 17:52:04.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager.py
--rw-rw-rw-   0        0        0     3804 2023-03-04 15:29:38.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager_data.py
--rw-rw-rw-   0        0        0      840 2022-03-31 17:32:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager_device.py
--rw-rw-rw-   0        0        0     2306 2023-03-04 15:38:58.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/ev_station_device.py
--rw-rw-rw-   0        0        0     8908 2021-12-25 15:07:55.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/location_device.py
--rw-rw-rw-   0        0        0     1489 2023-03-04 15:10:37.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/s0_counter_device.py
-drwxrwxrwx   0        0        0        0 2023-03-05 11:48:40.511857 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/
--rw-rw-rw-   0        0        0     1518 2023-03-05 11:48:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2023-03-05 11:48:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 11:48:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-05 11:48:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-03-05 11:48:40.000000 solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 17:40:57.688406 solarwatt-energymanager-py-1.3.0/
+-rw-rw-rw-   0        0        0     1092 2022-03-31 18:25:53.000000 solarwatt-energymanager-py-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1653 2023-06-25 17:40:57.689921 solarwatt-energymanager-py-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-06-25 17:39:10.000000 solarwatt-energymanager-py-1.3.0/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-18 09:59:04.000000 solarwatt-energymanager-py-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      749 2023-06-25 17:40:57.696247 solarwatt-energymanager-py-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 17:40:57.575359 solarwatt-energymanager-py-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 17:40:57.624605 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/
+-rw-rw-rw-   0        0        0      382 2023-03-04 15:31:44.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/__init__.py
+-rw-rw-rw-   0        0        0     4861 2022-04-04 17:49:19.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/battery_converter_device.py
+-rw-rw-rw-   0        0        0     2530 2023-06-25 17:36:42.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/device.py
+-rw-rw-rw-   0        0        0     2179 2022-03-31 17:52:04.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager.py
+-rw-rw-rw-   0        0        0     3804 2023-03-04 15:29:38.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager_data.py
+-rw-rw-rw-   0        0        0      840 2022-03-31 17:32:40.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager_device.py
+-rw-rw-rw-   0        0        0     2306 2023-03-04 15:38:58.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/ev_station_device.py
+-rw-rw-rw-   0        0        0     8908 2021-12-25 15:07:55.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/location_device.py
+-rw-rw-rw-   0        0        0     1489 2023-03-04 15:10:37.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/s0_counter_device.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:40:57.686394 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/
+-rw-rw-rw-   0        0        0     1653 2023-06-25 17:40:57.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2023-06-25 17:40:57.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:40:57.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 17:40:57.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-25 17:40:57.000000 solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/top_level.txt
```

### Comparing `solarwatt-energymanager-py-1.2.1/LICENSE` & `solarwatt-energymanager-py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/PKG-INFO` & `solarwatt-energymanager-py-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarwatt-energymanager-py
-Version: 1.2.1
+Version: 1.3.0
 Summary: Client to query the SOLARWATT EnergyManager.
 Home-page: https://github.com/Mas2112/solarwatt-energymanager-py
 Author: Masaru Shimizu
 Author-email: mshimizu@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mas2112/solarwatt-energymanager-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,19 @@
 data = await mgr.get_data()
 print(f'power_in={data.location_device.power_in}')
 print(f'power_out={data.location_device.power_out}')
 ```
 
 # Changelog
 
+## [1.3.0] - 2023-06-25
+
+### Changed
+- get_tag_value_as_* methods return None instead of empty string or zero if an error occurs
+
 ## [1.2.1] - 2023-03-05
 
 ### Added
 - Added support to read IdName from Device via get_device_name()
 
 ## [1.2.0] - 2023-03-04
```

### Comparing `solarwatt-energymanager-py-1.2.1/README.md` & `solarwatt-energymanager-py-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 data = await mgr.get_data()
 print(f'power_in={data.location_device.power_in}')
 print(f'power_out={data.location_device.power_out}')
 ```
 
 # Changelog
 
+## [1.3.0] - 2023-06-25
+
+### Changed
+- get_tag_value_as_* methods return None instead of empty string or zero if an error occurs
+
 ## [1.2.1] - 2023-03-05
 
 ### Added
 - Added support to read IdName from Device via get_device_name()
 
 ## [1.2.0] - 2023-03-04
```

### Comparing `solarwatt-energymanager-py-1.2.1/setup.cfg` & `solarwatt-energymanager-py-1.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6f6c 6172 7761 7474 2d65 6e65   = solarwatt-ene
 00000020: 7267 796d 616e 6167 6572 2d70 790d 0a76  rgymanager-py..v
-00000030: 6572 7369 6f6e 203d 2031 2e32 2e31 0d0a  ersion = 1.2.1..
+00000030: 6572 7369 6f6e 203d 2031 2e33 2e30 0d0a  ersion = 1.3.0..
 00000040: 6175 7468 6f72 203d 204d 6173 6172 7520  author = Masaru 
 00000050: 5368 696d 697a 750d 0a61 7574 686f 725f  Shimizu..author_
 00000060: 656d 6169 6c20 3d20 6d73 6869 6d69 7a75  email = mshimizu
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 436c 6965 6e74  ription = Client
 00000090: 2074 6f20 7175 6572 7920 7468 6520 534f   to query the SO
 000000a0: 4c41 5257 4154 5420 456e 6572 6779 4d61  LARWATT EnergyMa
```

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/battery_converter_device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/battery_converter_device.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Final, List
+from typing import Any, Dict, Final, List, Optional
 
 
 class Device:
     """The base definition for an EnergyManager device."""
 
     TAG_ID_NAME: Final[str] = "IdName"
 
@@ -23,36 +23,36 @@
     
     def get_device_name(self) -> str:
         device_name = self.get_tag_value_as_str(Device.TAG_ID_NAME).strip()
         if not device_name:
             return self.guid
         return device_name
 
-    def get_tag_value_as_str(self, tag_name) -> str:
+    def get_tag_value_as_str(self, tag_name) -> Optional[str]:
         """Get the item tag value as a string."""
         try:
             if tag_name in self.tag_items:
                 return str(self.tag_items[tag_name])
-            return ""
+            return None
         except Exception:
-            return ""
+            return None
 
-    def get_tag_value_as_int(self, tag_name) -> int:
+    def get_tag_value_as_int(self, tag_name) -> Optional[int]:
         """Get the item tag value as an int."""
         try:
             return int(float(self.tag_items[tag_name]))
         except Exception:
-            return int(0)
+            return None
 
-    def get_tag_value_as_float(self, tag_name) -> float:
+    def get_tag_value_as_float(self, tag_name) -> Optional[float]:
         """Get the item tag value as a float."""
         try:
             return float(self.tag_items[tag_name])
         except Exception:
-            return float(0)
+            return None
 
     @staticmethod
     def get_item_device_classes(item: dict) -> List[str]:
         """Get the devices classes of the items."""
         classes: List[str] = []
         if "deviceModel" in item:
             device_model_items = item["deviceModel"]
```

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager_data.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager_data.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/energy_manager_device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/energy_manager_device.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/ev_station_device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/ev_station_device.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/location_device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/location_device.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager/s0_counter_device.py` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager/s0_counter_device.py`

 * *Files identical despite different names*

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/PKG-INFO` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarwatt-energymanager-py
-Version: 1.2.1
+Version: 1.3.0
 Summary: Client to query the SOLARWATT EnergyManager.
 Home-page: https://github.com/Mas2112/solarwatt-energymanager-py
 Author: Masaru Shimizu
 Author-email: mshimizu@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mas2112/solarwatt-energymanager-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,19 @@
 data = await mgr.get_data()
 print(f'power_in={data.location_device.power_in}')
 print(f'power_out={data.location_device.power_out}')
 ```
 
 # Changelog
 
+## [1.3.0] - 2023-06-25
+
+### Changed
+- get_tag_value_as_* methods return None instead of empty string or zero if an error occurs
+
 ## [1.2.1] - 2023-03-05
 
 ### Added
 - Added support to read IdName from Device via get_device_name()
 
 ## [1.2.0] - 2023-03-04
```

### Comparing `solarwatt-energymanager-py-1.2.1/src/solarwatt_energymanager_py.egg-info/SOURCES.txt` & `solarwatt-energymanager-py-1.3.0/src/solarwatt_energymanager_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

