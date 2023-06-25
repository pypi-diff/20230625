# Comparing `tmp/py2n-0.3.2.tar.gz` & `tmp/py2n-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2n-0.3.2.tar", last modified: Mon Jun 19 17:13:21 2023, max compression
+gzip compressed data, was "py2n-0.4.0.tar", last modified: Sun Jun 25 15:14:58 2023, max compression
```

## Comparing `py2n-0.3.2.tar` & `py2n-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.132718 py2n-0.3.2/
--rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1631 2023-06-19 17:13:21.131213 py2n-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-06-19 17:12:49.000000 py2n-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.109142 py2n-0.3.2/py2n/
--rw-rw-rw-   0        0        0     5272 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/__init__.py
--rw-rw-rw-   0        0        0      375 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/const.py
--rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.3.2/py2n/exceptions.py
--rw-rw-rw-   0        0        0     1220 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/model.py
--rw-rw-rw-   0        0        0     5017 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.130211 py2n-0.3.2/py2n.egg-info/
--rw-rw-rw-   0        0        0     1631 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.3.2/py2n.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-19 17:13:21.132718 py2n-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-06-19 17:12:49.000000 py2n-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:14:58.823256 py2n-0.4.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1631 2023-06-25 15:14:58.822257 py2n-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      945 2023-06-19 17:12:49.000000 py2n-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 15:14:58.801692 py2n-0.4.0/py2n/
+-rw-rw-rw-   0        0        0     6785 2023-06-25 15:14:39.000000 py2n-0.4.0/py2n/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-06-25 15:14:39.000000 py2n-0.4.0/py2n/const.py
+-rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.4.0/py2n/exceptions.py
+-rw-rw-rw-   0        0        0     1362 2023-06-25 15:14:39.000000 py2n-0.4.0/py2n/model.py
+-rw-rw-rw-   0        0        0     6664 2023-06-25 15:14:39.000000 py2n-0.4.0/py2n/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:14:58.821257 py2n-0.4.0/py2n.egg-info/
+-rw-rw-rw-   0        0        0     1631 2023-06-25 15:14:58.000000 py2n-0.4.0/py2n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-25 15:14:58.000000 py2n-0.4.0/py2n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 15:14:58.000000 py2n-0.4.0/py2n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 15:14:58.000000 py2n-0.4.0/py2n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 15:14:58.000000 py2n-0.4.0/py2n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.4.0/py2n.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-25 15:14:58.823256 py2n-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-25 15:14:39.000000 py2n-0.4.0/setup.py
```

### Comparing `py2n-0.3.2/LICENSE` & `py2n-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py2n-0.3.2/PKG-INFO` & `py2n-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `py2n-0.3.2/README.md` & `py2n-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `py2n-0.3.2/py2n/exceptions.py` & `py2n-0.4.0/py2n/exceptions.py`

 * *Files identical despite different names*

### Comparing `py2n-0.3.2/py2n/model.py` & `py2n-0.4.0/py2n/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,28 @@
 
     id: int
     enabled: bool
     active: bool
     locked: bool
     mode: str | None #inactive switches do not return a value for "mode"
 
+@dataclass
+class Py2NDevicePort:
+    """2N Device IO port"""
+    id: str
+    type: str
+    state: bool
 
 @dataclass
 class Py2NDeviceData:
     """Data collected from a 2N device."""
 
     name: str
     model: str
     serial: str
     host: str
     mac: str
     firmware: str
     hardware: str
     uptime: datetime
     switches: list[Py2NDeviceSwitch]
+    ports: list[Py2NDevicePort]
```

### Comparing `py2n-0.3.2/py2n/utils.py` & `py2n-0.4.0/py2n/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,21 @@
     CONTENT_TYPE,
     API_SYSTEM_INFO,
     API_SYSTEM_STATUS,
     API_SYSTEM_RESTART,
     API_SWITCH_CAPS,
     API_SWITCH_STATUS,
     API_SWITCH_CONTROL,
+    API_IO_CAPS,
+    API_IO_CONTROL,
+    API_IO_STATUS,
     API_AUDIO_TEST,
 )
 
-from .model import Py2NConnectionData
+from .model import Py2NConnectionData, Py2NDevicePort
 
 from .exceptions import (
     DeviceConnectionError,
     DeviceUnsupportedError,
     ApiError,
     DeviceApiError,
 )
@@ -128,14 +131,58 @@
             aiohttp_session,
             options,
             f"http://{options.host}{API_SWITCH_CONTROL}?switch={switch_id}&action={'on' if on else 'off'}",
         )
     except DeviceApiError as err:
         raise
 
+async def get_port_caps(aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData) ->  list[dict]:
+    try:
+        result = await api_request(
+            aiohttp_session,
+            options,
+            f"http://{options.host}{API_IO_CAPS}"
+        )
+    except DeviceApiError as err:
+        raise
+
+    return result["ports"]
+
+async def get_port_status(aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData) ->  list[dict]:
+    try:
+        result = await api_request(
+            aiohttp_session,
+            options,
+            f"http://{options.host}{API_IO_STATUS}"
+        )
+    except DeviceApiError as err:
+        raise
+
+    return result["ports"]
+
+async def get_ports(aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData) ->  list[Py2NDevicePort]:
+    caps = await get_port_caps(aiohttp_session, options)
+    statuses = await get_port_status(aiohttp_session, options)
+    ports = []
+    for cap in caps:
+        for status in statuses:
+            if status["port"] == cap["port"]:
+                ports.append(Py2NDevicePort(cap["port"], cap["type"], status["state"]))
+                break
+    return ports
+
+async def set_port(aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData, port_id: str, on: bool) -> None:
+    try:
+        await api_request(
+            aiohttp_session,
+            options,
+            f"http://{options.host}{API_IO_CONTROL}?port={port_id}&action={'on' if on else 'off'}",
+        )
+    except DeviceApiError as err:
+        raise
 
 async def api_request(
     aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData, url: str
 ) -> dict[str, Any] | None:
     """Perform REST call to device."""
     try:
         response = await aiohttp_session.get(
```

### Comparing `py2n-0.3.2/py2n.egg-info/PKG-INFO` & `py2n-0.4.0/py2n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `py2n-0.3.2/setup.py` & `py2n-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for py2n."""
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.3.2"
+VERSION = "0.4.0"
 
 setup(
     name='py2n',
     version=VERSION,
     license="MIT",
     url="https://github.com/elektr0nisch/py2n",
     author="Linus Groschke",
```

