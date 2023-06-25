# Comparing `tmp/pyhackrf2-1.0.0.tar.gz` & `tmp/pyhackrf2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhackrf2-1.0.0.tar", last modified: Sun Jun 25 13:36:02 2023, max compression
+gzip compressed data, was "pyhackrf2-1.0.1.tar", last modified: Sun Jun 25 13:45:00 2023, max compression
```

## Comparing `pyhackrf2-1.0.0.tar` & `pyhackrf2-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:36:02.465555 pyhackrf2-1.0.0/
--rw-r--r--   0 alex       (501) staff       (20)     4130 2023-06-25 13:36:02.465394 pyhackrf2-1.0.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3819 2023-06-25 13:21:19.000000 pyhackrf2-1.0.0/README.md
--rw-r--r--   0 alex       (501) staff       (20)      401 2023-06-25 13:24:32.000000 pyhackrf2-1.0.0/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-25 13:36:02.465598 pyhackrf2-1.0.0/setup.cfg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:36:02.463193 pyhackrf2-1.0.0/src/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:36:02.464237 pyhackrf2-1.0.0/src/pyhackrf/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-05-27 23:45:06.000000 pyhackrf2-1.0.0/src/pyhackrf/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.0/src/pyhackrf/cinterface.py
--rw-r--r--   0 alex       (501) staff       (20)    18071 2023-05-29 22:26:21.000000 pyhackrf2-1.0.0/src/pyhackrf/libhackrf.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:36:02.465195 pyhackrf2-1.0.0/src/pyhackrf2.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     4130 2023-06-25 13:36:02.000000 pyhackrf2-1.0.0/src/pyhackrf2.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      250 2023-06-25 13:36:02.000000 pyhackrf2-1.0.0/src/pyhackrf2.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-25 13:36:02.000000 pyhackrf2-1.0.0/src/pyhackrf2.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-06-25 13:36:02.000000 pyhackrf2-1.0.0/src/pyhackrf2.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.319141 pyhackrf2-1.0.1/
+-rw-r--r--   0 alex       (501) staff       (20)     4131 2023-06-25 13:45:00.318980 pyhackrf2-1.0.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     3820 2023-06-25 13:42:40.000000 pyhackrf2-1.0.1/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      401 2023-06-25 13:44:17.000000 pyhackrf2-1.0.1/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-25 13:45:00.319189 pyhackrf2-1.0.1/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.316708 pyhackrf2-1.0.1/src/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.317829 pyhackrf2-1.0.1/src/pyhackrf/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-05-27 23:45:06.000000 pyhackrf2-1.0.1/src/pyhackrf/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.1/src/pyhackrf/cinterface.py
+-rw-r--r--   0 alex       (501) staff       (20)    18071 2023-05-29 22:26:21.000000 pyhackrf2-1.0.1/src/pyhackrf/libhackrf.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-25 13:45:00.318763 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     4131 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      250 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        9 2023-06-25 13:45:00.000000 pyhackrf2-1.0.1/src/pyhackrf2.egg-info/top_level.txt
```

### Comparing `pyhackrf2-1.0.0/PKG-INFO` & `pyhackrf2-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pyhackrf2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python bindings for libhackrf rewritten
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
-# pyhackrf
+# pyhackrf2
 
 A Python wrappper for libhackrf rewritten.
 
 # Description
 
 Python bindings for native HackRF library libhackrf that aims to implement all features of HackRF accessible via its C interface, but via convenient Pythonic class.
 
 Supports receive, transmit, sweep, setting all gains, baseband filter and bias tee.
 
 # Quick Example
 
 To take samples and plot the power spectral density:
 
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 from pylab import *     # for plotting
 
 hackrf = HackRF()
 
 hackrf.sample_rate = 20e6
 hackrf.center_freq = 88.5e6
 
@@ -40,15 +40,15 @@
 show()
 ```
 
 # More Example Use
 
 First, import class from module
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 ```
 
 
 Enumerate HackRF devices attached to host as strings of serial numbers:
 
 ```python
 print(HackRF.enumerate())
```

### Comparing `pyhackrf2-1.0.0/README.md` & `pyhackrf2-1.0.1/src/pyhackrf2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-# pyhackrf
+Metadata-Version: 2.1
+Name: pyhackrf2
+Version: 1.0.1
+Summary: Python bindings for libhackrf rewritten
+Classifier: Topic :: Communications :: Ham Radio
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
+# pyhackrf2
 
 A Python wrappper for libhackrf rewritten.
 
 # Description
 
 Python bindings for native HackRF library libhackrf that aims to implement all features of HackRF accessible via its C interface, but via convenient Pythonic class.
 
 Supports receive, transmit, sweep, setting all gains, baseband filter and bias tee.
 
 # Quick Example
 
 To take samples and plot the power spectral density:
 
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 from pylab import *     # for plotting
 
 hackrf = HackRF()
 
 hackrf.sample_rate = 20e6
 hackrf.center_freq = 88.5e6
 
@@ -30,15 +40,15 @@
 show()
 ```
 
 # More Example Use
 
 First, import class from module
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 ```
 
 
 Enumerate HackRF devices attached to host as strings of serial numbers:
 
 ```python
 print(HackRF.enumerate())
```

### Comparing `pyhackrf2-1.0.0/src/pyhackrf/cinterface.py` & `pyhackrf2-1.0.1/src/pyhackrf/cinterface.py`

 * *Files identical despite different names*

### Comparing `pyhackrf2-1.0.0/src/pyhackrf/libhackrf.py` & `pyhackrf2-1.0.1/src/pyhackrf/libhackrf.py`

 * *Files identical despite different names*

### Comparing `pyhackrf2-1.0.0/src/pyhackrf2.egg-info/PKG-INFO` & `pyhackrf2-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,23 @@
-Metadata-Version: 2.1
-Name: pyhackrf2
-Version: 1.0.0
-Summary: Python bindings for libhackrf rewritten
-Classifier: Topic :: Communications :: Ham Radio
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
-# pyhackrf
+# pyhackrf2
 
 A Python wrappper for libhackrf rewritten.
 
 # Description
 
 Python bindings for native HackRF library libhackrf that aims to implement all features of HackRF accessible via its C interface, but via convenient Pythonic class.
 
 Supports receive, transmit, sweep, setting all gains, baseband filter and bias tee.
 
 # Quick Example
 
 To take samples and plot the power spectral density:
 
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 from pylab import *     # for plotting
 
 hackrf = HackRF()
 
 hackrf.sample_rate = 20e6
 hackrf.center_freq = 88.5e6
 
@@ -40,15 +30,15 @@
 show()
 ```
 
 # More Example Use
 
 First, import class from module
 ```python
-from libhackrf import HackRF
+from pyhackrf2 import HackRF
 ```
 
 
 Enumerate HackRF devices attached to host as strings of serial numbers:
 
 ```python
 print(HackRF.enumerate())
```

