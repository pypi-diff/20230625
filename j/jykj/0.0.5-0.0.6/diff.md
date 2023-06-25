# Comparing `tmp/jykj-0.0.5.tar.gz` & `tmp/jykj-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.5.tar", last modified: Wed Jun 21 08:39:41 2023, max compression
+gzip compressed data, was "jykj-0.0.6.tar", last modified: Sun Jun 25 02:34:23 2023, max compression
```

## Comparing `jykj-0.0.5.tar` & `jykj-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.213119 jykj-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-21 08:39:41.212118 jykj-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.185112 jykj-0.0.5/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.5/jykj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.211139 jykj-0.0.5/jykj/business_model/
--rw-rw-rw-   0        0        0    17263 2023-06-20 02:59:17.000000 jykj-0.0.5/jykj/business_model/SHE.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.5/jykj/business_model/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.5/jykj/business_model/prevention.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.5/jykj/business_model/production.py
--rw-rw-rw-   0        0        0    14682 2023-06-20 02:56:19.000000 jykj-0.0.5/jykj/business_model/security.py
--rw-rw-rw-   0        0        0    29712 2023-06-21 08:39:19.000000 jykj-0.0.5/jykj/business_model/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:39:41.200118 jykj-0.0.5/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-21 08:39:41.000000 jykj-0.0.5/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 08:39:41.213119 jykj-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-21 08:20:45.000000 jykj-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.909490 jykj-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-25 02:34:23.909490 jykj-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.883490 jykj-0.0.6/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.6/jykj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.908492 jykj-0.0.6/jykj/business_model/
+-rw-rw-rw-   0        0        0    17263 2023-06-20 02:59:17.000000 jykj-0.0.6/jykj/business_model/SHE.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.6/jykj/business_model/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.6/jykj/business_model/prevention.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.6/jykj/business_model/production.py
+-rw-rw-rw-   0        0        0    14682 2023-06-20 02:56:19.000000 jykj-0.0.6/jykj/business_model/security.py
+-rw-rw-rw-   0        0        0    28542 2023-06-25 01:35:15.000000 jykj-0.0.6/jykj/business_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.903490 jykj-0.0.6/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 02:34:23.909490 jykj-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-25 01:34:36.000000 jykj-0.0.6/setup.py
```

### Comparing `jykj-0.0.5/LICENSE` & `jykj-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jykj-0.0.5/jykj/business_model/SHE.py` & `jykj-0.0.6/jykj/business_model/SHE.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.5/jykj/business_model/security.py` & `jykj-0.0.6/jykj/business_model/security.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.5/jykj/business_model/utils.py` & `jykj-0.0.6/jykj/business_model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 import cv2
 import math
-import jieba
-import joblib
 import numpy as np
 from typing import Union
 from scipy.optimize import linear_sum_assignment
 from filterpy.kalman import KalmanFilter
 
 
 def rela_to_abs(coords: list, resolution: list) -> list:
@@ -853,50 +851,7 @@
         tuple: x1, y1, x2, y2
     """
     kpts = np.array(kpts)
     min_x, min_y = np.min(kpts, axis=0)
     max_x, max_y = np.max(kpts, axis=0)
     return min_x, min_y, max_x, max_y
 
-
-MODEL = None
-TF = None
-def load_model(model_path: str, tf_path: str) -> None:
-    """"
-    加载贝叶斯分类器的模型和权重
-    参数：
-        model_path (str): 贝叶斯分类器模型的路径
-        tf_path (str): 贝叶斯分类器权重的路径
-
-    返回：
-        None
-    """
-    global MODEL 
-    global TF
-
-    MODEL = joblib.load(model_path)
-    TF = joblib.load(tf_path)
-
-
-def text_classification(name: str) -> str:
-    """
-    输入精英科技产品的系统名称，返回对应的产品线名称。
-
-    参数：
-        name (str): 精英科技产品的系统名称
-
-    返回：
-        str: 该系统对应的产品线名称
-    """
-    assert MODEL != None and TF != None
-    
-    words = jieba.cut(name)
-    s = ' '.join(words)
-
-    test_features = TF.transform([s]) 
-    predicted_labels = MODEL.predict(test_features)
-    predicted_probs = MODEL.predict_proba(test_features)
-    label, prob = predicted_labels[0], np.max(predicted_probs)
-    if prob < 0.3:
-        return "该系统没有对应的产品线！"
-    else:
-        return name + ": " + label
```

### Comparing `jykj-0.0.5/setup.py` & `jykj-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jykj",
-    version="0.0.5",
+    version="0.0.6",
     author="jykj",
     author_email="renshuai@jylink.com",
     description="",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

