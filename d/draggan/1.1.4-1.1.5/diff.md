# Comparing `tmp/draggan-1.1.4.tar.gz` & `tmp/draggan-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-ghxe6d99/draggan-1.1.4.tar", last modified: Sun Jun 25 12:37:28 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-cen8rpo_/draggan-1.1.5.tar", last modified: Sun Jun 25 13:02:37 2023, max compression
```

## Comparing `draggan-1.1.4.tar` & `draggan-1.1.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 12:37:28.000000 draggan-1.1.4/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5305 2023-06-25 09:47:53.000000 draggan-1.1.4/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-06-25 01:17:49.000000 draggan-1.1.4/draggan/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/deprecated/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-06-20 08:12:26.000000 draggan-1.1.4/draggan/deprecated/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7823 2023-06-20 08:13:46.000000 draggan-1.1.4/draggan/deprecated/api.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/deprecated/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.4/draggan/deprecated/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-06-20 08:12:26.000000 draggan-1.1.4/draggan/deprecated/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-06-20 08:12:26.000000 draggan-1.1.4/draggan/deprecated/utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11863 2023-06-25 09:37:14.000000 draggan-1.1.4/draggan/deprecated/web.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12037 2023-06-25 09:05:35.000000 draggan-1.1.4/draggan/draggan.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/stylegan2/dnnlib/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      478 2023-06-25 12:03:47.000000 draggan-1.1.4/draggan/stylegan2/dnnlib/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16627 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/dnnlib/util.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16504 2023-06-25 12:35:58.000000 draggan-1.1.4/draggan/stylegan2/legacy.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      438 2023-06-25 12:09:11.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5644 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/custom_ops.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10994 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/misc.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      438 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4376 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.cpp
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6147 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1280 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.h
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10047 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7677 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/conv2d_gradfix.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7591 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/conv2d_resample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2034 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/fma.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3299 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/grid_sample_gradfix.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4559 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.cpp
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    21050 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1836 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.h
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16287 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9710 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/persistence.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10707 2023-06-24 15:25:23.000000 draggan-1.1.4/draggan/stylegan2/torch_utils/training_stats.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan/stylegan2/training/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      448 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    26617 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/augment.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8642 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/dataset.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7999 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/loss.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    41518 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    27262 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/networks_stylegan3.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    21879 2023-06-25 12:28:55.000000 draggan-1.1.4/draggan/stylegan2/training/training_loop.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7300 2023-06-25 09:20:25.000000 draggan-1.1.4/draggan/utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11607 2023-06-25 12:34:40.000000 draggan-1.1.4/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2412 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-06-25 12:37:28.000000 draggan-1.1.4/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-06-25 12:37:28.000000 draggan-1.1.4/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1099 2023-06-25 12:37:19.000000 draggan-1.1.4/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 13:02:37.000000 draggan-1.1.5/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5305 2023-06-25 09:47:53.000000 draggan-1.1.5/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-06-25 01:17:49.000000 draggan-1.1.5/draggan/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/deprecated/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-06-20 08:12:26.000000 draggan-1.1.5/draggan/deprecated/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7823 2023-06-20 08:13:46.000000 draggan-1.1.5/draggan/deprecated/api.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/deprecated/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.5/draggan/deprecated/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-06-20 08:12:26.000000 draggan-1.1.5/draggan/deprecated/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-06-20 08:12:26.000000 draggan-1.1.5/draggan/deprecated/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11863 2023-06-25 09:37:14.000000 draggan-1.1.5/draggan/deprecated/web.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12037 2023-06-25 09:05:35.000000 draggan-1.1.5/draggan/draggan.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/stylegan2/dnnlib/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      478 2023-06-25 12:03:47.000000 draggan-1.1.5/draggan/stylegan2/dnnlib/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16627 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/dnnlib/util.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16504 2023-06-25 12:35:58.000000 draggan-1.1.5/draggan/stylegan2/legacy.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      438 2023-06-25 12:09:11.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5644 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/custom_ops.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10994 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/misc.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      438 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4376 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.cpp
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6147 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1280 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.h
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10047 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7677 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/conv2d_gradfix.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7591 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/conv2d_resample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2034 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/fma.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3299 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/grid_sample_gradfix.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4559 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.cpp
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    21050 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1836 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.h
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16287 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9710 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/persistence.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10707 2023-06-24 15:25:23.000000 draggan-1.1.5/draggan/stylegan2/torch_utils/training_stats.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan/stylegan2/training/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      448 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    26617 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/augment.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8642 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7999 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/loss.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    41518 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    27262 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/networks_stylegan3.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    21879 2023-06-25 12:28:55.000000 draggan-1.1.5/draggan/stylegan2/training/training_loop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7304 2023-06-25 13:02:10.000000 draggan-1.1.5/draggan/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11607 2023-06-25 12:34:40.000000 draggan-1.1.5/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2412 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-06-25 13:02:37.000000 draggan-1.1.5/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-06-25 13:02:37.000000 draggan-1.1.5/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1099 2023-06-25 13:02:28.000000 draggan-1.1.5/setup.py
```

### Comparing `draggan-1.1.4/README.md` & `draggan-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/api.py` & `draggan-1.1.5/draggan/deprecated/api.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/inversion.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/lpips/base_model.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/lpips/dist_model.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/lpips/networks_basic.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/lpips/pretrained_networks.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/lpips/util.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/model.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/conv2d_gradfix.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_act.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_bias_act.cpp` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d.cpp` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d.py` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.1.5/draggan/deprecated/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/utils.py` & `draggan-1.1.5/draggan/deprecated/utils.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/deprecated/web.py` & `draggan-1.1.5/draggan/deprecated/web.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/draggan.py` & `draggan-1.1.5/draggan/draggan.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/dnnlib/util.py` & `draggan-1.1.5/draggan/stylegan2/dnnlib/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/legacy.py` & `draggan-1.1.5/draggan/stylegan2/legacy.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/custom_ops.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/custom_ops.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/misc.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/misc.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.cpp` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.cu` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.h` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.h`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/bias_act.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/bias_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/conv2d_gradfix.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/conv2d_resample.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/conv2d_resample.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/fma.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/fma.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/grid_sample_gradfix.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/grid_sample_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.cpp` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.cu` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.h` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.h`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/ops/upfirdn2d.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/persistence.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/persistence.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/torch_utils/training_stats.py` & `draggan-1.1.5/draggan/stylegan2/torch_utils/training_stats.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/augment.py` & `draggan-1.1.5/draggan/stylegan2/training/augment.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/dataset.py` & `draggan-1.1.5/draggan/stylegan2/training/dataset.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/loss.py` & `draggan-1.1.5/draggan/stylegan2/training/loss.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/networks.py` & `draggan-1.1.5/draggan/stylegan2/training/networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/networks_stylegan3.py` & `draggan-1.1.5/draggan/stylegan2/training/networks_stylegan3.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/stylegan2/training/training_loop.py` & `draggan-1.1.5/draggan/stylegan2/training/training_loop.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan/utils.py` & `draggan-1.1.5/draggan/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                              miniters=1, desc=url.split('/')[-1]) as t:
         urllib.request.urlretrieve(url, filename=output_path, reporthook=t.update_to)
 
 
 def get_path(base_path):
     save_path = os.path.join(BASE_DIR, base_path)
     if not os.path.exists(save_path):
-        url = f"https://huggingface.co/aaronb/StyleGAN2/resolve/main/{base_path}"
+        url = f"https://huggingface.co/aaronb/StyleGAN2-pkl/resolve/main/{base_path}"
         print(f'{base_path} not found')
         print('Try to download from huggingface: ', url)
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         download_url(url, save_path)
         print('Downloaded to ', save_path)
     return save_path
```

### Comparing `draggan-1.1.4/draggan/web.py` & `draggan-1.1.5/draggan/web.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/draggan.egg-info/SOURCES.txt` & `draggan-1.1.5/draggan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggan-1.1.4/setup.py` & `draggan-1.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
     packages=find_packages(),
-    version='1.1.4',
+    version='1.1.5',
     package_data={
         'draggan': ['deprecated/stylegan2/op/fused_bias_act.cpp', 
                     'deprecated/stylegan2/op/upfirdn2d.cpp',
                     'deprecated/stylegan2/op/fused_bias_act_kernel.cu',
                     'deprecated/stylegan2/op/upfirdn2d_kernel.cu',
                     'stylegan2/torch_utils/ops/bias_act.cpp', 
                     'stylegan2/torch_utils/ops/upfirdn2d.cpp',
```

