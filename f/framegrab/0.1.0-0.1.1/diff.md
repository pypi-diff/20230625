# Comparing `tmp/framegrab-0.1.0.tar.gz` & `tmp/framegrab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.1.0.tar", max compression
+gzip compressed data, was "framegrab-0.1.1.tar", max compression
```

## Comparing `framegrab-0.1.0.tar` & `framegrab-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-04-20 22:29:00.275250 framegrab-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2906 2023-04-22 22:09:59.440073 framegrab-0.1.0/README.md
--rw-r--r--   0        0        0      494 2023-04-22 22:11:28.742891 framegrab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10372 2023-04-20 22:27:58.128025 framegrab-0.1.0/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2460 2023-04-20 22:27:58.128025 framegrab-0.1.0/src/framegrab/motion.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 framegrab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2906 2023-06-16 19:22:23.911372 framegrab-0.1.1/README.md
+-rw-r--r--   0        0        0      471 2023-06-25 18:57:35.749379 framegrab-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10360 2023-06-16 19:22:23.911782 framegrab-0.1.1/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2456 2023-06-24 01:53:17.596683 framegrab-0.1.1/src/framegrab/motion.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 framegrab-0.1.1/PKG-INFO
```

### Comparing `framegrab-0.1.0/LICENSE.txt` & `framegrab-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.0/README.md` & `framegrab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.0/src/framegrab/grabber.py` & `framegrab-0.1.1/src/framegrab/grabber.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 from threading import Lock, Thread
 
 import cv2
 import numpy as np
 import pafy
 
-logger = logging.getLogger("groundlight.stream")
+logger = logging.getLogger(__name__)
 
 
 class FrameGrabber(metaclass=ABCMeta):
     @staticmethod
     def create_grabber(stream=None, **kwargs):
         logger.debug(f"Input {stream=} (type {type(stream)}")
         if type(stream) == int:
```

### Comparing `framegrab-0.1.0/src/framegrab/motion.py` & `framegrab-0.1.1/src/framegrab/motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import numpy as np
 
-logger = logging.getLogger("groundlight.stream")
+logger = logging.getLogger(__name__)
 
 
 class MotionDetector:
     # Simple motion detector using the three frame differencing
     # commonly attributed to Collins, et. al A system for video surveillance and monitoring. Technical report, 2000
     # Defaults to 1% pixel difference threshold (good for many applications)
 
@@ -17,15 +17,15 @@
         """
         self.unused = True
         self.threshold = 50
         self.pixel_val_threshold = 50
         self.pixel_pct_threshold = pct_threshold
         self.log_pixel_percent = True
 
-    def pixel_threshold(self, img: np.ndarray, threshold_val: float = None):
+    def pixel_threshold(self, img: np.ndarray, threshold_val: float = None) -> bool:
         """Returns true if more then pixel_pct_threshold% of pixels have value greater than pixel_val_threshold"""
         if threshold_val is None:
             threshold_val = self.pixel_val_threshold
         total_pixels = np.prod(img.shape)
         hi_pixels = np.sum(img > threshold_val)
         pct_hi = float(hi_pixels) / float(total_pixels) * 100
         if pct_hi > self.pixel_pct_threshold:
```

### Comparing `framegrab-0.1.0/PKG-INFO` & `framegrab-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easily grab frames from cameras or streams
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: groundlight (>=0.7.8,<0.8.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
 Description-Content-Type: text/markdown
 
 # FrameGrab by Groundlight
 ## A user-friendly library for grabbing images from cameras or streams
```

