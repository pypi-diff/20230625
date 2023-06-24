# Comparing `tmp/scientific_plots-1.5.1.tar.gz` & `tmp/scientific_plots-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.5.1.tar", last modified: Fri Jun 23 10:16:20 2023, max compression
+gzip compressed data, was "scientific_plots-1.5.2.tar", last modified: Sat Jun 24 21:57:17 2023, max compression
```

## Comparing `scientific_plots-1.5.1.tar` & `scientific_plots-1.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-23 10:08:16.000000 scientific_plots-1.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/readme.md
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.1/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     6787 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-04 10:41:15.000000 scientific_plots-1.5.1/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-23 10:06:10.000000 scientific_plots-1.5.1/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18732 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 10:15:54.000000 scientific_plots-1.5.1/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.1/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.1/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-23 10:08:16.000000 scientific_plots-1.5.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.2/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.2/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18778 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.2/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-24 21:56:50.000000 scientific_plots-1.5.2/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.2/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.2/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_utilties.py
```

### Comparing `scientific_plots-1.5.1/PKG-INFO` & `scientific_plots-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.5.1
+Version: 1.5.2
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `scientific_plots-1.5.1/pyproject.toml` & `scientific_plots-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/readme.md` & `scientific_plots-1.5.2/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.5.2/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.5.2/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.5.2/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.5.2/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import annotations
 from typing import (
     Optional, Tuple, Iterable, Union, TypeVar, List, TypedDict, Any)
 from pathlib import Path
 from contextlib import contextmanager
 from collections.abc import Generator
 
+from ..ticker import Locator
 from ..figure import Figure
 from .. import colors, RCParams
 
 from scientific_plots.types_ import Vector, Matrix
 
 
 In = TypeVar("In", List[float], Tuple[float],
@@ -81,14 +82,16 @@
 
     def set_tick_params(self, pad: Optional[float] = None,
                         direction: str = "", color: str = "")\
         -> None: ...
 
     def set_major_formatter(self, format_str: str) -> None: ...
 
+    def set_major_locator(self, locator: Locator) -> None: ...
+
 
 class Spine:
     """Spine-class of axes."""
 
     def set_color(self, color: str) -> None: ...
 
     def set_linewidth(self, width: float) -> None: ...
```

### Comparing `scientific_plots-1.5.1/src/numba-stubs/__init__.pyi` & `scientific_plots-1.5.2/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots/data_analysis.py` & `scientific_plots-1.5.2/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots/default_plots.py` & `scientific_plots-1.5.2/src/scientific_plots/default_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from functools import wraps
 from typing import TypeVar, List, Tuple, Union, Callable, Optional
 from warnings import warn
 from textwrap import dedent
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+from matplotlib.ticker import MaxNLocator
 import numpy as np
 from numpy import amin, amax
 
 from .plot_settings import apply_styles, rwth_cycle
 from .types_ import Vector, Matrix
 
 mpl.use("Agg")
 
 In = TypeVar("In", List[float], Tuple[float],
              Vector)
 
-In2d = TypeVar("In2d", list[list[float]], list[Vector], tuple[Vector],
+In2D = TypeVar("In2D", list[list[float]], list[Vector], tuple[Vector],
                Matrix)
 
 
 def fix_inputs(input_1: In, input_2: In)\
         -> tuple[Vector, Vector]:
     """
     Remove nans and infinities from the input vectors.
@@ -157,15 +158,15 @@
     plt.legend()
     plt.tight_layout()
     plt.savefig(filename)
     plt.close()
 
 
 @apply_styles(three_d=True)
-def plot_surface(X: In2d, Y: In2d, Z: In2d,
+def plot_surface(X: In2D, Y: In2D, Z: In2D,
                  xlabel: str, ylabel: str, zlabel: str,
                  filename: Union[str, Path], *,
                  log_scale: bool = False,
                  set_z_lim: bool = True,
                  colorscheme: str = "rwth_gradient",
                  figsize: tuple[float, float] = (4.33, 3.5),
                  labelpad: Optional[float] = None,
@@ -214,20 +215,20 @@
         spine.set_visible(False)
 
     ax.xaxis.pane.set_alpha(0.3)
     ax.yaxis.pane.set_alpha(0.3)
     ax.zaxis.pane.set_alpha(0.3)
 
     if nbins is not None:
-        plt.locator_params(
-            nbins=nbins,
-            axis="x")
-        plt.locator_params(
-            nbins=nbins,
-            axis="y")
+        ax.xaxis.set_major_locator(
+            MaxNLocator(nbins)
+        )
+        ax.yaxis.set_major_locator(
+            MaxNLocator(nbins)
+        )
 
     fig.set_size_inches(*figsize)
     plt.tight_layout()
     plt.savefig(filename)
     plt.close()
```

### Comparing `scientific_plots-1.5.1/src/scientific_plots/plot_settings.py` & `scientific_plots-1.5.2/src/scientific_plots/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.5.2/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots/types_.py` & `scientific_plots-1.5.2/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots/utilities.py` & `scientific_plots-1.5.2/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.5.2/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.5.1
+Version: 1.5.2
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `scientific_plots-1.5.1/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.5.2/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scipy-stubs/fft.pyi` & `scientific_plots-1.5.2/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.5.2/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.5.2/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.5.2/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.5.2/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/tests/test_plot_manual.py` & `scientific_plots-1.5.2/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/tests/test_plots.py` & `scientific_plots-1.5.2/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/tests/test_types.py` & `scientific_plots-1.5.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.1/tests/test_utilties.py` & `scientific_plots-1.5.2/tests/test_utilties.py`

 * *Files identical despite different names*

