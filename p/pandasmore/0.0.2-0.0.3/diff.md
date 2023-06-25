# Comparing `tmp/pandasmore-0.0.2.tar.gz` & `tmp/pandasmore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmore-0.0.2.tar", last modified: Sun Jun 25 13:05:24 2023, max compression
+gzip compressed data, was "pandasmore-0.0.3.tar", last modified: Sun Jun 25 13:22:18 2023, max compression
```

## Comparing `pandasmore-0.0.2.tar` & `pandasmore-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:23.996715 pandasmore-0.0.2/.github/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/.github/workflows/
--rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.github/workflows/deploy.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.gitignore
--rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.2/LICENSE
--rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.2/MANIFEST.in
--rw-rw-r--   0 imb       (1000) imb       (1000)     4772 2023-06-25 13:05:24.000715 pandasmore-0.0.2/PKG-INFO
--rw-rw-r--   0 imb       (1000) imb       (1000)     3951 2023-06-25 12:55:28.000000 pandasmore-0.0.2/README.md
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/nbs/
--rw-r--r--   0 imb       (1000) imb       (1000)    61779 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/00_core.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.2/nbs/_quarto.yml
--rw-r--r--   0 imb       (1000) imb       (1000)    14674 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/index.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/nbdev.yml
--rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.2/nbs/sidebar.yml
--rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.2/nbs/styles.css
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/pandasmore/
--rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     1576 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/_modidx.py
--rw-r--r--   0 imb       (1000) imb       (1000)    12540 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/core.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/pandasmore.egg-info/
--rw-r--r--   0 imb       (1000) imb       (1000)     4772 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)      518 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/SOURCES.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/dependency_links.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/entry_points.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.2/pandasmore.egg-info/not-zip-safe
--rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/requires.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/top_level.txt
--rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-06-25 12:55:00.000000 pandasmore-0.0.2/settings.ini
--rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-25 13:05:24.000715 pandasmore-0.0.2/setup.cfg
--rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.2/setup.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.673146 pandasmore-0.0.3/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.665146 pandasmore-0.0.3/.github/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/.github/workflows/
+-rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.github/workflows/deploy.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.gitignore
+-rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.3/LICENSE
+-rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.3/MANIFEST.in
+-rw-rw-r--   0 imb       (1000) imb       (1000)     4779 2023-06-25 13:22:18.669146 pandasmore-0.0.3/PKG-INFO
+-rw-rw-r--   0 imb       (1000) imb       (1000)     3958 2023-06-25 13:21:43.000000 pandasmore-0.0.3/README.md
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/nbs/
+-rw-r--r--   0 imb       (1000) imb       (1000)    61779 2023-06-25 12:55:13.000000 pandasmore-0.0.3/nbs/00_core.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.3/nbs/_quarto.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)    14681 2023-06-25 13:20:37.000000 pandasmore-0.0.3/nbs/index.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-06-25 13:21:39.000000 pandasmore-0.0.3/nbs/nbdev.yml
+-rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.3/nbs/sidebar.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.3/nbs/styles.css
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/pandasmore/
+-rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/__init__.py
+-rw-rw-r--   0 imb       (1000) imb       (1000)     1576 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/_modidx.py
+-rw-r--r--   0 imb       (1000) imb       (1000)    12540 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/core.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/pandasmore.egg-info/
+-rw-r--r--   0 imb       (1000) imb       (1000)     4779 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/PKG-INFO
+-rw-r--r--   0 imb       (1000) imb       (1000)      518 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/SOURCES.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/dependency_links.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/entry_points.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.3/pandasmore.egg-info/not-zip-safe
+-rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/requires.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/top_level.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-06-25 13:21:28.000000 pandasmore-0.0.3/settings.ini
+-rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-25 13:22:18.673146 pandasmore-0.0.3/setup.cfg
+-rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.3/setup.py
```

### Comparing `pandasmore-0.0.2/.gitignore` & `pandasmore-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/LICENSE` & `pandasmore-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/PKG-INFO` & `pandasmore-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extends pandas with common functions used in finance and economics research
 Home-page: https://github.com/ionmihai/pandasmore
 Author: ionmihai
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -51,15 +51,15 @@
 
 First, we set up an example dataset to showcase the functions in this
 module.
 
 ``` python
 import pandas as pd
 import numpy as np
-import pandasmore as pdr
+import pandasmore as pdm
 ```
 
 ``` python
 raw = pd.DataFrame(np.random.rand(15,2), 
                     columns=list('AB'), 
                     index=pd.MultiIndex.from_product(
                         [[1,2, np.nan],[np.nan,'2010-01','2010-02','2010-02','2010-04']],
@@ -68,77 +68,77 @@
 raw
 ```
 
 <div>
 
 |     | firm_id | date    | A        | B        |
 |-----|---------|---------|----------|----------|
-| 0   | 1.0     | NaN     | 0.943132 | 0.981995 |
-| 1   | 1.0     | 2010-01 | 0.328816 | 0.473158 |
-| 2   | 1.0     | 2010-02 | 0.177921 | 0.835497 |
-| 3   | 1.0     | 2010-02 | 0.928199 | 0.743025 |
-| 4   | 1.0     | 2010-04 | 0.857208 | 0.742693 |
-| 5   | 2.0     | NaN     | 0.147470 | 0.357477 |
-| 6   | 2.0     | 2010-01 | 0.172676 | 0.978518 |
-| 7   | 2.0     | 2010-02 | 0.391758 | 0.574734 |
-| 8   | 2.0     | 2010-02 | 0.824737 | 0.863340 |
-| 9   | 2.0     | 2010-04 | 0.847638 | 0.293925 |
-| 10  | NaN     | NaN     | 0.969513 | 0.842419 |
-| 11  | NaN     | 2010-01 | 0.491236 | 0.194837 |
-| 12  | NaN     | 2010-02 | 0.854151 | 0.267796 |
-| 13  | NaN     | 2010-02 | 0.461259 | 0.010185 |
-| 14  | NaN     | 2010-04 | 0.735704 | 0.601400 |
+| 0   | 1.0     | NaN     | 0.249370 | 0.926335 |
+| 1   | 1.0     | 2010-01 | 0.282501 | 0.513859 |
+| 2   | 1.0     | 2010-02 | 0.804278 | 0.307171 |
+| 3   | 1.0     | 2010-02 | 0.828895 | 0.746789 |
+| 4   | 1.0     | 2010-04 | 0.569099 | 0.331814 |
+| 5   | 2.0     | NaN     | 0.533977 | 0.823457 |
+| 6   | 2.0     | 2010-01 | 0.207558 | 0.401378 |
+| 7   | 2.0     | 2010-02 | 0.086001 | 0.959371 |
+| 8   | 2.0     | 2010-02 | 0.054230 | 0.993980 |
+| 9   | 2.0     | 2010-04 | 0.062525 | 0.200272 |
+| 10  | NaN     | NaN     | 0.091012 | 0.635409 |
+| 11  | NaN     | 2010-01 | 0.866369 | 0.972394 |
+| 12  | NaN     | 2010-02 | 0.432087 | 0.837597 |
+| 13  | NaN     | 2010-02 | 0.878219 | 0.148009 |
+| 14  | NaN     | 2010-04 | 0.820386 | 0.834821 |
 
 </div>
 
 ``` python
-df = pdr.setup_tseries(raw.query('firm_id==1'),
+df = pdm.setup_tseries(raw.query('firm_id==1'),
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         | date    | dtdate     | firm_id | A        | B        |
 |---------|---------|------------|---------|----------|----------|
 | Mdate   |         |            |         |          |          |
-| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.328816 | 0.473158 |
-| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.928199 | 0.743025 |
-| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.857208 | 0.742693 |
+| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.282501 | 0.513859 |
+| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.828895 | 0.746789 |
+| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.569099 | 0.331814 |
 
 </div>
 
 ``` python
-df = pdr.setup_panel(raw,
+df = pdm.setup_panel(raw,
                         panel_ids='firm_id',
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         |         | date    | dtdate     | A        | B        |
 |---------|---------|---------|------------|----------|----------|
 | firm_id | Mdate   |         |            |          |          |
-| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.328816 | 0.473158 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.928199 | 0.743025 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.857208 | 0.742693 |
-| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.172676 | 0.978518 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.824737 | 0.863340 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.847638 | 0.293925 |
+| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.282501 | 0.513859 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.828895 | 0.746789 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.569099 | 0.331814 |
+| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.207558 | 0.401378 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.054230 | 0.993980 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.062525 | 0.200272 |
 
 </div>
 
 ``` python
-pdr.lag(df['A'])
+pdm.lag(df['A'])
 ```
 
-    permno  Mdate  
-    1       2010-01         NaN
-            2010-02    0.698770
-            2010-04         NaN
-    2       2010-01         NaN
-            2010-02    0.834091
-            2010-04         NaN
+    firm_id  Mdate  
+    1        2010-01         NaN
+             2010-02    0.282501
+             2010-04         NaN
+    2        2010-01         NaN
+             2010-02    0.207558
+             2010-04         NaN
     Name: A_lag1, dtype: float64
```

### Comparing `pandasmore-0.0.2/README.md` & `pandasmore-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 First, we set up an example dataset to showcase the functions in this
 module.
 
 ``` python
 import pandas as pd
 import numpy as np
-import pandasmore as pdr
+import pandasmore as pdm
 ```
 
 ``` python
 raw = pd.DataFrame(np.random.rand(15,2), 
                     columns=list('AB'), 
                     index=pd.MultiIndex.from_product(
                         [[1,2, np.nan],[np.nan,'2010-01','2010-02','2010-02','2010-04']],
@@ -46,77 +46,77 @@
 raw
 ```
 
 <div>
 
 |     | firm_id | date    | A        | B        |
 |-----|---------|---------|----------|----------|
-| 0   | 1.0     | NaN     | 0.943132 | 0.981995 |
-| 1   | 1.0     | 2010-01 | 0.328816 | 0.473158 |
-| 2   | 1.0     | 2010-02 | 0.177921 | 0.835497 |
-| 3   | 1.0     | 2010-02 | 0.928199 | 0.743025 |
-| 4   | 1.0     | 2010-04 | 0.857208 | 0.742693 |
-| 5   | 2.0     | NaN     | 0.147470 | 0.357477 |
-| 6   | 2.0     | 2010-01 | 0.172676 | 0.978518 |
-| 7   | 2.0     | 2010-02 | 0.391758 | 0.574734 |
-| 8   | 2.0     | 2010-02 | 0.824737 | 0.863340 |
-| 9   | 2.0     | 2010-04 | 0.847638 | 0.293925 |
-| 10  | NaN     | NaN     | 0.969513 | 0.842419 |
-| 11  | NaN     | 2010-01 | 0.491236 | 0.194837 |
-| 12  | NaN     | 2010-02 | 0.854151 | 0.267796 |
-| 13  | NaN     | 2010-02 | 0.461259 | 0.010185 |
-| 14  | NaN     | 2010-04 | 0.735704 | 0.601400 |
+| 0   | 1.0     | NaN     | 0.249370 | 0.926335 |
+| 1   | 1.0     | 2010-01 | 0.282501 | 0.513859 |
+| 2   | 1.0     | 2010-02 | 0.804278 | 0.307171 |
+| 3   | 1.0     | 2010-02 | 0.828895 | 0.746789 |
+| 4   | 1.0     | 2010-04 | 0.569099 | 0.331814 |
+| 5   | 2.0     | NaN     | 0.533977 | 0.823457 |
+| 6   | 2.0     | 2010-01 | 0.207558 | 0.401378 |
+| 7   | 2.0     | 2010-02 | 0.086001 | 0.959371 |
+| 8   | 2.0     | 2010-02 | 0.054230 | 0.993980 |
+| 9   | 2.0     | 2010-04 | 0.062525 | 0.200272 |
+| 10  | NaN     | NaN     | 0.091012 | 0.635409 |
+| 11  | NaN     | 2010-01 | 0.866369 | 0.972394 |
+| 12  | NaN     | 2010-02 | 0.432087 | 0.837597 |
+| 13  | NaN     | 2010-02 | 0.878219 | 0.148009 |
+| 14  | NaN     | 2010-04 | 0.820386 | 0.834821 |
 
 </div>
 
 ``` python
-df = pdr.setup_tseries(raw.query('firm_id==1'),
+df = pdm.setup_tseries(raw.query('firm_id==1'),
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         | date    | dtdate     | firm_id | A        | B        |
 |---------|---------|------------|---------|----------|----------|
 | Mdate   |         |            |         |          |          |
-| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.328816 | 0.473158 |
-| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.928199 | 0.743025 |
-| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.857208 | 0.742693 |
+| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.282501 | 0.513859 |
+| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.828895 | 0.746789 |
+| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.569099 | 0.331814 |
 
 </div>
 
 ``` python
-df = pdr.setup_panel(raw,
+df = pdm.setup_panel(raw,
                         panel_ids='firm_id',
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         |         | date    | dtdate     | A        | B        |
 |---------|---------|---------|------------|----------|----------|
 | firm_id | Mdate   |         |            |          |          |
-| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.328816 | 0.473158 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.928199 | 0.743025 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.857208 | 0.742693 |
-| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.172676 | 0.978518 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.824737 | 0.863340 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.847638 | 0.293925 |
+| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.282501 | 0.513859 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.828895 | 0.746789 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.569099 | 0.331814 |
+| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.207558 | 0.401378 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.054230 | 0.993980 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.062525 | 0.200272 |
 
 </div>
 
 ``` python
-pdr.lag(df['A'])
+pdm.lag(df['A'])
 ```
 
-    permno  Mdate  
-    1       2010-01         NaN
-            2010-02    0.698770
-            2010-04         NaN
-    2       2010-01         NaN
-            2010-02    0.834091
-            2010-04         NaN
+    firm_id  Mdate  
+    1        2010-01         NaN
+             2010-02    0.282501
+             2010-04         NaN
+    2        2010-01         NaN
+             2010-02    0.207558
+             2010-04         NaN
     Name: A_lag1, dtype: float64
```

### Comparing `pandasmore-0.0.2/nbs/00_core.ipynb` & `pandasmore-0.0.3/nbs/00_core.ipynb`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/nbs/index.ipynb` & `pandasmore-0.0.3/nbs/index.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997694907293293%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(2, 'import pandasmore as pdm')], delete: [2]}}, 8: "*

 * *            "{'outputs': {0: {'data': {'text/html': {insert: [(29, '      <td>0.249370</td>\\n'), "*

 * *            "(30, '      <td>0.926335</td>\\n'), (36, '      <td>0.282501</td>\\n'), (37, '      "*

 * *            "<td>0.513859</td>\\n'), (43, '      <td>0.804278</td>\\n'), (44, '      "*

 * *            "<td>0.307171</td>\\n'), (50, '      <td>0.828895</td>\\n'), (51, '      "*

 * *            "<td>0.746789</td>\\n'), (57, '     […]*

```diff
@@ -73,15 +73,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import numpy as np\n",
-                "import pandasmore as pdr"
+                "import pandasmore as pdm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
@@ -113,136 +113,136 @@
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.943132</td>\n",
-                            "      <td>0.981995</td>\n",
+                            "      <td>0.249370</td>\n",
+                            "      <td>0.926335</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.328816</td>\n",
-                            "      <td>0.473158</td>\n",
+                            "      <td>0.282501</td>\n",
+                            "      <td>0.513859</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.177921</td>\n",
-                            "      <td>0.835497</td>\n",
+                            "      <td>0.804278</td>\n",
+                            "      <td>0.307171</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.928199</td>\n",
-                            "      <td>0.743025</td>\n",
+                            "      <td>0.828895</td>\n",
+                            "      <td>0.746789</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.857208</td>\n",
-                            "      <td>0.742693</td>\n",
+                            "      <td>0.569099</td>\n",
+                            "      <td>0.331814</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.147470</td>\n",
-                            "      <td>0.357477</td>\n",
+                            "      <td>0.533977</td>\n",
+                            "      <td>0.823457</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.172676</td>\n",
-                            "      <td>0.978518</td>\n",
+                            "      <td>0.207558</td>\n",
+                            "      <td>0.401378</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.391758</td>\n",
-                            "      <td>0.574734</td>\n",
+                            "      <td>0.086001</td>\n",
+                            "      <td>0.959371</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.824737</td>\n",
-                            "      <td>0.863340</td>\n",
+                            "      <td>0.054230</td>\n",
+                            "      <td>0.993980</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.847638</td>\n",
-                            "      <td>0.293925</td>\n",
+                            "      <td>0.062525</td>\n",
+                            "      <td>0.200272</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.969513</td>\n",
-                            "      <td>0.842419</td>\n",
+                            "      <td>0.091012</td>\n",
+                            "      <td>0.635409</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.491236</td>\n",
-                            "      <td>0.194837</td>\n",
+                            "      <td>0.866369</td>\n",
+                            "      <td>0.972394</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.854151</td>\n",
-                            "      <td>0.267796</td>\n",
+                            "      <td>0.432087</td>\n",
+                            "      <td>0.837597</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.461259</td>\n",
-                            "      <td>0.010185</td>\n",
+                            "      <td>0.878219</td>\n",
+                            "      <td>0.148009</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.735704</td>\n",
-                            "      <td>0.601400</td>\n",
+                            "      <td>0.820386</td>\n",
+                            "      <td>0.834821</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "    firm_id     date         A         B\n",
-                            "0       1.0      NaN  0.943132  0.981995\n",
-                            "1       1.0  2010-01  0.328816  0.473158\n",
-                            "2       1.0  2010-02  0.177921  0.835497\n",
-                            "3       1.0  2010-02  0.928199  0.743025\n",
-                            "4       1.0  2010-04  0.857208  0.742693\n",
-                            "5       2.0      NaN  0.147470  0.357477\n",
-                            "6       2.0  2010-01  0.172676  0.978518\n",
-                            "7       2.0  2010-02  0.391758  0.574734\n",
-                            "8       2.0  2010-02  0.824737  0.863340\n",
-                            "9       2.0  2010-04  0.847638  0.293925\n",
-                            "10      NaN      NaN  0.969513  0.842419\n",
-                            "11      NaN  2010-01  0.491236  0.194837\n",
-                            "12      NaN  2010-02  0.854151  0.267796\n",
-                            "13      NaN  2010-02  0.461259  0.010185\n",
-                            "14      NaN  2010-04  0.735704  0.601400"
+                            "0       1.0      NaN  0.249370  0.926335\n",
+                            "1       1.0  2010-01  0.282501  0.513859\n",
+                            "2       1.0  2010-02  0.804278  0.307171\n",
+                            "3       1.0  2010-02  0.828895  0.746789\n",
+                            "4       1.0  2010-04  0.569099  0.331814\n",
+                            "5       2.0      NaN  0.533977  0.823457\n",
+                            "6       2.0  2010-01  0.207558  0.401378\n",
+                            "7       2.0  2010-02  0.086001  0.959371\n",
+                            "8       2.0  2010-02  0.054230  0.993980\n",
+                            "9       2.0  2010-04  0.062525  0.200272\n",
+                            "10      NaN      NaN  0.091012  0.635409\n",
+                            "11      NaN  2010-01  0.866369  0.972394\n",
+                            "12      NaN  2010-02  0.432087  0.837597\n",
+                            "13      NaN  2010-02  0.878219  0.148009\n",
+                            "14      NaN  2010-04  0.820386  0.834821"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -299,52 +299,52 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.328816</td>\n",
-                            "      <td>0.473158</td>\n",
+                            "      <td>0.282501</td>\n",
+                            "      <td>0.513859</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.928199</td>\n",
-                            "      <td>0.743025</td>\n",
+                            "      <td>0.828895</td>\n",
+                            "      <td>0.746789</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.857208</td>\n",
-                            "      <td>0.742693</td>\n",
+                            "      <td>0.569099</td>\n",
+                            "      <td>0.331814</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "            date     dtdate  firm_id         A         B\n",
                             "Mdate                                                   \n",
-                            "2010-01  2010-01 2010-01-01      1.0  0.328816  0.473158\n",
-                            "2010-02  2010-02 2010-02-01      1.0  0.928199  0.743025\n",
-                            "2010-04  2010-04 2010-04-01      1.0  0.857208  0.742693"
+                            "2010-01  2010-01 2010-01-01      1.0  0.282501  0.513859\n",
+                            "2010-02  2010-02 2010-02-01      1.0  0.828895  0.746789\n",
+                            "2010-04  2010-04 2010-04-01      1.0  0.569099  0.331814"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df = pdr.setup_tseries(raw.query('firm_id==1'),\n",
+                "df = pdm.setup_tseries(raw.query('firm_id==1'),\n",
                 "                        time_var='date', time_var_format=\"%Y-%m\",\n",
                 "                        freq='M')\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
@@ -389,106 +389,106 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.328816</td>\n",
-                            "      <td>0.473158</td>\n",
+                            "      <td>0.282501</td>\n",
+                            "      <td>0.513859</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.928199</td>\n",
-                            "      <td>0.743025</td>\n",
+                            "      <td>0.828895</td>\n",
+                            "      <td>0.746789</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.857208</td>\n",
-                            "      <td>0.742693</td>\n",
+                            "      <td>0.569099</td>\n",
+                            "      <td>0.331814</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.172676</td>\n",
-                            "      <td>0.978518</td>\n",
+                            "      <td>0.207558</td>\n",
+                            "      <td>0.401378</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.824737</td>\n",
-                            "      <td>0.863340</td>\n",
+                            "      <td>0.054230</td>\n",
+                            "      <td>0.993980</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.847638</td>\n",
-                            "      <td>0.293925</td>\n",
+                            "      <td>0.062525</td>\n",
+                            "      <td>0.200272</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                    date     dtdate         A         B\n",
                             "firm_id Mdate                                          \n",
-                            "1       2010-01  2010-01 2010-01-01  0.328816  0.473158\n",
-                            "        2010-02  2010-02 2010-02-01  0.928199  0.743025\n",
-                            "        2010-04  2010-04 2010-04-01  0.857208  0.742693\n",
-                            "2       2010-01  2010-01 2010-01-01  0.172676  0.978518\n",
-                            "        2010-02  2010-02 2010-02-01  0.824737  0.863340\n",
-                            "        2010-04  2010-04 2010-04-01  0.847638  0.293925"
+                            "1       2010-01  2010-01 2010-01-01  0.282501  0.513859\n",
+                            "        2010-02  2010-02 2010-02-01  0.828895  0.746789\n",
+                            "        2010-04  2010-04 2010-04-01  0.569099  0.331814\n",
+                            "2       2010-01  2010-01 2010-01-01  0.207558  0.401378\n",
+                            "        2010-02  2010-02 2010-02-01  0.054230  0.993980\n",
+                            "        2010-04  2010-04 2010-04-01  0.062525  0.200272"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df = pdr.setup_panel(raw,\n",
+                "df = pdm.setup_panel(raw,\n",
                 "                        panel_ids='firm_id',\n",
                 "                        time_var='date', time_var_format=\"%Y-%m\",\n",
                 "                        freq='M')\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "permno  Mdate  \n",
-                            "1       2010-01         NaN\n",
-                            "        2010-02    0.698770\n",
-                            "        2010-04         NaN\n",
-                            "2       2010-01         NaN\n",
-                            "        2010-02    0.834091\n",
-                            "        2010-04         NaN\n",
+                            "firm_id  Mdate  \n",
+                            "1        2010-01         NaN\n",
+                            "         2010-02    0.282501\n",
+                            "         2010-04         NaN\n",
+                            "2        2010-01         NaN\n",
+                            "         2010-02    0.207558\n",
+                            "         2010-04         NaN\n",
                             "Name: A_lag1, dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "pdr.lag(df['A'])"
+                "pdm.lag(df['A'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pandasmore-0.0.2/nbs/styles.css` & `pandasmore-0.0.3/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/pandasmore/_modidx.py` & `pandasmore-0.0.3/pandasmore/_modidx.py`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/pandasmore/core.py` & `pandasmore-0.0.3/pandasmore/core.py`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/pandasmore.egg-info/PKG-INFO` & `pandasmore-0.0.3/pandasmore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extends pandas with common functions used in finance and economics research
 Home-page: https://github.com/ionmihai/pandasmore
 Author: ionmihai
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -51,15 +51,15 @@
 
 First, we set up an example dataset to showcase the functions in this
 module.
 
 ``` python
 import pandas as pd
 import numpy as np
-import pandasmore as pdr
+import pandasmore as pdm
 ```
 
 ``` python
 raw = pd.DataFrame(np.random.rand(15,2), 
                     columns=list('AB'), 
                     index=pd.MultiIndex.from_product(
                         [[1,2, np.nan],[np.nan,'2010-01','2010-02','2010-02','2010-04']],
@@ -68,77 +68,77 @@
 raw
 ```
 
 <div>
 
 |     | firm_id | date    | A        | B        |
 |-----|---------|---------|----------|----------|
-| 0   | 1.0     | NaN     | 0.943132 | 0.981995 |
-| 1   | 1.0     | 2010-01 | 0.328816 | 0.473158 |
-| 2   | 1.0     | 2010-02 | 0.177921 | 0.835497 |
-| 3   | 1.0     | 2010-02 | 0.928199 | 0.743025 |
-| 4   | 1.0     | 2010-04 | 0.857208 | 0.742693 |
-| 5   | 2.0     | NaN     | 0.147470 | 0.357477 |
-| 6   | 2.0     | 2010-01 | 0.172676 | 0.978518 |
-| 7   | 2.0     | 2010-02 | 0.391758 | 0.574734 |
-| 8   | 2.0     | 2010-02 | 0.824737 | 0.863340 |
-| 9   | 2.0     | 2010-04 | 0.847638 | 0.293925 |
-| 10  | NaN     | NaN     | 0.969513 | 0.842419 |
-| 11  | NaN     | 2010-01 | 0.491236 | 0.194837 |
-| 12  | NaN     | 2010-02 | 0.854151 | 0.267796 |
-| 13  | NaN     | 2010-02 | 0.461259 | 0.010185 |
-| 14  | NaN     | 2010-04 | 0.735704 | 0.601400 |
+| 0   | 1.0     | NaN     | 0.249370 | 0.926335 |
+| 1   | 1.0     | 2010-01 | 0.282501 | 0.513859 |
+| 2   | 1.0     | 2010-02 | 0.804278 | 0.307171 |
+| 3   | 1.0     | 2010-02 | 0.828895 | 0.746789 |
+| 4   | 1.0     | 2010-04 | 0.569099 | 0.331814 |
+| 5   | 2.0     | NaN     | 0.533977 | 0.823457 |
+| 6   | 2.0     | 2010-01 | 0.207558 | 0.401378 |
+| 7   | 2.0     | 2010-02 | 0.086001 | 0.959371 |
+| 8   | 2.0     | 2010-02 | 0.054230 | 0.993980 |
+| 9   | 2.0     | 2010-04 | 0.062525 | 0.200272 |
+| 10  | NaN     | NaN     | 0.091012 | 0.635409 |
+| 11  | NaN     | 2010-01 | 0.866369 | 0.972394 |
+| 12  | NaN     | 2010-02 | 0.432087 | 0.837597 |
+| 13  | NaN     | 2010-02 | 0.878219 | 0.148009 |
+| 14  | NaN     | 2010-04 | 0.820386 | 0.834821 |
 
 </div>
 
 ``` python
-df = pdr.setup_tseries(raw.query('firm_id==1'),
+df = pdm.setup_tseries(raw.query('firm_id==1'),
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         | date    | dtdate     | firm_id | A        | B        |
 |---------|---------|------------|---------|----------|----------|
 | Mdate   |         |            |         |          |          |
-| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.328816 | 0.473158 |
-| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.928199 | 0.743025 |
-| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.857208 | 0.742693 |
+| 2010-01 | 2010-01 | 2010-01-01 | 1.0     | 0.282501 | 0.513859 |
+| 2010-02 | 2010-02 | 2010-02-01 | 1.0     | 0.828895 | 0.746789 |
+| 2010-04 | 2010-04 | 2010-04-01 | 1.0     | 0.569099 | 0.331814 |
 
 </div>
 
 ``` python
-df = pdr.setup_panel(raw,
+df = pdm.setup_panel(raw,
                         panel_ids='firm_id',
                         time_var='date', time_var_format="%Y-%m",
                         freq='M')
 df
 ```
 
 <div>
 
 |         |         | date    | dtdate     | A        | B        |
 |---------|---------|---------|------------|----------|----------|
 | firm_id | Mdate   |         |            |          |          |
-| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.328816 | 0.473158 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.928199 | 0.743025 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.857208 | 0.742693 |
-| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.172676 | 0.978518 |
-|         | 2010-02 | 2010-02 | 2010-02-01 | 0.824737 | 0.863340 |
-|         | 2010-04 | 2010-04 | 2010-04-01 | 0.847638 | 0.293925 |
+| 1       | 2010-01 | 2010-01 | 2010-01-01 | 0.282501 | 0.513859 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.828895 | 0.746789 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.569099 | 0.331814 |
+| 2       | 2010-01 | 2010-01 | 2010-01-01 | 0.207558 | 0.401378 |
+|         | 2010-02 | 2010-02 | 2010-02-01 | 0.054230 | 0.993980 |
+|         | 2010-04 | 2010-04 | 2010-04-01 | 0.062525 | 0.200272 |
 
 </div>
 
 ``` python
-pdr.lag(df['A'])
+pdm.lag(df['A'])
 ```
 
-    permno  Mdate  
-    1       2010-01         NaN
-            2010-02    0.698770
-            2010-04         NaN
-    2       2010-01         NaN
-            2010-02    0.834091
-            2010-04         NaN
+    firm_id  Mdate  
+    1        2010-01         NaN
+             2010-02    0.282501
+             2010-04         NaN
+    2        2010-01         NaN
+             2010-02    0.207558
+             2010-04         NaN
     Name: A_lag1, dtype: float64
```

### Comparing `pandasmore-0.0.2/pandasmore.egg-info/SOURCES.txt` & `pandasmore-0.0.3/pandasmore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.2/settings.ini` & `pandasmore-0.0.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pandasmore
 lib_name = pandasmore
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pandasmore
 nbs_path = nbs
 recursive = True
```

### Comparing `pandasmore-0.0.2/setup.py` & `pandasmore-0.0.3/setup.py`

 * *Files identical despite different names*

