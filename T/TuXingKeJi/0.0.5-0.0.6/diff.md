# Comparing `tmp/TuXingKeJi-0.0.5.tar.gz` & `tmp/TuXingKeJi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-bhwkolp1\TuXingKeJi-0.0.5.tar", last modified: Sun Jun 25 09:00:49 2023, max compression
+gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-ipdxb5qg\TuXingKeJi-0.0.6.tar", last modified: Sun Jun 25 09:11:54 2023, max compression
```

## Comparing `TuXingKeJi-0.0.5.tar` & `TuXingKeJi-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.883544 TuXingKeJi-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4419 2023-06-25 09:00:49.878541 TuXingKeJi-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3606 2023-05-23 02:16:57.000000 TuXingKeJi-0.0.5/README.md
--rw-rw-rw-   0        0        0      866 2023-06-25 08:56:53.000000 TuXingKeJi-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 09:00:49.884541 TuXingKeJi-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.578528 TuXingKeJi-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.755549 TuXingKeJi-0.0.5/src/TuXingKeJi/
--rw-rw-rw-   0        0        0    12287 2023-06-25 08:59:10.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/TuXingSDK.py
--rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/__init__.py
--rw-rw-rw-   0        0        0     2837 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/enumHelper.py
--rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/peripheral.py
--rw-rw-rw-   0        0        0     1324 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/serialHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.805531 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.870547 TuXingKeJi-0.0.5/tests/
--rw-rw-rw-   0        0        0      399 2023-05-23 01:40:49.000000 TuXingKeJi-0.0.5/tests/test.py
--rw-rw-rw-   0        0        0      393 2023-05-22 21:25:22.000000 TuXingKeJi-0.0.5/tests/test2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:11:54.722283 TuXingKeJi-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4419 2023-06-25 09:11:54.719285 TuXingKeJi-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3606 2023-05-23 02:16:57.000000 TuXingKeJi-0.0.6/README.md
+-rw-rw-rw-   0        0        0      866 2023-06-25 09:10:39.000000 TuXingKeJi-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:11:54.723282 TuXingKeJi-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 09:11:54.592287 TuXingKeJi-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:11:54.646284 TuXingKeJi-0.0.6/src/TuXingKeJi/
+-rw-rw-rw-   0        0        0    12290 2023-06-25 09:09:59.000000 TuXingKeJi-0.0.6/src/TuXingKeJi/TuXingSDK.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.6/src/TuXingKeJi/__init__.py
+-rw-rw-rw-   0        0        0     2837 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.6/src/TuXingKeJi/enumHelper.py
+-rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.6/src/TuXingKeJi/peripheral.py
+-rw-rw-rw-   0        0        0     1324 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.6/src/TuXingKeJi/serialHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:11:54.701280 TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-06-25 09:11:54.000000 TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-25 09:11:54.000000 TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:11:54.000000 TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 09:11:54.000000 TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 09:11:54.713285 TuXingKeJi-0.0.6/tests/
+-rw-rw-rw-   0        0        0      399 2023-05-23 01:40:49.000000 TuXingKeJi-0.0.6/tests/test.py
+-rw-rw-rw-   0        0        0      393 2023-05-22 21:25:22.000000 TuXingKeJi-0.0.6/tests/test2.py
```

### Comparing `TuXingKeJi-0.0.5/LICENSE` & `TuXingKeJi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.5/PKG-INFO` & `TuXingKeJi-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `TuXingKeJi-0.0.5/README.md` & `TuXingKeJi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.5/pyproject.toml` & `TuXingKeJi-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "TuXingKeJi"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="chenghao", email="chenghao.wang@uphf.fr" },
 ]
 description = "A python package for TuXingKeJi UAV control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TuXingKeJi-0.0.5/src/TuXingKeJi/TuXingSDK.py` & `TuXingKeJi-0.0.6/src/TuXingKeJi/TuXingSDK.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from enumHelper import ISRRT, Dir, Dir2, Rotate, QH, Color, State, FliPpt, Land, OFFON, ISRColor, XXFX, \
+from .enumHelper import ISRRT, Dir, Dir2, Rotate, QH, Color, State, FliPpt, Land, OFFON, ISRColor, XXFX, \
     MVColor, AllMode, ATGColor, ZY, SX
-from peripheral import Peripheral
-from serialHelper import hex_str
+from .peripheral import Peripheral
+from .serialHelper import hex_str
 
 
 #2023-5-22 名称修改完毕
 
 # 红外灯
 # 红外灯[ISR_RT]
 def get_infrared_hex_code(code: ISRRT):
```

### Comparing `TuXingKeJi-0.0.5/src/TuXingKeJi/enumHelper.py` & `TuXingKeJi-0.0.6/src/TuXingKeJi/enumHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.5/src/TuXingKeJi/peripheral.py` & `TuXingKeJi-0.0.6/src/TuXingKeJi/peripheral.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.5/src/TuXingKeJi/serialHelper.py` & `TuXingKeJi-0.0.6/src/TuXingKeJi/serialHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/PKG-INFO` & `TuXingKeJi-0.0.6/src/TuXingKeJi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

