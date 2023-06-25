# Comparing `tmp/PyMobileProvision-1.4.4.tar.gz` & `tmp/PyMobileProvision-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMobileProvision-1.4.4.tar", last modified: Wed Jun  7 04:47:03 2023, max compression
+gzip compressed data, was "PyMobileProvision-1.4.5.tar", last modified: Sun Jun 25 06:14:41 2023, max compression
```

## Comparing `PyMobileProvision-1.4.4.tar` & `PyMobileProvision-1.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.477977 PyMobileProvision-1.4.4/
--rw-r--r--   0 shaowei    (501) staff       (20)     1065 2019-05-17 03:04:35.000000 PyMobileProvision-1.4.4/LICENSE
--rw-r--r--   0 shaowei    (501) staff       (20)     5257 2023-06-07 04:47:03.477780 PyMobileProvision-1.4.4/PKG-INFO
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.476199 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/
--rw-r--r--   0 shaowei    (501) staff       (20)     5257 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/PKG-INFO
--rw-r--r--   0 shaowei    (501) staff       (20)      379 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/SOURCES.txt
--rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/dependency_links.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       66 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/entry_points.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       19 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/requires.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       16 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/top_level.txt
--rw-r--r--   0 shaowei    (501) staff       (20)     4267 2023-06-07 04:39:55.000000 PyMobileProvision-1.4.4/README.md
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.477341 PyMobileProvision-1.4.4/mobileprovision/
--rw-r--r--   0 shaowei    (501) staff       (20)      121 2019-11-20 12:06:23.000000 PyMobileProvision-1.4.4/mobileprovision/__init__.py
--rw-r--r--   0 shaowei    (501) staff       (20)     2992 2019-11-21 12:23:14.000000 PyMobileProvision-1.4.4/mobileprovision/command.py
--rwxr-xr-x   0 shaowei    (501) staff       (20)    10097 2023-06-07 04:44:55.000000 PyMobileProvision-1.4.4/mobileprovision/parser.py
--rw-r--r--   0 shaowei    (501) staff       (20)     2499 2019-11-27 03:30:49.000000 PyMobileProvision-1.4.4/mobileprovision/util.py
--rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-06-07 04:47:03.478047 PyMobileProvision-1.4.4/setup.cfg
--rw-r--r--   0 shaowei    (501) staff       (20)     1605 2023-06-07 04:40:01.000000 PyMobileProvision-1.4.4/setup.py
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-25 06:14:41.616982 PyMobileProvision-1.4.5/
+-rw-r--r--   0 shaowei    (501) staff       (20)     1065 2019-05-17 03:04:35.000000 PyMobileProvision-1.4.5/LICENSE
+-rw-r--r--   0 shaowei    (501) staff       (20)     5220 2023-06-25 06:14:41.616750 PyMobileProvision-1.4.5/PKG-INFO
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-25 06:14:41.614997 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/
+-rw-r--r--   0 shaowei    (501) staff       (20)     5220 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/PKG-INFO
+-rw-r--r--   0 shaowei    (501) staff       (20)      379 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/SOURCES.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/dependency_links.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       65 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/entry_points.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       19 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/requires.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       16 2023-06-25 06:14:41.000000 PyMobileProvision-1.4.5/PyMobileProvision.egg-info/top_level.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)     4267 2023-06-07 04:39:55.000000 PyMobileProvision-1.4.5/README.md
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-25 06:14:41.616292 PyMobileProvision-1.4.5/mobileprovision/
+-rw-r--r--   0 shaowei    (501) staff       (20)      121 2019-11-20 12:06:23.000000 PyMobileProvision-1.4.5/mobileprovision/__init__.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     2992 2019-11-21 12:23:14.000000 PyMobileProvision-1.4.5/mobileprovision/command.py
+-rwxr-xr-x   0 shaowei    (501) staff       (20)    10099 2023-06-25 06:11:19.000000 PyMobileProvision-1.4.5/mobileprovision/parser.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     2499 2019-11-27 03:30:49.000000 PyMobileProvision-1.4.5/mobileprovision/util.py
+-rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-06-25 06:14:41.617058 PyMobileProvision-1.4.5/setup.cfg
+-rw-r--r--   0 shaowei    (501) staff       (20)     1605 2023-06-25 06:12:33.000000 PyMobileProvision-1.4.5/setup.py
```

### Comparing `PyMobileProvision-1.4.4/LICENSE` & `PyMobileProvision-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.4/PKG-INFO` & `PyMobileProvision-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: PyMobileProvision
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python3, parse ".mobileprovision" file in MacOS System;
 Home-page: https://github.com/shede333/PyMobileProvision
 Author: shede333
 Author-email: 333wshw@163.com
-License: UNKNOWN
 Keywords: mobileprovision mobile provision MobileProvision profile profiles
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
@@ -131,9 +129,7 @@
 
 Android工程师任职要求：  
 1.本科以上学历，可使用英文交流者加分；  
 2.三年以上Android开发经验；  
 3.熟悉Android常用控件的使用并理解其原理；  
 4.熟悉Android Framework原理，阅读过Android源代码者优先；  
 5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
-
-
```

### Comparing `PyMobileProvision-1.4.4/PyMobileProvision.egg-info/PKG-INFO` & `PyMobileProvision-1.4.5/PyMobileProvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: PyMobileProvision
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python3, parse ".mobileprovision" file in MacOS System;
 Home-page: https://github.com/shede333/PyMobileProvision
 Author: shede333
 Author-email: 333wshw@163.com
-License: UNKNOWN
 Keywords: mobileprovision mobile provision MobileProvision profile profiles
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
@@ -131,9 +129,7 @@
 
 Android工程师任职要求：  
 1.本科以上学历，可使用英文交流者加分；  
 2.三年以上Android开发经验；  
 3.熟悉Android常用控件的使用并理解其原理；  
 4.熟悉Android Framework原理，阅读过Android源代码者优先；  
 5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
-
-
```

### Comparing `PyMobileProvision-1.4.4/README.md` & `PyMobileProvision-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.4/mobileprovision/command.py` & `PyMobileProvision-1.4.5/mobileprovision/command.py`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.4/mobileprovision/parser.py` & `PyMobileProvision-1.4.5/mobileprovision/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,16 @@
         return self._dev_cer_list
 
     def date_is_valid(self):
         """
         文件现在是否在有效日期范围内
         :return: 有效则返回true
         """
-        # 由于本地时间和服务端时间有偏差，特别是profile刚创建完的时候，起始时间兼容 60秒 误差
-        start_is_valid = (datetime.utcnow().timestamp() - self.creation_timestamp) > -60
+        # 由于本地时间和服务端时间有偏差，特别是profile刚创建完的时候，起始时间兼容 180秒 误差
+        start_is_valid = (datetime.utcnow().timestamp() - self.creation_timestamp) > -180
         return start_is_valid and (datetime.utcnow().timestamp() < self.expiration_timestamp)
 
     def app_id(self, is_need_prefix=False):
         """
         标示App的bundleID，例如：com.apple.xcode
         :param is_need_prefix: 是否需要带上ApplicationIdentifierPrefix前缀，默认False
         :return: 标示App的ID
```

### Comparing `PyMobileProvision-1.4.4/mobileprovision/util.py` & `PyMobileProvision-1.4.5/mobileprovision/util.py`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.4/setup.py` & `PyMobileProvision-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 # print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='PyMobileProvision',  # 包名字
-    version='1.4.4',  # 包版本
+    version='1.4.5',  # 包版本
     author='shede333',  # 作者
     author_email='333wshw@163.com',  # 作者邮箱
     keywords='mobileprovision mobile provision MobileProvision profile profiles',
     description='Python3, parse ".mobileprovision" file in MacOS System;',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/shede333/PyMobileProvision',  # 包的主页
```

