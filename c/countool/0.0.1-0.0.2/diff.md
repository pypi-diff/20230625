# Comparing `tmp/countool-0.0.1.tar.gz` & `tmp/countool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\countool-0.0.1.tar", last modified: Sun Jun 25 10:46:48 2023, max compression
+gzip compressed data, was "dist\countool-0.0.2.tar", last modified: Sun Jun 25 12:46:36 2023, max compression
```

## Comparing `countool-0.0.1.tar` & `countool-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 10:46:48.000000 countool-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-25 10:46:48.000000 countool-0.0.1/countool/
--rw-rw-rw-   0        0        0     3448 2023-06-25 10:26:04.000000 countool-0.0.1/countool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/requires.txt
--rw-rw-rw-   0        0        0      210 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 10:46:48.000000 countool-0.0.1/countool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 10:46:48.000000 countool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 10:46:48.000000 countool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-06-25 10:44:40.000000 countool-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/countool/
+-rw-rw-rw-   0        0        0     3509 2023-06-25 12:44:25.000000 countool-0.0.2/countool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      210 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 12:46:36.000000 countool-0.0.2/countool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-25 12:46:36.000000 countool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 12:46:36.000000 countool-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-06-25 12:44:34.000000 countool-0.0.2/setup.py
```

### Comparing `countool-0.0.1/countool/__init__.py` & `countool-0.0.2/countool/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import onnx_tool
 import torch
 import torch.nn as nn
 # import onnx
 import os
 from thop import profile, clever_format
 import netron
-
-def load_onnx_model(onnx_path):
-    onnx_model = onnx.load(onnx_path)
-    onnx.checker.check_model(onnx_model)
-    return onnx_model
-
-def load_pytorch_model(model_path):
-    model = torch.load(model_path)
-    return model
-
-def compare_model(onnx_model, pytorch_model, input_size, input_tensor):
-    onnx_input = input_tensor.cpu().numpy()
-    pytorch_input = input_tensor
-    onnx_output = onnx_tool.run_onnx_model(onnx_model, onnx_input)
-    pytorch_output = pytorch_model(pytorch_input)
-    print('onnx_output:', onnx_output)
-    print('pytorch_output:', pytorch_output)
-    print('onnx_output - pytorch_output:', onnx_output - pytorch_output)
+#
+# def load_onnx_model(onnx_path):
+#     onnx_model = onnx.load(onnx_path)
+#     onnx.checker.check_model(onnx_model)
+#     return onnx_model
+#
+# def load_pytorch_model(model_path):
+#     model = torch.load(model_path)
+#     return model
+#
+# def compare_model(onnx_model, pytorch_model, input_size, input_tensor):
+#     onnx_input = input_tensor.cpu().numpy()
+#     pytorch_input = input_tensor
+#     onnx_output = onnx_tool.run_onnx_model(onnx_model, onnx_input)
+#     pytorch_output = pytorch_model(pytorch_input)
+#     print('onnx_output:', onnx_output)
+#     print('pytorch_output:', pytorch_output)
+#     print('onnx_output - pytorch_output:', onnx_output - pytorch_output)
 
 def mkfolder(path):
     if isinstance(path, list):
         for p in path:
             if not os.path.exists(p):
                 os.makedirs(p)
                 print({p}, 'is created for saving the results.')
@@ -46,15 +46,16 @@
     assert isinstance(model, nn.Module), 'model must be a nn.Module'
     assert isinstance(input_shape, tuple), 'input_data must be a torch.tensor'
     assert isinstance(output_path, str), 'output_path must be a str'
     assert isinstance(use_onnx_tool, bool), 'use_onnx_tool must be a bool'
     if sufix not in ['.txt', '.csv']:
         raise ValueError('sufix must be txt or csv')
 
-    mkfolder(output_path)
+    # mkfolder(output_path)
+    # print(output_path)
     input_data = torch.randn(input_shape)
     model.eval()
 
     if use_opcounter:
         flops, params = profile(model, inputs=(input_data, ))
         flops, params = clever_format([flops, params], "%.3f")
         print("1.torch_Model profile...")
```

### Comparing `countool-0.0.1/countool.egg-info/PKG-INFO` & `countool-0.0.2/countool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.1/LICENSE.txt` & `countool-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countool-0.0.1/PKG-INFO` & `countool-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.1/README.md` & `countool-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `countool-0.0.1/setup.py` & `countool-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="countool",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于pip维护版本
+    version="0.0.2",  # 包版本号，便于pip维护版本
     author="Huii Ji",  # 作者，可以写自己的姓名
     author_email="752413464@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package of calculator for params/macs ",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuiiJi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

