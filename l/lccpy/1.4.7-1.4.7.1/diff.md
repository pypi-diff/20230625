# Comparing `tmp/lccpy-1.4.7.tar.gz` & `tmp/lccpy-1.4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.4.7.tar", last modified: Tue Jun 13 15:41:03 2023, max compression
+gzip compressed data, was "lccpy-1.4.7.1.tar", last modified: Sun Jun 25 12:26:19 2023, max compression
```

## Comparing `lccpy-1.4.7.tar` & `lccpy-1.4.7.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.7/LICENSE
--rw-r--r--   0        0        0      112 2023-06-13 05:52:50.378292 lccpy-1.4.7/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.7/lccpy/__init__.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.7/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      165 2023-06-13 11:57:21.300071 lccpy-1.4.7/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20497 2023-06-13 11:57:21.300071 lccpy-1.4.7/lccpy/asymongo/_core.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.7/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 lccpy-1.4.7/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    22791 2023-06-13 11:57:21.299172 lccpy-1.4.7/lccpy/asymysql/_core.py
--rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 lccpy-1.4.7/lccpy/coolapi/Licenses of dependent packages/tornado/LICENSE
--rw-r--r--   0        0        0       40 2023-05-28 06:10:27.855895 lccpy-1.4.7/lccpy/coolapi/__init__.py
--rw-r--r--   0        0        0     1668 2023-05-27 11:00:33.037396 lccpy-1.4.7/lccpy/coolapi/_core.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.7/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.7/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.7/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20915 2023-06-13 11:57:21.290462 lccpy-1.4.7/lccpy/coolmongo/_core.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.7/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    22817 2023-06-13 11:57:21.279654 lccpy-1.4.7/lccpy/coolmysql/_core.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.7/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       29 2023-06-13 11:40:05.743411 lccpy-1.4.7/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.7/lccpy/encrypt256/_core.py
--rw-r--r--   0        0        0       30 2023-06-13 11:40:37.720315 lccpy-1.4.7/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1586 2023-06-02 08:06:48.314577 lccpy-1.4.7/lccpy/increment/_core.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.7/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.7/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      179 2023-06-13 12:23:13.409389 lccpy-1.4.7/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.7/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    10266 2023-06-13 14:45:35.809939 lccpy-1.4.7/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      574 2023-06-13 15:36:41.801055 lccpy-1.4.7/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 lccpy-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.7.1/LICENSE
+-rw-r--r--   0        0        0      112 2023-06-13 05:52:50.378292 lccpy-1.4.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.7.1/lccpy/__init__.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.7.1/lccpy/asymongo/Dependent Packages/motor/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.300071 lccpy-1.4.7.1/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20497 2023-06-13 11:57:21.300071 lccpy-1.4.7.1/lccpy/asymongo/_core.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.7.1/lccpy/asymysql/Dependent Packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 lccpy-1.4.7.1/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    22791 2023-06-13 11:57:21.299172 lccpy-1.4.7.1/lccpy/asymysql/_core.py
+-rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 lccpy-1.4.7.1/lccpy/coolapi/Dependent Packages/tornado/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-28 06:10:27.855895 lccpy-1.4.7.1/lccpy/coolapi/__init__.py
+-rw-r--r--   0        0        0     1668 2023-05-27 11:00:33.037396 lccpy-1.4.7.1/lccpy/coolapi/_core.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.7.1/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.7.1/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.7.1/lccpy/coolmongo/Dependent Packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 lccpy-1.4.7.1/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20915 2023-06-13 11:57:21.290462 lccpy-1.4.7.1/lccpy/coolmongo/_core.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.7.1/lccpy/coolmysql/Dependent Packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 lccpy-1.4.7.1/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    22817 2023-06-13 11:57:21.279654 lccpy-1.4.7.1/lccpy/coolmysql/_core.py
+-rw-r--r--   0        0        0       27 2023-06-25 08:02:23.228282 lccpy-1.4.7.1/lccpy/cooltime/__init__.py
+-rw-r--r--   0        0        0     2770 2023-06-25 11:28:10.216367 lccpy-1.4.7.1/lccpy/cooltime/_core.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.7.1/lccpy/encrypt256/Dependent Packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       29 2023-06-13 11:40:05.743411 lccpy-1.4.7.1/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.7.1/lccpy/encrypt256/_core.py
+-rw-r--r--   0        0        0       30 2023-06-25 03:07:54.283832 lccpy-1.4.7.1/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1586 2023-06-25 03:07:49.948869 lccpy-1.4.7.1/lccpy/increment/_core.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.7.1/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.7.1/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      146 2023-06-25 08:00:40.735040 lccpy-1.4.7.1/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0    10230 2023-06-25 11:27:13.050158 lccpy-1.4.7.1/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      576 2023-06-25 11:35:56.015142 lccpy-1.4.7.1/pyproject.toml
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 lccpy-1.4.7.1/PKG-INFO
```

### Comparing `lccpy-1.4.7/LICENSE` & `lccpy-1.4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4.7.1/lccpy/asymongo/Dependent Packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/asymongo/_core.py` & `lccpy-1.4.7.1/lccpy/asymongo/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4.7.1/lccpy/asymysql/Dependent Packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/asymysql/_core.py` & `lccpy-1.4.7.1/lccpy/asymysql/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolapi/Licenses of dependent packages/tornado/LICENSE` & `lccpy-1.4.7.1/lccpy/coolapi/Dependent Packages/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolapi/_core.py` & `lccpy-1.4.7.1/lccpy/coolapi/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4.7.1/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4.7.1/lccpy/coolmongo/Dependent Packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolmongo/_core.py` & `lccpy-1.4.7.1/lccpy/coolmongo/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4.7.1/lccpy/coolmysql/Dependent Packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/coolmysql/_core.py` & `lccpy-1.4.7.1/lccpy/coolmysql/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4.7.1/lccpy/encrypt256/Dependent Packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/encrypt256/_core.py` & `lccpy-1.4.7.1/lccpy/encrypt256/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/increment/_core.py` & `lccpy-1.4.7.1/lccpy/increment/_core.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4.7.1/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.7/lccpy/vtype/_vtype.py` & `lccpy-1.4.7.1/lccpy/vtype/_vtype.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 '''
 Copyright [2023] [许灿标]
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 import re
-from decimal import Decimal
 from math import ceil
 from collections import deque
 import hashlib
 from hashlib import shake_256
 from fractions import Fraction
-from typing import Union, Any
+from typing import Any
 
 
 class missing_arguments_error(Exception): ...
 
 
 ########################################## vbool ##########################################
```

### Comparing `lccpy-1.4.7/pyproject.toml` & `lccpy-1.4.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.4.7"
+version = "1.4.7.1"
 description = "项目 <让Python更简单一点> 的依赖包"
 dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome", "tornado"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `lccpy-1.4.7/PKG-INFO` & `lccpy-1.4.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.4.7
+Version: 1.4.7.1
 Summary: 项目 <让Python更简单一点> 的依赖包
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
```

