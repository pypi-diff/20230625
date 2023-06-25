# Comparing `tmp/countool-0.0.2.tar.gz` & `tmp/countool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\countool-0.0.2.tar", last modified: Sun Jun 25 12:46:36 2023, max compression
+gzip compressed data, was "dist\countool-0.0.3.tar", last modified: Sun Jun 25 13:31:39 2023, max compression
```

## Comparing `countool-0.0.2.tar` & `countool-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/countool/
--rw-rw-rw-   0        0        0     3509 2023-06-25 12:44:25.000000 countool-0.0.2/countool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/requires.txt
--rw-rw-rw-   0        0        0      210 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 12:46:36.000000 countool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 12:46:36.000000 countool-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-06-25 12:44:34.000000 countool-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:31:39.000000 countool-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-25 13:31:38.000000 countool-0.0.3/countool/
+-rw-rw-rw-   0        0        0     3498 2023-06-25 13:31:15.000000 countool-0.0.3/countool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      210 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-25 13:31:39.000000 countool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 13:31:39.000000 countool-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-06-25 13:31:36.000000 countool-0.0.3/setup.py
```

### Comparing `countool-0.0.2/countool/__init__.py` & `countool-0.0.3/countool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             print("2.onnx_Model correct...")
             print('3.use onnx_tool to profile model...')
             modelpath = output_path
             onnx_tool.model_profile(modelpath)  # pass file name
             onnx_tool.model_profile(modelpath, savenode=f'{output_path[:-5]}' + sufix)  # save profile table to txt file
     if use_netron:
         print('4.use netron to visualize model...')
-        netron.start(output_path, port=8080)
+        netron.start(output_path)
 
 
 
 # if __name__ == "__main__":
 #     from pth2onnx import ControlNetHED_Apache2
 #     model = ControlNetHED_Apache2()
 #     model.eval()
```

### Comparing `countool-0.0.2/countool.egg-info/PKG-INFO` & `countool-0.0.3/countool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.2/LICENSE.txt` & `countool-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countool-0.0.2/PKG-INFO` & `countool-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.2/README.md` & `countool-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `countool-0.0.2/setup.py` & `countool-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="countool",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",  # 包版本号，便于pip维护版本
+    version="0.0.3",  # 包版本号，便于pip维护版本
     author="Huii Ji",  # 作者，可以写自己的姓名
     author_email="752413464@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package of calculator for params/macs ",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuiiJi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

