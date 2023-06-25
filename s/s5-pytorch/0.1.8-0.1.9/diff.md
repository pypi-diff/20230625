# Comparing `tmp/s5-pytorch-0.1.8.tar.gz` & `tmp/s5-pytorch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5-pytorch-0.1.8.tar", last modified: Sat May 27 11:43:28 2023, max compression
+gzip compressed data, was "s5-pytorch-0.1.9.tar", last modified: Sun Jun 25 10:32:41 2023, max compression
```

## Comparing `s5-pytorch-0.1.8.tar` & `s5-pytorch-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/
--rw-r--r--   0 null      (1000) null      (1000)    16727 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/LICENSE
--rw-r--r--   0 null      (1000) null      (1000)     2122 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)     1444 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/README.md
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.785534 s5-pytorch-0.1.8/s5/
--rw-r--r--   0 null      (1000) null      (1000)       24 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/__init__.py
--rw-r--r--   0 null      (1000) null      (1000)     8786 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/init.py
--rw-r--r--   0 null      (1000) null      (1000)    15899 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/jax_compat.py
--rw-r--r--   0 null      (1000) null      (1000)    17510 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/s5_model.py
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/s5_pytorch.egg-info/
--rw-r--r--   0 null      (1000) null      (1000)     2122 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)      253 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 null      (1000) null      (1000)        1 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 null      (1000) null      (1000)       34 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/requires.txt
--rw-r--r--   0 null      (1000) null      (1000)        3 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/top_level.txt
--rw-r--r--   0 null      (1000) null      (1000)       38 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/setup.cfg
--rw-r--r--   0 null      (1000) null      (1000)     1023 2023-05-27 11:41:40.000000 s5-pytorch-0.1.8/setup.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/
+-rw-r--r--   0 null      (1000) null      (1000)    16727 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/LICENSE
+-rw-r--r--   0 null      (1000) null      (1000)     2122 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)     1444 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/README.md
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.276875 s5-pytorch-0.1.9/s5/
+-rw-r--r--   0 null      (1000) null      (1000)       24 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/s5/__init__.py
+-rw-r--r--   0 null      (1000) null      (1000)     8786 2023-05-27 11:40:20.000000 s5-pytorch-0.1.9/s5/init.py
+-rw-r--r--   0 null      (1000) null      (1000)    15899 2023-06-25 09:50:15.000000 s5-pytorch-0.1.9/s5/jax_compat.py
+-rw-r--r--   0 null      (1000) null      (1000)    17474 2023-06-25 10:29:18.000000 s5-pytorch-0.1.9/s5/s5_model.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/s5_pytorch.egg-info/
+-rw-r--r--   0 null      (1000) null      (1000)     2122 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)      253 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 null      (1000) null      (1000)        1 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 null      (1000) null      (1000)       34 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/requires.txt
+-rw-r--r--   0 null      (1000) null      (1000)        3 2023-06-25 10:32:41.000000 s5-pytorch-0.1.9/s5_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 null      (1000) null      (1000)       38 2023-06-25 10:32:41.277875 s5-pytorch-0.1.9/setup.cfg
+-rw-r--r--   0 null      (1000) null      (1000)     1023 2023-06-25 10:32:18.000000 s5-pytorch-0.1.9/setup.py
```

### Comparing `s5-pytorch-0.1.8/LICENSE` & `s5-pytorch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.8/PKG-INFO` & `s5-pytorch-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: S5 - Simplified State Space Layers for Sequence Modeling - Pytorch
 Home-page: https://github.com/i404788/s5-pytorch
 Author: Ferris Kwaijtaal
 Author-email: ferris+gh@devdroplets.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s5-pytorch-0.1.8/README.md` & `s5-pytorch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.8/s5/init.py` & `s5-pytorch-0.1.9/s5/init.py`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.8/s5/jax_compat.py` & `s5-pytorch-0.1.9/s5/jax_compat.py`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.8/s5/s5_model.py` & `s5-pytorch-0.1.9/s5/s5_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         xs = torch.cat((xs, xs2), axis=-1)
 
     Du = functorch.vmap(lambda u: D * u)(input_sequence)
     return functorch.vmap(lambda x: (C_tilde @ x).real)(xs) + Du
 
 
 # Discretization functions
-@torch.jit.script
 def discretize_bilinear(Lambda, B_tilde, Delta):
     """Discretize a diagonalized, continuous-time linear SSM
     using bilinear transform method.
     Args:
         Lambda (complex64): diagonal state matrix              (P,)
         B_tilde (complex64): input matrix                      (P, H)
         Delta (float32): discretization step sizes             (P,)
@@ -85,15 +84,14 @@
     """
     Identity = torch.ones(Lambda.shape[0], device=Lambda.device)
     BL = 1 / (Identity - (Delta / 2.0) * Lambda)
     Lambda_bar = BL * (Identity + (Delta / 2.0) * Lambda)
     B_bar = (BL * Delta)[..., None] * B_tilde
     return Lambda_bar, B_bar
 
-@torch.jit.script
 def discretize_zoh(Lambda, B_tilde, Delta):
     """Discretize a diagonalized, continuous-time linear SSM
     using zero-order hold method.
     Args:
         Lambda (complex64): diagonal state matrix              (P,)
         B_tilde (complex64): input matrix                      (P, H)
         Delta (float32): discretization step sizes             (P,)
```

### Comparing `s5-pytorch-0.1.8/s5_pytorch.egg-info/PKG-INFO` & `s5-pytorch-0.1.9/s5_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: S5 - Simplified State Space Layers for Sequence Modeling - Pytorch
 Home-page: https://github.com/i404788/s5-pytorch
 Author: Ferris Kwaijtaal
 Author-email: ferris+gh@devdroplets.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s5-pytorch-0.1.8/setup.py` & `s5-pytorch-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='s5-pytorch',
     packages=find_packages(exclude=[]),
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     description='S5 - Simplified State Space Layers for Sequence Modeling - Pytorch',
     author='Ferris Kwaijtaal',
     author_email='ferris+gh@devdroplets.com',
     long_description_content_type='text/markdown',
     long_description=open('README.md', 'r').read(),
     url='https://github.com/i404788/s5-pytorch',
```

