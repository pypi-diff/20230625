# Comparing `tmp/scientific_plots-1.5.3.tar.gz` & `tmp/scientific_plots-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.5.3.tar", last modified: Sun Jun 25 00:18:23 2023, max compression
+gzip compressed data, was "scientific_plots-1.5.4.tar", last modified: Sun Jun 25 08:09:58 2023, max compression
```

## Comparing `scientific_plots-1.5.3.tar` & `scientific_plots-1.5.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-24 23:18:51.000000 scientific_plots-1.5.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    11604 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-24 23:56:16.000000 scientific_plots-1.5.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.3/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.3/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.599568 scientific_plots-1.5.3/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.3/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-24 23:10:04.000000 scientific_plots-1.5.3/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18778 2023-06-24 21:33:21.000000 scientific_plots-1.5.3/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.3/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 00:17:40.000000 scientific_plots-1.5.3/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.3/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.603567 scientific_plots-1.5.3/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11604 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1360 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-25 00:18:23.000000 scientific_plots-1.5.3/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 00:18:23.607568 scientific_plots-1.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.3/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.3/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.952930 scientific_plots-1.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-24 23:56:16.000000 scientific_plots-1.5.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.4/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 08:09:58.952930 scientific_plots-1.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.940930 scientific_plots-1.5.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.4/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.4/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.4/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-06-24 21:33:21.000000 scientific_plots-1.5.4/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.4/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.4/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.4/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.944930 scientific_plots-1.5.4/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 08:09:32.000000 scientific_plots-1.5.4/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8926 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-06-25 08:09:58.000000 scientific_plots-1.5.4/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-06-25 08:09:58.000000 scientific_plots-1.5.4/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 08:09:58.000000 scientific_plots-1.5.4/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-25 08:09:58.000000 scientific_plots-1.5.4/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-25 08:09:58.000000 scientific_plots-1.5.4/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 08:09:58.948930 scientific_plots-1.5.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.4/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-06-25 08:00:18.000000 scientific_plots-1.5.4/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.4/tests/test_utilties.py
```

### Comparing `scientific_plots-1.5.3/LICENSE.txt` & `scientific_plots-1.5.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/pyproject.toml` & `scientific_plots-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/readme.md` & `scientific_plots-1.5.4/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.5.4/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.5.4/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.5.4/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.5.4/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.5.4/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.5.4/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/numba-stubs/__init__.pyi` & `scientific_plots-1.5.4/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scientific_plots/data_analysis.py` & `scientific_plots-1.5.4/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scientific_plots/default_plots.py` & `scientific_plots-1.5.4/src/scientific_plots/default_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 This module contains a few functions, which can be used to
 generate plots quickly and with useful defaults"""
 from __future__ import annotations
 from pathlib import Path
 from functools import wraps
 from typing import TypeVar, List, Tuple, Union, Callable, Optional
-from warnings import warn
+from warnings import warn, filterwarnings, catch_warnings
 from textwrap import dedent
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 import numpy as np
 from numpy import amin, amax
@@ -115,15 +115,15 @@
 
 @apply_styles
 def plot_fit(X: In, Y: In,
              fit_function: Callable[..., float],
              xlabel: str, ylabel: str, filename: Union[str, Path], *,
              args: Optional[Tuple[float]] = None,
              logscale: bool = False) -> None:
-    """craetes a plot of data and a fit and saves it to 'filename'"""
+    """Creates a plot of data and a fit and saves it to 'filename'."""
     X, Y = fix_inputs(X, Y)  # type: ignore
     if not check_inputs(
             X, Y, xlabel, ylabel):
         return
 
     n_fit = 1000
 
@@ -223,16 +223,20 @@
             MaxNLocator(nbins)
         )
         ax.yaxis.set_major_locator(
             MaxNLocator(nbins)
         )
 
     fig.set_size_inches(*figsize)
-    plt.tight_layout()
-    plt.savefig(filename)
+
+    with catch_warnings():
+        filterwarnings("ignore", message=".*Tight layout")
+        plt.tight_layout()
+        plt.savefig(filename)
+
     plt.close()
 
 
 @apply_styles
 def plot(X: In, Y: In, xlabel: str, ylabel: str,
          filename: Union[Path, str], *, logscale: bool = False,
          ylim: Optional[tuple[float, float]] = None,
```

### Comparing `scientific_plots-1.5.3/src/scientific_plots/plot_settings.py` & `scientific_plots-1.5.4/src/scientific_plots/plot_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,15 +473,16 @@
                     set_sans_serif()
                     plt.savefig = new_save_simple("presentation", german=True)
                     _plot_function(*args, **kwargs)
 
             except errors:
                 if not three_d:
                     warn(dedent(""""Could not found style 'science'.
-                                Using a fallback-style."""), RuntimeWarning)
+                                The package was probably installed incorrectly.
+                                Using a fallback-style."""), ImportWarning)
                 # journal
                 with plt.style.context("fast"):
                     set_rwth_colors(three_d)
                     set_serif()
                     plt.savefig = new_save_simple("journal")
                     _plot_function(*args, **kwargs)
```

### Comparing `scientific_plots-1.5.3/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.5.4/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scientific_plots/types_.py` & `scientific_plots-1.5.4/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scientific_plots/utilities.py` & `scientific_plots-1.5.4/src/scientific_plots/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,17 @@
     Translate the given input string from lang2 to lang1 using google
     translate.
     """
     # one letter strings
     if len(string) <= 1:
         return string
 
+    if r"\times" in string:
+        return string
+
     try:
         translator = Translator()
         result: str
         result = translator.translate(string, lang1, lang2)
     except (OSError, MaxRetryError):
         return string
     return result
```

### Comparing `scientific_plots-1.5.3/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.5.4/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.txt
+COPYING.LESSER
 pyproject.toml
 readme.md
 src/cycler-stubs/__init__.pyi
 src/hurst-stubs/__init__.pyi
 src/matplotlib-stubs/__init__.pyi
 src/matplotlib-stubs/animation.pyi
 src/matplotlib-stubs/cm.pyi
```

### Comparing `scientific_plots-1.5.3/src/scipy-stubs/fft.pyi` & `scientific_plots-1.5.4/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.5.4/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.5.4/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.5.4/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.5.4/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/tests/test_plot_manual.py` & `scientific_plots-1.5.4/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/tests/test_plots.py` & `scientific_plots-1.5.4/tests/test_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 from numpy import linspace
 from pytest import mark
 
 from scientific_plots.types_ import Vector
 from scientific_plots.plot_settings import read_data_plot
 from scientific_plots.default_plots import (
-    plot, two_plots, two_axis_plots)
+    plot, two_plots, two_axis_plots, plot_surface)
 
 
 @mark.use_style
 def test_default_plot(tmp_path: Path) -> None:
     """
     test the default plot creation by 'plot'
     """
@@ -99,7 +99,23 @@
     two_axis_plots(
         x_test, y_test1, "plot1",
         x_test, y_test2, "plot2",
         "x", "y", "y2",
         tmp_path / filename,
         ticks=([1., 10.], ["a", "b"]))
     assert exists(tmp_path / filename)
+
+
+@mark.use_style
+def test_two_d_plot(tmp_path: Path) -> None:
+    """Test the creation of a two dimensional surface plot."""
+    x_test: Vector = linspace(0, 1e8, 1000)
+    y_test: Vector = linspace(0, 1e8, 1000)
+    x_test_grid, y_test_grid = np.meshgrid(
+        x_test, y_test)
+    z_grid = x_test_grid**2 - y_test_grid
+    filename = Path(".test_two_d_plot.tmp.pdf")
+    plot_surface(
+        x_test_grid, y_test_grid, z_grid,
+        "x-label", "y-label", "z-label",
+        tmp_path / filename)
+    assert exists(tmp_path / filename)
```

### Comparing `scientific_plots-1.5.3/tests/test_types.py` & `scientific_plots-1.5.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.3/tests/test_utilties.py` & `scientific_plots-1.5.4/tests/test_utilties.py`

 * *Files identical despite different names*

