# Comparing `tmp/scientific_plots-1.5.2.tar.gz` & `tmp/scientific_plots-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.5.2.tar", last modified: Sat Jun 24 21:57:17 2023, max compression
+gzip compressed data, was "scientific_plots-1.5.3.tar", last modified: Sun Jun 25 00:18:23 2023, max compression
```

## Comparing `scientific_plots-1.5.2.tar` & `scientific_plots-1.5.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-23 10:08:16.000000 scientific_plots-1.5.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.2/readme.md
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.424963 scientific_plots-1.5.2/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.2/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.2/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18778 2023-06-24 21:33:21.000000 scientific_plots-1.5.2/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.2/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-24 21:56:50.000000 scientific_plots-1.5.2/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.2/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.428963 scientific_plots-1.5.2/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-24 21:57:17.000000 scientific_plots-1.5.2/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:57:17.432963 scientific_plots-1.5.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.2/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.2/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-24 23:18:51.000000 scientific_plots-1.5.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    11604 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-24 23:56:16.000000 scientific_plots-1.5.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.3/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.3/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-24 23:10:04.000000 scientific_plots-1.5.3/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18778 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.3/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 00:17:40.000000 scientific_plots-1.5.3/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.3/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11604 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.3/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_utilties.py
```

### Comparing `scientific_plots-1.5.2/PKG-INFO` & `scientific_plots-1.5.3/readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: scientific_plots
-Version: 1.5.2
-Summary: Useful methods for plots used in science
-Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
-Keywords: Plotting,science,library,utilities,styling
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Scientific Plots
 Create and save plots in scientific style
 
 ## Table of Contents
 [[_TOC_]]
 
 ## Overview
```

### Comparing `scientific_plots-1.5.2/pyproject.toml` & `scientific_plots-1.5.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "scientific_plots"
 requires-python = ">=3.8"
 description = "Useful methods for plots used in science"
 readme = "readme.md"
 authors = [{name = "Felix Fischer", email = "f.fischer@ifas.rwth-aachen.de"}]
 classifiers = [
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    """License :: OSI Approved :: \
+    GNU Lesser General Public License v3 or later (LGPLv3+)""",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3"
 ]
 keywords = ["Plotting", "science", "library", "utilities", "styling"]
 
+license = {file = "LICENSE.txt"}
+
 dependencies = [
     "scipy",
     "numpy>=1.21",
     "matplotlib>=3.7",
     "SciencePlots",
     "python_translator",
     "requests",
@@ -30,14 +33,25 @@
     "flake8",
     "pytest",
     "types-urllib3",
     "twine>=4.0.0",
     "requests-toolbelt>=1.0.0"
 ]
 
+[build-system]
+requires = ["setuptools>42", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+package-data = {"*" = [
+    "py.typed",
+    "readme.md",
+    "*.pyi",
+    "LICENSE.txt"]}
+
 [tool.setuptools.dynamic]
 version = {attr = "scientific_plots.__version__"}
 
 [tool.mypy]
 python_version = "3.9"
 warn_unused_configs = true
 follow_imports_for_stubs = true
```

### Comparing `scientific_plots-1.5.2/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.5.3/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.5.3/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.5.3/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.5.3/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.5.3/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/numba-stubs/__init__.pyi` & `scientific_plots-1.5.3/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/data_analysis.py` & `scientific_plots-1.5.3/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/default_plots.py` & `scientific_plots-1.5.3/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/plot_settings.py` & `scientific_plots-1.5.3/src/scientific_plots/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.5.3/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/types_.py` & `scientific_plots-1.5.3/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots/utilities.py` & `scientific_plots-1.5.3/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.5.3/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+LICENSE.txt
 pyproject.toml
 readme.md
-setup.cfg
 src/cycler-stubs/__init__.pyi
 src/hurst-stubs/__init__.pyi
 src/matplotlib-stubs/__init__.pyi
 src/matplotlib-stubs/animation.pyi
 src/matplotlib-stubs/cm.pyi
 src/matplotlib-stubs/colors.pyi
 src/matplotlib-stubs/figure.pyi
```

### Comparing `scientific_plots-1.5.2/src/scipy-stubs/fft.pyi` & `scientific_plots-1.5.3/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.5.3/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.5.3/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.5.3/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.5.3/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/tests/test_plot_manual.py` & `scientific_plots-1.5.3/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/tests/test_plots.py` & `scientific_plots-1.5.3/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/tests/test_types.py` & `scientific_plots-1.5.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.2/tests/test_utilties.py` & `scientific_plots-1.5.3/tests/test_utilties.py`

 * *Files identical despite different names*

