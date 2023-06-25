# Comparing `tmp/TuXingKeJi-0.0.4.tar.gz` & `tmp/TuXingKeJi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-0gjg9io_\TuXingKeJi-0.0.4.tar", last modified: Tue May 23 02:18:56 2023, max compression
+gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-bhwkolp1\TuXingKeJi-0.0.5.tar", last modified: Sun Jun 25 09:00:49 2023, max compression
```

## Comparing `TuXingKeJi-0.0.4.tar` & `TuXingKeJi-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:18:56.344389 TuXingKeJi-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4419 2023-05-23 02:18:56.343391 TuXingKeJi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3606 2023-05-23 02:16:57.000000 TuXingKeJi-0.0.4/README.md
--rw-rw-rw-   0        0        0      866 2023-05-23 02:18:22.000000 TuXingKeJi-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 02:18:56.345389 TuXingKeJi-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 02:18:56.203305 TuXingKeJi-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 02:18:56.289305 TuXingKeJi-0.0.4/src/TuXingKeJi/
--rw-rw-rw-   0        0        0    10718 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.4/src/TuXingKeJi/TuXingSDK.py
--rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.4/src/TuXingKeJi/__init__.py
--rw-rw-rw-   0        0        0     2837 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.4/src/TuXingKeJi/enumHelper.py
--rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.4/src/TuXingKeJi/peripheral.py
--rw-rw-rw-   0        0        0     1324 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.4/src/TuXingKeJi/serialHelper.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:18:56.323390 TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-05-23 02:18:56.000000 TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-23 02:18:56.000000 TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:18:56.000000 TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 02:18:56.000000 TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 02:18:56.339390 TuXingKeJi-0.0.4/tests/
--rw-rw-rw-   0        0        0      399 2023-05-23 01:40:49.000000 TuXingKeJi-0.0.4/tests/test.py
--rw-rw-rw-   0        0        0      393 2023-05-22 21:25:22.000000 TuXingKeJi-0.0.4/tests/test2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.883544 TuXingKeJi-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4419 2023-06-25 09:00:49.878541 TuXingKeJi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3606 2023-05-23 02:16:57.000000 TuXingKeJi-0.0.5/README.md
+-rw-rw-rw-   0        0        0      866 2023-06-25 08:56:53.000000 TuXingKeJi-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:00:49.884541 TuXingKeJi-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.578528 TuXingKeJi-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.755549 TuXingKeJi-0.0.5/src/TuXingKeJi/
+-rw-rw-rw-   0        0        0    12287 2023-06-25 08:59:10.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/TuXingSDK.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/__init__.py
+-rw-rw-rw-   0        0        0     2837 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/enumHelper.py
+-rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/peripheral.py
+-rw-rw-rw-   0        0        0     1324 2023-05-23 01:46:30.000000 TuXingKeJi-0.0.5/src/TuXingKeJi/serialHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.805531 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 09:00:49.000000 TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 09:00:49.870547 TuXingKeJi-0.0.5/tests/
+-rw-rw-rw-   0        0        0      399 2023-05-23 01:40:49.000000 TuXingKeJi-0.0.5/tests/test.py
+-rw-rw-rw-   0        0        0      393 2023-05-22 21:25:22.000000 TuXingKeJi-0.0.5/tests/test2.py
```

### Comparing `TuXingKeJi-0.0.4/LICENSE` & `TuXingKeJi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.4/PKG-INFO` & `TuXingKeJi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `TuXingKeJi-0.0.4/README.md` & `TuXingKeJi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.4/pyproject.toml` & `TuXingKeJi-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "TuXingKeJi"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="chenghao", email="chenghao.wang@uphf.fr" },
 ]
 description = "A python package for TuXingKeJi UAV control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TuXingKeJi-0.0.4/src/TuXingKeJi/TuXingSDK.py` & `TuXingKeJi-0.0.5/src/TuXingKeJi/TuXingSDK.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from src.TuXingKeJi.enumHelper import *
-from src.TuXingKeJi.peripheral import Peripheral
-from src.TuXingKeJi.serialHelper import hex_str
+from enumHelper import ISRRT, Dir, Dir2, Rotate, QH, Color, State, FliPpt, Land, OFFON, ISRColor, XXFX, \
+    MVColor, AllMode, ATGColor, ZY, SX
+from peripheral import Peripheral
+from serialHelper import hex_str
 
 
+#2023-5-22 名称修改完毕
+
 # 红外灯
 # 红外灯[ISR_RT]
 def get_infrared_hex_code(code: ISRRT):
     return code.value
 
 
 class TuXingSDK:
@@ -191,14 +194,15 @@
 
     # 定位模式
     # 定位模式[OFFON]
     def set_relocation(self, status: OFFON):
         msg = " ".join(["AA FA 47 00 00 00", status.value, "00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
+
     # 红外发射
     # 发射红外数据[ISR_RT]
     def emit_appoint_data(self, status: ISRRT):
         msg = " ".join(["AA FA 30 00", status.value, "00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
     # 红外发射
@@ -227,14 +231,16 @@
 
     # 舵机
     # 舵机[distance]°
     def set_Servo(self, distance: int):
         msg = " ".join(["AA FA 33", hex_str("%02X" % distance), "00 00 00 00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
+
+
     # 机械手
     # 机械手[distance]°
     def set_hand(self, distance: int):
         msg = " ".join(["AA FA 34", hex_str("%02X" % distance), "00 00 00 00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
     # 激光
@@ -257,14 +263,15 @@
 
     # 二维码模式
     # 切换为[ALL_mode]模式
     def change_mode(self, mode: AllMode = AllMode.BY_DEFAULT):
         msg = " ".join(["AA FA A0", mode.value, "00 00 00 00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
+
     # 标签间距，根据实际场地调整，单位cm
     # 二维码标签间距[distance]cm
     def set_spacing(self, distance: int):
         msg = " ".join(["AA FA A2", hex_str("%02X" % distance), "00 00 00 00 00 00 00 00 FE"])
         self.__peripheral.write(msg)
 
     # 期望标签
@@ -292,7 +299,48 @@
         self.__peripheral.write(msg)
 
     # 角度校准
     # 飞机航向校准
     def calibration(self):
         msg = "AA FA 2A 00 00 00 00 00 00 00 00 00 FE"
         self.__peripheral.write(msg)
+
+    # ********************************************************************************************************
+    # 编队怠速
+    # TX230[direction]怠速
+    def BD_Unlock_uav(self, distance: int):
+        msg = " ".join(["AA FA C5", hex_str("%02X" % distance), "00 00 00 00 00 00 00 00 FE"])
+        self.__peripheral.write(msg)
+
+
+    # 编队起飞
+    # "TX230[distance]起飞[distance2]厘米[clour]",
+    def BD_take_off(self, distance: int, distance2: int, color: Color):
+        msg = " ".join(["AA FA C1", hex_str("%02X" % distance), hex_str("%04X" % distance2, 4), "00 00 00 00 00", color.value, "FE"])
+        self.__peripheral.write(msg)
+
+    # 编队降落
+    # "TX230[direction]降落[clour]",
+    def BD_landing(self, distance: int, color: Color):
+        msg = " ".join(["AA FA CF", hex_str("%02X" % distance), "00 00 00 00 00 00 00", color.value, "FE"])
+        self.__peripheral.write(msg)
+
+    # 期望标签
+    # "TX230[distance]飞到[distance2]标签，高度[distance3]厘米[clour]",
+    def BD_fly_ID(self, distance: int, distance2: int, distance3: int, color: Color):
+        msg = " ".join(["AA FA c2", hex_str("%02X" % distance), hex_str("%04X" % distance2, 4), hex_str("%04X" % distance3, 4), "00 00 00", color.value,"FE"])
+        self.__peripheral.write(msg)
+
+
+    # 编队结束
+    # 编队结束
+    def BD_end(self):
+        msg = "AA FA CE 00 00 00 00 00 00 00 00 00 FE"
+        self.__peripheral.write(msg)
+
+
+
+
+
+
+
+
```

### Comparing `TuXingKeJi-0.0.4/src/TuXingKeJi/enumHelper.py` & `TuXingKeJi-0.0.5/src/TuXingKeJi/enumHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.4/src/TuXingKeJi/peripheral.py` & `TuXingKeJi-0.0.5/src/TuXingKeJi/peripheral.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.4/src/TuXingKeJi/serialHelper.py` & `TuXingKeJi-0.0.5/src/TuXingKeJi/serialHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.4/src/TuXingKeJi.egg-info/PKG-INFO` & `TuXingKeJi-0.0.5/src/TuXingKeJi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

