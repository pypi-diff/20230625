# Comparing `tmp/focalnet-tf-0.0.2.1.tar.gz` & `tmp/focalnet-tf-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\focalnet-tf-0.0.2.1.tar", last modified: Fri Jun 16 23:49:16 2023, max compression
+gzip compressed data, was "dist\focalnet-tf-0.0.2.2.tar", last modified: Sun Jun 25 19:54:31 2023, max compression
```

## Comparing `focalnet-tf-0.0.2.1.tar` & `focalnet-tf-0.0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/
--rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4290 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet/
--rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2.1/focalnet/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2.1/focalnet/download_weights.py
--rw-rw-rw-   0        0        0     1740 2023-06-16 23:39:20.000000 focalnet-tf-0.0.2.1/focalnet/drop.py
--rw-rw-rw-   0        0        0    23191 2023-06-14 23:09:34.000000 focalnet-tf-0.0.2.1/focalnet/focalnet.py
--rw-rw-rw-   0        0        0     5289 2023-06-14 23:48:00.000000 focalnet-tf-0.0.2.1/focalnet/focalnet_utils.py
--rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-1k.json
--rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-21k.json
--rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-22k-reorder.json
-drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/
--rw-rw-rw-   0        0        0     4290 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-06-16 23:49:12.000000 focalnet-tf-0.0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/tests/
--rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2.1/tests/test_focalnet.py
--rw-rw-rw-   0        0        0    15498 2023-06-11 20:50:53.000000 focalnet-tf-0.0.2.1/tests/test_reproductible.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4290 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/focalnet/
+-rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2.2/focalnet/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2.2/focalnet/download_weights.py
+-rw-rw-rw-   0        0        0     2173 2023-06-25 00:23:28.000000 focalnet-tf-0.0.2.2/focalnet/drop.py
+-rw-rw-rw-   0        0        0    22980 2023-06-25 19:54:10.000000 focalnet-tf-0.0.2.2/focalnet/focalnet.py
+-rw-rw-rw-   0        0        0     5964 2023-06-18 21:54:05.000000 focalnet-tf-0.0.2.2/focalnet/focalnet_utils.py
+-rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-1k.json
+-rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-21k.json
+-rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-22k-reorder.json
+drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/
+-rw-rw-rw-   0        0        0     4290 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-06-18 18:44:10.000000 focalnet-tf-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/tests/
+-rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2.2/tests/test_focalnet.py
+-rw-rw-rw-   0        0        0    15552 2023-06-18 22:23:12.000000 focalnet-tf-0.0.2.2/tests/test_reproductible.py
```

### Comparing `focalnet-tf-0.0.2.1/LICENSE` & `focalnet-tf-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/PKG-INFO` & `focalnet-tf-0.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.2.1/README.md` & `focalnet-tf-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/focalnet/download_weights.py` & `focalnet-tf-0.0.2.2/focalnet/download_weights.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/focalnet/focalnet.py` & `focalnet-tf-0.0.2.2/focalnet/focalnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
                 kernel_size = 7; padding = 2; stride = 4
             else:
                 kernel_size = 3; padding = 1; stride = 2
             
             self.pad_proj = ZeroPadding2D(padding=padding)
             self.proj = Conv2D(filters=embed_dim, kernel_size=kernel_size, strides=stride, padding='valid', name="proj_conv" )
         else:
-            #print(embed_dim, patch_size)
             self.pad_proj = Identity()
             self.proj = Conv2D(filters=embed_dim, kernel_size=patch_size, strides=patch_size, name="proj_conv" )
         
         if norm_layer is not None:
             self.norm = norm_layer(epsilon=1e-5  )#norm_layer(embed_dim)
         else:
             self.norm = None
@@ -223,22 +222,22 @@
         self.input_resolution = input_resolution
         self.mlp_ratio = mlp_ratio
 
         self.focal_window = focal_window
         self.focal_level = focal_level
         self.use_postln = use_postln
 
-        self.norm1 = norm_layer(epsilon=1e-5, name="norm1")
+        self.norm1 = norm_layer(epsilon=1e-5)
         self.modulation = FocalModulation(
             dim, proj_drop=drop, focal_window=focal_window, focal_level=self.focal_level, 
             use_postln_in_modulation=use_postln_in_modulation, normalize_modulator=normalize_modulator
         )
 
         self.drop_path = DropPath(drop_path) if drop_path > 0. else Identity()
-        self.norm2 = norm_layer(epsilon=1e-5, name="norm2")
+        self.norm2 = norm_layer(epsilon=1e-5)
         mlp_hidden_dim = int(dim * mlp_ratio)
         self.mlp = Mlp(in_features=dim, hidden_features=mlp_hidden_dim, act_layer=act_layer, drop=drop)
 
         self.gamma_1 = 1.0
         self.gamma_2 = 1.0    
         if use_layerscale:
             self.gamma_1 =  tf.Variable(layerscale_value * tf.ones((dim)), trainable=True, name=name + "gamma_1" )
@@ -354,15 +353,14 @@
         modulators = []
         for blk in self.blocks:
             if return_modulator:
                 x, modulator = blk(x, H, W, return_modulator=return_modulator)
                 modulators.append(modulator)
             else:
                 x = blk(x, H, W, return_modulator=return_modulator)
-        #print(x.shape, H, W)
         if self.downsample is not None:
             x = tf.reshape(x, [-1,  H, W, x.shape[-1]])
             x, Ho, Wo = self.downsample(x)
         else:
             Ho, Wo = H, W
 
         if return_modulator:
@@ -402,15 +400,15 @@
                 patch_size=4, 
                 in_chans=3, 
                 num_classes=1000,
                 embed_dim=96, 
                 depths=[2, 2, 6, 2], 
                 mlp_ratio=4., 
                 drop_rate=0., 
-                drop_path_rate=0.1,
+                drop_path_rate=0.2,
                 norm_layer=LayerNormalization, 
                 patch_norm=True,
                 use_checkpoint=False,                 
                 focal_levels=[2, 2, 2, 2], 
                 focal_windows=[3, 3, 3, 3], 
                 use_conv_embed=False, 
                 use_layerscale=False, 
@@ -422,15 +420,14 @@
                 include_top=True,
                 name=None,
                 act_head=None,
                 **kwargs):
         super().__init__(name=name)
         if type(img_size) == int:
             img_size = (img_size, img_size)
-        
         assert type(img_size) == tuple
         self.num_layers = len(depths)
         embed_dim = [embed_dim * (2 ** i) for i in range(self.num_layers)]
 
         self.num_classes = num_classes
         self.embed_dim = embed_dim
         self.patch_norm = patch_norm
@@ -449,17 +446,15 @@
 
         num_patches = self.patch_embed.num_patches
         patches_resolution = self.patch_embed.patches_resolution
         self.patches_resolution = patches_resolution
         self.pos_drop = Dropout(drop_rate)
 
         # stochastic depth
-        #print(0, drop_path_rate, sum(depths))
         dpr = [x for x in tf.linspace(0., drop_path_rate, sum(depths)).numpy()]  # stochastic depth decay rule
- 
         # build layers
         self.layers_ = []
         for i_layer in range(self.num_layers):
             layer = BasicLayer(dim=embed_dim[i_layer], 
                                out_dim=embed_dim[i_layer+1] if (i_layer < self.num_layers - 1) else None,  
                                input_resolution=(patches_resolution[0] // (2 ** i_layer),
                                                  patches_resolution[1] // (2 ** i_layer)),
@@ -496,27 +491,25 @@
         x = self.pos_drop(x)
         for layer in self.layers_:
             if layer == self.layers_[-1] and return_modulator:
                 x, H, W, modulators = layer(x, H, W, return_modulator)
             else:
                 x, H, W = layer(x, H, W, return_modulator=False)
         x = self.norm(x)  # B L C
-        #print(H, W)
         if return_modulator:
             return x, modulators
         return x
 
     def call(self, x):
         if self.return_modulator:
             x, modulators = self.extract_features(x, return_modulator=self.return_modulator)
         else:
             x = self.extract_features(x, return_modulator=self.return_modulator)
         if self.avgpool is not None:
             x = self.avgpool(x) 
-        #print(x[0,:10])
         x = self.head(x)
         if self.return_modulator:
             return x, modulators
         return x
```

### Comparing `focalnet-tf-0.0.2.1/focalnet/focalnet_utils.py` & `focalnet-tf-0.0.2.2/focalnet/focalnet_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,14 +118,35 @@
         use_postln = True
         use_layerscale = True 
         use_postln_in_modulation= True 
         default_classes = 21842
     else: 
         raise("model name not found")
 
+
+    if "use_layerscale" in kwargs:
+        use_layerscale = kwargs["use_layerscale"]
+        del kwargs["use_layerscale"]
+
+    if "use_conv_embed" in kwargs: 
+        use_conv_embed = kwargs["use_conv_embed"]
+        del kwargs["use_conv_embed"]
+
+    if "use_postln" in kwargs:
+        use_postln = False 
+        del kwargs["use_postln"]
+
+    if "normalize_modulator" in kwargs:
+        normalize_modulator = kwargs["normalize_modulator"]
+        del kwargs["normalize_modulator"]
+
+    if "use_postln_in_modulation" in kwargs:
+        use_postln_in_modulation= kwargs["use_postln_in_modulation"]
+        del kwargs["use_postln_in_modulation"]
+        
     if num_classes is None and pretrained:
         num_classes = default_classes
     elif num_classes is None:
         num_classes = 0
 
     backbone = FocalNet(depths=depths, embed_dim=embed_dim, focal_windows=focal_windows, focal_levels=focal_levels, use_conv_embed=use_conv_embed, use_postln=use_postln,
                         use_layerscale=use_layerscale, normalize_modulator=normalize_modulator, use_postln_in_modulation=use_postln_in_modulation, num_classes=num_classes, **kwargs)
```

### Comparing `focalnet-tf-0.0.2.1/focalnet/imagenet-1k.json` & `focalnet-tf-0.0.2.2/focalnet/imagenet-1k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/focalnet/imagenet-21k.json` & `focalnet-tf-0.0.2.2/focalnet/imagenet-21k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/focalnet/imagenet-22k-reorder.json` & `focalnet-tf-0.0.2.2/focalnet/imagenet-22k-reorder.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/focalnet_tf.egg-info/PKG-INFO` & `focalnet-tf-0.0.2.2/focalnet_tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.2.1/setup.py` & `focalnet-tf-0.0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md', encoding="utf-8-sig") as f:
         README = f.read()
     return README
 
 
 setup(
     name='focalnet-tf',
-    version='0.0.2.1',    
+    version='0.0.2.2',    
     description='Re-implementation of FocalNet for tensorflow 2.X',
     author='Shiro-LK',
     author_email='shirosaki94@gmail.com',
     license='MIT License',
     packages=['focalnet'],
     package_data={'focalnet': ['imagenet-1k.json', 'imagenet-21k.json', 'imagenet-22k-reorder.json']},
     long_description=readme(),
```

### Comparing `focalnet-tf-0.0.2.1/tests/test_focalnet.py` & `focalnet-tf-0.0.2.2/tests/test_focalnet.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.1/tests/test_reproductible.py` & `focalnet-tf-0.0.2.2/tests/test_reproductible.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 import sys
+sys.path.append("G:/Projet-DL/Github/focalnet-tf")
+
 import os 
 import cv2 
 from focalnet.focalnet_utils import load_focalnet
 from focalnet_pt import load_focalnet as load_focalnetPT
 import pytest 
 import torch 
 from tensorflow.keras import backend as K
```

