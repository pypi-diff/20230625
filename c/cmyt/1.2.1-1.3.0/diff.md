# Comparing `tmp/cmyt-1.2.1.tar.gz` & `tmp/cmyt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmyt-1.2.1.tar", last modified: Mon Jun 19 12:04:50 2023, max compression
+gzip compressed data, was "cmyt-1.3.0.tar", last modified: Sun Jun 25 12:37:39 2023, max compression
```

## Comparing `cmyt-1.2.1.tar` & `cmyt-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.358384 cmyt-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-19 12:04:40.000000 cmyt-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-19 12:04:50.358384 cmyt-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-19 12:04:40.000000 cmyt-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/cm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt/colormaps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/algae.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/apricity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/arbre.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/dusk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/kelp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/octarine.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pastel.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_green.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_red.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/xray.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-19 12:04:40.000000 cmyt-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:04:50.358384 cmyt-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.358384 cmyt-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:39.530656 cmyt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-25 12:37:27.000000 cmyt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-25 12:37:39.530656 cmyt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-25 12:37:27.000000 cmyt-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:39.526656 cmyt-1.3.0/cmyt/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/cm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:39.530656 cmyt-1.3.0/cmyt/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/algae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/apricity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/arbre.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/dusk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/kelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/octarine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/pastel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/pixel_blue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/pixel_green.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/pixel_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/colormaps/xray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 12:37:27.000000 cmyt-1.3.0/cmyt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:39.526656 cmyt-1.3.0/cmyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-25 12:37:39.000000 cmyt-1.3.0/cmyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-25 12:37:39.000000 cmyt-1.3.0/cmyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 12:37:39.000000 cmyt-1.3.0/cmyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 12:37:39.000000 cmyt-1.3.0/cmyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 12:37:39.000000 cmyt-1.3.0/cmyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-25 12:37:27.000000 cmyt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 12:37:39.530656 cmyt-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:37:39.530656 cmyt-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 12:37:27.000000 cmyt-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-25 12:37:27.000000 cmyt-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-25 12:37:27.000000 cmyt-1.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-25 12:37:27.000000 cmyt-1.3.0/tests/test_utils.py
```

### Comparing `cmyt-1.2.1/LICENSE` & `cmyt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/PKG-INFO` & `cmyt-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.2.1
+Version: 1.3.0
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.2.1 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.3.0 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
```

### Comparing `cmyt-1.2.1/README.md` & `cmyt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/cm.py` & `cmyt-1.3.0/cmyt/cm.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/algae.py` & `cmyt-1.3.0/cmyt/colormaps/algae.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/apricity.py` & `cmyt-1.3.0/cmyt/colormaps/apricity.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/arbre.py` & `cmyt-1.3.0/cmyt/colormaps/arbre.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/dusk.py` & `cmyt-1.3.0/cmyt/colormaps/dusk.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/kelp.py` & `cmyt-1.3.0/cmyt/colormaps/kelp.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/octarine.py` & `cmyt-1.3.0/cmyt/colormaps/octarine.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/pastel.py` & `cmyt-1.3.0/cmyt/colormaps/pastel.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/colormaps/xray.py` & `cmyt-1.3.0/cmyt/colormaps/xray.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/cmyt/utils.py` & `cmyt-1.3.0/cmyt/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
-import re
 import sys
 from typing import TYPE_CHECKING, Dict, Final, Iterable, Literal, Optional, Tuple
 
-import matplotlib
+import matplotlib as mpl
 import numpy as np
 from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap
-from more_itertools import always_iterable
 
 # type aliases
 
 if TYPE_CHECKING:
     from matplotlib.axes import Axes
     from matplotlib.figure import Figure
 
@@ -33,33 +31,14 @@
         "pixel_green",
         "pixel_red",
         "xray",
     )
 )
 
 
-def version_tuple(version: str) -> Tuple[int, ...]:
-    elems = version.split(".")
-    if len(elems) > 3:
-        elems = elems[:3]
-
-    if not elems[-1].isnumeric():
-        # allow alpha/beta/release candidate versions
-        match = re.search(r"^\d+", elems[-1])
-        if match is None:
-            elems.pop()
-        else:
-            elems[-1] = match.group()
-
-    return tuple(int(_) for _ in elems)
-
-
-MPL_VERSION = version_tuple(matplotlib.__version__)
-
-
 def prefix_name(name: str) -> str:
     if not name.startswith(_CMYT_PREFIX):
         return f"{_CMYT_PREFIX}{name}"
     return name
 
 
 def unprefix_name(name: str) -> str:
@@ -75,60 +54,39 @@
         return name.removeprefix(_CMYT_PREFIX)
     else:
         if name.startswith(_CMYT_PREFIX):
             return name[len(_CMYT_PREFIX) :]
         return name
 
 
-def _register_mpl_cmap(cmap: Colormap) -> None:
-    """
-    An adapter for matplotlib that works transparently with
-    either API (historical and post 3.5.0) while dodging deprecation
-    warnings.
-    """
-    if MPL_VERSION >= (3, 5, 0):
-        matplotlib.colormaps.register(cmap)
-    else:
-        from matplotlib.cm import register_cmap
-
-        register_cmap(cmap=cmap)
-
-
 def register_colormap(
     name: str,
     *,
     color_dict: Optional[ColorDict] = None,
     colors: Optional[np.ndarray] = None,
 ) -> Tuple[LinearSegmentedColormap, LinearSegmentedColormap]:
     name = prefix_name(name)
 
     if color_dict is not None and colors is not None:
         raise TypeError("Either color_dict or colors must be provided, but not both")
     # register to MPL
     if color_dict is not None:
-        mpl_cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
+        cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
     elif colors is not None:
-        mpl_cmap = ListedColormap(colors, name=name, N=256)
+        cmap = ListedColormap(colors, name=name, N=256)
     else:
         raise TypeError("color_dict or colors must be provided")
-    mpl_cmap_r = mpl_cmap.reversed()
-    _register_mpl_cmap(mpl_cmap)
-    _register_mpl_cmap(mpl_cmap_r)
 
-    # return cmaps with unprefixed names for registration as importable objects
-    if MPL_VERSION >= (3, 4):
-        cmap = mpl_cmap.copy()
-    else:
-        if color_dict is not None:
-            cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
-        elif colors is not None:
-            cmap = ListedColormap(colors, name=name, N=256)
-    cmap.name = unprefix_name(name)
     cmap_r = cmap.reversed()
+    mpl.colormaps.register(cmap)
+    mpl.colormaps.register(cmap_r)
 
+    # return cmaps with unprefixed names for registration as importable objects
+    cmap.name = unprefix_name(cmap.name)
+    cmap_r.name = unprefix_name(cmap_r.name)
     return cmap, cmap_r
 
 
 graySCALE_CONVERSION_SPACE = "JCh"
 
 
 def to_grayscale(sRGB1: np.ndarray) -> np.ndarray:
@@ -194,18 +152,15 @@
     with_grayscale: bool
         Whether to display a grayscale version of each colorbar on top of the
         colorful version. This flag requires matplotlib 3.0 or greater.
         Defaults to False.
     """
     import matplotlib.pyplot as plt
 
-    if subset is None:
-        subset = cmyt_cmaps
-
-    cmaps = sorted(prefix_name(_) for _ in always_iterable(subset))
+    cmaps = sorted(prefix_name(_) for _ in (subset or cmyt_cmaps))
     if not cmaps:
         raise ValueError(f"Received invalid or empty subset: {subset}")
 
     # scale the image size by the number of cmaps
     fig, axes = plt.subplots(nrows=len(cmaps), figsize=(6, 2.6 * len(cmaps) / 10.0))
 
     for name, ax in zip(cmaps, axes):
```

### Comparing `cmyt-1.2.1/cmyt.egg-info/PKG-INFO` & `cmyt-1.3.0/cmyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.2.1
+Version: 1.3.0
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.2.1 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.3.0 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
```

### Comparing `cmyt-1.2.1/cmyt.egg-info/SOURCES.txt` & `cmyt-1.3.0/cmyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/pyproject.toml` & `cmyt-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmyt"
-version = "1.2.1"
 description = "A collection of Matplotlib colormaps from the yt project"
 authors = [
     { name = "The yt project", email = "yt-dev@python.org" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Matplotlib",
@@ -23,32 +22,34 @@
     "Typing :: Typed",
 ]
 keywords = [
     "visualization",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "colorspacious>=1.1.2",
-    "matplotlib>=3.2.0",
-    "more-itertools>=8.4",
+    "matplotlib>=3.5.0",
     "numpy>=1.17.4",
 ]
+dynamic = ["version"]
 
 [project.license]
 text = "BSD 3-Clause"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://yt-project.org/"
 Source = "https://github.com/yt-project/cmyt/"
 Tracker = "https://github.com/yt-project/cmyt/issues"
 
+[tool.setuptools.dynamic]
+version = {attr = "cmyt.__version__"}
+
 [tool.setuptools]
 license-files = [
     "LICENSE",
 ]
 include-package-data = false
 
 [tool.setuptools.packages.find]
```

### Comparing `cmyt-1.2.1/tests/test_integration.py` & `cmyt-1.3.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.1/tests/test_utils.py` & `cmyt-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

