# Comparing `tmp/pttp-0.0.2.tar.gz` & `tmp/pttp-0.0.3.tar.gz`

## Comparing `pttp-0.0.2.tar` & `pttp-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pttp-0.0.2/src/pttp/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pttp-0.0.2/src/pttp/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pttp-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pttp-0.0.2/LICENSE
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pttp-0.0.2/README.md
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 pttp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 pttp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 pttp-0.0.3/src/pttp/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pttp-0.0.3/src/pttp/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pttp-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pttp-0.0.3/LICENSE
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pttp-0.0.3/README.md
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 pttp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 pttp-0.0.3/PKG-INFO
```

### Comparing `pttp-0.0.2/src/pttp/__init__.py` & `pttp-0.0.3/src/pttp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Literal, Optional
 import json
 import runpy
 import sys
 import time
 import pathlib
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 @dataclass(slots=True, frozen=True)
 class Frame:
     name: str
     file: Optional[str]
     line: Optional[int]
@@ -141,17 +141,21 @@
         exporter='pttp',
     )
     with open(file.name, 'w') as f:
         json.dump(file, f, indent=2, cls=EnhancedJSONEncoder)
 
 
 _usage = """\
-usage: pttp.py [-m module | pyfile]
+usage: pttp.py [OPTIONS] [-m module | pyfile]
 
 Trace the Python program given by pyfile or -m module.
+
+Options:
+  --filter TEXT     Only include frames whose filenames contain this string.
+  -h, --help        Show this help message and exit.
 """
 
 
 def main():
     # Mostly copied from https://github.com/python/cpython/blob/8c4cf96a06e2483a11a4cb34c550df5bd22f990b/Lib/pdb.py#L1878
 
     import getopt
```

### Comparing `pttp-0.0.2/.gitignore` & `pttp-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pttp-0.0.2/LICENSE` & `pttp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pttp-0.0.2/README.md` & `pttp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pttp-0.0.2/pyproject.toml` & `pttp-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pttp-0.0.2/PKG-INFO` & `pttp-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pttp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python tracing profiler
 Project-URL: Documentation, https://github.com/vivster7/pttp#readme
 Project-URL: Issues, https://github.com/vivster7/pttp/issues
 Project-URL: Source, https://github.com/vivster7/pttp
 Author-email: Vivek Dasari <vivster7@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

