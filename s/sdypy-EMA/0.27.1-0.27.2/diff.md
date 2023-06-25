# Comparing `tmp/sdypy-EMA-0.27.1.tar.gz` & `tmp/sdypy-EMA-0.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy-EMA-0.27.1.tar", last modified: Sat Jun 24 09:21:49 2023, max compression
+gzip compressed data, was "sdypy-EMA-0.27.2.tar", last modified: Sun Jun 25 08:53:34 2023, max compression
```

## Comparing `sdypy-EMA-0.27.1.tar` & `sdypy-EMA-0.27.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/
--rw-rw-rw-   0        0        0     1091 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/LICENSE
--rw-rw-rw-   0        0        0     2913 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/PKG-INFO
--rw-rw-rw-   0        0        0     2489 2023-04-18 12:59:27.000000 sdypy-EMA-0.27.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.728487 sdypy-EMA-0.27.1/sdypy/
-drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/sdypy/EMA/
--rw-rw-rw-   0        0        0    40490 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/EMA.py
--rw-rw-rw-   0        0        0      176 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/__init__.py
--rw-rw-rw-   0        0        0     4779 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/sdypy/EMA/normal_modes.py
--rw-rw-rw-   0        0        0    18198 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/sdypy/EMA/pole_picking.py
--rw-rw-rw-   0        0        0     3516 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/stabilization.py
--rw-rw-rw-   0        0        0     4648 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/
--rw-rw-rw-   0        0        0     2913 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/setup.cfg
--rw-rw-rw-   0        0        0     1525 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-06 08:43:43.000000 sdypy-EMA-0.27.2/LICENSE
+-rw-rw-rw-   0        0        0     2874 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2489 2023-06-05 05:25:44.000000 sdypy-EMA-0.27.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-25 08:53:34.527446 sdypy-EMA-0.27.2/sdypy/
+drwxrwxrwx   0        0        0        0 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/sdypy/EMA/
+-rw-rw-rw-   0        0        0    40490 2023-06-24 08:41:06.000000 sdypy-EMA-0.27.2/sdypy/EMA/EMA.py
+-rw-rw-rw-   0        0        0      176 2023-06-25 08:51:59.000000 sdypy-EMA-0.27.2/sdypy/EMA/__init__.py
+-rw-rw-rw-   0        0        0     4779 2023-06-05 05:25:44.000000 sdypy-EMA-0.27.2/sdypy/EMA/normal_modes.py
+-rw-rw-rw-   0        0        0    18198 2023-06-05 05:25:44.000000 sdypy-EMA-0.27.2/sdypy/EMA/pole_picking.py
+-rw-rw-rw-   0        0        0     3522 2023-06-25 08:51:53.000000 sdypy-EMA-0.27.2/sdypy/EMA/stabilization.py
+-rw-rw-rw-   0        0        0     4648 2023-06-24 08:53:18.000000 sdypy-EMA-0.27.2/sdypy/EMA/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/
+-rw-rw-rw-   0        0        0     2874 2023-06-25 08:53:34.000000 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-25 08:53:34.000000 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:53:34.000000 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-25 08:53:34.000000 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 08:53:34.000000 sdypy-EMA-0.27.2/sdypy_EMA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-06-24 08:59:32.000000 sdypy-EMA-0.27.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:53:34.537481 sdypy-EMA-0.27.2/tests/
+-rw-rw-rw-   0        0        0     1400 2023-06-06 11:05:22.000000 sdypy-EMA-0.27.2/tests/test_basic.py
+-rw-rw-rw-   0        0        0     4113 2023-06-06 11:03:21.000000 sdypy-EMA-0.27.2/tests/test_data.py
```

### Comparing `sdypy-EMA-0.27.1/LICENSE` & `sdypy-EMA-0.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/PKG-INFO` & `sdypy-EMA-0.27.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.27.1
+Version: 0.27.2
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sdypy-EMA
 =========
 
 Experimental and operational modal analysis
@@ -114,8 +112,7 @@
    :target: https://doi.org/10.5281/zenodo.4016671
 
 .. _sdypy: https://github.com/sdypy/sdypy
 
 .. _pyEMA: https://github.com/ladisk/pyEMA
 
 .. _pyUFF: https://pypi.org/project/pyuff/
-
```

### Comparing `sdypy-EMA-0.27.1/README.rst` & `sdypy-EMA-0.27.2/README.rst`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/sdypy/EMA/EMA.py` & `sdypy-EMA-0.27.2/sdypy/EMA/EMA.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/sdypy/EMA/normal_modes.py` & `sdypy-EMA-0.27.2/sdypy/EMA/normal_modes.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/sdypy/EMA/pole_picking.py` & `sdypy-EMA-0.27.2/sdypy/EMA/pole_picking.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/sdypy/EMA/stabilization.py` & `sdypy-EMA-0.27.2/sdypy/EMA/stabilization.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                 xi_temp[:, n-2][xi_temp[:, n-2] == 0] = 1e-10
                 
                 fn_test[i, np.abs((fn[i] - fn_temp[:, n-2]) /
                                 fn_temp[:, n-2]) < err_fn] = 1
                 xi_test[i, np.abs((xi[i] - xi_temp[:, n-2]) /
                                 xi_temp[:, n-2]) < err_xi] = 1
 
-                fn_temp[i, n - 1] = fn[i]
-                xi_temp[i, n - 1] = xi[i]
+                fn_temp[i, n - 1] = fn[i][0]
+                xi_temp[i, n - 1] = xi[i][0]
 
                 test_fn[i, n-1] = np.sum(fn_test[i, :2*n])
                 test_xi[i, n-1] = np.sum(xi_test[i, :2*n])
 
     return fn_temp, xi_temp, test_fn, test_xi
```

### Comparing `sdypy-EMA-0.27.1/sdypy/EMA/tools.py` & `sdypy-EMA-0.27.2/sdypy/EMA/tools.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27.1/sdypy_EMA.egg-info/PKG-INFO` & `sdypy-EMA-0.27.2/sdypy_EMA.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.27.1
+Version: 0.27.2
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sdypy-EMA
 =========
 
 Experimental and operational modal analysis
@@ -114,8 +112,7 @@
    :target: https://doi.org/10.5281/zenodo.4016671
 
 .. _sdypy: https://github.com/sdypy/sdypy
 
 .. _pyEMA: https://github.com/ladisk/pyEMA
 
 .. _pyUFF: https://pypi.org/project/pyuff/
-
```

### Comparing `sdypy-EMA-0.27.1/setup.py` & `sdypy-EMA-0.27.2/setup.py`

 * *Files identical despite different names*

