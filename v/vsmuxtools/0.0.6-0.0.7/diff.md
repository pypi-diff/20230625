# Comparing `tmp/vsmuxtools-0.0.6.tar.gz` & `tmp/vsmuxtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.6.tar", last modified: Fri Jun  9 15:27:01 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.7.tar", last modified: Sat Jun 24 22:30:56 2023, max compression
```

## Comparing `vsmuxtools-0.0.6.tar` & `vsmuxtools-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1417 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-08 16:59:28.000000 vsmuxtools-0.0.6/README.md
--rw-rw-rw-   0        0        0     1100 2023-06-09 15:25:44.000000 vsmuxtools-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.292511 vsmuxtools-0.0.6/vsmuxtools/
--rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.6/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.306646 vsmuxtools-0.0.6/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.6/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     3910 2023-06-05 21:05:59.000000 vsmuxtools-0.0.6/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.6/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.308646 vsmuxtools-0.0.6/vsmuxtools/utils/
--rw-rw-rw-   0        0        0      127 2023-06-05 20:25:49.000000 vsmuxtools-0.0.6/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     5909 2023-06-05 20:52:26.000000 vsmuxtools-0.0.6/vsmuxtools/utils/audio.py
--rw-rw-rw-   0        0        0     8125 2023-06-05 20:47:48.000000 vsmuxtools-0.0.6/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.6/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.311159 vsmuxtools-0.0.6/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.6/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.6/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.6/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0    10096 2023-06-05 18:38:29.000000 vsmuxtools-0.0.6/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.304645 vsmuxtools-0.0.6/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0     1417 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:56.014985 vsmuxtools-0.0.7/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1417 2023-06-24 22:30:56.013985 vsmuxtools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-08 16:59:28.000000 vsmuxtools-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1100 2023-06-24 22:11:05.000000 vsmuxtools-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 22:30:56.014985 vsmuxtools-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:55.996981 vsmuxtools-0.0.7/vsmuxtools/
+-rw-rw-rw-   0        0        0      268 2023-06-23 22:54:04.000000 vsmuxtools-0.0.7/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:56.008983 vsmuxtools-0.0.7/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0      105 2023-06-23 22:50:34.000000 vsmuxtools-0.0.7/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     3910 2023-06-05 21:05:59.000000 vsmuxtools-0.0.7/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1495 2023-06-10 00:40:55.000000 vsmuxtools-0.0.7/vsmuxtools/extension/chapters.py
+-rw-rw-rw-   0        0        0     3990 2023-06-24 00:27:02.000000 vsmuxtools-0.0.7/vsmuxtools/extension/sub.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:56.011984 vsmuxtools-0.0.7/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0      127 2023-06-05 20:25:49.000000 vsmuxtools-0.0.7/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     5909 2023-06-05 20:52:26.000000 vsmuxtools-0.0.7/vsmuxtools/utils/audio.py
+-rw-rw-rw-   0        0        0     8125 2023-06-05 20:47:48.000000 vsmuxtools-0.0.7/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.7/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:56.013985 vsmuxtools-0.0.7/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.7/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.7/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3565 2023-06-11 12:35:17.000000 vsmuxtools-0.0.7/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0    10096 2023-06-05 18:38:29.000000 vsmuxtools-0.0.7/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:30:56.006983 vsmuxtools-0.0.7/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0     1417 2023-06-24 22:30:55.000000 vsmuxtools-0.0.7/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2023-06-24 22:30:55.000000 vsmuxtools-0.0.7/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 22:30:55.000000 vsmuxtools-0.0.7/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-24 22:30:55.000000 vsmuxtools-0.0.7/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 22:30:55.000000 vsmuxtools-0.0.7/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.6/LICENSE` & `vsmuxtools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/PKG-INFO` & `vsmuxtools-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.6/pyproject.toml` & `vsmuxtools-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.6"
+version = "0.0.7"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
     "numpy>=1.24.3",
-    "muxtools>=0.0.6",
+    "muxtools>=0.0.7",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.6/vsmuxtools/extension/audio.py` & `vsmuxtools-0.0.7/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.7/vsmuxtools/extension/chapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,14 @@
         :param fps:                 Needed for timestamp convertion. Gets the fps from the clip if src_file and otherwise assumes 24000/1001.
         :param _print:              Prints chapters after parsing and after trimming.
         """
         if isinstance(chapter_source, src_file):
             clip_fps = Fraction(chapter_source.src.fps_num, chapter_source.src.fps_den)
             self.fps = fps if fps else clip_fps
             self.chapters = parse_chapters_bdmv(chapter_source.file, self.fps, chapter_source.src.num_frames, _print)
-            if chapter_source.trim:
+            if self.chapters and chapter_source.trim:
                 self.trim(chapter_source.trim[0], chapter_source.trim[1], chapter_source.src.num_frames)
                 if _print:
                     print("After trim:")
                     self.print()
         else:
             super().__init__(chapter_source, fps if fps else Fraction(24000, 1001), _print)
```

### Comparing `vsmuxtools-0.0.6/vsmuxtools/utils/audio.py` & `vsmuxtools-0.0.7/vsmuxtools/utils/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.7/vsmuxtools/utils/src.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.7/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.7/vsmuxtools/video/resumable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-from pathlib import Path
+import os
 import re
 import subprocess
+from pathlib import Path
 from muxtools import ensure_path_exists, PathLike, get_executable, run_commandline, error, info
 
 
 def parse_keyframes(file: PathLike) -> list[int]:
+    pattern = re.compile(r"n:(?: +)?(?P<frame>\d+).*type:(?: +)?(?P<type>.)")
     file = ensure_path_exists(file, parse_keyframes)
     frames = list[int]()
-    ffprobe = get_executable("ffprobe")
-    args = [ffprobe, "-select_streams", "v", "-show_frames", "-show_entries", "frame=pict_type", str(file)]
+    # ffmpeg seems to be A LOT faster than ffprobe for this. (Maybe ffprobe can't multithread?)
+    ffmpeg = get_executable("ffmpeg")
+    out_var = "NUL" if os.name == "nt" else "/dev/null"
+    args = [ffmpeg, "-hide_banner", "-i", str(file), "-map", "0:v:0", "-filter:v", "showinfo", "-f", "null", out_var]
     out = subprocess.run(args, capture_output=True, text=True)
-    current = 0
-    for line in out.stdout.splitlines():
-        line = line.strip()
-        if line.startswith("pict_type"):
-            if line.split("=")[1] == "I":
-                frames.append(current)
-            current += 1
+    if out.returncode != 0:
+        error("Failed to parse video keyframes using ffmpeg!", parse_keyframes)
+        print(out.stderr)
+        print(out.stdout)
+        out.check_returncode()
+
+    for line in out.stderr.splitlines():
+        if "showinfo" in line:
+            matches = re.findall(pattern, line.strip())
+            if matches:
+                match = matches[0]
+                if match[1] == "I":
+                    frames.append(int(match[0]))
     return frames
 
 
 def merge_parts(last: Path, original_out: Path, keyframes: list[int], parts: list[Path], quiet: bool = True):
     # This function is partially stolen from vardautomation but with less weird abstraction
     mkvmerge = get_executable("mkvmerge")
     mkvextract = get_executable("mkvextract")
```

### Comparing `vsmuxtools-0.0.6/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.7/vsmuxtools/video/settings.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.6/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.7/vsmuxtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.6/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.7/vsmuxtools.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 vsmuxtools.egg-info/SOURCES.txt
 vsmuxtools.egg-info/dependency_links.txt
 vsmuxtools.egg-info/requires.txt
 vsmuxtools.egg-info/top_level.txt
 vsmuxtools/extension/__init__.py
 vsmuxtools/extension/audio.py
 vsmuxtools/extension/chapters.py
+vsmuxtools/extension/sub.py
 vsmuxtools/utils/__init__.py
 vsmuxtools/utils/audio.py
 vsmuxtools/utils/src.py
 vsmuxtools/utils/types.py
 vsmuxtools/video/__init__.py
 vsmuxtools/video/encoders.py
 vsmuxtools/video/resumable.py
```

