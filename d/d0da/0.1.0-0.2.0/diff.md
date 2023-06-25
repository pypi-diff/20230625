# Comparing `tmp/d0da-0.1.0.tar.gz` & `tmp/d0da-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d0da-0.1.0.tar", max compression
+gzip compressed data, was "d0da-0.2.0.tar", max compression
```

## Comparing `d0da-0.1.0.tar` & `d0da-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-30 06:31:10.741096 d0da-0.1.0/README.md
--rw-r--r--   0        0        0     4117 2023-05-30 06:31:45.719331 d0da-0.1.0/d0da/hidraw.py
--rw-r--r--   0        0        0      354 2023-05-30 06:30:51.261215 d0da-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 d0da-0.1.0/setup.py
--rw-r--r--   0        0        0      308 1970-01-01 00:00:00.000000 d0da-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-06-24 18:31:04.969370 d0da-0.2.0/README.md
+-rw-r--r--   0        0        0     1806 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/cli.py
+-rw-r--r--   0        0        0     3281 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_feature.py
+-rw-r--r--   0        0        0      322 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_report.proto
+-rw-r--r--   0        0        0     3150 2023-06-24 18:29:51.059153 d0da-0.2.0/d0da/d0da_report.py
+-rw-r--r--   0        0        0     3006 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_report_pb2.py
+-rw-r--r--   0        0        0     2978 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/device_linux.py
+-rw-r--r--   0        0        0     1589 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/helper.py
+-rw-r--r--   0        0        0     4118 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/hidraw.py
+-rw-r--r--   0        0        0      558 2023-06-25 14:05:33.425374 d0da-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 d0da-0.2.0/setup.py
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 d0da-0.2.0/PKG-INFO
```

### Comparing `d0da-0.1.0/d0da/hidraw.py` & `d0da-0.2.0/d0da/hidraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 BUS_HIL = 0x04
 BUS_BLUETOOTH = 0x05
 BUS_VIRTUAL = 0x06
 
 # hid.h
 _HID_MAX_DESCRIPTOR_SIZE = 4096
 
+
 # hidraw.h
 class _hidraw_report_descriptor(ctypes.Structure):
     _fields_ = [
         ("size", ctypes.c_uint),
         ("value", ctypes.c_ubyte * _HID_MAX_DESCRIPTOR_SIZE),
     ]
```

