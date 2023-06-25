# Comparing `tmp/labedf-1.2.0.tar.gz` & `tmp/labedf-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labedf-1.2.0.tar", last modified: Mon Feb  6 08:12:58 2023, max compression
+gzip compressed data, was "labedf-2.0.0.tar", last modified: Sun Jun 25 15:42:40 2023, max compression
```

## Comparing `labedf-1.2.0.tar` & `labedf-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 08:12:58.381930 labedf-1.2.0/
--rw-rw-rw-   0        0        0     1085 2023-01-20 04:06:07.000000 labedf-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     1740 2023-02-06 08:12:58.381930 labedf-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1390 2023-02-06 08:05:30.000000 labedf-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-06 08:12:58.372928 labedf-1.2.0/labedf/
--rw-rw-rw-   0        0        0       51 2023-02-06 08:07:45.000000 labedf-1.2.0/labedf/__init__.py
--rw-rw-rw-   0        0        0     3975 2023-01-23 06:52:31.000000 labedf-1.2.0/labedf/csv2.py
--rw-rw-rw-   0        0        0     4753 2023-01-20 04:06:07.000000 labedf-1.2.0/labedf/edf2.py
--rw-rw-rw-   0        0        0     2087 2023-02-06 07:57:18.000000 labedf-1.2.0/labedf/set2.py
-drwxrwxrwx   0        0        0        0 2023-02-06 08:12:58.380930 labedf-1.2.0/labedf/utilities/
--rw-rw-rw-   0        0        0        0 2023-01-20 04:06:07.000000 labedf-1.2.0/labedf/utilities/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-01-20 04:06:07.000000 labedf-1.2.0/labedf/utilities/edf.py
-drwxrwxrwx   0        0        0        0 2023-02-06 08:12:58.379930 labedf-1.2.0/labedf.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-02-06 08:12:57.000000 labedf-1.2.0/labedf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-02-06 08:12:58.000000 labedf-1.2.0/labedf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 08:12:57.000000 labedf-1.2.0/labedf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-02-06 08:12:58.000000 labedf-1.2.0/labedf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-06 08:12:58.000000 labedf-1.2.0/labedf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-06 08:12:58.381930 labedf-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-01-24 02:53:13.000000 labedf-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:42:40.853880 labedf-2.0.0/
+-rw-rw-rw-   0        0        0     1085 2022-11-10 09:00:50.000000 labedf-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      935 2023-06-25 15:42:40.851908 labedf-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-06-25 15:33:00.000000 labedf-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 15:42:40.832926 labedf-2.0.0/labedf/
+-rw-rw-rw-   0        0        0       45 2023-06-25 15:15:01.000000 labedf-2.0.0/labedf/__init__.py
+-rw-rw-rw-   0        0        0     3975 2023-06-25 15:06:44.000000 labedf-2.0.0/labedf/edf_csv.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:42:40.849903 labedf-2.0.0/labedf/utilities/
+-rw-rw-rw-   0        0        0        0 2022-11-10 09:00:50.000000 labedf-2.0.0/labedf/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1994 2022-11-20 11:27:14.000000 labedf-2.0.0/labedf/utilities/edf.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:42:40.845615 labedf-2.0.0/labedf.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-25 15:42:40.000000 labedf-2.0.0/labedf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-25 15:42:40.000000 labedf-2.0.0/labedf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 15:42:40.000000 labedf-2.0.0/labedf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-25 15:42:40.000000 labedf-2.0.0/labedf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-25 15:42:40.000000 labedf-2.0.0/labedf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 15:42:40.853880 labedf-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      760 2023-06-25 15:12:42.000000 labedf-2.0.0/setup.py
```

### Comparing `labedf-1.2.0/LICENSE` & `labedf-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labedf-1.2.0/labedf/csv2.py` & `labedf-2.0.0/labedf/edf_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from numpy import ndarray
 import pyedflib
 import labcsv
 from labcsv import DefaultHeaderName as DHName
 from typing import Callable, Optional
 from .utilities import edf
-def merge_csv2edf(edf_path:str,
+def merge_edf_csv(edf_path:str,
                 csv_path:str,
                 export_path:Optional[str] = None,
                 marker_names:list[str] = ["Marker"],
                 sync_marker_name:str = "sync",
                 marker_offset:Optional[tuple[float]] = (0,0),
                 label_header_name:str = None,
                 preprocessing_func:Optional[Callable[[list[ndarray]],list[ndarray]]] = None):
```

### Comparing `labedf-1.2.0/labedf/utilities/edf.py` & `labedf-2.0.0/labedf/utilities/edf.py`

 * *Files identical despite different names*

### Comparing `labedf-1.2.0/setup.py` & `labedf-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     url="https://github.com/s-n-1-0/labedf.py",
     download_url="https://github.com/s-n-1-0/labedf.py",
     version=labedf.__version__,
     description="Merge the lab.js csv file and the edf file.",
     install_requires=[
         "pyedflib>=0.1.30",
         "labcsv>=1.0.4",
-        "numpy>=1.22.4",
-        "h5py>=3.7.0",
-        "mne[hdf5]>=1.3.0"
+        "numpy>=1.22.4"
         ],
     packages=["labedf","labedf.utilities"],
     license="MIT",
     keywords= ["labjs","lab.js"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown"
 )
```

