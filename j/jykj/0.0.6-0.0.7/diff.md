# Comparing `tmp/jykj-0.0.6.tar.gz` & `tmp/jykj-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.6.tar", last modified: Sun Jun 25 02:34:23 2023, max compression
+gzip compressed data, was "jykj-0.0.7.tar", last modified: Sun Jun 25 06:47:55 2023, max compression
```

## Comparing `jykj-0.0.6.tar` & `jykj-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.909490 jykj-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-25 02:34:23.909490 jykj-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.883490 jykj-0.0.6/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.6/jykj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.908492 jykj-0.0.6/jykj/business_model/
--rw-rw-rw-   0        0        0    17263 2023-06-20 02:59:17.000000 jykj-0.0.6/jykj/business_model/SHE.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.6/jykj/business_model/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.6/jykj/business_model/prevention.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.6/jykj/business_model/production.py
--rw-rw-rw-   0        0        0    14682 2023-06-20 02:56:19.000000 jykj-0.0.6/jykj/business_model/security.py
--rw-rw-rw-   0        0        0    28542 2023-06-25 01:35:15.000000 jykj-0.0.6/jykj/business_model/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 02:34:23.903490 jykj-0.0.6/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 02:34:23.000000 jykj-0.0.6/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 02:34:23.909490 jykj-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-25 01:34:36.000000 jykj-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.067578 jykj-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-25 06:47:55.067578 jykj-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.049577 jykj-0.0.7/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.7/jykj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.065575 jykj-0.0.7/jykj/business_model/
+-rw-rw-rw-   0        0        0    17264 2023-06-25 06:46:54.000000 jykj-0.0.7/jykj/business_model/SHE.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.7/jykj/business_model/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.7/jykj/business_model/prevention.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.7/jykj/business_model/production.py
+-rw-rw-rw-   0        0        0    14683 2023-06-25 06:46:56.000000 jykj-0.0.7/jykj/business_model/security.py
+-rw-rw-rw-   0        0        0    28542 2023-06-25 01:35:15.000000 jykj-0.0.7/jykj/business_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.059575 jykj-0.0.7/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 06:47:55.068576 jykj-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-25 06:47:43.000000 jykj-0.0.7/setup.py
```

### Comparing `jykj-0.0.6/LICENSE` & `jykj-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jykj-0.0.6/jykj/business_model/SHE.py` & `jykj-0.0.7/jykj/business_model/SHE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from utils import rela_to_abs, pnpoly, min_bbox
+from .utils import rela_to_abs, pnpoly, min_bbox
 
 
 def persons_in_areas(persons_coords: list,
                      areas: list,
                      resolution: list = [],
                      h_offset: float = 0,
                      w_thresh: float = -1,
```

### Comparing `jykj-0.0.6/jykj/business_model/security.py` & `jykj-0.0.7/jykj/business_model/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cv2
 import sys
 import numpy as np
-from utils import goodness_of_fit, fit_line, rela_to_abs, pnpoly
+from .utils import goodness_of_fit, fit_line, rela_to_abs, pnpoly
 
 
 def pd(centers: list, thr: float) -> int:
     '''
         是否排队  根据多个目标中心点拟合直线，根据r2阈值判断是否排队
 
         参数：
```

### Comparing `jykj-0.0.6/jykj/business_model/utils.py` & `jykj-0.0.7/jykj/business_model/utils.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.6/setup.py` & `jykj-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jykj",
-    version="0.0.6",
+    version="0.0.7",
     author="jykj",
     author_email="renshuai@jylink.com",
     description="",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

