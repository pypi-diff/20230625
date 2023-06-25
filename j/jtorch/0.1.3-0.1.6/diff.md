# Comparing `tmp/jtorch-0.1.3.tar.gz` & `tmp/jtorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtorch-0.1.3.tar", last modified: Mon Apr  3 04:57:42 2023, max compression
+gzip compressed data, was "jtorch-0.1.6.tar", last modified: Sun Jun 25 15:05:25 2023, max compression
```

## Comparing `jtorch-0.1.3.tar` & `jtorch-0.1.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.649348 jtorch-0.1.3/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11621 2023-03-19 10:14:44.000000 jtorch-0.1.3/LICENSE.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       88 2023-03-19 10:14:44.000000 jtorch-0.1.3/MANIFEST.in
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-04-03 04:57:42.649348 jtorch-0.1.3/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4182 2023-03-19 10:14:44.000000 jtorch-0.1.3/README.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.606015 jtorch-0.1.3/python/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.606015 jtorch-0.1.3/python/jtorch/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6915 2023-03-31 13:34:57.000000 jtorch-0.1.3/python/jtorch/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4045 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/autograd.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/compiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      620 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/cuda.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      550 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/distributed.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      253 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/misc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.616848 jtorch-0.1.3/python/jtorch/nn/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1454 2023-03-31 08:48:40.000000 jtorch-0.1.3/python/jtorch/nn/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      209 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/nn/init.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.616848 jtorch-0.1.3/python/jtorch/nn/utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)        0 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/nn/utils/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       21 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/nn/utils/rnn.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      946 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/optim.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.616848 jtorch-0.1.3/python/jtorch/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2426 2023-04-03 01:50:53.000000 jtorch-0.1.3/python/jtorch/src/jtorch_core.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      890 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/src/jtorch_core.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.616848 jtorch-0.1.3/python/jtorch/test/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      547 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/test/test_conflict_func.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/test/test_function.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      676 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/test/test_misc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/test/test_tutorial.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.627681 jtorch-0.1.3/python/jtorch/tutorial/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1324 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad1.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2381 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad2.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3122 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad3.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2862 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad4.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad5_optim.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1963 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad6_module.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2507 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/auto_grad7_dynet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3040 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/tutorial/quickstart.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.638515 jtorch-0.1.3/python/jtorch/utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)       84 2023-04-01 23:25:04.000000 jtorch-0.1.3/python/jtorch/utils/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       22 2023-03-29 22:23:26.000000 jtorch-0.1.3/python/jtorch/utils/checkpoint.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2386 2023-04-01 23:25:04.000000 jtorch-0.1.3/python/jtorch/utils/data.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      330 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/utils/dtype.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      772 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/utils/pip_publish.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.638515 jtorch-0.1.3/python/jtorch/vision/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1475 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/_internally_replaced_utils.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.649348 jtorch-0.1.3/python/jtorch/vision/datasets/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      160 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/datasets/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    21973 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/datasets/mnist.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    19124 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/datasets/utils.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/datasets/vision.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       30 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/transforms.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    23314 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/jtorch/vision/utils.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.606015 jtorch-0.1.3/python/jtorch.egg-info/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-04-03 04:57:42.000000 jtorch-0.1.3/python/jtorch.egg-info/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1528 2023-04-03 04:57:42.000000 jtorch-0.1.3/python/jtorch.egg-info/SOURCES.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-04-03 04:57:42.000000 jtorch-0.1.3/python/jtorch.egg-info/dependency_links.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       25 2023-04-03 04:57:42.000000 jtorch-0.1.3/python/jtorch.egg-info/requires.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       13 2023-04-03 04:57:42.000000 jtorch-0.1.3/python/jtorch.egg-info/top_level.txt
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-03 04:57:42.649348 jtorch-0.1.3/python/torch/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1858 2023-04-01 23:25:04.000000 jtorch-0.1.3/python/torch/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       29 2023-03-19 10:14:44.000000 jtorch-0.1.3/python/torch/autograd.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-04-03 04:57:42.649348 jtorch-0.1.3/setup.cfg
--rw-r--r--   0 cjld      (1000) cjld      (1000)      885 2023-04-03 04:57:15.000000 jtorch-0.1.3/setup.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11621 2023-03-19 10:14:44.000000 jtorch-0.1.6/LICENSE.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       88 2023-03-19 10:14:44.000000 jtorch-0.1.6/MANIFEST.in
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-25 15:05:25.681466 jtorch-0.1.6/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4182 2023-03-19 10:14:44.000000 jtorch-0.1.6/README.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7823 2023-06-18 12:36:10.000000 jtorch-0.1.6/python/jtorch/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4045 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/autograd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      667 2023-06-06 14:38:33.000000 jtorch-0.1.6/python/jtorch/cuda.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      550 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/distributed.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      253 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/misc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/nn/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1472 2023-05-12 10:49:11.000000 jtorch-0.1.6/python/jtorch/nn/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      209 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/init.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/nn/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        0 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/utils/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       21 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/utils/rnn.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      979 2023-06-04 13:28:13.000000 jtorch-0.1.6/python/jtorch/optim.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2426 2023-04-03 01:50:53.000000 jtorch-0.1.6/python/jtorch/src/jtorch_core.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      899 2023-05-13 04:25:41.000000 jtorch-0.1.6/python/jtorch/src/jtorch_core.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      547 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_conflict_func.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_function.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      676 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_misc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_tutorial.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/tutorial/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1324 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad1.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2381 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3122 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad3.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2862 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad4.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad5_optim.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1963 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad6_module.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2507 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad7_dynet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3040 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/quickstart.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       84 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/jtorch/utils/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       22 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/utils/checkpoint.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2386 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/jtorch/utils/data.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      330 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/utils/dtype.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      772 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/utils/pip_publish.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/vision/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1475 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/_internally_replaced_utils.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/vision/datasets/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      160 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21973 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/mnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    19124 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/utils.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/vision.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       30 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/transforms.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23314 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/utils.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch.egg-info/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1528 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       25 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/requires.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       13 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/top_level.txt
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/torch/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1858 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/torch/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       29 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/torch/autograd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-25 15:05:25.681466 jtorch-0.1.6/setup.cfg
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      885 2023-06-25 15:00:37.000000 jtorch-0.1.6/setup.py
```

### Comparing `jtorch-0.1.3/LICENSE.txt` & `jtorch-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/PKG-INFO` & `jtorch-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtorch
-Version: 0.1.3
+Version: 0.1.6
 Summary: jtorch project
 Home-page: https://github.com/JITTorch/jtorch
 Author: jtorch
 Author-email: jtorch@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JITTorch/jtorch/issues
 Platform: UNKNOWN
```

### Comparing `jtorch-0.1.3/README.md` & `jtorch-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/__init__.py` & `jtorch-0.1.6/python/jtorch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,41 +8,57 @@
 org_bool = bool = type(True)
 
 import jtorch.compiler
 
 import jtorch_core
 from jtorch_core import *
 
+def handle_dtype(args, kw, dtype):
+    def convert(x):
+        if isinstance(x, jt.Var):
+            return x.cast(dtype)
+        return x
+    if dtype is not None:
+        if args is not None:
+            if isinstance(args, (tuple,list)):
+                args = [ convert(a) for a in args ]
+            else:
+                args = convert(x)
+        if kw is not None:
+            kw = { k:convert(v) for k,v in kw.items() }
+    return args, kw
 
 def wrapper(func):
     has_dtype = False
     if hasattr(func, "__code__"):
-        has_dtype = "dtype" in func.__code__.co_varnames
+        has_dtype = "dtype" in func.__code__.co_varnames[:func.__code__.co_argcount]
     def inner(*args, **kw):
         requires_grad = None
         dtype = None
         if "requires_grad" in kw:
             requires_grad = kw["requires_grad"]
             del kw["requires_grad"]
         if not has_dtype and "dtype" in kw:
             dtype = kw["dtype"]
             del kw["dtype"]
         if "device" in kw:
             del kw["device"]
+        args, kw = handle_dtype(args, kw, dtype)
         ret = func(*args, **kw)
         if requires_grad is not None:
             ret.requires_grad = requires_grad
         if dtype is not None:
             ret.astype(dtype)
         return ret
     return inner
         
 
 import inspect
 _wrapper_keys = set(["shape", "start", "size"])
+_wrapper_keys.add("x")
 for k,v in list(globals().items()):
     if callable(v) and not isinstance(v, type):
         try:
             spec = inspect.getfullargspec(v)
             args_name = spec[0]
             if len(args_name) and args_name[0] in _wrapper_keys:
                 globals()[k] = wrapper(v)
@@ -62,15 +78,14 @@
 Tensor.grad = property(grad_get, grad_set, grad_del)
 Tensor.retains_grad = property(retain_grad_get, retain_grad_set)
 def retain_grad(x:Tensor, value:bool=True):
     x.retains_grad = value
     return value
 Tensor.retain_grad = retain_grad
 
-Tensor.to = lambda self, device: self
 Tensor.dim = lambda self: self.ndim
 Tensor.ndimension = lambda self: self.ndim
 Tensor.nelement = lambda self: self.numel()
 Tensor.cuda = lambda self: self
 def device_get(x:Tensor):
     return device("cpu") if not jt.has_cuda or not jt.flags.use_cuda else device("cuda")
 Tensor.device = property(device_get)
@@ -110,25 +125,28 @@
 def make_module(cls):
     class TMod(ModuleMisc, cls):
         def __init__(self, *args, **kw):
             dtype = None
             if "dtype" in kw:
                 dtype = kw["dtype"]
                 del kw["dtype"]
+            self._dtype = dtype
             with jt.flag_scope(th_mode=0):
                 super().__init__(*args, **kw)
             for k,v in self.__dict__.items():
                 if not k.startswith("_") and isinstance(v, Var) \
                     and v.requires_grad:
                     v.retain_grad()
                 if dtype is not None and isinstance(v, Var):
                     v.assign(v.cast(dtype))
         def __call__(self, *args, **kw):
+            args, kw = handle_dtype(args, kw, self._dtype)
             return self.execute(*args, **kw)
         def forward(self, *args, **kw):
+            args, kw = handle_dtype(args, kw, self._dtype)
             return self.execute(*args, **kw)
         
         @property
         def training(self):
             if not hasattr(self, "is_train"):
                 self.is_train = True
             return self.is_train
@@ -171,14 +189,16 @@
     if len(args) >= 2 and isinstance(args[1], org_int):
         dim = args[1]
     elif "dim" in kw and isinstance(kw["dim"], org_int):
         dim = kw["dim"]
     if dim is not None:
         k, v = jt.argmin(*args, **kw)
         return v, k
+    elif len(args) == 2 and isinstance(args[1], jt.Var):
+        return jt.minimum(args[0], args[1])
     else:
         return jt.min(*args, **kw)
 Tensor.min = conflict_wrapper(jt.min, min)
 
 def max(*args, **kw):
     dim = None
     if "dim" in kw:
@@ -186,14 +206,16 @@
     if len(args) >= 2 and isinstance(args[1], org_int):
         dim = args[1]
     elif "dim" in kw and isinstance(kw["dim"], org_int):
         dim = kw["dim"]
     if dim is not None:
         k, v = jt.argmax(*args, **kw)
         return v, k
+    elif len(args) == 2 and isinstance(args[1], jt.Var):
+        return jt.maximum(args[0], args[1])
     else:
         return jt.max(*args, **kw)
 Tensor.max = conflict_wrapper(jt.max, max)
 
 def argsort(*args, **kw):
     k, v = jt.argsort(*args, **kw)
     return k
@@ -227,8 +249,9 @@
 def load(path, map_location="cpu"):
     return jt.load(path)
 
 def is_tensor(x):
     return isinstance(x, Tensor)
 
 manual_seed = jt.set_global_seed
-jt.flags.amp_level = 3
+jt.flags.amp_level = 3
+Size = jt.NanoVector
```

### Comparing `jtorch-0.1.3/python/jtorch/autograd.py` & `jtorch-0.1.6/python/jtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/compiler.py` & `jtorch-0.1.6/python/jtorch/compiler.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/distributed.py` & `jtorch-0.1.6/python/jtorch/distributed.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/nn/__init__.py` & `jtorch-0.1.6/python/jtorch/nn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import jtorch
 import jittor as jt
 
-from jtorch import make_module, Tensor, ModuleMisc
+from jtorch import make_module, Tensor, ModuleMisc, wrapper
 
 for k,v in jt.nn.__dict__.items():
     if callable(v):
-        globals()[k] = v
+        globals()[k] = wrapper(v)
 
 for k,v in jt.nn.__dict__.items():
     if isinstance(v, type) and issubclass(v, jt.Module):
         globals()[k] = make_module(v)
 
 class Module(ModuleMisc, jt.Module):
     def __call__(self, *args, **kw):
```

### Comparing `jtorch-0.1.3/python/jtorch/optim.py` & `jtorch-0.1.6/python/jtorch/optim.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         for pg in self.param_groups:
             pg["grads"] = [ 0 if p.grad is None else p.grad
                 for p in pg["params"] ]
             for p in pg["params"]:
                 if p.requires_grad:
                     params_has_grad.append(p)
         jt.sync(params_has_grad)
-
+        self.n_step += 1
+        
     def zero_grad(self):
         for pg in self.param_groups:
             pg["grads"] = [ None for p in pg["params"] ]
             for p in pg["params"]: p.grad = None
 
     def post_step(self):
         jt.flags.node_order = 0
```

### Comparing `jtorch-0.1.3/python/jtorch/src/jtorch_core.cc` & `jtorch-0.1.6/python/jtorch/src/jtorch_core.cc`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/src/jtorch_core.h` & `jtorch-0.1.6/python/jtorch/src/jtorch_core.h`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 // @pyjt(device)
 struct Device {
     string name;
     
     // @pyjt(__init__)
     Device(const string& name);
-    // @pyjt(__get__type)
+    // @pyjt(__get__type, __str__)
     inline string get_type() {return name;}
     // @pyjt(__get__index)
     inline int index() {return 0;}
 };
 
 // @pyjt(backward)
 void backward(VarHolder* x);
```

### Comparing `jtorch-0.1.3/python/jtorch/test/test_conflict_func.py` & `jtorch-0.1.6/python/jtorch/test/test_conflict_func.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/test/test_function.py` & `jtorch-0.1.6/python/jtorch/test/test_function.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/test/test_misc.py` & `jtorch-0.1.6/python/jtorch/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/test/test_tutorial.py` & `jtorch-0.1.6/python/jtorch/test/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad1.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad1.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad2.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad2.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad3.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad3.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad4.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad4.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad5_optim.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad5_optim.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad6_module.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad6_module.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/auto_grad7_dynet.py` & `jtorch-0.1.6/python/jtorch/tutorial/auto_grad7_dynet.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/tutorial/quickstart.py` & `jtorch-0.1.6/python/jtorch/tutorial/quickstart.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/utils/data.py` & `jtorch-0.1.6/python/jtorch/utils/data.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/utils/pip_publish.py` & `jtorch-0.1.6/python/jtorch/utils/pip_publish.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/vision/_internally_replaced_utils.py` & `jtorch-0.1.6/python/jtorch/vision/_internally_replaced_utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/vision/datasets/mnist.py` & `jtorch-0.1.6/python/jtorch/vision/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/vision/datasets/utils.py` & `jtorch-0.1.6/python/jtorch/vision/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/vision/datasets/vision.py` & `jtorch-0.1.6/python/jtorch/vision/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch/vision/utils.py` & `jtorch-0.1.6/python/jtorch/vision/utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/jtorch.egg-info/PKG-INFO` & `jtorch-0.1.6/python/jtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtorch
-Version: 0.1.3
+Version: 0.1.6
 Summary: jtorch project
 Home-page: https://github.com/JITTorch/jtorch
 Author: jtorch
 Author-email: jtorch@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JITTorch/jtorch/issues
 Platform: UNKNOWN
```

### Comparing `jtorch-0.1.3/python/jtorch.egg-info/SOURCES.txt` & `jtorch-0.1.6/python/jtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/python/torch/__init__.py` & `jtorch-0.1.6/python/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.3/setup.py` & `jtorch-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jtorch",
-    version="0.1.3",
+    version="0.1.6",
     author="jtorch",
     author_email="jtorch@qq.com",
     description="jtorch project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JITTorch/jtorch",
     project_urls={
```

