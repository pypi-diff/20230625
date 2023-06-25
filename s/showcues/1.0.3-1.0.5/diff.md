# Comparing `tmp/showcues-1.0.3.tar.gz` & `tmp/showcues-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showcues-1.0.3.tar", last modified: Tue Jun 20 18:07:23 2023, max compression
+gzip compressed data, was "showcues-1.0.5.tar", last modified: Sun Jun 25 18:09:08 2023, max compression
```

## Comparing `showcues-1.0.3.tar` & `showcues-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-20 18:07:23.767308 showcues-1.0.3/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-20 18:07:23.767308 showcues-1.0.3/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.3/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-20 18:07:23.767308 showcues-1.0.3/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.3/bin/showcues
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-20 18:07:23.767308 showcues-1.0.3/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-20 18:05:02.000000 showcues-1.0.3/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-20 18:07:23.767308 showcues-1.0.3/showcues.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-20 18:07:23.000000 showcues-1.0.3/showcues.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      202 2023-06-20 18:07:23.000000 showcues-1.0.3/showcues.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-20 18:07:23.000000 showcues-1.0.3/showcues.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       50 2023-06-20 18:07:23.000000 showcues-1.0.3/showcues.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        9 2023-06-20 18:07:23.000000 showcues-1.0.3/showcues.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    12920 2023-06-20 17:39:52.000000 showcues-1.0.3/showcues.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-25 18:09:08.056223 showcues-1.0.5/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.5/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.5/bin/showcues
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-25 18:09:08.056223 showcues-1.0.5/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-25 18:07:35.000000 showcues-1.0.5/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/showcues.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      202 2023-06-25 18:09:08.000000 showcues-1.0.5/showcues.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       50 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        9 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    13940 2023-06-25 02:22:06.000000 showcues-1.0.5/showcues.py
```

### Comparing `showcues-1.0.3/PKG-INFO` & `showcues-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.3
+Version: 1.0.5
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.3/setup.py` & `showcues-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 with open("version.py","r", encoding="utf-8") as latest:
-    version = latest.read().split("'")[1]
+    version = latest.read().split('"')[1]
 
 setuptools.setup(
     name="showcues",
     version=version,
     author="Adrian of Doom.",
     author_email="spam@iodisco.com",
     description="showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time",
```

### Comparing `showcues-1.0.3/showcues.egg-info/PKG-INFO` & `showcues-1.0.5/showcues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.3
+Version: 1.0.5
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.3/showcues.py` & `showcues-1.0.5/showcues.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import datetime
 import sys
 import time
 import threefive
 from threefive import Cue
+from iframes import IFramer
 from m3ufu import M3uFu, TagParser, HEADER_TAGS
 from new_reader import reader
 
 REV = "\033[7m"
 NORM = "\033[27m"
 
 
@@ -94,14 +95,15 @@
 
 class CuePuller:
     MEDIA_COUNT = 111
 
     def __init__(self):
         self.cues = []
         self.media = []
+        self.media_count = 101
         self.sidecar_file = "cp_sidecar.txt"
         self.base_uri = None
         self.iv = None
         self.key_uri = None
         self.last_iv = None
         self.last_key_uri = None
         self.event_id = 1
@@ -112,14 +114,16 @@
         self.reload = True
         self.sleep_duration = 0
         self.window_size = None
         self.sliding_window = None
         self.cue_state = None
         self.last_cue = None
         self.headers = []
+        self.pts = None
+        self.hls_pts = "HLS"
 
     def chk_aes(self, line):
         """
         chk_aes checks for AES encryption
         """
         if "#EXT-X-KEY" in line:
             tags = TagParser([line]).tags
@@ -174,16 +178,16 @@
     def add_cue(self, cue, line):
         """
         add_cue determines cue_state and
         calls six2five to replace time signals
         """
         cue = cue.replace("\r", "").replace("\n", "")
         if "CONT" not in line:
-            cue_stuff = f"{REV}{self.cue_state} {NORM}  {cue} "
-            media_stuff = f"\nMedia: {self.media[-1]}\n"
+            cue_stuff = f"{REV}{self.cue_state}{NORM} {cue} "
+            media_stuff = f"\n{REV}Media:{NORM} {self.media[-1]}\n"
             if cue == "#EXT-X-CUE-IN":
                 self.cue_state = "IN"
                 diff_stuff = f" {REV}Diff:{NORM} {round(self.break_timer - self.break_duration,3)}"
                 print(f"{iso8601()} {cue_stuff} {diff_stuff}{media_stuff}")
                 self.reset_break()
                 return line
             if cue.startswith("#EXT-X-CUE-OUT"):
@@ -278,41 +282,67 @@
         auto_cuein handles cue.command.autoreturn
         """
         if self.cue_state == "CONT":
             if self.break_timer and self.break_duration:
                 if self.break_timer >= self.break_duration:
                     self.cue_state = "IN"
                     print(
-                        f"{iso8601()} {REV}AUTO CUE-IN{NORM} Diff: {REV}{round(self.break_timer - self.break_duration,3)}{NORM} \nMedia: {self.media[-1]}\n"
+                        f"{iso8601()} {REV}AUTO{NORM} #EXT-X-CUE-IN{REV}Diff:{NORM}{round(self.break_timer - self.break_duration,3)} \n{REV}Media:{NORM} {self.media[-1]}\n"
                     )
                     self.reset_break()
                     return "\n#AUTO\n#EXT-X-CUE-IN\n" + line
         return line
 
     def reset_break(self):
+        """
+        reset_break resets
+        break_duration, break_timer,
+        and cue_state after a CUE-IN
+        """
         if self.cue_state == "IN":
             self.break_duration = None
             self.break_timer = None
             self.cue_state = None
 
     def extinf(self, line):
+        """
+        extinf parses lines that start with #EXTINF
+        for the segment duration.
+        """
         tags = TagParser([line]).tags
         if "#EXTINF" in tags:
             if isinstance(tags["#EXTINF"], str):
                 tags["#EXTINF"] = tags["#EXTINF"].rsplit(",", 1)[0]
             seg_time = round(float(tags["#EXTINF"]), 6)
             line = self.auto_cuein(line)
+            if self.pts is not None:
+                self.pts += seg_time
             if self.break_timer is not None:
                 self.break_timer += seg_time
         return line
 
     def new_media(self, media):
+        """
+        new_media check to see
+        if the media is new in a
+        live sliding window
+        """
         if media not in self.media:
             self.media.append(media)
-            self.media = self.media[-self.MEDIA_COUNT :]
+            if self.pts is None:
+                media = media.replace("\n", "")
+                if ".ts" in media:
+                    Iframer = IFramer(shush=True)
+                    iframes = Iframer.do(media)
+                    self.pts = iframes[0]
+                    self.hls_pts = "PTS"
+                else:
+                    self.pts = 0
+            # print(f"Starting {self.hls_pts} Time:{ self.pts}\n")
+            self.media = self.media[-self.window_size * 2 :]
             return True
         return False
 
     def parse_target_duration(self, line):
         if line.startswith("#EXT-X-TARGETDURATION"):
             self.sleep_duration = round((atoif(line.split(":")[1]) >> 1), 3)
 
@@ -384,18 +414,21 @@
 
 
 def cli():
     fu = M3uFu()
     fu.m3u8 = sys.argv[1]
     fu.decode()
     m3u8 = None
-    for segment in fu.segments:
-        if "#EXT-X-STREAM-INF" in segment.tags:
-            m3u8 = segment.media
-            cp = CuePuller()
-            print(m3u8)
-            cp.pull(m3u8)
-    print("variant m3u8 not found")
+    playlists = [
+        segment for segment in fu.segments if "#EXT-X-STREAM-INF" in segment.tags
+    ]
+    if playlists:
+        m3u8 = playlists[0].media
+    else:
+        m3u8 = sys.argv[1]
+    cp = CuePuller()
+    print(f"m3u8: {m3u8}\n")
+    cp.pull(m3u8)
 
 
 if __name__ == "__main__":
     cli()
```

