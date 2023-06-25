# Comparing `tmp/video_process-0.1.5.tar.gz` & `tmp/video_process-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.1.5.tar", max compression
+gzip compressed data, was "video_process-0.1.6.tar", max compression
```

## Comparing `video_process-0.1.5.tar` & `video_process-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-06-21 08:52:17.114548 video_process-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-21 08:43:34.831508 video_process-0.1.5/video_process/__init__.py
--rw-r--r--   0        0        0     3773 2023-06-21 08:39:17.232594 video_process-0.1.5/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1316 2023-06-21 08:31:08.374374 video_process-0.1.5/video_process/index.py
--rw-r--r--   0        0        0     1782 2023-06-21 08:16:52.008047 video_process-0.1.5/video_process/lib.py
--rw-r--r--   0        0        0     1941 2023-06-21 06:40:11.174245 video_process-0.1.5/video_process/subtitle.py
--rw-r--r--   0        0        0     2944 2023-06-21 06:40:24.748946 video_process-0.1.5/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-06-25 04:04:26.548272 video_process-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-21 08:43:34.831508 video_process-0.1.6/video_process/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-25 03:58:29.668830 video_process-0.1.6/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1316 2023-06-21 08:31:08.374374 video_process-0.1.6/video_process/index.py
+-rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.1.6/video_process/lib.py
+-rw-r--r--   0        0        0      664 2023-06-21 09:05:03.418463 video_process-0.1.6/video_process/subtitle.py
+-rw-r--r--   0        0        0     2944 2023-06-21 06:40:24.748946 video_process-0.1.6/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.6/PKG-INFO
```

### Comparing `video_process-0.1.5/video_process/graph_builder.py` & `video_process-0.1.6/video_process/graph_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     def overlay(self, x, y):
         self.stream = self.stream.filter("pad", width="iw", height="ih", x=x, y=y)
 
     def add_bg(self, bg, x, y):
         if bg["bg_type"] == "video":
             bg_video = ffmpeg.input(bg["bg_video_path"])
             bg_video = bg_video.filter(
+                "crop",
+                bg["crop"]["width"],
+                bg["crop"]["height"],
+                bg["crop"]["x"],
+                bg["crop"]["y"],
+            ).filter(
                 "scale",
                 width=self.width,
                 height=self.height,
                 force_original_aspect_ratio="decrease",
             )
             self.stream = ffmpeg.overlay(bg_video, self.stream, x=x, y=y)
         elif bg["bg_type"] == "image":
```

### Comparing `video_process-0.1.5/video_process/index.py` & `video_process-0.1.6/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.5/video_process/lib.py` & `video_process-0.1.6/video_process/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 
 # 腾讯云 COS 配置
 BUCKET_NAME = os.environ.get("BUCKET_NAME")
 COS_REGION = os.environ.get("COS_REGION", "ap-beijing")
@@ -47,11 +46,7 @@
         LocalFilePath=file_path,
         Key=key,
         PartSize=10,
         MAXThread=10,
         EnableMD5=False,
     )
     return response["ETag"]
-
-
-if __name__ == "__main__":
-    get_cos_url("71e52c67f5094e44b92ccaed93db15c5.jpg")
```

### Comparing `video_process-0.1.5/video_process/utils.py` & `video_process-0.1.6/video_process/utils.py`

 * *Files identical despite different names*

