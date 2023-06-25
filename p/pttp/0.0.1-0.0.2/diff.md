# Comparing `tmp/pttp-0.0.1.tar.gz` & `tmp/pttp-0.0.2.tar.gz`

## Comparing `pttp-0.0.1.tar` & `pttp-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 pttp-0.0.1/src/pttp/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pttp-0.0.1/src/pttp/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pttp-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pttp-0.0.1/LICENSE
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pttp-0.0.1/README.md
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 pttp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 pttp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pttp-0.0.2/src/pttp/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pttp-0.0.2/src/pttp/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pttp-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pttp-0.0.2/LICENSE
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pttp-0.0.2/README.md
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 pttp-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 pttp-0.0.2/PKG-INFO
```

### Comparing `pttp-0.0.1/src/pttp/__init__.py` & `pttp-0.0.2/src/pttp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Literal, Optional
 import json
 import runpy
 import sys
 import time
 import pathlib
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 @dataclass(slots=True, frozen=True)
 class Frame:
     name: str
     file: Optional[str]
     line: Optional[int]
@@ -60,14 +60,17 @@
         return super().default(o)
 
 
 # key: id(frame), value: (index, frame)
 frames: dict[str, tuple[int, Frame]] = {}
 events: list[FrameEvent] = []
 
+# filters used to filter out frames by matching filenames.
+filters: list[str] = []
+
 
 profiling_offset = 0
 waiting_to_enter_mainpyfile = True
 
 
 def profilefunc(frame: FrameType, event: str, arg: Any) -> object:
     t = time.perf_counter()
@@ -81,14 +84,17 @@
             if filename.endswith('runpy.py') and fnname == '_run_code':
                 waiting_to_enter_mainpyfile = False
             return
 
         if event != 'call' and event != 'return':
             return
 
+        if len(filters) > 0 and not any(f in filename for f in filters):
+            return
+
         if event == 'call':
             event_type = 'O'
             key = id(frame)
             if key not in frames:
                 idx = len(frames)
                 frames[key] = idx, Frame(fnname, filename, lineno)
             else:
@@ -101,22 +107,25 @@
             idx, _ = frames[key]
 
         events.append(FrameEvent(event_type, idx, t - profiling_offset))
     finally:
         profiling_offset += (time.perf_counter() - t)
 
 
-def write_profile_to_file(mainpyfile: str):
+def write_pttp_profile_to_file(mainpyfile: str):
     if len(events) <= 1:
         return
 
     sys.setprofile(None)
-    # Drop last event, it's this function.
-    events.pop()
-    frames.popitem()
+    # Drop last event if it's this function.
+    if frames:
+        _, lastframe = next(reversed(frames.values()))
+        if lastframe.name == 'write_pttp_profile_to_file':
+            events.pop()
+            frames.popitem()
 
     filename = pathlib.Path(mainpyfile).with_suffix('.speedscope.json')
     profile = EventedProfile(
         type='evented',
         name=str(filename),
         unit='seconds',
         startValue=events[0].at,
@@ -143,31 +152,35 @@
 
 
 def main():
     # Mostly copied from https://github.com/python/cpython/blob/8c4cf96a06e2483a11a4cb34c550df5bd22f990b/Lib/pdb.py#L1878
 
     import getopt
 
-    opts, args = getopt.getopt(sys.argv[1:], 'mh', ['help'])
+    opts, args = getopt.getopt(sys.argv[1:], 'mhf=', ['help', 'filter='])
 
     if not args:
         print(_usage)
         sys.exit(2)
 
     if any(opt in ['-h', '--help'] for opt, optarg in opts):
         print(_usage)
         sys.exit()
 
+    if any(opt in ['-f', '--filter'] for opt, optarg in opts):
+        global filters
+        filters = [optarg for opt, optarg in opts if opt in ['-f', '--filter']]
+
     # Hide "pttp.py" and options from argument list
     sys.argv[:] = args
 
     sys.setprofile(profilefunc)
     try:
         module_indicated = any(opt in ['-m'] for opt, optarg in opts)
         mainpyfile = args[0]
 
         if module_indicated:
             runpy._run_module_as_main(mainpyfile, alter_argv=False)
         else:
             runpy.run_path(mainpyfile, run_name='__main__')
     finally:
-        write_profile_to_file(mainpyfile)
+        write_pttp_profile_to_file(mainpyfile)
```

### Comparing `pttp-0.0.1/.gitignore` & `pttp-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pttp-0.0.1/LICENSE` & `pttp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pttp-0.0.1/README.md` & `pttp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pttp-0.0.1/pyproject.toml` & `pttp-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pttp-0.0.1/PKG-INFO` & `pttp-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pttp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python tracing profiler
 Project-URL: Documentation, https://github.com/vivster7/pttp#readme
 Project-URL: Issues, https://github.com/vivster7/pttp/issues
 Project-URL: Source, https://github.com/vivster7/pttp
 Author-email: Vivek Dasari <vivster7@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

