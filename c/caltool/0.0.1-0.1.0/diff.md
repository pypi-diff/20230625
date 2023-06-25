# Comparing `tmp/caltool-0.0.1.tar.gz` & `tmp/caltool-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\caltool-0.0.1.tar", last modified: Sun Jun 25 09:33:22 2023, max compression
+gzip compressed data, was "dist\caltool-0.1.0.tar", last modified: Sun Jun 25 09:52:11 2023, max compression
```

## Comparing `caltool-0.0.1.tar` & `caltool-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:33:22.000000 caltool-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool/
--rw-rw-rw-   0        0        0        2 2023-06-25 08:46:14.000000 caltool-0.0.1/caltool/utils.py
--rw-rw-rw-   0        0        0     3434 2023-06-25 09:25:56.000000 caltool-0.0.1/caltool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2387 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/requires.txt
--rw-rw-rw-   0        0        0      221 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 09:33:22.000000 caltool-0.0.1/caltool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 caltool-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2387 2023-06-25 09:33:22.000000 caltool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 caltool-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 09:33:22.000000 caltool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-06-25 09:27:36.000000 caltool-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:52:11.000000 caltool-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool/
+-rw-rw-rw-   0        0        0        2 2023-06-25 08:46:14.000000 caltool-0.1.0/caltool/utils.py
+-rw-rw-rw-   0        0        0     3434 2023-06-25 09:25:56.000000 caltool-0.1.0/caltool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2387 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      221 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 09:52:11.000000 caltool-0.1.0/caltool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 caltool-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2387 2023-06-25 09:52:11.000000 caltool-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 caltool-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:52:11.000000 caltool-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-06-25 09:51:16.000000 caltool-0.1.0/setup.py
```

### Comparing `caltool-0.0.1/caltool/__init__.py` & `caltool-0.1.0/caltool/__init__.py`

 * *Files identical despite different names*

### Comparing `caltool-0.0.1/caltool.egg-info/PKG-INFO` & `caltool-0.1.0/caltool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltool
-Version: 0.0.1
+Version: 0.1.0
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `caltool-0.0.1/LICENSE.txt` & `caltool-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caltool-0.0.1/PKG-INFO` & `caltool-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltool
-Version: 0.0.1
+Version: 0.1.0
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `caltool-0.0.1/README.md` & `caltool-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `caltool-0.0.1/setup.py` & `caltool-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="caltool",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于pip维护版本
+    version="0.1.0",  # 包版本号，便于pip维护版本
     author="Huii Ji",  # 作者，可以写自己的姓名
     author_email="752413464@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package of calculator for params/macs ",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuiiJi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     install_requires=[
-        'os',
         'torch',
         'onnx',
         'onnx-tool',
         'thop',
         'netron'
         # add any other dependencies here
     ],
```

