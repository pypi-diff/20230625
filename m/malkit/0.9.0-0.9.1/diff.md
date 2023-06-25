# Comparing `tmp/malkit-0.9.0.tar.gz` & `tmp/malkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malkit-0.9.0.tar", last modified: Fri Apr 22 07:31:42 2022, max compression
+gzip compressed data, was "malkit-0.9.1.tar", last modified: Tue May 24 02:05:56 2022, max compression
```

## Comparing `malkit-0.9.0.tar` & `malkit-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:42.055673 malkit-0.9.0/
--rw-rw-rw-   0        0        0     1082 2021-11-06 10:32:56.000000 malkit-0.9.0/LICENSE
--rw-rw-rw-   0        0        0       68 2021-11-06 10:33:03.000000 malkit-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2093 2022-04-22 07:31:42.056674 malkit-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      904 2021-11-30 02:50:21.000000 malkit-0.9.0/README.md
--rw-rw-rw-   0        0        0      246 2022-03-11 02:01:45.000000 malkit-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0     1449 2022-04-22 07:31:42.058675 malkit-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2020-12-05 11:36:39.000000 malkit-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:41.946649 malkit-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:41.981656 malkit-0.9.0/src/malkit/
--rw-rw-rw-   0        0        0      879 2022-04-22 07:31:05.000000 malkit-0.9.0/src/malkit/__init__.py
--rw-rw-rw-   0        0        0     1007 2021-12-23 12:23:58.000000 malkit-0.9.0/src/malkit/_parallel.py
--rw-rw-rw-   0        0        0       83 2021-11-09 07:10:02.000000 malkit-0.9.0/src/malkit/_typing.py
--rw-rw-rw-   0        0        0     2859 2021-12-24 06:10:50.000000 malkit-0.9.0/src/malkit/byte.py
--rw-rw-rw-   0        0        0     3683 2021-12-22 07:46:58.000000 malkit-0.9.0/src/malkit/image.py
--rw-rw-rw-   0        0        0        0 2021-11-30 02:00:04.000000 malkit-0.9.0/src/malkit/py.typed
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:42.039669 malkit-0.9.0/src/malkit/torch/
--rw-rw-rw-   0        0        0      461 2021-11-30 02:16:56.000000 malkit-0.9.0/src/malkit/torch/__init__.py
--rw-rw-rw-   0        0        0     3731 2021-12-22 09:10:51.000000 malkit-0.9.0/src/malkit/torch/checkpoint.py
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:42.052673 malkit-0.9.0/src/malkit/torch/data/
--rw-rw-rw-   0        0        0      115 2022-04-19 08:02:30.000000 malkit-0.9.0/src/malkit/torch/data/__init__.py
--rw-rw-rw-   0        0        0     2925 2022-04-19 08:01:55.000000 malkit-0.9.0/src/malkit/torch/data/_dataset.py
--rw-rw-rw-   0        0        0      498 2022-04-19 07:52:56.000000 malkit-0.9.0/src/malkit/torch/data/_loader.py
--rw-rw-rw-   0        0        0     1272 2022-04-19 10:46:02.000000 malkit-0.9.0/src/malkit/torch/data/binary.py
--rw-rw-rw-   0        0        0     7760 2021-12-22 09:00:55.000000 malkit-0.9.0/src/malkit/torch/dataset.py
--rw-rw-rw-   0        0        0     1589 2022-03-15 01:43:56.000000 malkit-0.9.0/src/malkit/torch/models.py
--rw-rw-rw-   0        0        0     4642 2021-11-29 09:30:29.000000 malkit-0.9.0/src/malkit/utils.py
-drwxrwxrwx   0        0        0        0 2022-04-22 07:31:42.027667 malkit-0.9.0/src/malkit.egg-info/
--rw-rw-rw-   0        0        0     2093 2022-04-22 07:31:41.000000 malkit-0.9.0/src/malkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2022-04-22 07:31:41.000000 malkit-0.9.0/src/malkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-22 07:31:41.000000 malkit-0.9.0/src/malkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-07 02:36:00.000000 malkit-0.9.0/src/malkit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      103 2022-04-22 07:31:41.000000 malkit-0.9.0/src/malkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-04-22 07:31:41.000000 malkit-0.9.0/src/malkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.123558 malkit-0.9.1/
+-rw-rw-rw-   0        0        0     1082 2021-11-06 10:32:56.000000 malkit-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0       68 2021-11-06 10:33:03.000000 malkit-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2089 2022-05-24 02:05:56.124559 malkit-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      904 2021-11-30 02:50:21.000000 malkit-0.9.1/README.md
+-rw-rw-rw-   0        0        0      246 2022-03-11 02:01:45.000000 malkit-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1449 2022-05-24 02:05:56.125558 malkit-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2020-12-05 11:36:39.000000 malkit-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.068551 malkit-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.086554 malkit-0.9.1/src/malkit/
+-rw-rw-rw-   0        0        0      879 2022-05-24 02:05:13.000000 malkit-0.9.1/src/malkit/__init__.py
+-rw-rw-rw-   0        0        0     1007 2021-12-23 12:23:58.000000 malkit-0.9.1/src/malkit/_parallel.py
+-rw-rw-rw-   0        0        0       83 2021-11-09 07:10:02.000000 malkit-0.9.1/src/malkit/_typing.py
+-rw-rw-rw-   0        0        0     2859 2021-12-24 06:10:50.000000 malkit-0.9.1/src/malkit/byte.py
+-rw-rw-rw-   0        0        0     3683 2021-12-22 07:46:58.000000 malkit-0.9.1/src/malkit/image.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 02:00:04.000000 malkit-0.9.1/src/malkit/py.typed
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.114558 malkit-0.9.1/src/malkit/torch/
+-rw-rw-rw-   0        0        0      461 2021-11-30 02:16:56.000000 malkit-0.9.1/src/malkit/torch/__init__.py
+-rw-rw-rw-   0        0        0     3731 2021-12-22 09:10:51.000000 malkit-0.9.1/src/malkit/torch/checkpoint.py
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.119560 malkit-0.9.1/src/malkit/torch/data/
+-rw-rw-rw-   0        0        0      115 2022-04-19 08:02:30.000000 malkit-0.9.1/src/malkit/torch/data/__init__.py
+-rw-rw-rw-   0        0        0     2925 2022-04-19 08:01:55.000000 malkit-0.9.1/src/malkit/torch/data/_dataset.py
+-rw-rw-rw-   0        0        0      498 2022-04-19 07:52:56.000000 malkit-0.9.1/src/malkit/torch/data/_loader.py
+-rw-rw-rw-   0        0        0     1272 2022-04-19 10:46:02.000000 malkit-0.9.1/src/malkit/torch/data/binary.py
+-rw-rw-rw-   0        0        0     7760 2021-12-22 09:00:55.000000 malkit-0.9.1/src/malkit/torch/dataset.py
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.122558 malkit-0.9.1/src/malkit/torch/models/
+-rw-rw-rw-   0        0        0        0 2022-05-24 02:01:09.000000 malkit-0.9.1/src/malkit/torch/models/__init__.py
+-rw-rw-rw-   0        0        0     1918 2022-05-24 02:00:10.000000 malkit-0.9.1/src/malkit/torch/models/malconv.py
+-rw-rw-rw-   0        0        0     4642 2021-11-29 09:30:29.000000 malkit-0.9.1/src/malkit/utils.py
+drwxrwxrwx   0        0        0        0 2022-05-24 02:05:56.108557 malkit-0.9.1/src/malkit.egg-info/
+-rw-rw-rw-   0        0        0     2089 2022-05-24 02:05:55.000000 malkit-0.9.1/src/malkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2022-05-24 02:05:56.000000 malkit-0.9.1/src/malkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-24 02:05:55.000000 malkit-0.9.1/src/malkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-07 02:36:00.000000 malkit-0.9.1/src/malkit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      103 2022-05-24 02:05:55.000000 malkit-0.9.1/src/malkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-05-24 02:05:56.000000 malkit-0.9.1/src/malkit.egg-info/top_level.txt
```

### Comparing `malkit-0.9.0/LICENSE` & `malkit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/PKG-INFO` & `malkit-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Malware analysis toolkit for machine learning
 Home-page: https://github.com/xymy/malkit
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -46,9 +46,7 @@
 Install from PyPI:
 
 ```shell
 $ pip install malkit
 ```
 
 If you want to use `malkit.torch`, you should install PyTorch manually since it is not declared as a dependency.
-
-
```

### Comparing `malkit-0.9.0/README.md` & `malkit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/setup.cfg` & `malkit-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/__init__.py` & `malkit-0.9.1/src/malkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     "categorize_folders",
     "split_labels",
     "build_srcs_dsts",
     "convert_bytes_to_binary",
     "convert_bytes_to_binary_parallel",
 ]
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `malkit-0.9.0/src/malkit/_parallel.py` & `malkit-0.9.1/src/malkit/_parallel.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/byte.py` & `malkit-0.9.1/src/malkit/byte.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/image.py` & `malkit-0.9.1/src/malkit/image.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/torch/checkpoint.py` & `malkit-0.9.1/src/malkit/torch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/torch/data/_dataset.py` & `malkit-0.9.1/src/malkit/torch/data/_dataset.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/torch/data/binary.py` & `malkit-0.9.1/src/malkit/torch/data/binary.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/torch/dataset.py` & `malkit-0.9.1/src/malkit/torch/dataset.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit/torch/models.py` & `malkit-0.9.1/src/malkit/torch/models/malconv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 import torch
 import torch.nn as nn
+from torch import Tensor
 
 
 class MalConv(nn.Module):
     """The MalConv model.
 
     References:
         - Edward Raff et al. 2018. Malware Detection by Eating a Whole EXE.
@@ -21,14 +22,16 @@
         channels: int = 128,
         kernel_size: int = 512,
         stride: int = 512,
         padding_idx: Optional[int] = 256,
     ) -> None:
         super().__init__()
 
+        self.num_classes = num_classes
+
         # By default, num_embeddings (257) = byte (0-255) + padding (256).
         self.embedding = nn.Embedding(num_embeddings, embedding_dim, padding_idx=padding_idx)
 
         self.conv1 = nn.Conv1d(embedding_dim, channels, kernel_size=kernel_size, stride=stride, bias=True)
         self.conv2 = nn.Conv1d(embedding_dim, channels, kernel_size=kernel_size, stride=stride, bias=True)
 
         self.maxpool = nn.AdaptiveMaxPool1d(1)
@@ -36,20 +39,29 @@
         self.fc = nn.Sequential(
             nn.Flatten(),
             nn.Linear(channels, channels),
             nn.ReLU(inplace=True),
             nn.Linear(channels, num_classes),
         )
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
+    def _embed(self, x: Tensor) -> Tensor:
+        # Perform embedding.
         x = self.embedding(x)
 
         # Treat embedding dimension as channel.
         x = x.permute(0, 2, 1)
+        return x
 
+    def _forward_embedded(self, x: Tensor) -> Tensor:
         # Perform gated convolution.
         x = self.conv1(x) * torch.sigmoid(self.conv2(x))
 
+        # Perform global max pooling.
         x = self.maxpool(x)
 
         x = self.fc(x)
         return x
+
+    def forward(self, x: Tensor) -> Tensor:
+        x = self._embed(x)
+        x = self._forward_embedded(x)
+        return x
```

### Comparing `malkit-0.9.0/src/malkit/utils.py` & `malkit-0.9.1/src/malkit/utils.py`

 * *Files identical despite different names*

### Comparing `malkit-0.9.0/src/malkit.egg-info/PKG-INFO` & `malkit-0.9.1/src/malkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Malware analysis toolkit for machine learning
 Home-page: https://github.com/xymy/malkit
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -46,9 +46,7 @@
 Install from PyPI:
 
 ```shell
 $ pip install malkit
 ```
 
 If you want to use `malkit.torch`, you should install PyTorch manually since it is not declared as a dependency.
-
-
```

### Comparing `malkit-0.9.0/src/malkit.egg-info/SOURCES.txt` & `malkit-0.9.1/src/malkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 src/malkit.egg-info/dependency_links.txt
 src/malkit.egg-info/not-zip-safe
 src/malkit.egg-info/requires.txt
 src/malkit.egg-info/top_level.txt
 src/malkit/torch/__init__.py
 src/malkit/torch/checkpoint.py
 src/malkit/torch/dataset.py
-src/malkit/torch/models.py
 src/malkit/torch/data/__init__.py
 src/malkit/torch/data/_dataset.py
 src/malkit/torch/data/_loader.py
-src/malkit/torch/data/binary.py
+src/malkit/torch/data/binary.py
+src/malkit/torch/models/__init__.py
+src/malkit/torch/models/malconv.py
```

