# Comparing `tmp/draggan-1.1.0b2.tar.gz` & `tmp/draggan-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-icj4gqjm/draggan-1.1.0b2.tar", last modified: Mon May 29 12:57:49 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-ak8548rj/draggan-1.1.1.tar", last modified: Sun Jun 25 09:45:14 2023, max compression
```

## Comparing `draggan-1.1.0b2.tar` & `draggan-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-29 12:57:49.000000 draggan-1.1.0b2/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5960 2023-05-28 15:08:51.000000 draggan-1.1.0b2/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-05-28 12:23:03.000000 draggan-1.1.0b2/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7733 2023-05-29 12:57:30.000000 draggan-1.1.0b2/draggan/api.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-05-28 02:36:05.000000 draggan-1.1.0b2/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.0b2/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.0b2/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-05-28 14:55:40.000000 draggan-1.1.0b2/draggan/utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11723 2023-05-28 13:54:13.000000 draggan-1.1.0b2/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      862 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-29 12:57:49.000000 draggan-1.1.0b2/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      618 2023-05-29 12:57:40.000000 draggan-1.1.0b2/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 09:45:14.000000 draggan-1.1.1/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5122 2023-06-20 08:15:06.000000 draggan-1.1.1/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-06-25 01:17:49.000000 draggan-1.1.1/draggan/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan/deprecated/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan/deprecated/stylegan2/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan/deprecated/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.1/draggan/deprecated/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.1/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.1/draggan/deprecated/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.1/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12037 2023-06-25 09:05:35.000000 draggan-1.1.1/draggan/draggan.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-24 15:25:23.000000 draggan-1.1.1/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7300 2023-06-25 09:20:25.000000 draggan-1.1.1/draggan/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11481 2023-06-25 09:29:11.000000 draggan-1.1.1/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      479 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-06-25 09:45:14.000000 draggan-1.1.1/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-06-25 09:45:14.000000 draggan-1.1.1/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1110 2023-06-25 09:44:06.000000 draggan-1.1.1/setup.py
```

### Comparing `draggan-1.1.0b2/README.md` & `draggan-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # DragGAN
 [![PyPI](https://img.shields.io/pypi/v/draggan)](https://pypi.org/project/draggan/) 
+[![support](https://img.shields.io/badge/Support-macOS%20%7C%20Windows%20%7C%20Linux-blue)](#running-locally)
 
-:boom:  [`Colab Demo`](https://colab.research.google.com/github/Zeqiang-Lai/DragGAN/blob/master/colab.ipynb) | [`InternGPT Free Online Demo`](https://github.com/OpenGVLab/InternGPT) | [`Local Deployment`](#running-locally)
+:boom:  [`Colab Demo`](https://colab.research.google.com/github/Zeqiang-Lai/DragGAN/blob/master/colab.ipynb) | [`InternGPT Demo`](https://github.com/OpenGVLab/InternGPT) |  [`Local Deployment`](#running-locally) 
 
+🤗  [`Huggingface Demo1`](https://huggingface.co/spaces/fffiloni/DragGAN) | [`Huggingface Demo2`](https://huggingface.co/spaces/wuutiing2/DragGAN_pytorch) 
+<!-- 
+❌ [`OpenXLab Demo1`](https://app-center-159608-7842-ap7840x.1.openxlab.space) |
+[`OpenXLab Demo2`](https://app-center-159608-4865-v1j68a2.1.openxlab.space) |
+[`OpenXLab Demo3`](https://app-center-159608-2913-rzrk7pl.0.openxlab.space)
+ -->
 <!-- pip install draggan -i https://pypi.org/simple/ -->
 
-> **An out-of-box online demo is integrated in [InternGPT](https://github.com/OpenGVLab/InternGPT) - a super cool pointing-language-driven visual interactive system. Enjoy for free.:lollipop:**
-> 
-> Note for Colab, remember to select a GPU via `Runtime/Change runtime type` (`代码执行程序/更改运行时类型`).
+> **Note for Colab, remember to select a GPU via `Runtime/Change runtime type` (`代码执行程序/更改运行时类型`).**
 
-Implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
+Unofficial implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
 
 <p float="left">
   <img src="assets/mouse.gif" width="200" />
   <img src="assets/nose.gif" width="200" /> 
   <img src="assets/cat.gif" width="200" />
   <img src="assets/horse.gif" width="200" />
 </p>
@@ -29,92 +34,43 @@
 
 ![demo](assets/paper.png)
 
 ## News
 
 :star2: **What's New**
 
+- [2023/5/29] A new version is in beta, install via `pip install draggan==1.1.0b2`, includes speed improvement and more models.
 - [2023/5/25] DragGAN is on PyPI, simple install via `pip install draggan`. Also addressed the common CUDA problems https://github.com/Zeqiang-Lai/DragGAN/issues/38  https://github.com/Zeqiang-Lai/DragGAN/issues/12
 - [2023/5/25] We now support StyleGAN2-ada with much higher quality and more types of images. Try it by selecting models started with "ada".
+- [2023/5/24] An out-of-box online demo is integrated in [InternGPT](https://github.com/OpenGVLab/InternGPT) - a super cool pointing-language-driven visual interactive system. Enjoy for free.:lollipop:
 - [2023/5/24] Custom Image with GAN inversion is supported, but it is possible that your custom images are distorted  due to the limitation of GAN inversion. Besides, it is also possible the manipulations fail due to the limitation of our implementation.
 
 :star2: **Changelog**
 
-- [x] Tweak performance.
+- [x] Add a docker image, thanks [@egbaydarov](https://github.com/egbaydarov).
+- [ ] PTI GAN inversion https://github.com/Zeqiang-Lai/DragGAN/issues/71#issuecomment-1573461314
+- [x] Tweak performance, See [v2](https://github.com/Zeqiang-Lai/DragGAN/tree/v2).
 - [x] Improving installation experience, DragGAN is now on [PyPI](https://pypi.org/project/draggan).
-- [x] Automatically determining the number of iterations.
+- [x] Automatically determining the number of iterations, See [v2](https://github.com/Zeqiang-Lai/DragGAN/tree/v2).
 - [ ] Allow to save video without point annotations, custom image size.
 - [x] Support StyleGAN2-ada.
 - [x] Integrate into [InternGPT](https://github.com/OpenGVLab/InternGPT)
 - [x] Custom Image with GAN inversion.
 - [x] Download generated image and generation trajectory.
 - [x] Controlling generation process with GUI.
 - [x] Automatically download stylegan2 checkpoint.
 - [x] Support movable region, multiple handle points.
 - [x] Gradio and Colab Demo.
 
 > This project is now a sub-project of [InternGPT](https://github.com/OpenGVLab/InternGPT) for interactive image editing. Future updates of more cool tools beyond DragGAN would be added in [InternGPT](https://github.com/OpenGVLab/InternGPT). 
 
-
 ## Running Locally
 
-### With PyPI
-
-📑 [Step by Step Tutorial](https://zeqiang-lai.github.io/blog/en/posts/drag_gan/) | [中文部署教程](https://zeqiang-lai.github.io/blog/posts/ai/drag_gan/)
-
-We recommend to use Conda to install requirements.
-
-```bash
-conda create -n draggan python=3.7
-conda activate draggan
-```
-
-Install PyTorch following the [official instructions](https://pytorch.org/get-started/locally/)
-```bash
-conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia 
-```
-
-Install DragGAN
-```bash
-pip install draggan
-# If you meet ERROR: Could not find a version that satisfies the requirement draggan (from versions: none), use
-pip install draggan -i https://pypi.org/simple/
-```
-
-Launch the Gradio demo
-
-```bash
-python -m draggan.web
-# running on cpu
-python -m draggan.web --device cpu
-```
-
-### Clone and Install 
-
-Ensure you have a GPU and CUDA installed. We use Python 3.7 for testing, other versions (>= 3.7) of Python should work too, but not tested. We recommend to use [Conda](https://conda.io/projects/conda/en/stable/user-guide/install/download.html) to prepare all the requirements.
-
-For Windows users, you might encounter some issues caused by StyleGAN custom ops, youd could find some solutions from the [issues pannel](https://github.com/Zeqiang-Lai/DragGAN/issues). We are also working on a more friendly package without setup.
-
-```bash
-git clone https://github.com/Zeqiang-Lai/DragGAN.git
-cd DragGAN
-conda create -n draggan python=3.7
-conda activate draggan
-pip install -r requirements.txt
-```
-
-Launch the Gradio demo
-
-```bash
-python gradio_app.py
-# running on cpu
-python gradio_app.py --device cpu
-```
+Please refer to [INSTALL.md](INSTALL.md).
 
-> If you have any issue for downloading the checkpoint, you could manually download it from [here](https://huggingface.co/aaronb/StyleGAN2/tree/main) and put it into the folder `checkpoints`.
 
 ## Citation
 
 ```bibtex
 @inproceedings{pan2023draggan,
     title={Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold}, 
     author={Pan, Xingang and Tewari, Ayush, and Leimk{\"u}hler, Thomas and Liu, Lingjie and Meka, Abhimitra and Theobalt, Christian},
@@ -124,14 +80,14 @@
 ```
 
 
 ## Acknowledgement
 
 [Official DragGAN](https://github.com/XingangPan/DragGAN) &ensp; [DragGAN-Streamlit](https://github.com/skimai/DragGAN) &ensp; [StyleGAN2](https://github.com/NVlabs/stylegan2)  &ensp; [StyleGAN2-pytorch](https://github.com/rosinality/stylegan2-pytorch)  &ensp; [StyleGAN2-Ada](https://github.com/NVlabs/stylegan2-ada-pytorch)   &ensp;  [StyleGAN-Human](https://github.com/stylegan-human/StyleGAN-Human) &ensp;  [Self-Distilled-StyleGAN](https://github.com/self-distilled-stylegan/self-distilled-internet-photos)
 
-Welcome to discuss with us and continuously improve the user experience of DragGAN.
-Reach us with this WeChat QR Code.
+<!-- Welcome to discuss with us and continuously improve the user experience of DragGAN.
+Reach us with this WeChat QR Code. -->
 
-<p align="left"><img width="300" alt="image" src="https://github.com/Zeqiang-Lai/DragGAN/assets/26198430/cd6b1602-dc19-442f-9ced-a441d4c81aec"></p> 
+<p align="left"><img width="300" alt="image" src="https://github.com/Zeqiang-Lai/DragGAN/assets/26198430/385304d2-d15f-4019-9199-f603d04568fa"></p>
```

### Comparing `draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.1.1/draggan/deprecated/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.1.1/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.1.1/draggan/deprecated/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.1.1/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b2/draggan/utils.py` & `draggan-1.1.1/draggan/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import PIL.ImageDraw
 import torch
 import torch.optim
 from tqdm import tqdm
 
 BASE_DIR = os.environ.get(
     'DRAGGAN_HOME',
-    os.path.join(os.path.expanduser('~'), 'draggan', 'checkpoints')
+    os.path.join(os.path.expanduser('~'), 'draggan', 'checkpoints-pkl')
 )
 
 
 class DownloadProgressBar(tqdm):
     def update_to(self, b=1, bsize=1, tsize=None):
         if tsize is not None:
             self.total = tsize
```

### Comparing `draggan-1.1.0b2/draggan/web.py` & `draggan-1.1.1/draggan/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,50 @@
 import gradio as gr
 import torch
 import numpy as np
 import imageio
 from PIL import Image
 import uuid
 
-from .api import drag_gan, stylegan2
-from .stylegan2.inversion import inverse_image
 from . import utils
+from .draggan import drag_gan
+from . import draggan as draggan
 
 device = 'cuda'
 
 
 SIZE_TO_CLICK_SIZE = {
     1024: 8,
     512: 5,
     256: 2
 }
 
 CKPT_SIZE = {
-    'stylegan2-ffhq-config-f.pt': 1024,
-    'stylegan2-cat-config-f.pt': 256,
-    'stylegan2-church-config-f.pt': 256,
-    'stylegan2-horse-config-f.pt': 256,
-    'ada/ffhq.pt': 1024,
-    'ada/afhqcat.pt': 512,
-    'ada/afhqdog.pt': 512,
-    'ada/afhqwild.pt': 512,
-    'ada/brecahad.pt': 512,
-    'ada/metfaces.pt': 512,
-    'human/v2_512.pt': 512,
-    'human/v2_1024.pt': 1024,
-    'self_distill/bicycles_256.pt': 256,
-    'self_distill/dogs_1024.pt': 1024,
-    'self_distill/elephants_512.pt': 512,
-    'self_distill/giraffes_512.pt': 512,
-    'self_distill/horses_256.pt': 256,
-    'self_distill/lions_512.pt': 512,
-    'self_distill/parrots_512.pt': 512,
+    'stylegan2-ffhq-config-f.pkl': 1024,
+    'stylegan2-cat-config-f.pkl': 256,
+    'stylegan2-church-config-f.pkl': 256,
+    'stylegan2-horse-config-f.pkl': 256,
+    'ada/ffhq.pkl': 1024,
+    'ada/afhqcat.pkl': 512,
+    'ada/afhqdog.pkl': 512,
+    'ada/afhqwild.pkl': 512,
+    'ada/brecahad.pkl': 512,
+    'ada/metfaces.pkl': 512,
+    'human/v2_512.pkl': 512,
+    'human/v2_1024.pkl': 1024,
+    'self_distill/bicycles_256.pkl': 256,
+    'self_distill/dogs_1024.pkl': 1024,
+    'self_distill/elephants_512.pkl': 512,
+    'self_distill/giraffes_512.pkl': 512,
+    'self_distill/horses_256.pkl': 256,
+    'self_distill/lions_512.pkl': 512,
+    'self_distill/parrots_512.pkl': 512,
 }
 
-DEFAULT_CKPT = 'self_distill/lions_512.pt'
-
-
-class ModelWrapper:
-    def __init__(self, **kwargs):
-        self.g_ema = stylegan2(**kwargs).to(device)
+DEFAULT_CKPT = 'ada/afhqcat.pkl'
 
 
 def to_image(tensor):
     tensor = tensor.squeeze(0).permute(1, 2, 0)
     arr = tensor.detach().cpu().numpy()
     arr = (arr - arr.min()) / (arr.max() - arr.min())
     arr = arr * 255
@@ -68,104 +63,106 @@
         image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
         return image, not target_point
     points['handle'].append([evt.index[1], evt.index[0]])
     image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
     return image, not target_point
 
 
-def on_drag(model, points, max_iters, state, size, mask):
+def on_drag(model, points, max_iters, state, size, mask, lr_box):
     if len(points['handle']) == 0:
         raise gr.Error('You must select at least one handle point and target point.')
     if len(points['handle']) != len(points['target']):
         raise gr.Error('You have uncompleted handle points, try to selct a target point or undo the handle point.')
     max_iters = int(max_iters)
-    latent = state['latent']
-    noise = state['noise']
-    F = state['F']
+    W = state['W']
 
     handle_points = [torch.tensor(p, device=device).float() for p in points['handle']]
     target_points = [torch.tensor(p, device=device).float() for p in points['target']]
 
     if mask.get('mask') is not None:
         mask = Image.fromarray(mask['mask']).convert('L')
         mask = np.array(mask) == 255
 
         mask = torch.from_numpy(mask).float().to(device)
         mask = mask.unsqueeze(0).unsqueeze(0)
     else:
         mask = None
 
     step = 0
-    for sample2, latent, F, handle_points in drag_gan(model.g_ema, latent, noise, F,
-                                                      handle_points, target_points, mask,
-                                                      max_iters=max_iters):
-        image = to_image(sample2)
-
-        state['F'] = F
-        state['latent'] = latent
-        state['sample'] = sample2
+    for image, W, handle_points in drag_gan(W, model['G'],
+                                            handle_points, target_points, mask,
+                                            max_iters=max_iters, lr=lr_box):
         points['handle'] = [p.cpu().numpy().astype('int') for p in handle_points]
         image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
 
         state['history'].append(image)
         step += 1
         yield image, state, step
 
 
 def on_reset(points, image, state):
-    return {'target': [], 'handle': []}, to_image(state['sample']), False
+    return {'target': [], 'handle': []}, state['img'], False
 
 
 def on_undo(points, image, state, size):
-    image = to_image(state['sample'])
+    image = state['img']
 
     if len(points['target']) < len(points['handle']):
         points['handle'] = points['handle'][:-1]
     else:
         points['handle'] = points['handle'][:-1]
         points['target'] = points['target'][:-1]
 
     image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
     return points, image, False
 
 
 def on_change_model(selected, model):
     size = CKPT_SIZE[selected]
-    model = ModelWrapper(size=size, ckpt=selected)
-    g_ema = model.g_ema
-    sample_z = torch.randn([1, 512], device=device)
-    latent, noise = g_ema.prepare([sample_z])
-    sample, F = g_ema.generate(latent, noise)
+
+    G = draggan.load_model(utils.get_path(selected), device=device)
+    model = {'G': G}
+    W = draggan.generate_W(
+        G,
+        seed=int(1),
+        device=device,
+        truncation_psi=0.8,
+        truncation_cutoff=8,
+    )
+    img, _ = draggan.generate_image(W, G, device=device)
 
     state = {
-        'latent': latent,
-        'noise': noise,
-        'F': F,
-        'sample': sample,
+        'W': W,
+        'img': img,
         'history': []
     }
-    return model, state, to_image(sample), to_image(sample), size
+
+    return model, state, img, img, size
 
 
-def on_new_image(model):
-    g_ema = model.g_ema
-    sample_z = torch.randn([1, 512], device=device)
-    latent, noise = g_ema.prepare([sample_z])
-    sample, F = g_ema.generate(latent, noise)
+def on_new_image(model, seed):
+    G = model['G']
+    W = draggan.generate_W(
+        G,
+        seed=int(seed),
+        device=device,
+        truncation_psi=0.8,
+        truncation_cutoff=8,
+    )
+    img, _ = draggan.generate_image(W, G, device=device)
 
     state = {
-        'latent': latent,
-        'noise': noise,
-        'F': F,
-        'sample': sample,
+        'W': W,
+        'img': img,
         'history': []
     }
+
     points = {'target': [], 'handle': []}
     target_point = False
-    return to_image(sample), to_image(sample), state, points, target_point
+    return img, img, state, points, target_point
 
 
 def on_max_iter_change(max_iters):
     return gr.update(maximum=max_iters)
 
 
 def on_save_files(image, state):
@@ -204,31 +201,25 @@
     return img
 
 
 def main():
     torch.cuda.manual_seed(25)
 
     with gr.Blocks() as demo:
-        wrapped_model = ModelWrapper(ckpt=DEFAULT_CKPT, size=CKPT_SIZE[DEFAULT_CKPT])
-        model = gr.State(wrapped_model)
-        sample_z = torch.randn([1, 512], device=device)
-        latent, noise = wrapped_model.g_ema.prepare([sample_z])
-        sample, F = wrapped_model.g_ema.generate(latent, noise)
-
         gr.Markdown(
             """
             # DragGAN
             
             Unofficial implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
             
             [Our Implementation](https://github.com/Zeqiang-Lai/DragGAN) | [Official Implementation](https://github.com/XingangPan/DragGAN) (Not released yet)
 
             ## Tutorial
             
-            1. (Optional) Draw a mask indicate the movable region.
+            1. (Opklional) Draw a mask indicate the movable region.
             2. Setup a least one pair of handle point and target point.
             3. Click "Drag it". 
             
             ## Hints
             
             - Handle points (Blue): the point you want to drag.
             - Target points (Red): the destination you want to drag towards to.
@@ -237,38 +228,50 @@
             
             - We now support dragging user uploaded image by GAN inversion.
             - **Please upload your image at `Setup Handle Points` pannel.** Upload it from `Draw a Mask` would cause errors for now.
             - Due to the limitation of GAN inversion, 
                 - You might wait roughly 1 minute to see the GAN version of the uploaded image.
                 - The shown image might be slightly difference from the uploaded one.
                 - It could also fail to invert the uploaded image and generate very poor results.
-                - Idealy, you should choose the closest model of the uploaded image. For example, choose `stylegan2-ffhq-config-f.pt` for human face. `stylegan2-cat-config-f.pt` for cat.
+                - Idealy, you should choose the closest model of the uploaded image. For example, choose `stylegan2-ffhq-config-f.pkl` for human face. `stylegan2-cat-config-f.pkl` for cat.
                 
             > Please fire an issue if you have encounted any problem. Also don't forgot to give a star to the [Official Repo](https://github.com/XingangPan/DragGAN), [our project](https://github.com/Zeqiang-Lai/DragGAN) could not exist without it.
             """,
         )
+        G = draggan.load_model(utils.get_path(DEFAULT_CKPT), device=device)
+        model = gr.State({'G': G})
+        W = draggan.generate_W(
+            G,
+            seed=int(1),
+            device=device,
+            truncation_psi=0.8,
+            truncation_cutoff=8,
+        )
+        img, F0 = draggan.generate_image(W, G, device=device)
+
         state = gr.State({
-            'latent': latent,
-            'noise': noise,
-            'F': F,
-            'sample': sample,
+            'W': W,
+            'img': img,
             'history': []
         })
         points = gr.State({'target': [], 'handle': []})
         size = gr.State(CKPT_SIZE[DEFAULT_CKPT])
         target_point = gr.State(False)
 
         with gr.Row():
             with gr.Column(scale=0.3):
                 with gr.Accordion("Model"):
                     model_dropdown = gr.Dropdown(choices=list(CKPT_SIZE.keys()), value=DEFAULT_CKPT,
                                                  label='StyleGAN2 model')
-                    max_iters = gr.Slider(1, 500, 20, step=1, label='Max Iterations')
+                    seed = gr.Number(value=1, label='Seed', precision=0)
                     new_btn = gr.Button('New Image')
                 with gr.Accordion('Drag'):
+                    with gr.Row():
+                        lr_box = gr.Number(value=2e-3, label='Learning Rate')
+                        max_iters = gr.Slider(1, 500, 20, step=1, label='Max Iterations')
 
                     with gr.Row():
                         with gr.Column(min_width=100):
                             reset_btn = gr.Button('Reset All')
                         with gr.Column(min_width=100):
                             undo_btn = gr.Button('Undo Last')
                     with gr.Row():
@@ -277,31 +280,30 @@
                 with gr.Accordion('Save', visible=False) as save_panel:
                     files = gr.Files(value=[])
 
                 progress = gr.Slider(value=0, maximum=20, label='Progress', interactive=False)
 
             with gr.Column():
                 with gr.Tabs():
-                    img = to_image(sample)
                     with gr.Tab('Setup Handle Points', id='input'):
                         image = gr.Image(img).style(height=512, width=512)
                     with gr.Tab('Draw a Mask', id='mask') as masktab:
                         mask = gr.ImageMask(img, label='Mask').style(height=512, width=512)
 
         image.select(on_click, [image, target_point, points, size], [image, target_point])
         image.upload(on_image_change, [model, size, image], [image, mask, state, points, target_point])
         mask.upload(on_mask_change, [mask], [image])
-        btn.click(on_drag, inputs=[model, points, max_iters, state, size, mask], outputs=[image, state, progress]).then(
+        btn.click(on_drag, inputs=[model, points, max_iters, state, size, mask, lr_box], outputs=[image, state, progress]).then(
             on_show_save, outputs=save_panel).then(
             on_save_files, inputs=[image, state], outputs=[files]
         )
         reset_btn.click(on_reset, inputs=[points, image, state], outputs=[points, image, target_point])
         undo_btn.click(on_undo, inputs=[points, image, state, size], outputs=[points, image, target_point])
         model_dropdown.change(on_change_model, inputs=[model_dropdown, model], outputs=[model, state, image, mask, size])
-        new_btn.click(on_new_image, inputs=[model], outputs=[image, mask, state, points, target_point])
+        new_btn.click(on_new_image, inputs=[model, seed], outputs=[image, mask, state, points, target_point])
         max_iters.change(on_max_iter_change, inputs=max_iters, outputs=progress)
         masktab.select(lambda: gr.update(value=None), outputs=[mask]).then(on_select_mask_tab, inputs=[state], outputs=[mask])
     return demo
 
 
 if __name__ == '__main__':
     import argparse
```

