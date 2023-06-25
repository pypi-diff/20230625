# Comparing `tmp/zedstat-0.0.98.tar.gz` & `tmp/zedstat-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zedstat-0.0.98.tar", last modified: Tue Nov  1 03:41:47 2022, max compression
+gzip compressed data, was "dist/zedstat-0.0.99.tar", last modified: Thu Nov  3 16:19:14 2022, max compression
```

## Comparing `zedstat-0.0.98.tar` & `zedstat-0.0.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-01 03:41:47.386084 zedstat-0.0.98/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1065 2022-09-02 21:21:15.000000 zedstat-0.0.98/LICENSE
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      165 2022-09-02 20:46:04.000000 zedstat-0.0.98/MANIFEST.in
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     2141 2022-11-01 03:41:47.385084 zedstat-0.0.98/PKG-INFO
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1309 2022-09-06 19:09:45.000000 zedstat-0.0.98/README.rst
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       38 2022-11-01 03:41:47.386084 zedstat-0.0.98/setup.cfg
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1673 2022-09-02 20:45:48.000000 zedstat-0.0.98/setup.py
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       23 2022-10-31 11:30:37.000000 zedstat-0.0.98/version.py
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-01 03:41:47.384084 zedstat-0.0.98/zedstat/
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-01 03:41:47.385084 zedstat-0.0.98/zedstat/.ipynb_checkpoints/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)    87302 2022-10-31 01:48:33.000000 zedstat-0.0.98/zedstat/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       72 2022-10-25 22:16:24.000000 zedstat-0.0.98/zedstat/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)   198590 2022-10-31 21:26:36.000000 zedstat-0.0.98/zedstat/Untitled-Copy1.ipynb
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)    87302 2022-10-28 04:30:10.000000 zedstat-0.0.98/zedstat/Untitled.ipynb
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1852 2022-09-02 21:42:55.000000 zedstat-0.0.98/zedstat/__init__.py
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      795 2022-09-06 18:38:17.000000 zedstat-0.0.98/zedstat/mwauc.py
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     2248 2022-09-06 18:36:48.000000 zedstat-0.0.98/zedstat/textable.py
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)    22394 2022-10-31 11:29:59.000000 zedstat-0.0.98/zedstat/zedstat.py
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-01 03:41:47.385084 zedstat-0.0.98/zedstat.egg-info/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     2141 2022-11-01 03:41:47.000000 zedstat-0.0.98/zedstat.egg-info/PKG-INFO
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      444 2022-11-01 03:41:47.000000 zedstat-0.0.98/zedstat.egg-info/SOURCES.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)        1 2022-11-01 03:41:47.000000 zedstat-0.0.98/zedstat.egg-info/dependency_links.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       38 2022-11-01 03:41:47.000000 zedstat-0.0.98/zedstat.egg-info/requires.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)        8 2022-11-01 03:41:47.000000 zedstat-0.0.98/zedstat.egg-info/top_level.txt
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-03 16:19:14.000000 zedstat-0.0.99/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1065 2022-11-03 15:39:07.000000 zedstat-0.0.99/LICENSE
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      165 2022-11-03 15:39:07.000000 zedstat-0.0.99/MANIFEST.in
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2482 2022-11-03 16:19:14.000000 zedstat-0.0.99/PKG-INFO
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1309 2022-11-03 15:39:07.000000 zedstat-0.0.99/README.rst
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2022-11-03 16:19:14.000000 zedstat-0.0.99/setup.cfg
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1673 2022-11-03 15:39:07.000000 zedstat-0.0.99/setup.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       23 2022-11-03 16:19:12.000000 zedstat-0.0.99/version.py
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat/
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat/.ipynb_checkpoints/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)    87302 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       72 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)   198590 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/Untitled-Copy1.ipynb
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)    87302 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/Untitled.ipynb
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1852 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/__init__.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      795 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/mwauc.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2248 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/textable.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)    22394 2022-11-03 15:39:07.000000 zedstat-0.0.99/zedstat/zedstat.py
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     2482 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/PKG-INFO
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      444 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        1 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/requires.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        8 2022-11-03 16:19:14.000000 zedstat-0.0.99/zedstat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `zedstat-0.0.98/LICENSE` & `zedstat-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/PKG-INFO` & `zedstat-0.0.99/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 Metadata-Version: 2.1
 Name: zedstat
-Version: 0.0.98
+Version: 0.0.99
 Summary: Statistics tools for ML models and deployment
 Home-page: https://github.com/zeroknowledgediscovery/zedstat
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/zedstat/archive/0.0.98.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/zedstat/archive/0.0.99.tar.gz
+Description: ===============
+        zedstat
+        ===============
+        
+        .. image:: https://zed.uchicago.edu/logo/logo_zedstat.png
+           :height: 150px
+           :align: center 
+        
+        .. image:: https://zenodo.org/badge/529991779.svg
+           :target: https://zenodo.org/badge/latestdoi/529991779
+        
+        .. class:: no-web no-pdf
+        
+        :Author: ZeD@UChicago <zed.uchicago.edu>
+        :Description: Tools for ML statistics 
+        :Documentation: https://zeroknowledgediscovery.github.io/zedstat/
+        :Example: https://github.com/zeroknowledgediscovery/zedstat/blob/master/examples/example1.ipynb
+        		
+        **Usage:**
+        
+        .. code-block::
+        
+           from zedstat import zedstat
+           zt=zedstat.processRoc(df=pd.read_csv('roc.csv'),
+                   order=3, 
+                   total_samples=100000,
+                   positive_samples=100,
+                   alpha=0.01,
+                   prevalence=.002)
+        
+           zt.smooth(STEP=0.001)
+           zt.allmeasures(interpolate=True)
+           zt.usample(precision=3)
+           zt.getBounds()
+        
+           print(zt.auc())
+        
+           # find the high precision and high sensitivity operating points
+           zt.operating_zone(LRminus=.65)
+           rf0,txt0=zt.interpret(fpr=zt._operating_zone.fpr.values[0],number_of_positives=10)
+           rf1,txt1=zt.interpret(fpr=zt._operating_zone.fpr.values[1],number_of_positives=10)
+           display(zt._operating_zone)
+           print('high precision operation:\n','\n '.join(txt0))
+           print('high recall operation:\n','\n '.join(txt1))
+        
 Keywords: machine learning,statistics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-===============
-zedstat
-===============
-
-.. image:: https://zed.uchicago.edu/logo/logo_zedstat.png
-   :height: 150px
-   :align: center 
-
-.. image:: https://zenodo.org/badge/529991779.svg
-   :target: https://zenodo.org/badge/latestdoi/529991779
-
-.. class:: no-web no-pdf
-
-:Author: ZeD@UChicago <zed.uchicago.edu>
-:Description: Tools for ML statistics 
-:Documentation: https://zeroknowledgediscovery.github.io/zedstat/
-:Example: https://github.com/zeroknowledgediscovery/zedstat/blob/master/examples/example1.ipynb
-		
-**Usage:**
-
-.. code-block::
-
-   from zedstat import zedstat
-   zt=zedstat.processRoc(df=pd.read_csv('roc.csv'),
-           order=3, 
-           total_samples=100000,
-           positive_samples=100,
-           alpha=0.01,
-           prevalence=.002)
-
-   zt.smooth(STEP=0.001)
-   zt.allmeasures(interpolate=True)
-   zt.usample(precision=3)
-   zt.getBounds()
-
-   print(zt.auc())
-
-   # find the high precision and high sensitivity operating points
-   zt.operating_zone(LRminus=.65)
-   rf0,txt0=zt.interpret(fpr=zt._operating_zone.fpr.values[0],number_of_positives=10)
-   rf1,txt1=zt.interpret(fpr=zt._operating_zone.fpr.values[1],number_of_positives=10)
-   display(zt._operating_zone)
-   print('high precision operation:\n','\n '.join(txt0))
-   print('high recall operation:\n','\n '.join(txt1))
-
-
```

### Comparing `zedstat-0.0.98/README.rst` & `zedstat-0.0.99/README.rst`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/setup.py` & `zedstat-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb` & `zedstat-0.0.99/zedstat/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/Untitled-Copy1.ipynb` & `zedstat-0.0.99/zedstat/Untitled-Copy1.ipynb`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/Untitled.ipynb` & `zedstat-0.0.99/zedstat/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/__init__.py` & `zedstat-0.0.99/zedstat/__init__.py`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/mwauc.py` & `zedstat-0.0.99/zedstat/mwauc.py`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/textable.py` & `zedstat-0.0.99/zedstat/textable.py`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat/zedstat.py` & `zedstat-0.0.99/zedstat/zedstat.py`

 * *Files identical despite different names*

### Comparing `zedstat-0.0.98/zedstat.egg-info/PKG-INFO` & `zedstat-0.0.99/zedstat.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 Metadata-Version: 2.1
 Name: zedstat
-Version: 0.0.98
+Version: 0.0.99
 Summary: Statistics tools for ML models and deployment
 Home-page: https://github.com/zeroknowledgediscovery/zedstat
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/zedstat/archive/0.0.98.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/zedstat/archive/0.0.99.tar.gz
+Description: ===============
+        zedstat
+        ===============
+        
+        .. image:: https://zed.uchicago.edu/logo/logo_zedstat.png
+           :height: 150px
+           :align: center 
+        
+        .. image:: https://zenodo.org/badge/529991779.svg
+           :target: https://zenodo.org/badge/latestdoi/529991779
+        
+        .. class:: no-web no-pdf
+        
+        :Author: ZeD@UChicago <zed.uchicago.edu>
+        :Description: Tools for ML statistics 
+        :Documentation: https://zeroknowledgediscovery.github.io/zedstat/
+        :Example: https://github.com/zeroknowledgediscovery/zedstat/blob/master/examples/example1.ipynb
+        		
+        **Usage:**
+        
+        .. code-block::
+        
+           from zedstat import zedstat
+           zt=zedstat.processRoc(df=pd.read_csv('roc.csv'),
+                   order=3, 
+                   total_samples=100000,
+                   positive_samples=100,
+                   alpha=0.01,
+                   prevalence=.002)
+        
+           zt.smooth(STEP=0.001)
+           zt.allmeasures(interpolate=True)
+           zt.usample(precision=3)
+           zt.getBounds()
+        
+           print(zt.auc())
+        
+           # find the high precision and high sensitivity operating points
+           zt.operating_zone(LRminus=.65)
+           rf0,txt0=zt.interpret(fpr=zt._operating_zone.fpr.values[0],number_of_positives=10)
+           rf1,txt1=zt.interpret(fpr=zt._operating_zone.fpr.values[1],number_of_positives=10)
+           display(zt._operating_zone)
+           print('high precision operation:\n','\n '.join(txt0))
+           print('high recall operation:\n','\n '.join(txt1))
+        
 Keywords: machine learning,statistics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-===============
-zedstat
-===============
-
-.. image:: https://zed.uchicago.edu/logo/logo_zedstat.png
-   :height: 150px
-   :align: center 
-
-.. image:: https://zenodo.org/badge/529991779.svg
-   :target: https://zenodo.org/badge/latestdoi/529991779
-
-.. class:: no-web no-pdf
-
-:Author: ZeD@UChicago <zed.uchicago.edu>
-:Description: Tools for ML statistics 
-:Documentation: https://zeroknowledgediscovery.github.io/zedstat/
-:Example: https://github.com/zeroknowledgediscovery/zedstat/blob/master/examples/example1.ipynb
-		
-**Usage:**
-
-.. code-block::
-
-   from zedstat import zedstat
-   zt=zedstat.processRoc(df=pd.read_csv('roc.csv'),
-           order=3, 
-           total_samples=100000,
-           positive_samples=100,
-           alpha=0.01,
-           prevalence=.002)
-
-   zt.smooth(STEP=0.001)
-   zt.allmeasures(interpolate=True)
-   zt.usample(precision=3)
-   zt.getBounds()
-
-   print(zt.auc())
-
-   # find the high precision and high sensitivity operating points
-   zt.operating_zone(LRminus=.65)
-   rf0,txt0=zt.interpret(fpr=zt._operating_zone.fpr.values[0],number_of_positives=10)
-   rf1,txt1=zt.interpret(fpr=zt._operating_zone.fpr.values[1],number_of_positives=10)
-   display(zt._operating_zone)
-   print('high precision operation:\n','\n '.join(txt0))
-   print('high recall operation:\n','\n '.join(txt1))
-
-
```

