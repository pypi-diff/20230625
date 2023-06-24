# Comparing `tmp/muxtools-0.0.6.tar.gz` & `tmp/muxtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.6.tar", last modified: Fri Jun  9 15:26:25 2023, max compression
+gzip compressed data, was "muxtools-0.0.7.tar", last modified: Sat Jun 24 22:29:31 2023, max compression
```

## Comparing `muxtools-0.0.6.tar` & `muxtools-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.454151 muxtools-0.0.6/
--rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1619 2023-06-09 15:26:25.453150 muxtools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-06-08 16:58:55.000000 muxtools-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.418472 muxtools-0.0.6/muxtools/
--rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.436677 muxtools-0.0.6/muxtools/audio/
--rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.6/muxtools/audio/__init__.py
--rw-rw-rw-   0        0        0    10057 2023-06-08 16:32:38.000000 muxtools-0.0.6/muxtools/audio/audioutils.py
--rw-rw-rw-   0        0        0    14850 2023-06-05 21:23:22.000000 muxtools-0.0.6/muxtools/audio/encoders.py
--rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.6/muxtools/audio/extractors.py
--rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.6/muxtools/audio/memecoders.py
--rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.6/muxtools/audio/tools.py
--rw-rw-rw-   0        0        0     7680 2023-06-09 13:58:58.000000 muxtools-0.0.6/muxtools/cli.py
--rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.6/muxtools/functions.py
--rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.437677 muxtools-0.0.6/muxtools/misc/
--rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.6/muxtools/misc/__init__.py
--rw-rw-rw-   0        0        0     7596 2023-06-04 11:54:07.000000 muxtools-0.0.6/muxtools/misc/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.441181 muxtools-0.0.6/muxtools/muxing/
--rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/muxing/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-06-06 22:31:04.000000 muxtools-0.0.6/muxtools/muxing/mux.py
--rw-rw-rw-   0        0        0     4452 2023-06-05 21:11:08.000000 muxtools-0.0.6/muxtools/muxing/muxfiles.py
--rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/muxing/tmdb.py
--rw-rw-rw-   0        0        0     7136 2023-06-09 14:58:00.000000 muxtools-0.0.6/muxtools/muxing/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.444638 muxtools-0.0.6/muxtools/subtitle/
--rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/subtitle/__init__.py
--rw-rw-rw-   0        0        0     2578 2023-06-07 23:13:50.000000 muxtools-0.0.6/muxtools/subtitle/font.py
--rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/subtitle/styles.py
--rw-rw-rw-   0        0        0    20827 2023-06-04 13:49:24.000000 muxtools-0.0.6/muxtools/subtitle/sub.py
--rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/subtitle/subutils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.453150 muxtools-0.0.6/muxtools/utils/
--rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/convert.py
--rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.6/muxtools/utils/download.py
--rw-rw-rw-   0        0        0     1468 2023-06-04 13:18:33.000000 muxtools-0.0.6/muxtools/utils/env.py
--rw-rw-rw-   0        0        0     5383 2023-06-05 20:41:17.000000 muxtools-0.0.6/muxtools/utils/files.py
--rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/format.py
--rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/glob.py
--rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/utils/log.py
--rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.6/muxtools/utils/parsing.py
--rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.6/muxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.431549 muxtools-0.0.6/muxtools.egg-info/
--rw-rw-rw-   0        0        0     1619 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1335 2023-06-09 15:25:29.000000 muxtools-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 15:26:25.454151 muxtools-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.783994 muxtools-0.0.7/
+-rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1619 2023-06-24 22:29:31.783994 muxtools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-08 16:58:55.000000 muxtools-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.655965 muxtools-0.0.7/muxtools/
+-rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.692973 muxtools-0.0.7/muxtools/audio/
+-rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.7/muxtools/audio/__init__.py
+-rw-rw-rw-   0        0        0    10159 2023-06-20 14:25:16.000000 muxtools-0.0.7/muxtools/audio/audioutils.py
+-rw-rw-rw-   0        0        0    14849 2023-06-18 10:30:40.000000 muxtools-0.0.7/muxtools/audio/encoders.py
+-rw-rw-rw-   0        0        0    16812 2023-06-20 17:04:41.000000 muxtools-0.0.7/muxtools/audio/extractors.py
+-rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.7/muxtools/audio/memecoders.py
+-rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.7/muxtools/audio/tools.py
+-rw-rw-rw-   0        0        0     7674 2023-06-24 00:38:47.000000 muxtools-0.0.7/muxtools/cli.py
+-rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.7/muxtools/functions.py
+-rw-rw-rw-   0        0        0     4849 2023-06-14 19:12:56.000000 muxtools-0.0.7/muxtools/main.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.700975 muxtools-0.0.7/muxtools/misc/
+-rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.7/muxtools/misc/__init__.py
+-rw-rw-rw-   0        0        0     9586 2023-06-18 11:36:50.000000 muxtools-0.0.7/muxtools/misc/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.721979 muxtools-0.0.7/muxtools/muxing/
+-rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/muxing/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-06-18 09:43:06.000000 muxtools-0.0.7/muxtools/muxing/mux.py
+-rw-rw-rw-   0        0        0     4452 2023-06-18 10:30:26.000000 muxtools-0.0.7/muxtools/muxing/muxfiles.py
+-rw-rw-rw-   0        0        0     6371 2023-06-09 19:34:03.000000 muxtools-0.0.7/muxtools/muxing/tmdb.py
+-rw-rw-rw-   0        0        0     7136 2023-06-09 14:58:00.000000 muxtools-0.0.7/muxtools/muxing/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.741984 muxtools-0.0.7/muxtools/subtitle/
+-rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/subtitle/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-06-18 12:00:44.000000 muxtools-0.0.7/muxtools/subtitle/font.py
+-rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.7/muxtools/subtitle/styles.py
+-rw-rw-rw-   0        0        0    22179 2023-06-24 21:08:56.000000 muxtools-0.0.7/muxtools/subtitle/sub.py
+-rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.7/muxtools/subtitle/subutils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.782994 muxtools-0.0.7/muxtools/utils/
+-rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     4103 2023-06-24 21:10:24.000000 muxtools-0.0.7/muxtools/utils/convert.py
+-rw-rw-rw-   0        0        0     4285 2023-06-24 00:48:20.000000 muxtools-0.0.7/muxtools/utils/download.py
+-rw-rw-rw-   0        0        0     1468 2023-06-04 13:18:33.000000 muxtools-0.0.7/muxtools/utils/env.py
+-rw-rw-rw-   0        0        0     5383 2023-06-05 20:41:17.000000 muxtools-0.0.7/muxtools/utils/files.py
+-rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/utils/format.py
+-rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.7/muxtools/utils/glob.py
+-rw-rw-rw-   0        0        0     1731 2023-06-20 14:58:08.000000 muxtools-0.0.7/muxtools/utils/log.py
+-rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.7/muxtools/utils/parsing.py
+-rw-rw-rw-   0        0        0     3402 2023-06-18 10:28:24.000000 muxtools-0.0.7/muxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:29:31.666967 muxtools-0.0.7/muxtools.egg-info/
+-rw-rw-rw-   0        0        0     1619 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 22:29:31.000000 muxtools-0.0.7/muxtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1335 2023-06-24 22:11:09.000000 muxtools-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 22:29:31.783994 muxtools-0.0.7/setup.cfg
```

### Comparing `muxtools-0.0.6/LICENSE` & `muxtools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/PKG-INFO` & `muxtools-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.6/README.md` & `muxtools-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/__init__.py` & `muxtools-0.0.7/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/audio/audioutils.py` & `muxtools-0.0.7/muxtools/audio/audioutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import re
 import subprocess
-from shutil import rmtree
 from pymediainfo import Track
-from functools import cmp_to_key
 from pymediainfo import MediaInfo
 
 from ..utils.files import make_output
 from ..muxing.muxfiles import AudioFile
 from ..utils.log import debug, warn, error
 from ..utils.download import get_executable
 from ..utils.env import get_temp_workdir, run_commandline
@@ -72,16 +70,16 @@
     form = trackinfo.format.lower()
     if input.is_lossy():
         warn(f"It's strongly recommended to not reencode lossy audio! ({trackinfo.format})", caller, 5)
 
     if form == "wave" or container.format.lower() == "wave":
         if not (trackinfo.bit_depth > 16 and dither):
             return input
-    if valid_type == ValidInputType.AIFF_OR_FLAC:
-        valid_type = ValidInputType.AIFF
+    if valid_type == ValidInputType.AIFF_OR_FLAC or ValidInputType.W64_OR_FLAC:
+        valid_type = ValidInputType.AIFF if valid_type == ValidInputType.AIFF_OR_FLAC else ValidInputType.W64
         if (form == "flac" or container.format.lower() == "flac") and not (trackinfo.bit_depth > 16 and dither):
             return input
 
     if valid_type == ValidInputType.FLAC:
         return get_flac(input)
     else:
         return get_pcm(input)
@@ -200,28 +198,30 @@
 
 def has_libFDK() -> bool:
     """
     Returns if whatever installation of ffmpeg being used has been compiled with libFDK
     """
     exe = get_executable("ffmpeg")
     p = subprocess.run([exe, "-encoders"], capture_output=True, text=True)
-    for line in p.stderr.splitlines():
+    output = p.stderr + p.stdout
+    for line in output.splitlines():
         if "libfdk_aac" in line.lower():
             return True
     return False
 
 
 def has_libFLAC() -> bool:
     """
     Returns if whatever installation of qaac being used has libFLAC
     and as such can accept flac input
     """
     exe = get_executable("qaac")
     p = subprocess.run([exe, "--check"], capture_output=True, text=True)
-    for line in p.stderr.splitlines():
+    output = p.stderr + p.stdout
+    for line in output.splitlines():
         if "libflac" in line.lower():
             return True
     return False
 
 
 def qaac_compatcheck():
     if not has_libFLAC():
```

### Comparing `muxtools-0.0.6/muxtools/audio/encoders.py` & `muxtools-0.0.7/muxtools/audio/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
         if not isinstance(input, AudioFile):
             input = AudioFile.from_file(input, self)
         flaccl = get_executable("flac")
         output = make_output(input.file, "flac", "libflac", self.output)
         source = ensure_valid_in(
-            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.W64_OR_FLAC, supports_pipe=False
         )
         debug(f"Encoding '{input.file.stem}' to FLAC using libFLAC...", self)
 
         args = [flaccl, f"-{self.compression_level}", str(source.file.resolve()) if isinstance(source, AudioFile) else "-"]
         args.extend(["-o", str(output)])
         if self.append:
             args.extend(splitcommand(self.append))
```

### Comparing `muxtools-0.0.6/muxtools/audio/extractors.py` & `muxtools-0.0.7/muxtools/audio/extractors.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/audio/memecoders.py` & `muxtools-0.0.7/muxtools/audio/memecoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/audio/tools.py` & `muxtools-0.0.7/muxtools/audio/tools.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/cli.py` & `muxtools-0.0.7/muxtools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from .utils.download import unpack_all
 from .utils.env import get_temp_workdir
 from .utils.files import clean_temp_files
 
 CONF = "([green bold]Y[/] | [red]n[/])"
 
 LINKS = [
-    "https://www.rarewares.org/files/lossless/flac_dll-1.4.2-x86-nonXP.zip",
-    "https://github.com/xiph/flac/releases/download/1.4.2/flac-1.4.2-win.zip",
+    "https://www.rarewares.org/files/lossless/flac_dll-1.4.3-x86.zip",
+    "https://github.com/xiph/flac/releases/download/1.4.3/flac-1.4.3-win.zip",
     "https://github.com/dbry/WavPack/releases/download/5.6.0/wavpack-5.6.0-dll.zip",
     "https://github.com/libsndfile/libsndfile/releases/download/1.2.0/libsndfile-1.2.0-win64.zip",
     "https://files.catbox.moe/bkj665.7z",  # Sourced from https://github.com/AnimMouse/QTFiles/ but the file there can't be extracted by py7zr
 ]
 
 
 def install_libraries():
```

### Comparing `muxtools-0.0.6/muxtools/functions.py` & `muxtools-0.0.7/muxtools/functions.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/main.py` & `muxtools-0.0.7/muxtools/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,114 @@
-import os
-import json
-from typing import Self
-from pathlib import Path
-from dataclasses import dataclass
-from configparser import ConfigParser
-
-from .utils.log import error
-
-
-@dataclass
-class Setup:
-    """
-    Something like an environment used for a lot of functions in this package.
-    Mostly used for muxing and data locations (work directory and what not).
-
-    If you want to change any of the variables AFTER initialization make sure to use the `Setup.edit` function to do so.
-    Read its docstring to get why.
-
-    :param episode:                 Episode identifier used for workdir and muxing
-    :param config_file:             An ini file where the config will be loaded from.
-                                    You can disable this by leaving it empty or setting None.
-                                    Make sure you set the relevant variables in this constructor in that case.
-                                    You can also set other, technically, not existing variables in there and access them from python after.
-
-    :param bdmv_dir:                Convenience path for sources and what not.
-    :param show_name:               The name of the show. Used for the $show$ placeholder in muxing.
-    :param allow_binary_download:   This will download any executables needed for doing what you're requesting to do.
-                                    For example x265, opusenc, etc.
-    :param clean_work_dirs:         Cleanup the work directories after muxing. Might be useful if you're muxing a ton of stuff.
-    :param out_dir:                 The folder the muxed files will go into.
-    :param out_name:                The naming template applied to the muxed files.
-    :param mkv_title_naming:        The naming template applied to the mkv title.
-    :param work_dir:                In case you want to set a custom work directory for all the temp files.
-    :param debug:                   Enable or Disable various, possibly interesting, debug output of all functions in this package.
-    """
-
-    episode: str = "01"
-    config_file: str = "config.ini"
-
-    bdmv_dir: str = "BDMV"
-    show_name: str = "Nice Series"
-    allow_binary_download: bool = True
-    clean_work_dirs: bool = False
-    out_dir: str = "premux"
-    out_name: str = "$show$ - $ep$ (premux)"
-    mkv_title_naming: str = r"$show$ - $ep$"
-    work_dir: str | None = None
-    debug: bool = True
-
-    def __post_init__(self):
-        if self.config_file:
-            config = ConfigParser()
-            config_name = self.config_file
-
-            if not os.path.exists(config_name):
-                config["SETUP"] = {
-                    "bdmv_dir": self.bdmv_dir,
-                    "show_name": self.show_name,
-                    "allow_binary_download": self.allow_binary_download,
-                    "clean_work_dirs": self.clean_work_dirs,
-                    "out_dir": self.out_dir,
-                    "out_name": self.out_name,
-                    "mkv_title_naming": self.mkv_title_naming,
-                    "debug": self.debug,
-                }
-
-                with open(config_name, "w") as config_file:
-                    config.write(config_file)
-
-                raise error(f"Template config created at {Path(config_name).resolve()}.\nPlease set it up!")
-
-            config.read(config_name)
-            settings = config["SETUP"]
-
-            valid_bools = ["true", "1", "t", "y", "yes"]
-            for key in settings:
-                if hasattr(self, key) and isinstance(getattr(self, key), bool):
-                    setattr(self, key, True if settings[key].lower() in valid_bools else False)
-                else:
-                    setattr(self, key, settings[key])
-
-        if not self.work_dir:
-            self.work_dir = Path(os.getcwd(), "_workdir", self.episode)
-
-        self.work_dir.mkdir(parents=True, exist_ok=True)
-        self.work_dir = str(self.work_dir)
-
-        from .utils.env import save_setup
-
-        save_setup(self)
-
-    def edit(self, attr: str, value: any) -> Self:
-        """
-        Sets a variable inside of Setup and saves it to the environment variables.
-        You should use this to apply any changes because other functions will not make use of them otherwise!
-
-        :param attr:        The name of the variable/attribute you want to change
-        :param value:       The value this variable/attribute will have.
-        """
-        setattr(self, attr, value)
-
-        from .utils.env import save_setup
-
-        save_setup(self)
-        return self
-
-    def _toJson(self) -> str:
-        return json.dumps(self.__dict__)
+from __future__ import annotations
+
+import os
+import json
+from typing import TypeVar
+from pathlib import Path
+from dataclasses import dataclass
+from configparser import ConfigParser
+
+from .utils.log import error
+
+@dataclass
+class Setup:
+    """
+    Something like an environment used for a lot of functions in this package.
+    Mostly used for muxing and data locations (work directory and what not).
+
+    If you want to change any of the variables AFTER initialization make sure to use the `Setup.edit` function to do so.
+    Read its docstring to get why.
+
+    :param episode:                 Episode identifier used for workdir and muxing
+    :param config_file:             An ini file where the config will be loaded from.
+                                    You can disable this by leaving it empty or setting None.
+                                    Make sure you set the relevant variables in this constructor in that case.
+                                    You can also set other, technically, not existing variables in there and access them from python after.
+
+    :param bdmv_dir:                Convenience path for sources and what not.
+    :param show_name:               The name of the show. Used for the $show$ placeholder in muxing.
+    :param allow_binary_download:   This will download any executables needed for doing what you're requesting to do.
+                                    For example x265, opusenc, etc.
+    :param clean_work_dirs:         Cleanup the work directories after muxing. Might be useful if you're muxing a ton of stuff.
+    :param out_dir:                 The folder the muxed files will go into.
+    :param out_name:                The naming template applied to the muxed files.
+    :param mkv_title_naming:        The naming template applied to the mkv title.
+    :param work_dir:                In case you want to set a custom work directory for all the temp files.
+    :param debug:                   Enable or Disable various, possibly interesting, debug output of all functions in this package.
+    """
+
+    episode: str = "01"
+    config_file: str = "config.ini"
+
+    bdmv_dir: str = "BDMV"
+    show_name: str = "Nice Series"
+    allow_binary_download: bool = True
+    clean_work_dirs: bool = False
+    out_dir: str = "premux"
+    out_name: str = "$show$ - $ep$ (premux)"
+    mkv_title_naming: str = r"$show$ - $ep$"
+    work_dir: str | None = None
+    debug: bool = True
+
+    def __post_init__(self):
+        if self.config_file:
+            config = ConfigParser()
+            config_name = self.config_file
+
+            if not os.path.exists(config_name):
+                config["SETUP"] = {
+                    "bdmv_dir": self.bdmv_dir,
+                    "show_name": self.show_name,
+                    "allow_binary_download": self.allow_binary_download,
+                    "clean_work_dirs": self.clean_work_dirs,
+                    "out_dir": self.out_dir,
+                    "out_name": self.out_name,
+                    "mkv_title_naming": self.mkv_title_naming,
+                    "debug": self.debug,
+                }
+
+                with open(config_name, "w") as config_file:
+                    config.write(config_file)
+
+                raise error(f"Template config created at {Path(config_name).resolve()}.\nPlease set it up!")
+
+            config.read(config_name)
+            settings = config["SETUP"]
+
+            valid_bools = ["true", "1", "t", "y", "yes"]
+            for key in settings:
+                if hasattr(self, key) and isinstance(getattr(self, key), bool):
+                    setattr(self, key, True if settings[key].lower() in valid_bools else False)
+                else:
+                    setattr(self, key, settings[key])
+
+        if not self.work_dir:
+            self.work_dir = Path(os.getcwd(), "_workdir", self.episode)
+
+        self.work_dir = Path(self.work_dir)
+        self.work_dir.mkdir(parents=True, exist_ok=True)
+        self.work_dir = str(self.work_dir)
+
+        from .utils.env import save_setup
+
+        save_setup(self)
+
+    def edit(self: SetupSelf, attr: str, value: any) -> SetupSelf:
+        """
+        Sets a variable inside of Setup and saves it to the environment variables.
+        You should use this to apply any changes because other functions will not make use of them otherwise!
+
+        :param attr:        The name of the variable/attribute you want to change
+        :param value:       The value this variable/attribute will have.
+        """
+        setattr(self, attr, value)
+
+        from .utils.env import save_setup
+
+        save_setup(self)
+        return self
+
+    def _toJson(self) -> str:
+        return json.dumps(self.__dict__)
+
+
+SetupSelf = TypeVar('SetupSelf', bound=Setup)
```

### Comparing `muxtools-0.0.6/muxtools/misc/chapters.py` & `muxtools-0.0.7/muxtools/misc/chapters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 from datetime import timedelta
 from fractions import Fraction
 from pathlib import Path
-from typing import Self
+from typing import TypeVar
 import os
+import re
 
-
-from ..utils.log import error, info
+from ..subtitle.sub import SubFile
+from ..utils.log import error, info, warn
 from ..utils.glob import GlobSearch
 from ..utils.download import get_executable
 from ..utils.types import Chapter, PathLike
 from ..utils.parsing import parse_ogm, parse_xml
 from ..utils.files import clean_temp_files, ensure_path_exists, ensure_path
 from ..utils.env import get_temp_workdir, get_workdir, run_commandline
 from ..utils.convert import format_timedelta, frame_to_timedelta, timedelta_to_frame
@@ -53,15 +56,15 @@
                 current = list(ch)
                 current[0] = frame_to_timedelta(current[0], self.fps)
                 chapters.append(tuple(current))
             else:
                 chapters.append(ch)
         self.chapters = chapters
 
-    def trim(self, trim_start: int = 0, trim_end: int = 0, num_frames: int = 0) -> Self:
+    def trim(self: ChaptersSelf, trim_start: int = 0, trim_end: int = 0, num_frames: int = 0) -> ChaptersSelf:
         """
         Trims the chapters
         """
         if trim_start > 0:
             chapters: list[Chapter] = []
             for chapter in self.chapters:
                 if timedelta_to_frame(chapter[0]) == 0:
@@ -83,15 +86,15 @@
                 for chapter in self.chapters:
                     if timedelta_to_frame(chapter[0], self.fps) < trim_end:
                         chapters.append(chapter)
                 self.chapters = chapters
 
         return self
 
-    def set_names(self, names: list[str | None]) -> Self:
+    def set_names(self: ChaptersSelf, names: list[str | None]) -> ChaptersSelf:
         """
         Renames the chapters
 
         :param names:   List of names
         """
         old: list[str] = [chapter[1] for chapter in self.chapters]
         if len(names) > len(old):
@@ -104,15 +107,15 @@
             current = list(self.chapters[i])
             current[1] = name
             chapters.append(tuple(current))
 
         self.chapters = chapters
         return self
 
-    def add(self, chapters: Chapter | list[Chapter], index: int = 0) -> Self:
+    def add(self: ChaptersSelf, chapters: Chapter | list[Chapter], index: int = 0) -> ChaptersSelf:
         """
         Adds a chapter at the specified index
         """
         if isinstance(chapters, tuple):
             chapters = [chapters]
         else:
             chapters = chapters
@@ -176,17 +179,57 @@
                     f"CHAPTER{i:02d}={format_timedelta(chapter[0])}\nCHAPTER{i:02d}NAME=" f'{chapter[1] if chapter[1] else ""}\n'
                     for i, chapter in enumerate(self.chapters)
                 ]
             )
         return out_file
 
     @staticmethod
+    def from_sub(file: PathLike | SubFile, fps: Fraction = Fraction(24000, 1001), _print: bool = True, encoding: str = "utf_8_sig") -> "Chapters":
+        """
+        Extract chapters from an ass file or a SubFile.
+
+        :param file:            Input ass file or SubFile
+        :param fps:             FPS passed to the chapter class for further operations
+        :param _print:          Prints the chapters after parsing
+        :param encoding:        Encoding used to read the ass file if need be
+        """
+        from ass import parse_file, Comment
+
+        if isinstance(file, SubFile):
+            doc = file._read_doc()
+        else:
+            file = ensure_path_exists(file, "Chapters")
+            with open(file if not file else file, "r", encoding=encoding) as reader:
+                doc = parse_file(reader)
+
+        pattern = re.compile(r"\{([^\\].+?)\}")
+        chapters = list[Chapter]()
+        for line in doc.events:
+            effect = str(line.effect).lower()
+            if "chapter" in effect or "chptr" in effect:
+                match = pattern.search(line.text)
+                if match:
+                    chapters.append((line.start, match.group(1)))
+                elif isinstance(line, Comment) and line.text:
+                    chapters.append((line.start, str(line.text).strip()))
+                else:
+                    warn(f"Chapter {(len(chapters) + 1):02.0f} does not have a name!", "Chapters")
+                    chapters.append((line.start, ""))
+
+        if not chapters:
+            warn(f"Could not find any chapters in subtitle!", "Chapters")
+        ch = Chapters(chapters, fps)
+        if _print and chapters:
+            ch.print()
+        return ch
+
+    @staticmethod
     def from_mkv(file: PathLike, fps: Fraction = Fraction(24000, 1001), _print: bool = True, quiet: bool = True) -> "Chapters":
         """
-        Extract subtitle from mkv.
+        Extract chapters from mkv.
 
         :param file:            Input mkv file
         :param fps:             FPS passed to the chapter class for further operations
         :param _print:          Prints the chapters after parsing
         """
         caller = "Chapters.from_mkv"
         file = ensure_path_exists(file, caller)
@@ -195,7 +238,10 @@
         out = Path(get_temp_workdir(), f"{file.stem}_chapters.txt")
         args = [mkvextract, str(file), "chapters", "-s", str(out)]
         if run_commandline(args, quiet):
             raise error("Failed to extract chapters!", caller)
         chapters = Chapters(out, fps, _print)
         clean_temp_files()
         return chapters
+
+
+ChaptersSelf = TypeVar("ChaptersSelf", bound=Chapters)
```

### Comparing `muxtools-0.0.6/muxtools/muxing/mux.py` & `muxtools-0.0.7/muxtools/muxing/mux.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,29 @@
         elif isinstance(track, MuxingFile):
             if not isinstance(track, FontFile):
                 warn("It's strongly recommended to pass tracks to ensure naming and tagging instead of MuxingFiles directly!", "Mux", 1)
             track = track.to_track()
             args.extend(splitcommand(track.mkvmerge_args()))
             continue
         elif isinstance(track, Chapters):
+            if not track.chapters:
+                warn("Chapters are None or empty!", "Mux")
+                continue
+
             args.extend(["--chapters", track.to_file()])
             continue
         elif isinstance(track, Path) or isinstance(track, str) or isinstance(track, GlobSearch):
             # Failsave for if someone passes Chapters().to_file() or a txt/xml file
             track = ensure_path_exists(track, "Mux")
             if track.suffix.lower() in [".txt", ".xml"]:
                 args.extend(["--chapters", track.resolve()])
                 continue
-
+        elif track is None:
+            continue
+        
         raise error("Only _track, MuxingFiles or Chapters types are supported as muxing input!", "Mux")
 
     if mkvtitle:
         args.extend(["--title", mkvtitle])
 
     debug("Running the mux...", "Mux")
     if run_commandline(args, quiet) > 1:
```

### Comparing `muxtools-0.0.6/muxtools/muxing/muxfiles.py` & `muxtools-0.0.7/muxtools/muxing/muxfiles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/muxing/tmdb.py` & `muxtools-0.0.7/muxtools/muxing/tmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,31 +49,31 @@
                             Be aware that some metadata might just not exist in your requested language. Check beforehand.
 
     :param write_title:     Writes the episode title to the `DESCRIPTION` mkv tag if True
     :param write_ids:       Writes the IDs (IMDB, TVDB, TMDB) to their respective mkv tags if True
     :param write_date:      Writes the episode release date to the `DATE_RELEASED` mkv tag if True
     :param write_cover:     Download episode thumbnail from TMDB to use as cover art attachment for the MKV.
     :param write_summary:   Writes the series summary/synopsis to the `SUMMARY` mkv tag if True
-    :param write_synposis:  Writes the individual episode synopsis to the `SYNOPSIS` mkv tag if True
+    :param write_synopsis:  Writes the individual episode synopsis to the `SYNOPSIS` mkv tag if True
     """
 
     id: int
     season: int = 1
     movie: bool = False
     language: str = "en-US"
 
     write_ids: bool = True
     write_date: bool = True
     write_title: bool = False
     write_cover: bool = False
     write_summary: bool = False
-    write_synposis: bool = False
+    write_synopsis: bool = False
 
     def needs_xml(self) -> bool:
-        return self.write_ids or self.write_date or self.write_title or self.write_summary or self.write_synposis
+        return self.write_ids or self.write_date or self.write_title or self.write_summary or self.write_synopsis
 
     def get_media_meta(self) -> MediaMetadata:
         url = f"{BASE_URL}/{'movie' if self.movie else 'tv'}/{self.id}?language={self.language}"
         headers = {"accept": "application/json", "Authorization": f"Bearer {API_KEY}"}
         response = requests.get(url, headers=headers)
 
         if response.status_code > 202:
@@ -137,15 +137,15 @@
             if self.movie:
                 if media.release_date:
                     tags.update(DATE_RELEASED=media.release_date)
             else:
                 tags.update(DATE_RELEASED=episode.release_date)
         if self.write_summary:
             tags.update(SUMMARY=media.summary)
-        if self.write_synposis and not self.movie:
+        if self.write_synopsis and not self.movie:
             tags.update(SYNOPSIS=episode.synopsis)
 
         outfile = make_output("tags", "xml")
         main = ET.Element("Tags")
         tag = ET.SubElement(main, "Tag")
         target = ET.SubElement(tag, "Targets")
         targettype = ET.SubElement(target, "TargetTypeValue")
```

### Comparing `muxtools-0.0.6/muxtools/muxing/tracks.py` & `muxtools-0.0.7/muxtools/muxing/tracks.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/subtitle/font.py` & `muxtools-0.0.7/muxtools/subtitle/font.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-import logging
 import os
 import shutil
-
-from ..utils.env import get_workdir
-
-logging.getLogger("matplotlib").setLevel(logging.CRITICAL)
-logging.getLogger("matplotlib.font_manager").setLevel(logging.CRITICAL)
-
-import matplotlib
-
-matplotlib.use("agg", force=True)
-
+import logging
 from pathlib import Path
 
-
-from ..utils.log import debug, warn
 from .sub import SubFile, FontFile
+from ..utils.env import get_workdir
+from ..utils.log import debug, warn
 
 
 def _weight_to_name(weight: int) -> str:
     match weight:
         case 100:
             return "Thin"
         case 200:
```

### Comparing `muxtools-0.0.6/muxtools/subtitle/styles.py` & `muxtools-0.0.7/muxtools/subtitle/styles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/subtitle/sub.py` & `muxtools-0.0.7/muxtools/subtitle/sub.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,501 +1,519 @@
-from ass import Document, Comment, Dialogue, Style, parse as parseDoc
-from dataclasses import dataclass
-from datetime import timedelta
-from fractions import Fraction
-from pathlib import Path
-from typing import Self
-import shutil
-import json
-import re
-import os
-
-from .subutils import dummy_video, has_arch_resampler
-from ..utils.glob import GlobSearch
-from ..utils.download import get_executable
-from ..utils.types import PathLike, TrackType
-from ..utils.log import debug, error, info, warn
-from ..utils.convert import frame_to_timedelta, timedelta_to_frame
-from ..utils.env import get_temp_workdir, get_workdir, run_commandline
-from ..utils.files import ensure_path_exists, get_absolute_track, make_output, clean_temp_files, uniquify_path
-from ..muxing.muxfiles import MuxingFile
-
-__all__ = ["FontFile", "SubFile", "DEFAULT_DIALOGUE_STYLES"]
-
-
-DEFAULT_DIALOGUE_STYLES = ["default", "main", "alt", "overlap", "flashback", "top", "italics"]
-
-
-@dataclass
-class FontFile(MuxingFile):
-    pass
-
-
-@dataclass
-class SubFile(MuxingFile):
-    """
-    Utility class representing a subtitle file with various functions to run on.
-
-    :param file:            Can be a string, Path object or GlobSearch.
-                            If the GlobSearch returns multiple results or if a list was passed it will merge them.
-
-    :param container_delay: Set a container delay used in the muxing process later.
-    :param source:          The file this sub originates from, will be set by the constructor.
-    :param encoding:        Encoding used for reading and writing the subtitle files.
-    """
-
-    encoding = "utf_8_sig"
-
-    def __post_init__(self):
-        if isinstance(self.file, GlobSearch):
-            self.file = self.file.paths
-
-        if isinstance(self.file, list) and len(self.file) > 1:
-            debug("Merging sub files...", self)
-            docs: list[Document] = []
-            for f in self.file:
-                f = ensure_path_exists(f, self)
-                with open(f, "r", encoding=self.encoding) as read:
-                    docs.append(parseDoc(read))
-
-            main = docs[0]
-            existing_styles = [style.name for style in (main.styles)]
-            docs.remove(main)
-
-            for doc in docs:
-                main.events.extend(doc.events)
-                for style in doc.styles:
-                    if style.name.casefold() in [s.casefold() for s in existing_styles]:
-                        warn(f"Ignoring style '{style.name}' due to preexisting style of the same name.", self)
-                        continue
-                    main.styles.append(style)
-
-            self.source = self.file[0]
-            out = make_output(self.file[0], "ass", "merged")
-            with open(out, "w", encoding=self.encoding) as writer:
-                main.dump_file(writer)
-
-            self.file = out
-            debug("Done")
-        else:
-            self.file = ensure_path_exists(self.file, self)
-            self.source = self.file
-            if not os.path.samefile(self.file.parent, get_workdir()):
-                out = make_output(self.file, "ass", "vof")
-                with open(out, "w", encoding=self.encoding) as writer:
-                    self._read_doc().dump_file(writer)
-                self.file = out
-
-    def _read_doc(self, file: PathLike | None = None) -> Document:
-        with open(self.file if not file else file, "r", encoding=self.encoding) as reader:
-            return parseDoc(reader)
-
-    def __update_doc(self, doc: Document):
-        with open(self.file, "w", encoding=self.encoding) as writer:
-            doc.dump_file(writer)
-
-    def clean_styles(self) -> Self:
-        """
-        Deletes unused styles from the document
-        """
-        doc = self._read_doc()
-        used_styles = {line.style for line in doc.events if line.TYPE == "Dialogue"}
-        doc.styles = [style for style in doc.styles if style.name in used_styles]
-        self.__update_doc(doc)
-        return self
-
-    def autoswapper(self, allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES, print_swaps: bool = False) -> Self:
-        """
-        autoswapper does the swapping.
-        Too lazy to explain
-
-        :param allowed_styles:      List of allowed styles to do the swapping on
-                                    Will run on every line if passed `None`
-        :param print_swaps:         Prints the swaps
-
-        :return:                    This SubTrack
-        """
-        doc = self._read_doc()
-
-        events = []
-
-        for i, line in enumerate(doc.events):
-            if not allowed_styles or line.style.lower() in (style.lower() for style in allowed_styles):
-                to_swap: dict = {}
-                # {*}This will be replaced{*With this}
-                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\*([^}*]+)\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(2)}{{*{match.group(1)}}}"})
-
-                # This sentence is no longer{** incomplete}
-                for match in re.finditer(re.compile(r"\{\*\*([^}]+)\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(1)}{{*}}"})
-
-                # This sentence is no longer{*} incomplete{*}
-                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\* *\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{**{match.group(1)}}}"})
-                # print(to_swap)
-                for key, val in to_swap.items():
-                    if print_swaps:
-                        info(f'autoswapper: Swapped "{key}" for "{val}" on line {i}', self)
-                    line.text = line.text.replace(key, val)
-
-            if line.effect.strip() == "***" or line.name.strip() == "***":
-                if isinstance(line, Comment):
-                    line.TYPE = "Dialogue"
-                elif isinstance(line, Dialogue):
-                    line.TYPE = "Comment"
-
-            events.append(line)
-
-        doc.events = events
-        self.__update_doc(doc)
-        return self
-
-    def unfuck_cr(
-        self,
-        default_style: str = "Default",
-        keep_flashback: bool = True,
-        dialogue_styles: list[str] | None = ["main", "default", "narrator", "narration"],
-        top_styles: list[str] | None = ["top"],
-        italics_styles: list[str] | None = ["italics", "internal"],
-    ) -> Self:
-        """
-        Removes any top and italics styles and replaces them with tags.
-
-        :param default_style:       The default style that everything will be set to
-        :param keep_flashback:      If not it will set the flashback styles to default_style
-        :param dialogue_styles:     Styles that will be set to default_style
-        :param top_styles:          Styles that will be set to default_style and an8 added to tags
-        :param italics_styles:      Styles that will be set to default_style and i1 added to tags
-        """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            add_italics_tag = False
-            if italics_styles:
-                for s in italics_styles:
-                    if s.casefold() in line.style.casefold():
-                        add_italics_tag = True
-                        if "flashback" in line.style.lower():
-                            line.style = default_style if not keep_flashback else "Flashback"
-                        else:
-                            line.style = default_style
-                        break
-            add_top_tag = False
-            if top_styles:
-                for s in top_styles:
-                    if s.casefold() in line.style.casefold():
-                        add_top_tag = True
-                        if "flashback" in line.style.lower():
-                            line.style = default_style if not keep_flashback else "Flashback"
-                        else:
-                            line.style = default_style
-                        break
-            if add_italics_tag and add_top_tag:
-                line.text = R"{\i1\an8}" + line.text
-            elif add_italics_tag:
-                line.text = R"{\i1}" + line.text
-            elif add_top_tag:
-                line.text = R"{\an8}" + line.text
-
-            if not keep_flashback:
-                if "flashback" in line.style.lower():
-                    line.style = default_style
-            else:
-                if line.style == "flashback":
-                    line.style = "Flashback"
-            if dialogue_styles:
-                for s in dialogue_styles:
-                    if s.casefold() in line.style.casefold():
-                        line.style = default_style
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self.clean_styles()
-
-    def shift_0(self, fps: Fraction = Fraction(24000, 1001), allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES) -> Self:
-        """
-        Does the famous shift by 0 frames to fix frame timing issues.
-        (It's basically just converting time to frame and back)
-
-        This does not currently exactly reproduce the aegisub behaviour but it should have the same effect.
-
-        :param fps:             The fps fraction used for conversions
-        :param allowed_styles:  A list of style names this will run on. Will run on every line if None.
-        """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            if not allowed_styles or line.style.lower() in allowed_styles:
-                line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps), fps)
-                line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps), fps)
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self
-
-    def syncpoint_merge(
-        self,
-        syncpoint: str,
-        mergefile: PathLike | GlobSearch,
-        use_actor_field: bool = False,
-        use_frames: bool = False,
-        fps: Fraction = Fraction(24000, 1001),
-        override_p1: int | timedelta = None,
-        add_offset: int | timedelta = None,
-    ) -> Self:
-        """
-        Merge other sub files (Opening/Ending kfx for example) with offsetting by syncpoints
-
-        :param syncpoint:           The syncpoint to be used
-        :param mergefile:           The file to be merged
-        :param use_actor_field:     Search the actor field instead of the effect field for the syncpoint
-        :param use_frames:          Uses frames to shift lines instead of direct timestamps
-        :param fps:                 The fps to go off of for the conversion
-        :param override_p1:         A manual override of the initial syncpoint
-                                    Obviously either a frame number or timedelta
-
-        :return:                    This SubTrack
-        """
-        mergefile = ensure_path_exists(mergefile, self)
-        was_merged = False
-
-        doc = self._read_doc()
-        mergedoc = self._read_doc(mergefile)
-
-        events = []
-        tomerge = []
-        existing_styles = [style.name for style in doc.styles]
-
-        if isinstance(add_offset, int) and not use_frames:
-            add_offset = frame_to_timedelta(add_offset, fps)
-
-        for line in doc.events:
-            events.append(line)
-            if was_merged:
-                continue
-            field = line.name if use_actor_field else line.effect
-            if (
-                field.lower().strip() == syncpoint.lower().strip()
-                or line.text.lower().strip() == syncpoint.lower().strip()
-                or override_p1 is not None
-            ):
-                was_merged = True
-                start = line.start if override_p1 is None else override_p1
-                offset: timedelta | int = None
-                for l in mergedoc.events:
-                    lfield = l.name if use_actor_field else l.effect
-                    if lfield.lower().strip() == syncpoint.lower().strip() or l.text.lower().strip() == syncpoint.lower().strip():
-                        mergedoc.events.remove(l)
-                        if use_frames:
-                            offset = timedelta_to_frame(start - l.start, fps)
-                        else:
-                            offset = start - l.start
-
-                        if add_offset:
-                            offset += add_offset
-                        break
-
-                for l in sorted(mergedoc.events, key=lambda event: event.start):
-                    if offset is None:
-                        if use_frames:
-                            offset = timedelta_to_frame(start - l.start, fps)
-                        else:
-                            offset = start - l.start
-
-                        if add_offset:
-                            offset += add_offset
-
-                        l.start = start
-                        l.end = l.end + (frame_to_timedelta(offset, fps) if use_frames else offset)
-                    else:
-                        l.start = l.start + (frame_to_timedelta(offset, fps) if use_frames else offset)
-                        l.end = l.end + (frame_to_timedelta(offset, fps) if use_frames else offset)
-                    tomerge.append(l)
-
-        if was_merged:
-            events.extend(tomerge)
-            # Merge the styles in aswell
-            for style in mergedoc.styles:
-                if style.name in existing_styles:
-                    continue
-                doc.styles.append(style)
-
-            doc.events = events
-            self.__update_doc(doc)
-        else:
-            warn(f"Syncpoint '{syncpoint}' was not found!", self)
-
-        return self
-
-    def collect_fonts(self, use_system_fonts: bool = True, search_current_dir: bool = True, additional_fonts: list[PathLike] = []) -> list[FontFile]:
-        """
-        Collects fonts for current subtitle.
-
-        :param use_system_fonts:        Parses and checks against all installed fonts
-        :param search_current_dir:      Recursively checks the current work directory for fonts
-        :param additional_fonts:        Can be a directory or a path to a file directly (or a list of either)
-
-        :return:                        A list of FontFile objects
-        """
-
-        if not isinstance(additional_fonts, list):
-            additional_fonts = [additional_fonts]
-
-        if search_current_dir:
-            additional_fonts.append(os.getcwd())
-
-        resolved_paths: list[Path] = []
-
-        for f in additional_fonts:
-            f = ensure_path_exists(f, self, True)
-            if f.is_dir():
-                resolved_paths.extend([file for file in f.rglob("*.ttf")])
-                resolved_paths.extend([file for file in f.rglob("*.otf")])
-            else:
-                if f.suffix.lower() not in ["ttf", "otf"]:
-                    raise error(f"'{f.name}' is not a font!", self)
-                resolved_paths.append(f)
-        from .font import collect_fonts as collect
-
-        debug(f"Collecting fonts for '{self.file.stem}'...", self)
-
-        return collect(self, use_system_fonts, resolved_paths)
-
-    def restyle(self, styles: Style | list[Style], clean_after: bool = True, delete_existing: bool = False) -> Self:
-        """
-        Add (and replace existing) styles to the subtitle file.
-
-        :param styles:          Either a single or a list of ass Styles
-        :param clean_after:     Clean unused styles after
-        :param delete_existing: Delete all existing styles before adding new ones
-        """
-        if not isinstance(styles, list):
-            styles = [styles]
-
-        styles = styles.copy()
-
-        doc = self._read_doc()
-        if delete_existing:
-            doc.styles = []
-
-        names = [style.name.casefold() for style in styles]
-        existing = [style for style in doc.styles if style.name.casefold() not in names]
-        styles.extend(existing)
-        doc.styles = styles
-
-        self.__update_doc(doc)
-        if clean_after:
-            return self.clean_styles()
-        else:
-            return self
-
-    def resample(
-        self,
-        video: PathLike | None = None,
-        src_width: int | None = None,
-        src_height: int | None = None,
-        use_arch: bool | None = None,
-        quiet: bool = True,
-    ) -> Self:
-        """
-        Resample subtitles to match the resolution of the specified video.
-
-        :param video:           Path to a video. Will resort to a 1080p dummy video if None.
-        :param src_width:       The width of the resolution the subs are currently at
-        :param src_height:      The height of the resolution the subs are currently at
-                                Both of the above params will be taken from the sub file if not given.
-                                (Assuming 640 x 360 if nothing is given in the document)
-
-        :param use_arch:        Uses arch1t3cht's perspective resampler script to fix any perspective stuff after resampling.
-                                This requires arch.Resample.moon in either of your autoload folders.
-                                None means it will use it if it can find the script. True will try to force it.
-        """
-        aegicli = get_executable("aegisub-cli", False)
-        video = dummy_video(1920, 1080) if not video else ensure_path_exists(video, self)
-        doc = self._read_doc()
-
-        if not src_width:
-            src_width = doc.info.get("PlayResX", 640)
-
-        if not src_height:
-            src_height = doc.info.get("PlayResY", 360)
-
-        if use_arch is None:
-            use_arch = has_arch_resampler()
-
-        output = Path(get_temp_workdir(), f"{self.file.stem}_resampled.ass")
-        args = [aegicli, "--video", str(video.resolve()), str(self.file.resolve()), str(output), "tool/resampleres"]
-        if run_commandline(args, quiet):
-            raise error("Failed to resample subtitles!", self)
-
-        if use_arch:
-            prevout = output
-            output = Path(get_temp_workdir(), f"{self.file.stem}_resampled_arch.ass")
-
-            # fmt: off
-            dialog_json = json.dumps({"button": 0, "values": {"srcresx": src_width, "srcresy": src_height, "centerorg": "false"}})
-            args = [aegicli, "--video", str(video.resolve()), "--dialog", dialog_json, "--automation", "arch.Resample.moon", str(prevout), str(output), "Resample Perspective"]
-            # fmt: on
-            if run_commandline(args, quiet):
-                raise error("Failed to resample perspective of subtitles!", self)
-
-        self.file.unlink(True)
-        self.file = shutil.copy(output, self.file)
-        clean_temp_files()
-        return self
-
-    def separate_signs(self, styles: list[str] = DEFAULT_DIALOGUE_STYLES) -> Self:
-        """
-        Basically deletes lines that have any of the passed styles.
-
-        :param styles:      List of style names to get rid of
-        """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            skip = False
-            for style in styles:
-                if str(line.style).strip().casefold() == style.strip().casefold():
-                    skip = True
-                    break
-
-            if skip:
-                continue
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self.clean_styles()
-
-    def copy(self) -> "SubFile":
-        """
-        Creates a new copy of the current SubFile object, including its file.
-        So you can run anything on the new one without impacting the other one.
-        """
-        doc = self._read_doc()
-        new_path = uniquify_path(self.file)
-        with open(new_path, "w", encoding=self.encoding) as writer:
-            doc.dump_file(writer)
-
-        return SubFile(new_path, self.container_delay, self.source)
-
-    @staticmethod
-    def from_mkv(file: PathLike, track: int = 0, preserve_delay: bool = False, quiet: bool = True) -> "SubFile":
-        """
-        Extract subtitle from mkv.
-
-        :param file:            Input mkv file
-        :param track:           Relative track number
-        :param preserve_delay:  Preserve existing container delay
-        """
-        caller = "SubFile.from_mkv"
-        file = ensure_path_exists(file, caller)
-        track = get_absolute_track(file, track, TrackType.SUB, caller)
-        if track.format != "ASS":
-            raise error("The selected track is not an ASS subtitle.", caller)
-
-        mkvextract = get_executable("mkvextract")
-        out = Path(get_workdir(), f"{file.stem}_{track.track_id}.ass")
-        args = [mkvextract, str(file), "tracks", f"{track.track_id}:{str(out)}"]
-        if run_commandline(args, quiet):
-            raise error("Failed to extract subtitle!", caller)
-        return SubFile(out, 0 if not preserve_delay else getattr(track, "delay_relative_to_video", 0))
+from __future__ import annotations
+
+from ass import Document, Comment, Dialogue, Style, parse as parseDoc
+from dataclasses import dataclass
+from datetime import timedelta
+from fractions import Fraction
+from pathlib import Path
+from typing import TypeVar
+import shutil
+import json
+import re
+import os
+
+from .subutils import dummy_video, has_arch_resampler
+from ..utils.glob import GlobSearch
+from ..utils.download import get_executable
+from ..utils.types import PathLike, TrackType
+from ..utils.log import debug, error, info, warn
+from ..utils.convert import frame_to_timedelta, timedelta_to_frame
+from ..utils.env import get_temp_workdir, get_workdir, run_commandline
+from ..utils.files import ensure_path_exists, get_absolute_track, make_output, clean_temp_files, uniquify_path
+from ..muxing.muxfiles import MuxingFile
+
+__all__ = ["FontFile", "SubFile", "DEFAULT_DIALOGUE_STYLES"]
+
+
+DEFAULT_DIALOGUE_STYLES = ["default", "main", "alt", "overlap", "flashback", "top", "italics"]
+
+
+@dataclass
+class FontFile(MuxingFile):
+    pass
+
+
+@dataclass
+class SubFile(MuxingFile):
+    """
+    Utility class representing a subtitle file with various functions to run on.
+
+    :param file:            Can be a string, Path object or GlobSearch.
+                            If the GlobSearch returns multiple results or if a list was passed it will merge them.
+
+    :param container_delay: Set a container delay used in the muxing process later.
+    :param source:          The file this sub originates from, will be set by the constructor.
+    :param encoding:        Encoding used for reading and writing the subtitle files.
+    """
+
+    encoding = "utf_8_sig"
+
+    def __post_init__(self):
+        if isinstance(self.file, GlobSearch):
+            self.file = self.file.paths
+
+        if isinstance(self.file, list) and len(self.file) > 1:
+            debug("Merging sub files...", self)
+            docs: list[Document] = []
+            for f in self.file:
+                f = ensure_path_exists(f, self)
+                with open(f, "r", encoding=self.encoding) as read:
+                    docs.append(parseDoc(read))
+
+            main = docs[0]
+            existing_styles = [style.name for style in (main.styles)]
+            docs.remove(main)
+
+            for doc in docs:
+                main.events.extend(doc.events)
+                for style in doc.styles:
+                    if style.name.casefold() in [s.casefold() for s in existing_styles]:
+                        warn(f"Ignoring style '{style.name}' due to preexisting style of the same name.", self)
+                        continue
+                    main.styles.append(style)
+
+            self.source = self.file[0]
+            out = make_output(self.file[0], "ass", "merged")
+            with open(out, "w", encoding=self.encoding) as writer:
+                main.dump_file(writer)
+
+            self.file = out
+            debug("Done")
+        else:
+            self.file = ensure_path_exists(self.file, self)
+            self.source = self.file
+            if not os.path.samefile(self.file.parent, get_workdir()):
+                out = make_output(self.file, "ass", "vof")
+                with open(out, "w", encoding=self.encoding) as writer:
+                    self._read_doc().dump_file(writer)
+                self.file = out
+
+    def _read_doc(self, file: PathLike | None = None) -> Document:
+        with open(self.file if not file else file, "r", encoding=self.encoding) as reader:
+            return parseDoc(reader)
+
+    def __update_doc(self, doc: Document):
+        with open(self.file, "w", encoding=self.encoding) as writer:
+            doc.dump_file(writer)
+
+    def clean_styles(self: SubFileSelf) -> SubFileSelf:
+        """
+        Deletes unused styles from the document
+        """
+        doc = self._read_doc()
+        used_styles = {line.style for line in doc.events if line.TYPE == "Dialogue"}
+        doc.styles = [style for style in doc.styles if style.name in used_styles]
+        self.__update_doc(doc)
+        return self
+
+    def clean_garbage(self: SubFileSelf) -> SubFileSelf:
+        """
+        Removes the "Aegisub Project Garbage" section from the file
+        """
+        doc = self._read_doc()
+        doc.sections.pop("Aegisub Project Garbage", None)
+        self.__update_doc(doc)
+        return self
+
+    def autoswapper(self: SubFileSelf, allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES, print_swaps: bool = False) -> SubFileSelf:
+        """
+        autoswapper does the swapping.
+        Too lazy to explain
+
+        :param allowed_styles:      List of allowed styles to do the swapping on
+                                    Will run on every line if passed `None`
+        :param print_swaps:         Prints the swaps
+
+        :return:                    This SubTrack
+        """
+        doc = self._read_doc()
+
+        events = []
+
+        for i, line in enumerate(doc.events):
+            if not allowed_styles or line.style.lower() in (style.lower() for style in allowed_styles):
+                to_swap: dict = {}
+                # {*}This will be replaced{*With this}
+                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\*([^}*]+)\}"), line.text):
+                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(2)}{{*{match.group(1)}}}"})
+
+                # This sentence is no longer{** incomplete}
+                for match in re.finditer(re.compile(r"\{\*\*([^}]+)\}"), line.text):
+                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(1)}{{*}}"})
+
+                # This sentence is no longer{*} incomplete{*}
+                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\* *\}"), line.text):
+                    to_swap.update({f"{match.group(0)}": f"{{**{match.group(1)}}}"})
+                # print(to_swap)
+                for key, val in to_swap.items():
+                    if print_swaps:
+                        info(f'autoswapper: Swapped "{key}" for "{val}" on line {i}', self)
+                    line.text = line.text.replace(key, val)
+
+            if line.effect.strip() == "***" or line.name.strip() == "***":
+                if isinstance(line, Comment):
+                    line.TYPE = "Dialogue"
+                elif isinstance(line, Dialogue):
+                    line.TYPE = "Comment"
+
+            events.append(line)
+
+        doc.events = events
+        self.__update_doc(doc)
+        return self
+
+    def unfuck_cr(
+        self: SubFileSelf,
+        default_style: str = "Default",
+        keep_flashback: bool = True,
+        dialogue_styles: list[str] | None = ["main", "default", "narrator", "narration"],
+        top_styles: list[str] | None = ["top"],
+        italics_styles: list[str] | None = ["italics", "internal"],
+    ) -> SubFileSelf:
+        """
+        Removes any top and italics styles and replaces them with tags.
+
+        :param default_style:       The default style that everything will be set to
+        :param keep_flashback:      If not it will set the flashback styles to default_style
+        :param dialogue_styles:     Styles that will be set to default_style
+        :param top_styles:          Styles that will be set to default_style and an8 added to tags
+        :param italics_styles:      Styles that will be set to default_style and i1 added to tags
+        """
+        doc = self._read_doc()
+        events = []
+        for line in doc.events:
+            add_italics_tag = False
+            if italics_styles:
+                for s in italics_styles:
+                    if s.casefold() in line.style.casefold():
+                        add_italics_tag = True
+                        if "flashback" in line.style.lower():
+                            line.style = default_style if not keep_flashback else "Flashback"
+                        else:
+                            line.style = default_style
+                        break
+            add_top_tag = False
+            if top_styles:
+                for s in top_styles:
+                    if s.casefold() in line.style.casefold():
+                        add_top_tag = True
+                        if "flashback" in line.style.lower():
+                            line.style = default_style if not keep_flashback else "Flashback"
+                        else:
+                            line.style = default_style
+                        break
+            if add_italics_tag and add_top_tag:
+                line.text = R"{\i1\an8}" + line.text
+            elif add_italics_tag:
+                line.text = R"{\i1}" + line.text
+            elif add_top_tag:
+                line.text = R"{\an8}" + line.text
+
+            if not keep_flashback:
+                if "flashback" in line.style.lower():
+                    line.style = default_style
+            else:
+                if line.style == "flashback":
+                    line.style = "Flashback"
+            if dialogue_styles:
+                for s in dialogue_styles:
+                    if s.casefold() in line.style.casefold():
+                        line.style = default_style
+            events.append(line)
+        doc.events = events
+        self.__update_doc(doc)
+        return self.clean_styles()
+
+    def shift_0(self: SubFileSelf, fps: Fraction = Fraction(24000, 1001), allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES) -> SubFileSelf:
+        """
+        Does the famous shift by 0 frames to fix frame timing issues.
+        (It's basically just converting time to frame and back)
+
+        This does not currently exactly reproduce the aegisub behaviour but it should have the same effect.
+
+        :param fps:             The fps fraction used for conversions
+        :param allowed_styles:  A list of style names this will run on. Will run on every line if None.
+        """
+        doc = self._read_doc()
+        events = []
+        for line in doc.events:
+            if not allowed_styles or line.style.lower() in allowed_styles:
+                line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps), fps, True)
+                line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps), fps, True)
+            events.append(line)
+        doc.events = events
+        self.__update_doc(doc)
+        return self
+
+    def syncpoint_merge(
+        self: SubFileSelf,
+        syncpoint: str,
+        mergefile: PathLike | GlobSearch,
+        use_actor_field: bool = False,
+        use_frames: bool = False,
+        fps: Fraction = Fraction(24000, 1001),
+        override_p1: int | timedelta = None,
+        add_offset: int | timedelta = None,
+    ) -> SubFileSelf:
+        """
+        Merge other sub files (Opening/Ending kfx for example) with offsetting by syncpoints
+
+        :param syncpoint:           The syncpoint to be used
+        :param mergefile:           The file to be merged
+        :param use_actor_field:     Search the actor field instead of the effect field for the syncpoint
+        :param use_frames:          Uses frames to shift lines instead of direct timestamps
+        :param fps:                 The fps to go off of for the conversion
+        :param override_p1:         A manual override of the initial syncpoint
+                                    Obviously either a frame number or timedelta
+
+        :return:                    This SubTrack
+        """
+        mergefile = ensure_path_exists(mergefile, self)
+        was_merged = False
+
+        doc = self._read_doc()
+        mergedoc = self._read_doc(mergefile)
+
+        events = []
+        tomerge = []
+        existing_styles = [style.name for style in doc.styles]
+
+        if isinstance(add_offset, int) and not use_frames:
+            add_offset = frame_to_timedelta(add_offset, fps, True)
+
+        for line in doc.events:
+            events.append(line)
+            if was_merged:
+                continue
+            field = line.name if use_actor_field else line.effect
+            if (
+                field.lower().strip() == syncpoint.lower().strip()
+                or line.text.lower().strip() == syncpoint.lower().strip()
+                or override_p1 is not None
+            ):
+                was_merged = True
+                start = line.start if override_p1 is None else override_p1
+                offset: timedelta | int = None
+                for l in mergedoc.events:
+                    lfield = l.name if use_actor_field else l.effect
+                    if lfield.lower().strip() == syncpoint.lower().strip() or l.text.lower().strip() == syncpoint.lower().strip():
+                        mergedoc.events.remove(l)
+                        if use_frames:
+                            offset = timedelta_to_frame(start - l.start, fps)
+                        else:
+                            offset = start - l.start
+
+                        if add_offset:
+                            offset += add_offset
+                        break
+
+                for l in sorted(mergedoc.events, key=lambda event: event.start):
+                    if offset is None:
+                        if use_frames:
+                            offset = timedelta_to_frame(start - l.start, fps)
+                        else:
+                            offset = start - l.start
+
+                        if add_offset:
+                            offset += add_offset
+
+                        l.start = start
+                        l.end = l.end + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
+                    else:
+                        l.start = l.start + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
+                        l.end = l.end + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
+                    tomerge.append(l)
+
+        if was_merged:
+            events.extend(tomerge)
+            # Merge the styles in aswell
+            for style in mergedoc.styles:
+                if style.name in existing_styles:
+                    continue
+                doc.styles.append(style)
+
+            doc.events = events
+            self.__update_doc(doc)
+        else:
+            warn(f"Syncpoint '{syncpoint}' was not found!", self)
+
+        return self
+
+    def collect_fonts(self, use_system_fonts: bool = True, search_current_dir: bool = True, additional_fonts: list[PathLike] = []) -> list[FontFile]:
+        """
+        Collects fonts for current subtitle.
+
+        :param use_system_fonts:        Parses and checks against all installed fonts
+        :param search_current_dir:      Recursively checks the current work directory for fonts
+        :param additional_fonts:        Can be a directory or a path to a file directly (or a list of either)
+
+        :return:                        A list of FontFile objects
+        """
+
+        if not isinstance(additional_fonts, list):
+            additional_fonts = [additional_fonts]
+
+        if search_current_dir:
+            additional_fonts.append(os.getcwd())
+
+        resolved_paths: list[Path] = []
+
+        for f in additional_fonts:
+            f = ensure_path_exists(f, self, True)
+            if f.is_dir():
+                resolved_paths.extend([file for file in f.rglob("*.ttf")])
+                resolved_paths.extend([file for file in f.rglob("*.otf")])
+            else:
+                if f.suffix.lower() not in ["ttf", "otf"]:
+                    raise error(f"'{f.name}' is not a font!", self)
+                resolved_paths.append(f)
+        from .font import collect_fonts as collect
+
+        debug(f"Collecting fonts for '{self.file.stem}'...", self)
+
+        return collect(self, use_system_fonts, resolved_paths)
+
+    def restyle(self: SubFileSelf, styles: Style | list[Style], clean_after: bool = True, delete_existing: bool = False) -> SubFileSelf:
+        """
+        Add (and replace existing) styles to the subtitle file.
+
+        :param styles:          Either a single or a list of ass Styles
+        :param clean_after:     Clean unused styles after
+        :param delete_existing: Delete all existing styles before adding new ones
+        """
+        if not isinstance(styles, list):
+            styles = [styles]
+
+        styles = styles.copy()
+
+        doc = self._read_doc()
+        if delete_existing:
+            doc.styles = []
+
+        names = [style.name.casefold() for style in styles]
+        existing = [style for style in doc.styles if style.name.casefold() not in names]
+        styles.extend(existing)
+        doc.styles = styles
+
+        self.__update_doc(doc)
+        if clean_after:
+            return self.clean_styles()
+        else:
+            return self
+
+    def resample(
+        self: SubFileSelf,
+        video: PathLike | None = None,
+        src_width: int | None = None,
+        src_height: int | None = None,
+        use_arch: bool | None = None,
+        quiet: bool = True,
+    ) -> SubFileSelf:
+        """
+        Resample subtitles to match the resolution of the specified video.
+
+        :param video:           Path to a video. Will resort to a 1080p dummy video if None.
+        :param src_width:       The width of the resolution the subs are currently at
+        :param src_height:      The height of the resolution the subs are currently at
+                                Both of the above params will be taken from the sub file if not given.
+                                (Assuming 640 x 360 if nothing is given in the document)
+
+        :param use_arch:        Uses arch1t3cht's perspective resampler script to fix any perspective stuff after resampling.
+                                This requires arch.Resample.moon in either of your autoload folders.
+                                None means it will use it if it can find the script. True will try to force it.
+        """
+        aegicli = get_executable("aegisub-cli", False)
+        video = dummy_video(1920, 1080) if not video else ensure_path_exists(video, self)
+        doc = self._read_doc()
+
+        if not src_width:
+            src_width = doc.info.get("PlayResX", 640)
+
+        if not src_height:
+            src_height = doc.info.get("PlayResY", 360)
+
+        if use_arch is None:
+            use_arch = has_arch_resampler()
+
+        output = Path(get_temp_workdir(), f"{self.file.stem}_resampled.ass")
+        args = [aegicli, "--video", str(video.resolve()), str(self.file.resolve()), str(output), "tool/resampleres"]
+        if run_commandline(args, quiet):
+            raise error("Failed to resample subtitles!", self)
+
+        if use_arch:
+            prevout = output
+            output = Path(get_temp_workdir(), f"{self.file.stem}_resampled_arch.ass")
+
+            # fmt: off
+            dialog_json = json.dumps({"button": 0, "values": {"srcresx": src_width, "srcresy": src_height, "centerorg": "false"}})
+            args = [aegicli, "--video", str(video.resolve()), "--dialog", dialog_json, "--automation", "arch.Resample.moon", str(prevout), str(output), "Resample Perspective"]
+            # fmt: on
+            if run_commandline(args, quiet):
+                raise error("Failed to resample perspective of subtitles!", self)
+
+        self.file.unlink(True)
+        self.file = shutil.copy(output, self.file)
+        clean_temp_files()
+        return self
+
+    def separate_signs(self: SubFileSelf, styles: list[str] = DEFAULT_DIALOGUE_STYLES, inverse: bool = False) -> SubFileSelf:
+        """
+        Basically deletes lines that have any of the passed styles.
+
+        :param styles:      List of style names to get rid of
+        :param inverse:     Treat the list as the opposite. Will remove lines that *don't* have any of those steals.
+        """
+        doc = self._read_doc()
+        events = []
+        for line in doc.events:
+            skip = inverse
+            for style in styles:
+                if str(line.style).strip().casefold() == style.strip().casefold():
+                    skip = not inverse
+                    break
+
+            if skip:
+                continue
+            events.append(line)
+        doc.events = events
+        self.__update_doc(doc)
+        return self.clean_styles()
+
+    def copy(self: SubFileSelf) -> SubFileSelf:
+        """
+        Creates a new copy of the current SubFile object, including its file.
+        So you can run anything on the new one without impacting the other one.
+        """
+        doc = self._read_doc()
+        new_path = uniquify_path(self.file)
+        with open(new_path, "w", encoding=self.encoding) as writer:
+            doc.dump_file(writer)
+
+        new = self.__class__(new_path, self.container_delay, self.source)
+        new.encoding = self.encoding
+        return new
+
+    @classmethod
+    def from_mkv(cls: type[SubFileSelf], file: PathLike, track: int = 0, preserve_delay: bool = False, quiet: bool = True) -> SubFileSelf:
+        """
+        Extract subtitle from mkv.
+
+        :param file:            Input mkv file
+        :param track:           Relative track number
+        :param preserve_delay:  Preserve existing container delay
+        """
+        caller = "SubFile.from_mkv"
+        file = ensure_path_exists(file, caller)
+        track = get_absolute_track(file, track, TrackType.SUB, caller)
+        if track.format != "ASS":
+            raise error("The selected track is not an ASS subtitle.", caller)
+
+        mkvextract = get_executable("mkvextract")
+        out = Path(get_workdir(), f"{file.stem}_{track.track_id}.ass")
+        args = [mkvextract, str(file), "tracks", f"{track.track_id}:{str(out)}"]
+        if run_commandline(args, quiet):
+            raise error("Failed to extract subtitle!", caller)
+
+        return cls(out, 0 if not preserve_delay else getattr(track, "delay_relative_to_video", 0), file)
+
+
+SubFileSelf = TypeVar("SubFileSelf", bound=SubFile)
```

### Comparing `muxtools-0.0.6/muxtools/subtitle/subutils.py` & `muxtools-0.0.7/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/convert.py` & `muxtools-0.0.7/muxtools/utils/convert.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,45 +34,62 @@
     Converts a timedelta to a frame number.
 
     :param time:    The timedelta
     :param fps:     A Fraction containing fps_num and fps_den
 
     :return:        The resulting frame number
     """
-
-    s = Decimal(time.total_seconds())
+    ms = Decimal(time.total_seconds()) * 1000
     fps_dec = _fraction_to_decimal(fps)
-    return round((s * fps_dec))
 
+    upper_bound = (ms + Decimal(0.5)) * fps_dec / 1000
+    trunc_frame = int(upper_bound)
+
+    if upper_bound == trunc_frame:
+        return trunc_frame - 1
+
+    return trunc_frame
 
-def frame_to_timedelta(f: int, fps: Fraction = Fraction(24000, 1001)) -> timedelta:
+
+def frame_to_timedelta(f: int, fps: Fraction = Fraction(24000, 1001), compensate: bool = False) -> timedelta:
     """
     Converts a frame number to a timedelta.
     Mostly used in the conversion for manually defined chapters.
 
-    :param f:       The frame number
-    :param fps:     A Fraction containing fps_num and fps_den
+    :param f:           The frame number
+    :param fps:         A Fraction containing fps_num and fps_den
+    :param compensate:  Whether or not to place the the timestamp in the middle of said frame
+                        Useful for subtitles, not so much for audio where you'd wanna be accurate
 
-    :return:        The resulting timedelta
+    :return:            The resulting timedelta
     """
+    if not f:
+        return timedelta(seconds=0)
     fps_dec = _fraction_to_decimal(fps)
     seconds = Decimal(f) / fps_dec
-    return timedelta(seconds=float(seconds))
+    if not compensate:
+        return timedelta(seconds=float(seconds))
+    else:
+        t1 = timedelta(seconds=float(seconds))
+        t2 = timedelta(seconds=float(Decimal(f + 1) / fps_dec))
+        return t1 + (t2 - t1) / 2
 
 
-def frame_to_ms(f: int, fps: Fraction = Fraction(24000, 1001)) -> timedelta:
+def frame_to_ms(f: int, fps: Fraction = Fraction(24000, 1001), compensate: bool = False) -> timedelta:
     """
     Converts a frame number to it's ms value.
 
-    :param f:       The frame number
-    :param fps:     A Fraction containing fps_num and fps_den
+    :param f:           The frame number
+    :param fps:         A Fraction containing fps_num and fps_den
+    :param compensate:  Whether or not to place the the timestamp in the middle of said frame
+                        Useful for subtitles, not so much for audio where you'd wanna be accurate
 
-    :return:        The resulting ms
+    :return:            The resulting ms
     """
-    td = frame_to_timedelta(f, fps)
+    td = frame_to_timedelta(f, fps, compensate)
     return td.total_seconds() * 1000
 
 
 def format_timedelta(time: timedelta, precision: int = 3) -> str:
     """
     Formats a timedelta to hh:mm:ss.s[*precision] and pads with 0 if there aren't more numbers to work with.
     Mostly to be used for ogm/xml files.
```

### Comparing `muxtools-0.0.6/muxtools/utils/download.py` & `muxtools-0.0.7/muxtools/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
     url: str
     alias: list[str] | None = None
 
 
 # fmt: off
 # Feel free to compare the hashes if you don't like the custom files
 tools = [
-    Tool("CUETools.FLACCL.cmd", "https://github.com/gchudov/cuetools.net/releases/download/v2.2.3/CUETools_2.2.3.zip", ["flaccl"]),
+    Tool("CUETools.FLACCL.cmd", "https://github.com/gchudov/cuetools.net/releases/download/v2.2.4/CUETools_2.2.4.zip", ["flaccl"]),
     # non-free builds for libfdk_aac if one so desires
-    Tool("ffmpeg", "https://github.com/AnimMouse/ffmpeg-autobuild/releases/download/m-2023-05-08-05-43/ffmpeg-f009f84-3e8c1fa-win64-nonfree.7z", ["ffprobe"]),
-    Tool("mkvmerge", "https://www.videohelp.com/download/mkvtoolnix-64-bit-76.0.7z", ['mkvextract', 'mkvinfo', 'mkvpropedit']), 
-    Tool("eac3to", "https://files.catbox.moe/k0gzt0.7z"), # Custom package because of removed sounds and updated libFlac
+    Tool("ffmpeg", "https://github.com/AnimMouse/ffmpeg-autobuild/releases/download/m-2023-06-12-17-58/ffmpeg-09621fd-9b0e37c-win64-nonfree.7z", ["ffprobe"]),
+    Tool("mkvmerge", "https://mkvtoolnix.download/windows/releases/77.0/mkvtoolnix-64-bit-77.0.7z", ['mkvextract', 'mkvinfo', 'mkvpropedit']), 
+    Tool("eac3to", "https://files.catbox.moe/hn9oms.7z"), # Custom package because of removed sounds and updated libFlac
     Tool("x264", "https://github.com/DJATOM/x264-aMod/releases/download/r3101+20/x264-aMod-x64-core164-r3101+20.7z"),
     Tool("x265", "https://github.com/DJATOM/x265-aMod/releases/download/3.5+67/x265-x64-v3.5+67-aMod-gcc12.2.1+opt.7z"),
-    Tool("qaac", "https://files.catbox.moe/cxtxm4.7z"), # 2.79 with flac, w64 and iTunes libraries included
+    Tool("qaac", "https://files.catbox.moe/z9q796.7z"), # 2.79 with flac, w64 and iTunes libraries included
     Tool("opusenc", "https://archive.mozilla.org/pub/opus/win32/opus-tools-0.2-opus-1.3.zip"),
-    Tool("flac", "https://github.com/xiph/flac/releases/download/1.4.2/flac-1.4.2-win.zip"),
+    Tool("flac", "https://github.com/xiph/flac/releases/download/1.4.3/flac-1.4.3-win.zip"),
     Tool("wavpack", "https://github.com/dbry/WavPack/releases/download/5.6.0/wavpack-5.6.0-x64.zip")
 ]
 # fmt: on
 
 # TODO: check CPU to decide on which x264/5 file to use
```

### Comparing `muxtools-0.0.6/muxtools/utils/env.py` & `muxtools-0.0.7/muxtools/utils/env.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/files.py` & `muxtools-0.0.7/muxtools/utils/files.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/format.py` & `muxtools-0.0.7/muxtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/glob.py` & `muxtools-0.0.7/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/log.py` & `muxtools-0.0.7/muxtools/utils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from rich.logging import RichHandler
 import time
 import inspect
 
-__all__ = ["crit", "debug", "error", "exit", "info", "logger"]
+__all__ = ["crit", "debug", "error", "exit", "info", "warn", "logger"]
 
-FORMAT = "%(message)s"  # %(name)s |
-logging.basicConfig(level="NOTSET", format=FORMAT, datefmt="[%X]", handlers=[RichHandler(markup=True, omit_repeated_times=False, show_path=False)])
+FORMAT = "%(name)s | %(message)s"  #
+logging.basicConfig(format=FORMAT, datefmt="[%X]", handlers=[RichHandler(markup=True, omit_repeated_times=False, show_path=False)])
 
-logger = logging.getLogger("vodesauto")
+logger = logging.getLogger("muxtools")
+logger.setLevel(logging.DEBUG)
 
 
 def _format_msg(msg: str, caller: any) -> str:
     if caller and not isinstance(caller, str):
         caller = caller.__class__.__qualname__ if hasattr(caller, "__class__") and caller.__class__.__name__ not in ["function", "method"] else caller
         caller = caller.__name__ if not isinstance(caller, str) else caller
     return msg if caller is None else f"[bold]{caller}:[/] {msg}"
```

### Comparing `muxtools-0.0.6/muxtools/utils/parsing.py` & `muxtools-0.0.7/muxtools/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/muxtools/utils/types.py` & `muxtools-0.0.7/muxtools/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 
 class ValidInputType(IntEnum):
     FLAC = 1
     AIFF = 2
     W64 = 3
     AIFF_OR_FLAC = 4
+    W64_OR_FLAC = 5
 
 
 @dataclass
 class AudioFrame:
     """
     A dataclass representing ffmpeg's `ashowdata` filter output.
```

### Comparing `muxtools-0.0.6/muxtools.egg-info/PKG-INFO` & `muxtools-0.0.7/muxtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.6/muxtools.egg-info/SOURCES.txt` & `muxtools-0.0.7/muxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.6/pyproject.toml` & `muxtools-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 [project]
 name = "muxtools"
-version = "0.0.6"
+version = "0.0.7"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
-    "fontcollector>=2.1.0",
+    "fontcollector>=2.1.1",
     "ass>=0.5.3",
     "wget>=3.2",
     "py7zr>=0.20.5",
     "pymediainfo>=6.0.1",
     "rich>=13.1.0",
     "pyparsebluray>=0.1.4",
 ]
```

