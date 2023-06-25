# Comparing `tmp/d0da-0.2.0.tar.gz` & `tmp/d0da-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d0da-0.2.0.tar", max compression
+gzip compressed data, was "d0da-0.3.0.tar", max compression
```

## Comparing `d0da-0.2.0.tar` & `d0da-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      715 2023-06-24 18:31:04.969370 d0da-0.2.0/README.md
--rw-r--r--   0        0        0     1806 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/cli.py
--rw-r--r--   0        0        0     3281 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_feature.py
--rw-r--r--   0        0        0      322 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_report.proto
--rw-r--r--   0        0        0     3150 2023-06-24 18:29:51.059153 d0da-0.2.0/d0da/d0da_report.py
--rw-r--r--   0        0        0     3006 2023-06-24 09:02:02.956277 d0da-0.2.0/d0da/d0da_report_pb2.py
--rw-r--r--   0        0        0     2978 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/device_linux.py
--rw-r--r--   0        0        0     1589 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/helper.py
--rw-r--r--   0        0        0     4118 2023-06-24 09:02:02.957277 d0da-0.2.0/d0da/hidraw.py
--rw-r--r--   0        0        0      558 2023-06-25 14:05:33.425374 d0da-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 d0da-0.2.0/setup.py
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 d0da-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-06-24 18:31:04.969370 d0da-0.3.0/README.md
+-rw-r--r--   0        0        0     1806 2023-06-24 09:02:02.956277 d0da-0.3.0/d0da/cli.py
+-rw-r--r--   0        0        0     3281 2023-06-24 09:02:02.956277 d0da-0.3.0/d0da/d0da_feature.py
+-rw-r--r--   0        0        0      322 2023-06-24 09:02:02.956277 d0da-0.3.0/d0da/d0da_report.proto
+-rw-r--r--   0        0        0     3150 2023-06-24 18:29:51.059153 d0da-0.3.0/d0da/d0da_report.py
+-rw-r--r--   0        0        0     3006 2023-06-24 09:02:02.956277 d0da-0.3.0/d0da/d0da_report_pb2.py
+-rw-r--r--   0        0        0     2978 2023-06-24 09:02:02.957277 d0da-0.3.0/d0da/device_linux.py
+-rw-r--r--   0        0        0     1589 2023-06-24 09:02:02.957277 d0da-0.3.0/d0da/helper.py
+-rw-r--r--   0        0        0     4118 2023-06-24 09:02:02.957277 d0da-0.3.0/d0da/hidraw.py
+-rw-r--r--   0        0        0      633 2023-06-25 14:22:08.513515 d0da-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 d0da-0.3.0/setup.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 d0da-0.3.0/PKG-INFO
```

### Comparing `d0da-0.2.0/README.md` & `d0da-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/cli.py` & `d0da-0.3.0/d0da/cli.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/d0da_feature.py` & `d0da-0.3.0/d0da/d0da_feature.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/d0da_report.py` & `d0da-0.3.0/d0da/d0da_report.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/d0da_report_pb2.py` & `d0da-0.3.0/d0da/d0da_report_pb2.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/device_linux.py` & `d0da-0.3.0/d0da/device_linux.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/helper.py` & `d0da-0.3.0/d0da/helper.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/d0da/hidraw.py` & `d0da-0.3.0/d0da/hidraw.py`

 * *Files identical despite different names*

### Comparing `d0da-0.2.0/setup.py` & `d0da-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0', 'protobuf>=4.23.2,<5.0.0']
 
+extras_require = \
+{'linux': ['pyudev>=0.24.1,<0.25.0', 'ioctl-opt>=1.3,<2.0']}
+
 entry_points = \
 {'console_scripts': ['d0da-cli = d0da.cli:main']}
 
 setup_kwargs = {
     'name': 'd0da',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Wooting D0DA protocol',
     'long_description': "# Wooting D0DA Protocol\n\n## Introduction\n\nWooting has been very generous in supplying Open Source (!) SDKs for their hardware, only, the SDKs aren't\nvery thoroughly documented, limited to a single use case and written in C.\n\nThis repository tries to fill in these gaps, it generated the packets and the used fields are described. It also\ndescribes what the packets do and in what order they should be sent.\n\n## Features\n\n- Technical documentation\n- Command line interface (d0da-cli) for sending packets to the keyboard\n- Unit tests\n\n## Limitations\n\n- Linux only (for now)\n- Wooting 60HE (ARM) only, though the packets should be compatible with other keyboards.\n\n## Installation\n\nRun:\n\n```bash\npipx install d0da\n```\n",
     'author': 'Dick Marinus',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `d0da-0.2.0/PKG-INFO` & `d0da-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: d0da
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wooting D0DA protocol
 Author: Dick Marinus
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: linux
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: ioctl-opt (>=1.3,<2.0) ; extra == "linux"
 Requires-Dist: protobuf (>=4.23.2,<5.0.0)
+Requires-Dist: pyudev (>=0.24.1,<0.25.0) ; extra == "linux"
 Description-Content-Type: text/markdown
 
 # Wooting D0DA Protocol
 
 ## Introduction
 
 Wooting has been very generous in supplying Open Source (!) SDKs for their hardware, only, the SDKs aren't
```

