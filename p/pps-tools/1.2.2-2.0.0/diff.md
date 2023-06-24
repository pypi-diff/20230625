# Comparing `tmp/pps-tools-1.2.2.tar.gz` & `tmp/pps-tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pps-tools-1.2.2.tar", last modified: Sat Oct  8 15:12:18 2022, max compression
+gzip compressed data, was "pps-tools-2.0.0.tar", last modified: Sat Jun 24 21:55:04 2023, max compression
```

## Comparing `pps-tools-1.2.2.tar` & `pps-tools-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 15:12:18.281058 pps-tools-1.2.2/
--rw-r--r--   0 stefan     (501) staff       (20)     1074 2021-07-21 01:13:42.000000 pps-tools-1.2.2/LICENSE
--rw-r--r--   0 stefan     (501) staff       (20)     4134 2022-10-08 15:12:18.281124 pps-tools-1.2.2/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)     3501 2021-10-06 23:42:14.000000 pps-tools-1.2.2/README.md
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 15:12:18.279509 pps-tools-1.2.2/pps_tools/
--rw-r--r--   0 stefan     (501) staff       (20)       67 2022-10-08 15:07:09.000000 pps-tools-1.2.2/pps_tools/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)       63 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/__main__.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 15:12:18.280811 pps-tools-1.2.2/pps_tools/data/
--rw-r--r--   0 stefan     (501) staff       (20)     1261 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/data/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)      933 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/data/common.py
--rw-r--r--   0 stefan     (501) staff       (20)     1485 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/data/freebsd.py
--rw-r--r--   0 stefan     (501) staff       (20)     1768 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/data/linux.py
--rw-r--r--   0 stefan     (501) staff       (20)     4260 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/io.py
--rw-r--r--   0 stefan     (501) staff       (20)     4336 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pps_tools/main.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 15:12:18.280327 pps-tools-1.2.2/pps_tools.egg-info/
--rw-r--r--   0 stefan     (501) staff       (20)     4134 2022-10-08 15:12:18.000000 pps-tools-1.2.2/pps_tools.egg-info/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)      381 2022-10-08 15:12:18.000000 pps-tools-1.2.2/pps_tools.egg-info/SOURCES.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2022-10-08 15:12:18.000000 pps-tools-1.2.2/pps_tools.egg-info/dependency_links.txt
--rw-r--r--   0 stefan     (501) staff       (20)       10 2022-10-08 15:12:18.000000 pps-tools-1.2.2/pps_tools.egg-info/top_level.txt
--rw-r--r--   0 stefan     (501) staff       (20)       90 2021-10-06 23:41:46.000000 pps-tools-1.2.2/pyproject.toml
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 15:12:18.280939 pps-tools-1.2.2/scripts/
--rwxr-xr-x   0 stefan     (501) staff       (20)       50 2021-07-21 01:13:42.000000 pps-tools-1.2.2/scripts/pps-tools
--rw-r--r--   0 stefan     (501) staff       (20)      910 2022-10-08 15:12:18.281421 pps-tools-1.2.2/setup.cfg
--rw-r--r--   0 stefan     (501) staff       (20)       37 2021-07-23 21:50:21.000000 pps-tools-1.2.2/setup.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 21:55:04.198287 pps-tools-2.0.0/
+-rw-r--r--   0 stefan     (501) staff       (20)     1074 2021-07-21 01:13:42.000000 pps-tools-2.0.0/LICENSE
+-rw-r--r--   0 stefan     (501) staff       (20)     4337 2023-06-24 21:55:04.198166 pps-tools-2.0.0/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)     3501 2021-10-06 23:42:14.000000 pps-tools-2.0.0/README.md
+-rw-r--r--   0 stefan     (501) staff       (20)     1137 2023-06-24 21:50:54.000000 pps-tools-2.0.0/pyproject.toml
+-rw-r--r--   0 stefan     (501) staff       (20)       38 2023-06-24 21:55:04.198322 pps-tools-2.0.0/setup.cfg
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 21:55:04.196054 pps-tools-2.0.0/src/
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 21:55:04.196848 pps-tools-2.0.0/src/pps_tools/
+-rw-r--r--   0 stefan     (501) staff       (20)       66 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)       63 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/__main__.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 21:55:04.198013 pps-tools-2.0.0/src/pps_tools/data/
+-rw-r--r--   0 stefan     (501) staff       (20)     1261 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/data/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)      929 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/data/common.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1485 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/data/freebsd.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1770 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/data/linux.py
+-rw-r--r--   0 stefan     (501) staff       (20)     4451 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/io.py
+-rw-r--r--   0 stefan     (501) staff       (20)     4151 2023-06-24 21:50:54.000000 pps-tools-2.0.0/src/pps_tools/main.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 21:55:04.197555 pps-tools-2.0.0/src/pps_tools.egg-info/
+-rw-r--r--   0 stefan     (501) staff       (20)     4337 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)      468 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       50 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/entry_points.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       47 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/requires.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       10 2023-06-24 21:55:04.000000 pps-tools-2.0.0/src/pps_tools.egg-info/top_level.txt
```

### Comparing `pps-tools-1.2.2/LICENSE` & `pps-tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pps-tools-1.2.2/PKG-INFO` & `pps-tools-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: pps-tools
-Version: 1.2.2
+Version: 2.0.0
 Summary: Pure Python implementation of RFC2783 PPS tools.
-Home-page: https://gitlab.com/srfilipek/pps-tools
-Author: Stefan R. Filipek
-Author-email: srfilipek@gmail.com
+Author-email: "Stefan R. Filipek" <srfilipek@gmail.com>
+Project-URL: Homepage, https://gitlab.com/srfilipek/pps-tools
 Project-URL: Bug Tracker, https://gitlab.com/srfilipek/pps-tools/-/issues
 Keywords: pps,pps-tools,ppstools,RFC2783,pulse,per,second
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking :: Time Synchronization
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Overview
 This is a Pure Python PPS interface following RFC2783. A PPPPS interface,
 if you would.
 
 This has the unfortunate task of rolling-up some system and implementation
```

### Comparing `pps-tools-1.2.2/README.md` & `pps-tools-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pps-tools-1.2.2/pps_tools/data/__init__.py` & `pps-tools-2.0.0/src/pps_tools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pps-tools-1.2.2/pps_tools/data/common.py` & `pps-tools-2.0.0/src/pps_tools/data/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,24 +19,20 @@
 PPS_TSFMT_TSPEC = 0x1000
 PPS_TSFMT_NTPFP = 0x2000
 
 # Helper for printing out mode information
 MODE_BITS = (
     (PPS_CAPTUREASSERT, "PPS_CAPTUREASSERT"),
     (PPS_CAPTURECLEAR, "PPS_CAPTURECLEAR"),
-
     (PPS_OFFSETASSERT, "PPS_OFFSETASSERT"),
     (PPS_OFFSETCLEAR, "PPS_OFFSETCLEAR"),
-
     (PPS_ECHOASSERT, "PPS_ECHOASSERT"),
     (PPS_ECHOCLEAR, "PPS_ECHOCLEAR"),
-
     (PPS_CANWAIT, "PPS_CANWAIT"),
     (PPS_CANPOLL, "PPS_CANPOLL"),
-
     (PPS_TSFMT_TSPEC, "PPS_TSFMT_TSPEC"),
     (PPS_TSFMT_NTPFP, "PPS_TSFMT_NTPFP"),
 )
 
 
 def ioc(direction, group, count, size=0):
     return direction | (size << 16) | (ord(group) << 8) | count
```

### Comparing `pps-tools-1.2.2/pps_tools/data/freebsd.py` & `pps-tools-2.0.0/src/pps_tools/data/freebsd.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,13 +52,13 @@
 
 
 _IOC_V = 0x20000000
 _IOC_R = 0x40000000
 _IOC_W = 0x80000000
 _IOC_RW = _IOC_R | _IOC_W
 
-PPS_IOC_CREATE = common.ioc(_IOC_V, '1', 1)
-PPS_IOC_DESTROY = common.ioc(_IOC_V, '1', 2)
-PPS_IOC_SETPARAMS = common.ioc(_IOC_W, '1', 3, ctypes.sizeof(PpsParams))
-PPS_IOC_GETPARAMS = common.ioc(_IOC_R, '1', 4, ctypes.sizeof(PpsParams))
-PPS_IOC_GETCAP = common.ioc(_IOC_R, '1', 5, ctypes.sizeof(ctypes.c_int))
-PPS_IOC_FETCH = common.ioc(_IOC_RW, '1', 6, ctypes.sizeof(PpsFetchArgs))
+PPS_IOC_CREATE = common.ioc(_IOC_V, "1", 1)
+PPS_IOC_DESTROY = common.ioc(_IOC_V, "1", 2)
+PPS_IOC_SETPARAMS = common.ioc(_IOC_W, "1", 3, ctypes.sizeof(PpsParams))
+PPS_IOC_GETPARAMS = common.ioc(_IOC_R, "1", 4, ctypes.sizeof(PpsParams))
+PPS_IOC_GETCAP = common.ioc(_IOC_R, "1", 5, ctypes.sizeof(ctypes.c_int))
+PPS_IOC_FETCH = common.ioc(_IOC_RW, "1", 6, ctypes.sizeof(PpsFetchArgs))
```

### Comparing `pps-tools-1.2.2/pps_tools/data/linux.py` & `pps-tools-2.0.0/src/pps_tools/data/linux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import ctypes
 
 from . import common
 
 
 class Timespec(ctypes.Structure):
     """Mirror pps_ktime"""
+
     _fields_ = (
         ("tv_sec", ctypes.c_int64),
         ("tv_nsec", ctypes.c_int32),
         ("flags", ctypes.c_uint32),  # 0 = time specified, 1 otherwise
     )
 
 
 class PpsTime(ctypes.Union):
     """Not in the kernel interface. For compatibility between FreeBSD and Linux code"""
+
     _fields_ = (
         ("tspec", Timespec),
         # ("ntpfp", NtpFp),
     )
 
 
 class PpsInfo(ctypes.Structure):
@@ -56,11 +58,11 @@
 
 
 # Does not exist in Linux
 PPS_IOC_CREATE = None
 PPS_IOC_DESTROY = None
 
 # The Linux PPS defines accidentally used pointers instead of structs for sizeof()
-PPS_IOC_GETPARAMS = common.ioc(_IOC_R, 'p', 0xa1, ctypes.sizeof(ctypes.c_void_p))
-PPS_IOC_SETPARAMS = common.ioc(_IOC_W, 'p', 0xa2, ctypes.sizeof(ctypes.c_void_p))
-PPS_IOC_GETCAP = common.ioc(_IOC_R, 'p', 0xa3, ctypes.sizeof(ctypes.c_void_p))
-PPS_IOC_FETCH = common.ioc(_IOC_RW, 'p', 0xa4, ctypes.sizeof(ctypes.c_void_p))
+PPS_IOC_GETPARAMS = common.ioc(_IOC_R, "p", 0xA1, ctypes.sizeof(ctypes.c_void_p))
+PPS_IOC_SETPARAMS = common.ioc(_IOC_W, "p", 0xA2, ctypes.sizeof(ctypes.c_void_p))
+PPS_IOC_GETCAP = common.ioc(_IOC_R, "p", 0xA3, ctypes.sizeof(ctypes.c_void_p))
+PPS_IOC_FETCH = common.ioc(_IOC_RW, "p", 0xA4, ctypes.sizeof(ctypes.c_void_p))
```

### Comparing `pps-tools-1.2.2/pps_tools/io.py` & `pps-tools-2.0.0/src/pps_tools/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,126 @@
 import ctypes
 import fcntl
 import os
+from typing import Optional, Union
 
 from . import data
 
 
 class PpsFile:
     """A Pythonic RFC2783 interface to PPS devices on the system.
 
     Python data types are taken and returned by the methods here, with conversion to underlying C data types as needed.
     The abstraction of these types is contained in the data submodule, as well as the per-platform IOCTL constants.
 
     Note that the code in here should avoid making platform introspection. Attempt to write the code in a way that
     works for all supported platforms.
     """
-    def __init__(self, spec):
+
+    def __init__(self, spec: Union[str, int]):
         """Open and initialize a PPS device
 
         Args:
-            spec (str, int): PPS device path (str) or file descriptor (int)
+            spec: PPS device path (str) or file descriptor (int)
         """
         if isinstance(spec, int):
             self._fd = spec
         else:
             self._fd = os.open(spec, os.O_RDWR)
         self._create()
 
-    def __enter__(self):
+    def __enter__(self) -> "PpsFile":
         return self
 
-    def __exit__(self, *exc):
+    def __exit__(self, *exc) -> None:
         self.close()
 
-    def _create(self):
+    def _create(self) -> None:
         if data.PPS_IOC_CREATE is not None:
             fcntl.ioctl(self._fd, data.PPS_IOC_CREATE)
 
-    def _destroy(self):
+    def _destroy(self) -> None:
         if data.PPS_IOC_DESTROY is not None:
             fcntl.ioctl(self._fd, data.PPS_IOC_DESTROY)
 
-    def close(self):
+    def close(self) -> None:
         """Destroy and close the underlying file descriptor."""
         self._destroy()
         os.close(self._fd)
         self._fd = None
 
     @property
-    def closed(self):
+    def closed(self) -> bool:
         """Return True if the underlying file descriptor has been properly closed"""
         return self._fd is None
 
-    def get_params(self):
+    def get_params(self) -> dict:
         """Get the currently set parameters.
 
         The returned dictionary mirrors the arguments used for set_params.
 
         Returns:
-            dict: A dictionary with assert_offset, clear_offset, api_version, and mode.
+            A dictionary with assert_offset, clear_offset, api_version, and mode.
         """
         params = data.PpsParams()
         fcntl.ioctl(self._fd, data.PPS_IOC_GETPARAMS, params)
         return {
             "assert_offset": data.timespec_to_float(params.assert_off_tu),
             "clear_offset": data.timespec_to_float(params.clear_off_tu),
             "api_version": params.api_version,
             "mode": params.mode,
         }
 
-    def set_params(self, assert_offset=0, clear_offset=0, api_version=1, mode=data.PPS_CAPTUREASSERT):
+    def set_params(
+        self,
+        assert_offset: float = 0,
+        clear_offset: float = 0,
+        api_version: int = 1,
+        mode: int = data.PPS_CAPTUREASSERT,
+    ) -> None:
         """Set parameters for the PPS interface.
 
         The arguments mirror the dictionary keys in get_params().
 
         Args:
-            assert_offset (float): Time offset to add to assert timestamps
-            clear_offset (float): Time offset to add to clear timestamps
-            api_version (int): Reported API version. Often has no bearing on the device.
-            mode (int): Mode bits, as defined by data.PPS_* constants
+            assert_offset: Time offset to add to assert timestamps
+            clear_offset: Time offset to add to clear timestamps
+            api_version: Reported API version. Often has no bearing on the device.
+            mode: Mode bits, as defined by data.PPS_* constants
 
         See also: get_cap()
         """
         assert_offset = data.PpsTime(tspec=data.float_to_timespec(assert_offset))
         clear_offset = data.PpsTime(tspec=data.float_to_timespec(clear_offset))
         params = data.PpsParams(
             api_version=api_version,
             mode=mode,
             assert_off_tu=assert_offset,
             clear_off_tu=clear_offset,
         )
         fcntl.ioctl(self._fd, data.PPS_IOC_SETPARAMS, params)
 
-    def get_cap(self):
+    def get_cap(self) -> int:
         """Obtain the interface mode bits.
 
         Returns:
-           int: Mode bits in the data module to examine.
+           Mode bits in the data module to examine.
         """
         cap = ctypes.c_int()
         fcntl.ioctl(self._fd, data.PPS_IOC_GETCAP, cap)
         return cap.value
 
-    def fetch(self, timeout=None):
+    def fetch(self, timeout: Optional[float] = None) -> dict:
         """Obtain the most recent timestamps captured for the PPS source.
 
         Args:
-            timeout (float): Number of seconds to wait. None = indefinite.
+            timeout: Number of seconds to wait. None = indefinite.
 
         Returns:
-            dict: assert_seq, clear_seq, assert_time, clear_time, and mode.
+            Dictionary with assert_seq, clear_seq, assert_time, clear_time, and mode keys
         """
         fetch_args = data.PpsFetchArgs(
             tsformat=data.PPS_TSFMT_TSPEC,
             timeout=data.float_to_timespec(timeout),
         )
 
         fcntl.ioctl(self._fd, data.PPS_IOC_FETCH, fetch_args)
```

### Comparing `pps-tools-1.2.2/pps_tools/main.py` & `pps-tools-2.0.0/src/pps_tools/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import sys
 import time
+from typing import Optional
 
-from . import __version__
-from . import data
-from . import io
+from . import __version__, data, io
 
 EDGE_FMT = "{name} {count} @ {time:0.9f}"
 
 
 def _mode_str(mode):
     return ", ".join(desc for bv, desc in data.MODE_BITS if mode & bv)
 
@@ -22,48 +21,42 @@
         print("Warning: Cannot wait on PPS event. Will sleep instead.")
         do_sleep = True
 
     while True:
         event = pps_file.fetch(timeout=timeout)
         edges = []
 
-        if event['mode'] & data.PPS_CAPTUREASSERT:
-            edges.append(EDGE_FMT.format(
-                name="assert",
-                count=event['assert_seq'],
-                time=event['assert_time']))
-
-        if event['mode'] & data.PPS_CAPTURECLEAR:
-            edges.append(EDGE_FMT.format(
-                name="clear",
-                count=event['clear_seq'],
-                time=event['clear_time']))
+        if event["mode"] & data.PPS_CAPTUREASSERT:
+            edges.append(EDGE_FMT.format(name="assert", count=event["assert_seq"], time=event["assert_time"]))
+
+        if event["mode"] & data.PPS_CAPTURECLEAR:
+            edges.append(EDGE_FMT.format(name="clear", count=event["clear_seq"], time=event["clear_time"]))
 
         print(" ; ".join(edges))
         if do_sleep:
             time.sleep(1)
 
 
-def info(pps_file):
+def info(pps_file: io.PpsFile):
     """Print out the current configuration for the given PPS device."""
     cap = pps_file.get_cap()
     cap_dict = data.cap_to_dict(cap)
     par = pps_file.get_params()
-    mode_str = _mode_str(par['mode'])
+    mode_str = _mode_str(par["mode"])
 
-    print("API Version         : {}".format(par['api_version']))
-    print("Assert Offset       : {}".format(par['assert_offset']))
-    print("Clear Offset        : {}".format(par['clear_offset']))
-    print("Current Mode        : 0x{:02x} - {}".format(par['mode'], mode_str))
+    print("API Version         : {}".format(par["api_version"]))
+    print("Assert Offset       : {}".format(par["assert_offset"]))
+    print("Clear Offset        : {}".format(par["clear_offset"]))
+    print("Current Mode        : 0x{:02x} - {}".format(par["mode"], mode_str))
     print("Capabilities        : 0x{}".format(cap))
     for k, v in cap_dict.items():
         print("  {:18}: {}".format(k, v))
 
 
-def params(pps_file, **kwargs):
+def params(pps_file: io.PpsFile, **kwargs):
     """Get and update the configuration for the given PPS device.
 
     This will print the updated configuration at the end.
     """
     par = pps_file.get_params()
 
     # Conditionally update the parameters
@@ -77,65 +70,48 @@
     if updated:
         pps_file.set_params(**par)
 
     # Get latest state and print
     info(pps_file)
 
 
-def main(args=None):
+def main(args: Optional[list[str]] = None):
     if args is None:
         args = sys.argv
 
     parser = argparse.ArgumentParser("pps-tools")
-    parser.add_argument(
-        "--version", action="store_true", default=False,
-        help="Print the current version and exit"
-    )
+    parser.add_argument("--version", action="store_true", default=False, help="Print the current version and exit")
 
     subparsers = parser.add_subparsers()
 
     # fetch command
-    p_fetch = subparsers.add_parser(
-        "fetch",
-        help="Fetch pulse events and print out information."
-    )
-    p_fetch.add_argument(
-        "--timeout", "-t", type=float, default=None,
-        help="Timeout for each fetch in seconds."
-    )
+    p_fetch = subparsers.add_parser("fetch", help="Fetch pulse events and print out information.")
+    p_fetch.add_argument("--timeout", "-t", type=float, default=None, help="Timeout for each fetch in seconds.")
     p_fetch.add_argument("pps_path", type=str, help="PPS device file to open")
     p_fetch.set_defaults(func=fetch)
 
     # params command
-    p_params = subparsers.add_parser(
-        "params",
-        help="Read and/or set parameters for the given PPS device."
-    )
+    p_params = subparsers.add_parser("params", help="Read and/or set parameters for the given PPS device.")
     p_params.add_argument(
-        "--mode", "-m", type=int, default=None,
-        help="Integer mode value. See the RFC Mode bit definitions."
+        "--mode", "-m", type=int, default=None, help="Integer mode value. See the RFC Mode bit definitions."
     )
     p_params.add_argument(
-        "--api_version", "-v", type=int, default=None,
-        help="Control the API version (doesn't really do anything)"
+        "--api_version", "-v", type=int, default=None, help="Control the API version (doesn't really do anything)"
     )
     p_params.add_argument(
-        "--assert_offset", "-a", type=float, default=None,
-        help="Assert offset, in seconds (floating point)"
+        "--assert_offset", "-a", type=float, default=None, help="Assert offset, in seconds (floating point)"
     )
     p_params.add_argument(
-        "--clear_offset", "-c", type=float, default=None,
-        help="Clear offset, in seconds (floating point)"
+        "--clear_offset", "-c", type=float, default=None, help="Clear offset, in seconds (floating point)"
     )
     p_params.add_argument("pps_path", type=str, help="PPS device file to open")
     p_params.set_defaults(func=params)
 
     # Parse and run
-    args = parser.parse_args(args[1:])
-    arg_dict = args.__dict__
+    arg_dict = parser.parse_args(args[1:]).__dict__
 
     if arg_dict.pop("version", False):
         print("pps-tools v{}".format(__version__))
         exit(0)
 
     func = arg_dict.pop("func", None)
     pps_path = arg_dict.pop("pps_path", None)
```

### Comparing `pps-tools-1.2.2/pps_tools.egg-info/PKG-INFO` & `pps-tools-2.0.0/src/pps_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: pps-tools
-Version: 1.2.2
+Version: 2.0.0
 Summary: Pure Python implementation of RFC2783 PPS tools.
-Home-page: https://gitlab.com/srfilipek/pps-tools
-Author: Stefan R. Filipek
-Author-email: srfilipek@gmail.com
+Author-email: "Stefan R. Filipek" <srfilipek@gmail.com>
+Project-URL: Homepage, https://gitlab.com/srfilipek/pps-tools
 Project-URL: Bug Tracker, https://gitlab.com/srfilipek/pps-tools/-/issues
 Keywords: pps,pps-tools,ppstools,RFC2783,pulse,per,second
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking :: Time Synchronization
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Overview
 This is a Pure Python PPS interface following RFC2783. A PPPPS interface,
 if you would.
 
 This has the unfortunate task of rolling-up some system and implementation
```

