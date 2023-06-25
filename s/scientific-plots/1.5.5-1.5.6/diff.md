# Comparing `tmp/scientific_plots-1.5.5.tar.gz` & `tmp/scientific_plots-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.5.5.tar", last modified: Sun Jun 25 08:32:58 2023, max compression
+gzip compressed data, was "scientific_plots-1.5.6.tar", last modified: Sun Jun 25 09:26:09 2023, max compression
```

## Comparing `scientific_plots-1.5.5.tar` & `scientific_plots-1.5.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.5.5/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)    11607 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.5.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.5/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.892830 scientific_plots-1.5.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.892830 scientific_plots-1.5.5/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.892830 scientific_plots-1.5.5/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.892830 scientific_plots-1.5.5/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.5/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.5/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.5/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.896830 scientific_plots-1.5.5/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.5/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.5/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.896830 scientific_plots-1.5.5/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.5/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.5/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.896830 scientific_plots-1.5.5/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.896830 scientific_plots-1.5.5/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.896830 scientific_plots-1.5.5/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-25 08:15:40.000000 scientific_plots-1.5.5/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.5.5/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.5.5/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 08:32:17.000000 scientific_plots-1.5.5/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8926 2023-06-25 08:00:18.000000 scientific_plots-1.5.5/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11607 2023-06-25 08:32:58.000000 scientific_plots-1.5.5/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1363 2023-06-25 08:32:58.000000 scientific_plots-1.5.5/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 08:32:58.000000 scientific_plots-1.5.5/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-25 08:32:58.000000 scientific_plots-1.5.5/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-25 08:32:58.000000 scientific_plots-1.5.5/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:32:58.900830 scientific_plots-1.5.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.5/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2023-06-25 08:00:18.000000 scientific_plots-1.5.5/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.5/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.306044 scientific_plots-1.5.6/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.5.6/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-06-25 09:26:09.306044 scientific_plots-1.5.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.5.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.6/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 09:26:09.306044 scientific_plots-1.5.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.294044 scientific_plots-1.5.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.6/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.6/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.6/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.6/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.6/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.6/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.6/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.298044 scientific_plots-1.5.6/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.302044 scientific_plots-1.5.6/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-25 09:05:46.000000 scientific_plots-1.5.6/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.5.6/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.5.6/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 09:25:42.000000 scientific_plots-1.5.6/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.5.6/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.302044 scientific_plots-1.5.6/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-06-25 09:26:09.000000 scientific_plots-1.5.6/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-06-25 09:26:09.000000 scientific_plots-1.5.6/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:26:09.000000 scientific_plots-1.5.6/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-25 09:26:09.000000 scientific_plots-1.5.6/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-25 09:26:09.000000 scientific_plots-1.5.6/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.302044 scientific_plots-1.5.6/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.302044 scientific_plots-1.5.6/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:26:09.302044 scientific_plots-1.5.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.6/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3672 2023-06-25 09:13:03.000000 scientific_plots-1.5.6/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.6/tests/test_utilties.py
```

### Comparing `scientific_plots-1.5.5/COPYING.LESSER` & `scientific_plots-1.5.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/PKG-INFO` & `scientific_plots-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.5.5
+Version: 1.5.6
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.5.5/pyproject.toml` & `scientific_plots-1.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/readme.md` & `scientific_plots-1.5.6/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.5.6/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.5.6/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.5.6/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.5.6/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.5.6/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.5.6/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/numba-stubs/__init__.pyi` & `scientific_plots-1.5.6/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/data_analysis.py` & `scientific_plots-1.5.6/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/default_plots.py` & `scientific_plots-1.5.6/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/plot_settings.py` & `scientific_plots-1.5.6/src/scientific_plots/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.5.6/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/types_.py` & `scientific_plots-1.5.6/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scientific_plots/utilities.py` & `scientific_plots-1.5.6/src/scientific_plots/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         "valve": "Ventil",
         "relative pressure": "Relativdruck",
         "absolute pressure": "Absolutdruck",
         "relative": "relativ",
         "absolute": "absolut",
         "plot": "Graph"
     })
-    if not reverse:
+    if not reverse and r"\times" not in string:
         for key, value in _dict.items():
             if key in string.lower():
                 string = re.sub(key, value, string, flags=re.IGNORECASE)
                 break
         else:
             string = use_translator(string, "german", "english")
     else:
```

### Comparing `scientific_plots-1.5.5/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.5.6/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.5.5
+Version: 1.5.6
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.5.5/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.5.6/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scipy-stubs/fft.pyi` & `scientific_plots-1.5.6/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.5.6/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.5.6/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.5.6/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.5.6/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/tests/test_plot_manual.py` & `scientific_plots-1.5.6/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/tests/test_plots.py` & `scientific_plots-1.5.6/tests/test_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,18 +104,19 @@
         ticks=([1., 10.], ["a", "b"]))
     assert exists(tmp_path / filename)
 
 
 @mark.use_style
 def test_two_d_plot(tmp_path: Path) -> None:
     """Test the creation of a two dimensional surface plot."""
-    x_test: Vector = linspace(0, 1e8, 1000)
-    y_test: Vector = linspace(0, 1e8, 1000)
+    x_test: Vector = linspace(1, 1e8, 1000)
+    y_test: Vector = linspace(1, 1e8, 1000)
     x_test_grid, y_test_grid = np.meshgrid(
         x_test, y_test)
-    z_grid = x_test_grid**2 - y_test_grid
+    z_grid = x_test_grid**2 + y_test_grid
     filename = Path(".test_two_d_plot.tmp.pdf")
     plot_surface(
         x_test_grid, y_test_grid, z_grid,
         "x-label", "y-label", "z-label",
-        tmp_path / filename)
+        tmp_path / filename,
+        log_scale=True)
     assert exists(tmp_path / filename)
```

### Comparing `scientific_plots-1.5.5/tests/test_types.py` & `scientific_plots-1.5.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.5/tests/test_utilties.py` & `scientific_plots-1.5.6/tests/test_utilties.py`

 * *Files identical despite different names*

