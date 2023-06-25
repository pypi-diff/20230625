# Comparing `tmp/vc-filter-1.1.6.tar.gz` & `tmp/vc-filter-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vc-filter-1.1.6.tar", last modified: Wed Jan 18 10:45:55 2023, max compression
+gzip compressed data, was "vc-filter-1.1.7.tar", last modified: Sun Jun 25 07:57:13 2023, max compression
```

## Comparing `vc-filter-1.1.6.tar` & `vc-filter-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-18 10:45:55.467603 vc-filter-1.1.6/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-01-18 10:45:55.467316 vc-filter-1.1.6/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     2762 2022-01-30 19:57:29.000000 vc-filter-1.1.6/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-01-18 10:45:55.467676 vc-filter-1.1.6/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1120 2023-01-18 10:21:14.000000 vc-filter-1.1.6/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-18 10:45:55.465181 vc-filter-1.1.6/vc_filter/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       37 2022-01-02 07:31:26.000000 vc-filter-1.1.6/vc_filter/__init__.py
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     5128 2023-01-18 10:27:20.000000 vc-filter-1.1.6/vc_filter/code.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-18 10:45:55.466931 vc-filter-1.1.6/vc_filter.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-01-18 10:45:55.000000 vc-filter-1.1.6/vc_filter.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      222 2023-01-18 10:45:55.000000 vc-filter-1.1.6/vc_filter.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-01-18 10:45:55.000000 vc-filter-1.1.6/vc_filter.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       29 2023-01-18 10:45:55.000000 vc-filter-1.1.6/vc_filter.egg-info/requires.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       10 2023-01-18 10:45:55.000000 vc-filter-1.1.6/vc_filter.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.960876 vc-filter-1.1.7/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-06-25 07:57:13.960573 vc-filter-1.1.7/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     2762 2022-01-30 19:57:29.000000 vc-filter-1.1.7/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-25 07:57:13.960975 vc-filter-1.1.7/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1120 2023-06-25 07:50:58.000000 vc-filter-1.1.7/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.958372 vc-filter-1.1.7/vc_filter/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       37 2022-01-02 07:31:26.000000 vc-filter-1.1.7/vc_filter/__init__.py
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     5143 2023-06-25 07:51:49.000000 vc-filter-1.1.7/vc_filter/code.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.960106 vc-filter-1.1.7/vc_filter.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      222 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       29 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/requires.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       10 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/top_level.txt
```

### Comparing `vc-filter-1.1.6/PKG-INFO` & `vc-filter-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vc-filter
-Version: 1.1.6
+Version: 1.1.7
 Summary: VC Filter is a new edge detection algorithm based on the Visual Cortex study
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vc-filter-1.1.6/README.md` & `vc-filter-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vc-filter-1.1.6/setup.py` & `vc-filter-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="vc-filter",
-    version="1.1.6",
+    version="1.1.7",
     description="VC Filter is a new edge detection algorithm based on the Visual Cortex study",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `vc-filter-1.1.6/vc_filter/code.py` & `vc-filter-1.1.7/vc_filter/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Jan-18-2023
+# Jun-25-2023
 # code.py
 
 import cv2 as cv
 import numpy as np
 
 
 def vc_filter(image):
@@ -166,15 +166,15 @@
 
 
 def dft_rotate(dft, height_dft, width_dft, angle):
 
     re = dft[:, :, 0]
     im = dft[:, :, 1]
 
-    M = cv.getRotationMatrix2D((width_dft / 2, height_dft / 2), angle, 1)
+    matrix = cv.getRotationMatrix2D((width_dft / 2, height_dft / 2), angle, 1)
 
-    re_rot = cv.warpAffine(re, M, (width_dft, height_dft))
-    im_rot = cv.warpAffine(im, M, (width_dft, height_dft))
+    re_rot = cv.warpAffine(re, matrix, (width_dft, height_dft))
+    im_rot = cv.warpAffine(im, matrix, (width_dft, height_dft))
 
     dft_rot = cv.merge([re_rot, im_rot])
 
     return dft_rot
```

### Comparing `vc-filter-1.1.6/vc_filter.egg-info/PKG-INFO` & `vc-filter-1.1.7/vc_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vc-filter
-Version: 1.1.6
+Version: 1.1.7
 Summary: VC Filter is a new edge detection algorithm based on the Visual Cortex study
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

