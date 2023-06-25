# Comparing `tmp/ffmpegcv-0.3.2.tar.gz` & `tmp/ffmpegcv-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.3.2.tar", last modified: Wed Jun  7 05:49:57 2023, max compression
+gzip compressed data, was "dist/ffmpegcv-0.3.3.tar", last modified: Sun Jun 25 17:02:33 2023, max compression
```

## Comparing `ffmpegcv-0.3.2.tar` & `ffmpegcv-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11279 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11066 2023-06-07 05:48:36.000000 ffmpegcv-0.3.2/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10453 2023-05-30 19:18:41.000000 ffmpegcv-0.3.2/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     9732 2023-05-30 14:58:25.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1685 2022-05-19 12:21:02.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_grey.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1474 2022-06-04 11:24:12.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_hflip.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.2/ffmpegcv/stream_info.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2731 2023-05-30 15:03:32.000000 ffmpegcv-0.3.2/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11279 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      487 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      650 2023-06-07 05:13:57.000000 ffmpegcv-0.3.2/setup.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12787 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12568 2023-06-23 19:09:37.000000 ffmpegcv-0.3.3/README.md
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10529 2023-06-23 17:47:32.000000 ffmpegcv-0.3.3/ffmpegcv/__init__.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_framepick.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_laggy.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2259 2023-06-24 13:18:20.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.3/ffmpegcv/stream_info.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.3/ffmpegcv/video_info.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12787 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      458 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/setup.cfg
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-25 17:02:06.000000 ffmpegcv-0.3.3/setup.py
```

### Comparing `ffmpegcv-0.3.2/PKG-INFO` & `ffmpegcv-0.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.2
-Home-page: https://pypi.org/project/ffmpegcv/
+Version: 0.3.3
+Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
+![Python versions](https://img.shields.io/badge/Python-3.6%2B-blue.svg)
+[![PyPI version](https://img.shields.io/pypi/v/ffmpegcv.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ffmpegcv/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/ffmpegcv.svg)](https://pypistats.org/packages/ffmpegcv)
+![Code size](https://shields.io/github/languages/code-size/chenxinfeng4/ffmpegcv
+)
+![Last Commit](https://shields.io/github/last-commit/chenxinfeng4/ffmpegcv)
+
+English Version | [中文版本](./README_CN.md)
+
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
-- The ffmpegcv support **RGB** & BGR format as you like.
+- The ffmpegcv support **RGB** & BGR & GRAY format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
 In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
-Functions:
+## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
+- `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+- `FFmpegReaderNoblock`: Read a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -79,15 +90,15 @@
 | h264        | √             | √                | √    | ×             | √                | √    |
 | h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
 | mjpeg       | √             | √                | ×    | √             | √                | ×    |
 | mpeg        | √             | √                | ×    | √             | √                | ×    |
 | others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
 
 ## Benchmark
-*On the way...*
+*On the way...（maybe never）*
 
 
 ## Video Reader
 ---
 The ffmpegcv is just similar to opencv in api.
 ```python
 # open cv
@@ -129,17 +140,17 @@
 ```python
 cap_cpu = ffmpegcv.VideoCapture(file)
 cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
 cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
 cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
 ```
 
-Use rgb24 instead of bgr24
+Use `rgb24` instead of `bgr24`. The `gray` version would be more efficient.
 ```python
-cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
+cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24') #rgb24, bgr24, gray
 ret, frame = cap.read()
 plt.imshow(frame)
 ```
 
 ### ROI Operations
 You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
 
@@ -323,7 +334,27 @@
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 ```
+
+## FFmpegReaderNoblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+
+```python
+#Proxy any VideoCapture args and kargs
+vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+
+# this is fast
+def cpu_tense(): time.sleep(0.01)
+for _ in tqdm.trange(1000):
+    ret, img = vid_noblock.read() #current img is already buffered, take no time
+    cpu_tense()                   #meanwhile, the next img is buffering in background
+
+# this is slow
+vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
+for _ in tqdm.trange(2000):
+    ret, img = vid.read()         #this read will block cpu, take time
+    cpu_tense()
+```
```

### Comparing `ffmpegcv-0.3.2/README.md` & `ffmpegcv-0.3.3/ffmpegcv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,43 @@
+Metadata-Version: 2.1
+Name: ffmpegcv
+Version: 0.3.3
+Home-page: https://github.com/chenxinfeng4/ffmpegcv
+Author: chenxf
+Author-email: cxf529125853@163.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # FFMPEGCV is an alternative to OPENCV for video read and write.
+![Python versions](https://img.shields.io/badge/Python-3.6%2B-blue.svg)
+[![PyPI version](https://img.shields.io/pypi/v/ffmpegcv.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ffmpegcv/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/ffmpegcv.svg)](https://pypistats.org/packages/ffmpegcv)
+![Code size](https://shields.io/github/languages/code-size/chenxinfeng4/ffmpegcv
+)
+![Last Commit](https://shields.io/github/last-commit/chenxinfeng4/ffmpegcv)
+
+English Version | [中文版本](./README_CN.md)
+
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
-- The ffmpegcv support **RGB** & BGR format as you like.
+- The ffmpegcv support **RGB** & BGR & GRAY format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
 In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
-Functions:
+## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
+- `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+- `FFmpegReaderNoblock`: Read a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -70,15 +90,15 @@
 | h264        | √             | √                | √    | ×             | √                | √    |
 | h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
 | mjpeg       | √             | √                | ×    | √             | √                | ×    |
 | mpeg        | √             | √                | ×    | √             | √                | ×    |
 | others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
 
 ## Benchmark
-*On the way...*
+*On the way...（maybe never）*
 
 
 ## Video Reader
 ---
 The ffmpegcv is just similar to opencv in api.
 ```python
 # open cv
@@ -120,17 +140,17 @@
 ```python
 cap_cpu = ffmpegcv.VideoCapture(file)
 cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
 cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
 cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
 ```
 
-Use rgb24 instead of bgr24
+Use `rgb24` instead of `bgr24`. The `gray` version would be more efficient.
 ```python
-cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
+cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24') #rgb24, bgr24, gray
 ret, frame = cap.read()
 plt.imshow(frame)
 ```
 
 ### ROI Operations
 You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
 
@@ -313,8 +333,28 @@
 import ffmpegcv
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
-```
+```
+
+## FFmpegReaderNoblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+
+```python
+#Proxy any VideoCapture args and kargs
+vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+
+# this is fast
+def cpu_tense(): time.sleep(0.01)
+for _ in tqdm.trange(1000):
+    ret, img = vid_noblock.read() #current img is already buffered, take no time
+    cpu_tense()                   #meanwhile, the next img is buffering in background
+
+# this is slow
+vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
+for _ in tqdm.trange(2000):
+    ret, img = vid.read()         #this read will block cpu, take time
+    cpu_tense()
+```
```

### Comparing `ffmpegcv-0.3.2/ffmpegcv/__init__.py` & `ffmpegcv-0.3.3/ffmpegcv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .ffmpeg_reader import FFmpegReader, FFmpegReaderNV
 from .ffmpeg_writer import FFmpegWriter, FFmpegWriterNV
 from .ffmpeg_reader_camera import FFmpegReaderCAM
 from .ffmpeg_reader_stream import FFmpegReaderStream
+from .ffmpeg_reader_noblock import FFmpegReaderNoblock
 from .video_info import get_num_NVIDIA_GPUs
 import shutil
 from subprocess import DEVNULL, check_output
 
 
 def _check():
     if not shutil.which("ffmpeg") or not shutil.which("ffprobe"):
@@ -16,15 +17,15 @@
         )
 
 
 _check()
 
 _check_nvidia_init = None
 
-
+__version__ = '0.3.3'
 def _check_nvidia():
     global _check_nvidia_init
     run = lambda x: check_output(x, shell=True, stderr=DEVNULL)
     if _check_nvidia_init is None:
         calling_output = run("ffmpeg -h encoder=hevc_nvenc")
         if "AVOptions" not in calling_output.decode("utf-8"):
             raise RuntimeError(
```

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_framepick.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_framepick.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         resize,
         resize_keepratio,
         resize_keepratioalign,
     ):
         assert os.path.exists(filename) and os.path.isfile(
             filename
         ), f"{filename} not exists"
-        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12", "gray"]
 
         vid = FFmpegReader()
         videoinfo = get_info(filename)
         vid.width = videoinfo.width
         vid.height = videoinfo.height
         vid.fps = videoinfo.fps
         vid.count = videoinfo.count
@@ -99,72 +99,76 @@
                 }
                 assert (
                     resize_keepratioalign in paddings
                 ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
                 padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
 
-        if any([cropopt, scaleopt, padopt]):
-            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt] if x)
+        pix_fmtopt = 'extractplanes=y' if pix_fmt=='gray' else ''
+        if any([cropopt, scaleopt, padopt, pix_fmtopt]):
+            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt, pix_fmtopt] if x)
             filteropt = f"-vf {filterstr}"
         else:
             filteropt = ""
 
-        args = (
+        vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning "
             f' -vcodec {vid.codec} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
         )
 
-        vid.process = run_async(args)
+        vid.process = run_async(vid.ffmpeg_cmd)
         vid.size = (vid.width, vid.height)
         vid.pix_fmt = pix_fmt
         assert (not pix_fmt == "yuv420p") or (
             vid.height % 2 == 0 and vid.width % 2 == 0
         ), "yuv420p must be even"
         vid.out_numpy_shape = {
             "rgb24": (vid.height, vid.width, 3),
             "bgr24": (vid.height, vid.width, 3),
             "nv12": (int(vid.height * 1.5), vid.width),
             "yuv420p": (int(vid.height * 1.5), vid.width),
+            "gray": (vid.height, vid.width, 1)
         }[pix_fmt]
         return vid
 
     def read_gray(self):
         # It's an experimental function
         # return 'ret, img_gray'
         # img_gray: Height x Width x 1
+        if self.pix_fmt == "gray":
+            return self.read()
+        
         assert self.pix_fmt in ("nv12", "yuv420p")
         ret, img = self.read()
         if not ret:
             return False, None
         assert img.shape == (int(self.height * 1.5), self.width)
         img_gray = img[: self.height, :, None]
         return True, img_gray
 
     def read(self):
         in_bytes = self.process.stdout.read(np.prod(self.out_numpy_shape))
         if not in_bytes:
             self.release()
             return False, None
         self.iframe += 1
-        img = None
         img = np.frombuffer(in_bytes, np.uint8).reshape(self.out_numpy_shape)
         return True, img
 
     def release(self):
         release_process(self.process)
 
     def close(self):
         return self.release()
 
 
 class FFmpegReaderNV(FFmpegReader):
     def _get_opts(
-        vid, videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign
+        vid, videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign, isgray
     ):
         vid.origin_width = videoinfo.width
         vid.origin_height = videoinfo.height
         vid.fps = videoinfo.fps
         vid.count = videoinfo.count
         vid.width, vid.height = vid.origin_width, vid.origin_height
         vid.codec = videoinfo.codec
@@ -216,14 +220,20 @@
                 assert (
                     resize_keepratioalign in paddings
                 ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
                 padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
                 filteropt = f"-vf {padopt}"
 
+        if isgray:
+            if filteropt:
+                filteropt=f'{filteropt},extractplanes=y'
+            else:
+                filteropt=f'-vf extractplanes=y'
+        
         vid.size = (vid.width, vid.height)
         return cropopt, scaleopt, filteropt
 
     @staticmethod
     def VideoReader(
         filename,
         pix_fmt,
@@ -232,39 +242,41 @@
         resize_keepratio,
         resize_keepratioalign,
         gpu,
     ):
         assert os.path.exists(filename) and os.path.isfile(
             filename
         ), f"{filename} not exists"
-        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12", "gray"]
         numGPU = get_num_NVIDIA_GPUs()
         assert numGPU > 0, "No GPU found"
         gpu = int(gpu) % numGPU if gpu is not None else 0
         assert (
             resize is None or len(resize) == 2
         ), "resize must be a tuple of (width, height)"
         videoinfo = get_info(filename)
         vid = FFmpegReaderNV()
+        isgray = pix_fmt == "gray"
         cropopt, scaleopt, filteropt = vid._get_opts(
-            videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign
+            videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign, isgray
         )
         vid.codecNV = decoder_to_nvidia(vid.codec)
 
-        args = (
+        vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning -hwaccel cuda -hwaccel_device {gpu} "
             f' -vcodec {vid.codecNV} {cropopt} {scaleopt} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
         )
 
-        vid.process = run_async(args)
+        vid.process = run_async(vid.ffmpeg_cmd)
         vid.pix_fmt = pix_fmt
         assert (not pix_fmt == "yuv420p") or (
             vid.height % 2 == 0 and vid.width % 2 == 0
         ), "yuv420p must be even"
         vid.out_numpy_shape = {
             "rgb24": (vid.height, vid.width, 3),
             "bgr24": (vid.height, vid.width, 3),
             "yuv420p": (int(vid.height * 1.5), vid.width),
             "nv12": (int(vid.height * 1.5), vid.width),
+            "gray": (vid.height, vid.width, 1)
         }[pix_fmt]
         return vid
```

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_laggy.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_laggy.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_stream.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_stream.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_writer.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.3/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.2/ffmpegcv/video_info.py` & `ffmpegcv-0.3.3/ffmpegcv/video_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import subprocess
 from subprocess import Popen, PIPE
 import re
 from collections import namedtuple
 import xml.etree.ElementTree as ET
 
+scan_the_whole = {'mkv', 'flv', 'ts'} #scan the whole file to the count, slow
 
-def get_info(video):
-    cmd = 'ffprobe -v quiet -print_format xml -select_streams v:0 -count_packets -show_format -show_streams "{}"'.format(video)
+def get_info(video:str):
+    do_scan_the_whole = video.split('.')[-1] in scan_the_whole
+    use_count_packets = '-count_packets' if do_scan_the_whole else ''
+    cmd = 'ffprobe -v quiet -print_format xml -select_streams v:0 {} -show_format -show_streams "{}"'.format(use_count_packets, video)
     output = subprocess.check_output(cmd, shell=True)
     root = ET.fromstring(output)
     assert (root[0].tag, root[0][0].tag) == ("streams", "stream")
     vinfo = root[0][0].attrib
 
     VideoInfo = namedtuple(
         "VideoInfo", ["width", "height", "fps", "count", "codec", "duration"]
     )
     outinfo = dict()
     outinfo['width'] = int(vinfo['width'])
     outinfo['height'] = int(vinfo['height'])
     outinfo['fps'] = eval(vinfo['r_frame_rate'])
-    outinfo['count'] = int(vinfo['nb_read_packets']) #nb_read_packets | nb_frames
+    outinfo['count'] = int(vinfo['nb_read_packets' if do_scan_the_whole
+                         else 'nb_frames']) #nb_read_packets | nb_frames
     outinfo['codec'] = vinfo['codec_name']
-    outinfo['duration'] = float(vinfo['duration'])
+    outinfo['duration'] = (float(vinfo['duration']) if 'duration' in vinfo
+                            else outinfo['count']/outinfo['fps'])
     videoinfo = VideoInfo(**outinfo)
 
     return videoinfo
 
 
 def get_num_NVIDIA_GPUs():
     cmd = "ffmpeg -f lavfi -i nullsrc -c:v h264_nvenc -gpu list -f null -"
@@ -87,11 +92,15 @@
         stderr=stderr_stream,
         shell=isinstance(args, str),
         bufsize=bufsize,
     )
 
 
 def release_process(process):
-    process.stdin.close()
-    process.stdout.close()
-    process.terminate()
-    process.wait()
+    if hasattr(process, "stdin"):
+        process.stdin.close()
+    if hasattr(process, "stdout"):
+        process.stdout.close()
+    if hasattr(process, "terminate"):
+        process.terminate()
+    if hasattr(process, "wait"):
+        process.wait()
```

### Comparing `ffmpegcv-0.3.2/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1
-Name: ffmpegcv
-Version: 0.3.2
-Home-page: https://pypi.org/project/ffmpegcv/
-Author: chenxf
-Author-email: cxf529125853@163.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # FFMPEGCV is an alternative to OPENCV for video read and write.
+![Python versions](https://img.shields.io/badge/Python-3.6%2B-blue.svg)
+[![PyPI version](https://img.shields.io/pypi/v/ffmpegcv.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ffmpegcv/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/ffmpegcv.svg)](https://pypistats.org/packages/ffmpegcv)
+![Code size](https://shields.io/github/languages/code-size/chenxinfeng4/ffmpegcv
+)
+![Last Commit](https://shields.io/github/last-commit/chenxinfeng4/ffmpegcv)
+
+English Version | [中文版本](./README_CN.md)
+
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
-- The ffmpegcv support **RGB** & BGR format as you like.
+- The ffmpegcv support **RGB** & BGR & GRAY format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
 In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
-Functions:
+## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
+- `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+- `FFmpegReaderNoblock`: Read a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -79,15 +81,15 @@
 | h264        | √             | √                | √    | ×             | √                | √    |
 | h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
 | mjpeg       | √             | √                | ×    | √             | √                | ×    |
 | mpeg        | √             | √                | ×    | √             | √                | ×    |
 | others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
 
 ## Benchmark
-*On the way...*
+*On the way...（maybe never）*
 
 
 ## Video Reader
 ---
 The ffmpegcv is just similar to opencv in api.
 ```python
 # open cv
@@ -129,17 +131,17 @@
 ```python
 cap_cpu = ffmpegcv.VideoCapture(file)
 cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
 cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
 cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
 ```
 
-Use rgb24 instead of bgr24
+Use `rgb24` instead of `bgr24`. The `gray` version would be more efficient.
 ```python
-cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
+cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24') #rgb24, bgr24, gray
 ret, frame = cap.read()
 plt.imshow(frame)
 ```
 
 ### ROI Operations
 You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
 
@@ -323,7 +325,27 @@
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 ```
+
+## FFmpegReaderNoblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+
+```python
+#Proxy any VideoCapture args and kargs
+vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+
+# this is fast
+def cpu_tense(): time.sleep(0.01)
+for _ in tqdm.trange(1000):
+    ret, img = vid_noblock.read() #current img is already buffered, take no time
+    cpu_tense()                   #meanwhile, the next img is buffering in background
+
+# this is slow
+vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
+for _ in tqdm.trange(2000):
+    ret, img = vid.read()         #this read will block cpu, take time
+    cpu_tense()
+```
```

### Comparing `ffmpegcv-0.3.2/setup.py` & `ffmpegcv-0.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.2', # 版本号
+    version='0.3.3', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
-    url='https://pypi.org/project/ffmpegcv/',
+    url='https://github.com/chenxinfeng4/ffmpegcv',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # 添加依赖项
     python_requires='>=3.6',
     install_requires=[
         'numpy',
```

