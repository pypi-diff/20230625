# Comparing `tmp/pointnet-0.0.2.tar.gz` & `tmp/pointnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointnet-0.0.2.tar", last modified: Fri Jun 23 23:13:09 2023, max compression
+gzip compressed data, was "pointnet-0.0.3.tar", last modified: Sat Jun 24 22:16:09 2023, max compression
```

## Comparing `pointnet-0.0.2.tar` & `pointnet-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:13:09.480347 pointnet-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 23:12:59.000000 pointnet-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 23:13:09.480347 pointnet-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-23 23:12:59.000000 pointnet-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:13:09.480347 pointnet-0.0.2/pointnet/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 23:12:59.000000 pointnet-0.0.2/pointnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-23 23:12:59.000000 pointnet-0.0.2/pointnet/pointnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-23 23:12:59.000000 pointnet-0.0.2/pointnet/pointnet2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-23 23:12:59.000000 pointnet-0.0.2/pointnet/taichi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 23:12:59.000000 pointnet-0.0.2/pointnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:13:09.480347 pointnet-0.0.2/pointnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 23:13:09.000000 pointnet-0.0.2/pointnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 23:13:09.000000 pointnet-0.0.2/pointnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:13:09.000000 pointnet-0.0.2/pointnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 23:13:09.000000 pointnet-0.0.2/pointnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:13:09.000000 pointnet-0.0.2/pointnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:13:09.480347 pointnet-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-23 23:12:59.000000 pointnet-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:16:09.414361 pointnet-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-24 22:15:59.000000 pointnet-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-24 22:16:09.414361 pointnet-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-24 22:15:59.000000 pointnet-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:16:09.414361 pointnet-0.0.3/pointnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-24 22:15:59.000000 pointnet-0.0.3/pointnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-24 22:15:59.000000 pointnet-0.0.3/pointnet/pointnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-06-24 22:15:59.000000 pointnet-0.0.3/pointnet/pointnet2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-24 22:15:59.000000 pointnet-0.0.3/pointnet/taichi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-24 22:15:59.000000 pointnet-0.0.3/pointnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:16:09.414361 pointnet-0.0.3/pointnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-24 22:16:09.000000 pointnet-0.0.3/pointnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-24 22:16:09.000000 pointnet-0.0.3/pointnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:16:09.000000 pointnet-0.0.3/pointnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-24 22:16:09.000000 pointnet-0.0.3/pointnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 22:16:09.000000 pointnet-0.0.3/pointnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:16:09.414361 pointnet-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-24 22:15:59.000000 pointnet-0.0.3/setup.py
```

### Comparing `pointnet-0.0.2/LICENSE` & `pointnet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.2/PKG-INFO` & `pointnet-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: PointNet - Pytorch
 Home-page: https://github.com/kentechx/pointnet
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pointnet-0.0.2/README.md` & `pointnet-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ```bash
 pip install pointnet -i https://pypi.org/simple
 ```
 
 ## Usage
 
 ### PointNet
+
 Perform classification with inputs xyz coordinates:
 
 ```python
 import torch
 from pointnet import PointNetCls
 
 model = PointNetCls(in_dim=3, out_dim=40)
@@ -56,49 +57,54 @@
 
 model = PointNetSeg(3, 40)
 x = torch.randn(16, 3, 1024)
 logits = model(x)
 ```
 
 ### PointNet2
-PointNet2 uses [taichi](https://github.com/taichi-dev/taichi) to accelerate the computation of ball query. You need to 
+
+PointNet2 uses [taichi](https://github.com/taichi-dev/taichi) to accelerate the computation of ball query. You need to
 initialize taichi before using PointNet2.
 
 Perform classification with inputs xyz coordinates:
 
 ```python
 import torch
 from pointnet import PointNet2SSGCls
 
 import taichi as ti
+
 ti.init(arch=ti.cuda)
 
 model = PointNet2SSGCls(in_dim=3, out_dim=40).cuda()
 x = torch.randn(16, 3, 1024).cuda()
 logits = model(x)
 ```
 
-
-
 ## Performance
-Classification accuracy on ModelNet40 dataset (2048 points, see [modelnet40_experiments](
+
+Classification accuracy on ModelNet40 dataset (see [modelnet40_experiments](
 https://github.com/kentechx/modelnet40_experiments) for details):
 
-| Model                   | Overall Accuracy |
-|-------------------------|------------------|
-| PointNet                | 89.4%            |
+| Model                | input | Overall Accuracy |
+|----------------------|-------|------------------|
+| PointNet (official)  | xyz   | 89.2%            |
+| PointNet             | xyz   | 90.7%            |
+| PointNet2 (official) | xyz   | 90.7%            |
+| PointNet2SSG         | xyz   | 90.7%            |
+| PointNet2MSG         | xyz   | 92.1%            |
 
 ## Other Implementationss
+
 [charlesq34/pointnet](https://github.com/charlesq34/pointnet)
 
 [fxia22/pointnet.pytorch](https://github.com/fxia22/pointnet.pytorch)
 
 [yanx27/Pointnet_Pointnet2_pytorch](https://github.com/yanx27/Pointnet_Pointnet2_pytorch)
 
-
 ## References
 
 ```bibtex
 @article{qi2017pointnet,
   title={Pointnet: Deep learning on point sets for 3d classification and segmentation},
   author={Qi, Charles R and Su, Hao and Mo, Kaichun and Guibas, Leonidas J},
   booktitle={Proceedings of the IEEE conference on computer vision and pattern recognition},
```

### Comparing `pointnet-0.0.2/pointnet/pointnet.py` & `pointnet-0.0.3/pointnet/pointnet.py`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.2/pointnet/utils.py` & `pointnet-0.0.3/pointnet/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     b, n = src.shape[:2]
     m = query.shape[1]
     dists = torch.cdist(query, src)  # (b, m, n)
     idx = repeat(torch.arange(n, device=src.device), 'n -> b m n', b=b, m=m)
     idx = torch.where(dists > radius, n, idx)
     idx = idx.sort(dim=-1).values[:, :, :k]  # (b, m, k)
     idx = torch.where(idx == n, idx[:, :, [0]], idx)
-    return idx
+    _dists = dists.gather(-1, idx)  # (b, m, k)
+    return idx, _dists
```

### Comparing `pointnet-0.0.2/pointnet.egg-info/PKG-INFO` & `pointnet-0.0.3/pointnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: PointNet - Pytorch
 Home-page: https://github.com/kentechx/pointnet
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pointnet-0.0.2/setup.py` & `pointnet-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pointnet',
     packages=find_packages(),
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='PointNet - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/pointnet',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

