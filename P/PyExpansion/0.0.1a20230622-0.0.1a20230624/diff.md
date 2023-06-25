# Comparing `tmp/PyExpansion-0.0.1a20230622.tar.gz` & `tmp/PyExpansion-0.0.1a20230624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpansion-0.0.1a20230622.tar", last modified: Wed Jun 21 17:26:17 2023, max compression
+gzip compressed data, was "PyExpansion-0.0.1a20230624.tar", last modified: Sun Jun 25 02:54:37 2023, max compression
```

## Comparing `PyExpansion-0.0.1a20230622.tar` & `PyExpansion-0.0.1a20230624.tar`

### file list

```diff
@@ -1,42 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/
--rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230622/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230622/MANIFEST.in
--rw-rw-rw-   0        0        0     1141 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:16.992141 PyExpansion-0.0.1a20230622/PyExpansion/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230622/PyExpansion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.023391 PyExpansion-0.0.1a20230622/PyExpansion/application/
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.039012 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/
--rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.054633 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/
--rw-rw-rw-   0        0        0     8513 2023-06-21 15:35:07.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Malaysia.py
--rw-rw-rw-   0        0        0     2899 2023-06-21 16:10:29.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Singapore.py
--rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-06-21 15:48:39.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/base.py
--rw-rw-rw-   0        0        0     1016 2023-06-21 15:31:03.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/main.py
--rw-rw-rw-   0        0        0      621 2023-06-21 16:51:40.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/status_code_list.py
--rw-rw-rw-   0        0        0     1760 2023-06-21 16:53:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/tests.py
--rw-rw-rw-   0        0        0      473 2023-06-18 15:13:16.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/version.py
--rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.085878 PyExpansion-0.0.1a20230622/PyExpansion/common/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/basic_function.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.085878 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/
--rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/__init__.py
--rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/main.py
--rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/status_code_list.py
--rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/tests.py
--rw-rw-rw-   0        0        0     1166 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/message.py
--rw-rw-rw-   0        0        0      532 2023-06-18 16:08:44.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/status_code_list.py
--rw-rw-rw-   0        0        0     1069 2023-06-18 08:38:41.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/utils.py
--rw-rw-rw-   0        0        0     2532 2023-06-18 15:13:08.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/version_history.py
--rw-rw-rw-   0        0        0       28 2023-06-21 16:56:25.000000 PyExpansion-0.0.1a20230622/PyExpansion/version.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.007766 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/
--rw-rw-rw-   0        0        0     1141 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      980 2023-06-21 17:09:08.000000 PyExpansion-0.0.1a20230622/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-06-21 17:16:35.000000 PyExpansion-0.0.1a20230622/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.606905 PyExpansion-0.0.1a20230624/
+-rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230624/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230624/MANIFEST.in
+-rw-rw-rw-   0        0        0     1465 2023-06-25 02:54:37.606905 PyExpansion-0.0.1a20230624/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.465707 PyExpansion-0.0.1a20230624/PyExpansion/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230624/PyExpansion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.481881 PyExpansion-0.0.1a20230624/PyExpansion/application/
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.481881 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.513171 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/
+-rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.528748 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/
+-rw-rw-rw-   0        0        0     8543 2023-06-24 15:35:29.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/Malaysia.py
+-rw-rw-rw-   0        0        0     2913 2023-06-24 10:35:35.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/Singapore.py
+-rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-24 15:35:22.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/base.py
+-rw-rw-rw-   0        0        0     1090 2023-06-24 09:43:29.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/main.py
+-rw-rw-rw-   0        0        0      509 2023-06-24 15:34:57.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/status_code_list.py
+-rw-rw-rw-   0        0        0     1827 2023-06-24 09:46:15.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/tests.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 15:31:40.000000 PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.544378 PyExpansion-0.0.1a20230624/PyExpansion/common/
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/basic_function.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.544378 PyExpansion-0.0.1a20230624/PyExpansion/common/constants/
+-rw-rw-rw-   0        0        0        0 2023-06-24 09:11:08.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/constants/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-06-24 09:13:45.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/constants/common.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.560042 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.575663 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/lists/
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/lists/__init__.py
+-rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/lists/main.py
+-rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/lists/status_code_list.py
+-rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/data_type/lists/tests.py
+-rw-rw-rw-   0        0        0      989 2023-06-24 10:06:05.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/message.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.575663 PyExpansion-0.0.1a20230624/PyExpansion/common/status_code/
+-rw-rw-rw-   0        0        0        0 2023-06-24 07:45:47.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/status_code/__init__.py
+-rw-rw-rw-   0        0        0     9071 2023-06-25 01:23:17.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/status_code/http_code.py
+-rw-rw-rw-   0        0        0      283 2023-06-25 02:14:18.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/status_code/utils.py
+-rw-rw-rw-   0        0        0     2978 2023-06-24 15:34:07.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/utils.py
+-rw-rw-rw-   0        0        0     2718 2023-06-24 08:09:05.000000 PyExpansion-0.0.1a20230624/PyExpansion/common/version_history.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.591232 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.606905 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/PyBrainFuck/
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:30:05.000000 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/PyBrainFuck/__init__.py
+-rw-rw-rw-   0        0        0     4943 2023-06-25 02:22:18.000000 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/PyBrainFuck/main.py
+-rw-rw-rw-   0        0        0      430 2023-06-25 02:23:03.000000 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/PyBrainFuck/tests.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:29:40.000000 PyExpansion-0.0.1a20230624/PyExpansion/just_for_fun/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-06-25 02:48:09.000000 PyExpansion-0.0.1a20230624/PyExpansion/version.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:54:37.481881 PyExpansion-0.0.1a20230624/PyExpansion.egg-info/
+-rw-rw-rw-   0        0        0     1465 2023-06-25 02:54:37.000000 PyExpansion-0.0.1a20230624/PyExpansion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1572 2023-06-25 02:54:37.000000 PyExpansion-0.0.1a20230624/PyExpansion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 02:54:37.000000 PyExpansion-0.0.1a20230624/PyExpansion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 02:54:37.000000 PyExpansion-0.0.1a20230624/PyExpansion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1304 2023-06-25 02:34:04.000000 PyExpansion-0.0.1a20230624/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 02:54:37.606905 PyExpansion-0.0.1a20230624/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-06-21 17:16:35.000000 PyExpansion-0.0.1a20230624/setup.py
```

### Comparing `PyExpansion-0.0.1a20230622/LICENSE.txt` & `PyExpansion-0.0.1a20230624/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230622/PKG-INFO` & `PyExpansion-0.0.1a20230624/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: PyExpansion
-Version: 0.0.1a20230622
+Version: 0.0.1a20230624
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Overviews
 
 ![PyPI](https://img.shields.io/pypi/v/pyexpansion) &nbsp;
 ![License: MIT](https://img.shields.io/github/license/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub issues](https://img.shields.io/github/issues/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/weitaoyap111/pyexpansion)&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/pyexpansion?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/pyexpansion)&nbsp;
 
-Python script that suddenly come to my idea
+Python script that suddenly come to my idea <br>
 Will update more...
 
 # Installation
 How to install:
-```python
+```
 pip install pyexpansion
 ```
 
 # Library List:
 ## 1) PyIC
 ### What is this?
 - Python Script that extract the ic information from ic word.
 
 ### How to use it?
 - You can refer to PyIC\tests.py.
 
+### Want knows more? 
+you can read at PyIC\README.md
+
+## 2) PyBrainFuck
+### What is this?
+- Python Script that decode and encode using BrainFuck.
+
+### How to use it?
+- You can refer to PyBrainFuck\tests.py.
+
+### Want knows more? 
+you can read at PyBrainFuck\README.md
+
+# Projects Status
 ### Updated
 - Apply for Malaysia Only
 - Singapore Added
+- PyBrainFuck is added
 
 # Author
 Copyright (c) 2023 Wei Tao Yap
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Malaysia.py` & `PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/Malaysia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from datetime import datetime
 
 from PyExpansion.common import message
-from PyExpansion.application.PyIC.country import base
-from PyExpansion.application.PyIC import status_code_list
+from PyExpansion.application.human_resource.PyIC import status_code_list
+from PyExpansion.application.human_resource.PyIC.country import base
 
 
 class PyIC(base.PyICBase):
     country = "Malaysia"
-    ic_pattern = "############"
+    word_pattern = "############"
 
     """
-    YYMMDD PB ###G
+    YYMMDDPB###G
 
     YY  - last 2 number of the year of birth
     MM  - number of month of birth
     DD  - number of day of birth
     PB  - place of birth
     ### - generic special number generated by the National Registration Department of Malaysia's computer system
     G   - Gender of person, odd number is male, even number is female
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Singapore.py` & `PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/country/Singapore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PyExpansion.common import message
-from PyExpansion.application.PyIC.country import base
-from PyExpansion.application.PyIC import status_code_list
+from PyExpansion.application.human_resource.PyIC.country import base
+from PyExpansion.application.human_resource.PyIC import status_code_list
 
 
 class PyIC(base.PyICBase):
     country = "Singapore"
-    ic_pattern = "C########"
+    word_pattern = "C########"
 
     """
     @xxxxxxx#
     
     @ is a letter that can be "S", "T", "F", "G" or "M" depending on the status of the holder.
     Singapore citizens and permanent residents born before 1 January 2000 are assigned the letter "S".
     Singapore citizens and permanent residents born on or after 1 January 2000 are assigned the letter "T".
@@ -48,28 +48,28 @@
 
     valid_list = {
         "1": "JZIHGFEDCBA",
         "0": "XWUTRQPNMLK",
     }
 
     def valid_ic(self):
-        choice = self.ic_word[0]
+        choice = self.word[0]
 
         # calc
         v_list = 0
         multiple_v = [2, 7, 6, 5, 4, 3, 2]
         for x in range(1, 8):
-            v_list += int(self.ic_word[x]) * multiple_v[x-1]
+            v_list += int(self.word[x]) * multiple_v[x-1]
 
         v_list = v_list % 11
 
         if choice == "S" or choice == "T":
-            return self.valid_list["1"][v_list] == self.ic_word[len(self.ic_word)-1]
+            return self.valid_list["1"][v_list] == self.word[len(self.word)-1]
         elif choice == "F" or choice == "G" or choice == "M":
-            return self.valid_list["0"][v_list] == self.ic_word[len(self.ic_word)-1]
+            return self.valid_list["0"][v_list] == self.word[len(self.word)-1]
         else:
             return None
 
     def get_detail(self):
         if not self.get_info():
             return message.error_default_message(False)
         else:
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/base.py` & `PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-from PyExpansion.common import utils
-from PyExpansion.application.PyIC import status_code_list
+from PyExpansion.common import utils, message
+from PyExpansion.application.human_resource.PyIC import status_code_list
+from PyExpansion.application.human_resource.PyIC.country import Malaysia, Singapore
 
 
-class PyICBase(utils.BaseClass):
-    country = ""  # country name
-    separator = "-"  # symbol use in ic for separator purpose
-    max_length_after_separator = 3  # how many group separate by separator
-    ic_pattern = ""  # pattern of ic, # mean number, C mean character, S mean symbol
-    symbol_list = "[@_!#$%^&*()<>?/\\|}{~:]"  # use for symbol check
-    abc_list = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+class PyIC(utils.ErrorBase):
+    code_list = status_code_list.code_list
 
-    def __init__(self, ic_word: str):
+    def __init__(self, country, ic_word):
+        self.country = country
         self.ic_word = ic_word
+        self.py_ic = self._router()
 
-    def _valid_length(self):
-        return True if len(self.ic_word) == len(self.ic_pattern) else False
-
-    def _check_ic_word_same_as_pattern(self):
-        for count, x in enumerate(self.ic_pattern):
-            if x == "#":  # number
-                try:
-                    v = int(self.ic_word[count])
-                except:
-                    return False
-            elif x == "C":  # character
-                return False if self.ic_word[count] not in self.abc_list else True
-            elif x == "S":  # symbol
-                return False if self.ic_word[count] not in self.symbol_list else True
-            else:
-                return False
-        return True
-
-    def _verify(self):
-        if not self._valid_length():
-            self.error_code = status_code_list.error_code_3
+    def _router(self):
+        if self.country == "Malaysia":
+            return Malaysia.PyIC(self.ic_word)
+        elif self.country == "Singapore":
+            return Singapore.PyIC(self.ic_word)
+        else:
             return None
+
+    def get_detail(self):
+        if self._router():
+            return self._router().get_detail()
+        else:
+            self.error_code = status_code_list.error_code_1
+            return message.error_default_message(False)
+
+    def check_error(self):
+        if self._router():
+            return self._router().check_error()
         else:
-            if not self._check_ic_word_same_as_pattern():
-                self.error_code = status_code_list.error_code_2
-                return None
-            else:
-                return self.ic_word
+            return utils.ErrorBase.check_error(self)
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/tests.py` & `PyExpansion-0.0.1a20230624/PyExpansion/application/human_resource/PyIC/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyExpansion.application.PyIC import main
+from PyExpansion.application.human_resource.PyIC import main
 
 test_case_material = [
     {
         "country": "M",
         "ic_word": "123456478",
         "test_condition": "Invalid Country",
         "special": "",
@@ -47,9 +47,10 @@
     print("Test Condition: ", x["test_condition"])
     test_case = main.PyIC(x["country"], x["ic_word"])
     print("Case %s (sample: %s): " % (str(count), x["ic_word"]), test_case.get_detail())
     print("Error Check Case %s: " % str(count), test_case.check_error())
     if x.get("special", ""):
         print("This function", x["special"])
     if x["country"] == "Singapore":
-        print("Is Valid: ", main.Singapore.PyIC(x["ic_word"]).valid_ic())
+        print("Extra Function For Singapore")
+        print("Is IC Valid ?: ", main.Singapore.PyIC(x["ic_word"]).valid_ic())
     print("\n")
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/common/message.py` & `PyExpansion-0.0.1a20230624/PyExpansion/common/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-from . import status_code_list as scl
+from .status_code import utils
 
 
 def return_response(code: int, message: str, info=None):
     return {"code": code, "message": message, "info": info}
 
 
 def return_single_response(message: str):
     return {"message": message}
 
 
-def get_code_description(code: str, code_description=None):
-    if code_description is None:
-        code_description = scl.code_list
-    return code_description[code]
-
-
 def return_response_with_code_list(code: str, list_code=None, info=None):
     """
     :param code: response status
     :param list_code: list of the code, default is use code_list
     :param info: information that bring from function to function, default is None
     :return: code, flag [True if info is none else false], message of the code, information
     """
     return_data = dict()
     return_data.update({"code": code})
     return_data.update(error_default_message(True) if info else error_default_message(False))
-    return_data.update({"message": get_code_description(code, list_code)})
+    return_data.update({"message": utils.get_code_description(code, list_code)})
     return_data.update({"info": info})
     return return_data
 
 
 def error_default_message(error: bool):
     return {"flag": error}
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion/common/version_history.py` & `PyExpansion-0.0.1a20230624/PyExpansion/common/version_history.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 from datetime import datetime
+import json
 
 from PyExpansion.common import basic_function
 
 
 class VersionHistoryBase(object):
     """
     version format: {{major version}}.{{minor version}}.{{patch version}}{{version|a}}{{date|yyyymmdd}}
     example: 0.0.1a20230618
     major version, minor version and patch version: must be in number (>=0)
     version: either alpha(a) or stable(s)
     date: last update
     """
-    application_name = ""
-    list_version = []
-    list_description = []
-    length_of_date = 8
+    _length_of_date = 8
+
+    _list_version = []
 
     def __init__(self):
         self._update_all()
+        self.write_or_update_version_file()
+
+    def default_setup(self, application_name, version, description="1st Version"):
+        return {
+            "application_name": application_name,
+            "version": version,
+            "description": description,
+        }
 
     def _update_all(self):
-        list_functions = dir(self)
-        search_names1 = "version_"
-        search_names2 = "description_for_version_"
+        search_names = "version_"
         function_found_lists_v = list()
-        function_found_lists_d = list()
+        list_functions = dir(self)
+
         for function_name in list_functions:
-            if function_name.startswith(search_names1):
+            if function_name.startswith(search_names):
                 function_found_lists_v.append(function_name)
-            if function_name.startswith(search_names2):
-                function_found_lists_d.append(function_name)
+
         for x in function_found_lists_v:
             if basic_function.check_function_exist(self, x):
-                self.list_version.append(getattr(self, x)())
-        for x in function_found_lists_d:
-            if basic_function.check_function_exist(self, x):
-                self.list_description.append(getattr(self, x)())
+                self._list_version.append(getattr(self, x)())
 
     def total_version(self):
-        return len(self.list_version)
+        return len(self._list_version)
 
     def get_latest_version(self):
-        return self.list_version[-1]
+        return self._list_version[-1]["version"]
 
-    def get_version_info(self, version):
+    def get_version_list(self):
+        return self._list_version
+
+    def get_version_info(self, version=None):
+        if not version:
+            version = self.get_latest_version()
         get_version = version.split(".")
         if len(get_version) != 3:
             raise Exception("Version pattern error")
         else:
             [major_version, minor_version, patch] = get_version
-            patch_version = patch[:len(patch)-self.length_of_date-1]
-            stable_alpha = patch[len(patch)-self.length_of_date-1:len(patch)-self.length_of_date]
-            update_date = patch[len(patch)-self.length_of_date:len(patch)]
+            patch_version = patch[:len(patch)-self._length_of_date-1]
+            stable_alpha = patch[len(patch)-self._length_of_date-1:len(patch)-self._length_of_date]
+            update_date = patch[len(patch)-self._length_of_date:len(patch)]
 
             return_data = dict()
             return_data.update({"major_version": major_version})
             return_data.update({"minor_version": minor_version})
             return_data.update({"patch_version": patch_version})
             return_data.update({"stable_alpha": "Stable" if stable_alpha == "s" else "Alpha"})
             return_data.update({"update_date": datetime.strptime(update_date, "%Y%m%d").date()})
             return return_data
+
+    def write_or_update_version_file(self):
+        with open("version.json", "w") as outfile:
+            json.dump(self._list_version, outfile)
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion.egg-info/PKG-INFO` & `PyExpansion-0.0.1a20230624/PyExpansion.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: PyExpansion
-Version: 0.0.1a20230622
+Version: 0.0.1a20230624
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Overviews
 
 ![PyPI](https://img.shields.io/pypi/v/pyexpansion) &nbsp;
 ![License: MIT](https://img.shields.io/github/license/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub issues](https://img.shields.io/github/issues/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/weitaoyap111/pyexpansion)&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/pyexpansion?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/pyexpansion)&nbsp;
 
-Python script that suddenly come to my idea
+Python script that suddenly come to my idea <br>
 Will update more...
 
 # Installation
 How to install:
-```python
+```
 pip install pyexpansion
 ```
 
 # Library List:
 ## 1) PyIC
 ### What is this?
 - Python Script that extract the ic information from ic word.
 
 ### How to use it?
 - You can refer to PyIC\tests.py.
 
+### Want knows more? 
+you can read at PyIC\README.md
+
+## 2) PyBrainFuck
+### What is this?
+- Python Script that decode and encode using BrainFuck.
+
+### How to use it?
+- You can refer to PyBrainFuck\tests.py.
+
+### Want knows more? 
+you can read at PyBrainFuck\README.md
+
+# Projects Status
 ### Updated
 - Apply for Malaysia Only
 - Singapore Added
+- PyBrainFuck is added
 
 # Author
 Copyright (c) 2023 Wei Tao Yap
```

### Comparing `PyExpansion-0.0.1a20230622/PyExpansion.egg-info/SOURCES.txt` & `PyExpansion-0.0.1a20230624/PyExpansion.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,35 @@
 PyExpansion/__init__.py
 PyExpansion/version.py
 PyExpansion.egg-info/PKG-INFO
 PyExpansion.egg-info/SOURCES.txt
 PyExpansion.egg-info/dependency_links.txt
 PyExpansion.egg-info/top_level.txt
 PyExpansion/application/__init__.py
-PyExpansion/application/PyIC/__init__.py
-PyExpansion/application/PyIC/main.py
-PyExpansion/application/PyIC/status_code_list.py
-PyExpansion/application/PyIC/tests.py
-PyExpansion/application/PyIC/version.py
-PyExpansion/application/PyIC/country/Malaysia.py
-PyExpansion/application/PyIC/country/Singapore.py
-PyExpansion/application/PyIC/country/__init__.py
-PyExpansion/application/PyIC/country/base.py
-PyExpansion/application/PyIC/country/malaysia.py
+PyExpansion/application/human_resource/__init__.py
+PyExpansion/application/human_resource/PyIC/__init__.py
+PyExpansion/application/human_resource/PyIC/main.py
+PyExpansion/application/human_resource/PyIC/status_code_list.py
+PyExpansion/application/human_resource/PyIC/tests.py
+PyExpansion/application/human_resource/PyIC/country/Malaysia.py
+PyExpansion/application/human_resource/PyIC/country/Singapore.py
+PyExpansion/application/human_resource/PyIC/country/__init__.py
+PyExpansion/application/human_resource/PyIC/country/base.py
 PyExpansion/common/__init__.py
 PyExpansion/common/basic_function.py
 PyExpansion/common/message.py
-PyExpansion/common/status_code_list.py
 PyExpansion/common/utils.py
 PyExpansion/common/version_history.py
+PyExpansion/common/constants/__init__.py
+PyExpansion/common/constants/common.py
 PyExpansion/common/data_type/__init__.py
 PyExpansion/common/data_type/lists/__init__.py
 PyExpansion/common/data_type/lists/main.py
 PyExpansion/common/data_type/lists/status_code_list.py
-PyExpansion/common/data_type/lists/tests.py
+PyExpansion/common/data_type/lists/tests.py
+PyExpansion/common/status_code/__init__.py
+PyExpansion/common/status_code/http_code.py
+PyExpansion/common/status_code/utils.py
+PyExpansion/just_for_fun/__init__.py
+PyExpansion/just_for_fun/PyBrainFuck/__init__.py
+PyExpansion/just_for_fun/PyBrainFuck/main.py
+PyExpansion/just_for_fun/PyBrainFuck/tests.py
```

### Comparing `PyExpansion-0.0.1a20230622/README.md` & `PyExpansion-0.0.1a20230624/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,45 @@
 
 ![PyPI](https://img.shields.io/pypi/v/pyexpansion) &nbsp;
 ![License: MIT](https://img.shields.io/github/license/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub issues](https://img.shields.io/github/issues/weitaoyap111/pyexpansion)&nbsp;
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/weitaoyap111/pyexpansion)&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/pyexpansion?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/pyexpansion)&nbsp;
 
-Python script that suddenly come to my idea
+Python script that suddenly come to my idea <br>
 Will update more...
 
 # Installation
 How to install:
-```python
+```
 pip install pyexpansion
 ```
 
 # Library List:
 ## 1) PyIC
 ### What is this?
 - Python Script that extract the ic information from ic word.
 
 ### How to use it?
 - You can refer to PyIC\tests.py.
 
+### Want knows more? 
+you can read at PyIC\README.md
+
+## 2) PyBrainFuck
+### What is this?
+- Python Script that decode and encode using BrainFuck.
+
+### How to use it?
+- You can refer to PyBrainFuck\tests.py.
+
+### Want knows more? 
+you can read at PyBrainFuck\README.md
+
+# Projects Status
 ### Updated
 - Apply for Malaysia Only
 - Singapore Added
+- PyBrainFuck is added
 
 # Author
 Copyright (c) 2023 Wei Tao Yap
```

### Comparing `PyExpansion-0.0.1a20230622/setup.py` & `PyExpansion-0.0.1a20230624/setup.py`

 * *Files identical despite different names*

