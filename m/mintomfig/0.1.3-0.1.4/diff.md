# Comparing `tmp/mintomfig-0.1.3.tar.gz` & `tmp/mintomfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintomfig-0.1.3.tar", max compression
+gzip compressed data, was "mintomfig-0.1.4.tar", max compression
```

## Comparing `mintomfig-0.1.3.tar` & `mintomfig-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.3/README.md
--rw-r--r--   0        0        0     1772 2023-06-08 05:41:44.062190 mintomfig-0.1.3/mintomfig/__init__.py
--rw-r--r--   0        0        0      295 2023-06-08 05:41:16.215492 mintomfig-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.4/README.md
+-rw-r--r--   0        0        0     1820 2023-06-25 04:11:07.553130 mintomfig-0.1.4/mintomfig/__init__.py
+-rw-r--r--   0        0        0      295 2023-06-25 04:11:24.009740 mintomfig-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.4/PKG-INFO
```

### Comparing `mintomfig-0.1.3/mintomfig/__init__.py` & `mintomfig-0.1.4/mintomfig/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import sys
 import toml
+from pathlib import Path
 
 from xdg import xdg_config_home
 
 
-def canonical_config_dir():
+def canonical_config_dir() -> Path:
     # on linux, use xdg_config_home
     # on windows, use appdata
     # on macos, use HOME/Library/Preferences
     if sys.platform == "linux":
         return xdg_config_home()
     elif sys.platform == "win32":
-        return os.environ["APPDATA"]
+        return Path(os.environ["APPDATA"])
     elif sys.platform == "darwin":
-        return os.path.expanduser("~/Library/Preferences")
+        return Path(os.environ["HOME"]) / "Library" / "Preferences"
 
 
 def canonical_config_base(app_name):
     return canonical_config_dir() / app_name
 
 
 def canonical_config_file(app_name, config_file_name):
```

### Comparing `mintomfig-0.1.3/PKG-INFO` & `mintomfig-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintomfig
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

