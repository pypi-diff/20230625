# Comparing `tmp/simulated-bifurcation-1.1.0.tar.gz` & `tmp/simulated-bifurcation-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulated-bifurcation-1.1.0.tar", last modified: Sun Jun 25 19:04:54 2023, max compression
+gzip compressed data, was "simulated-bifurcation-1.1.1.tar", last modified: Sun Jun 25 19:12:59 2023, max compression
```

## Comparing `simulated-bifurcation-1.1.0.tar` & `simulated-bifurcation-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.474398 simulated-bifurcation-1.1.0/
--rw-rw-rw-   0        0        0     1123 2023-04-30 10:03:26.000000 simulated-bifurcation-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      460 2023-06-25 19:04:54.474398 simulated-bifurcation-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8949 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/README.md
--rw-rw-rw-   0        0        0      215 2023-06-25 19:04:54.476396 simulated-bifurcation-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-06-25 19:04:46.000000 simulated-bifurcation-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.391415 simulated-bifurcation-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.419401 simulated-bifurcation-1.1.0/src/simulated_bifurcation/
--rw-rw-rw-   0        0        0       97 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/__init__.py
--rw-rw-rw-   0        0        0     5250 2023-06-25 18:59:06.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/interface.py
--rw-rw-rw-   0        0        0    10533 2023-06-25 18:58:05.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/ising.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.439399 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/
--rw-rw-rw-   0        0        0       42 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/__init__.py
--rw-rw-rw-   0        0        0     1537 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/partitioning.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.453397 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/
--rw-rw-rw-   0        0        0       88 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/__init__.py
--rw-rw-rw-   0        0        0     4197 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/integer.py
--rw-rw-rw-   0        0        0     1082 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/markowitz.py
--rw-rw-rw-   0        0        0     3705 2023-06-25 18:30:47.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/qubo.py
--rw-rw-rw-   0        0        0    13605 2023-06-25 18:54:34.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.433402 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/
--rw-rw-rw-   0        0        0      460 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.469399 simulated-bifurcation-1.1.0/test/
--rw-rw-rw-   0        0        0     2676 2023-06-25 08:57:26.000000 simulated-bifurcation-1.1.0/test/test_ising.py
--rw-rw-rw-   0        0        0      217 2023-06-25 17:52:32.000000 simulated-bifurcation-1.1.0/test/test_ising_interface.py
--rw-rw-rw-   0        0        0     1393 2023-06-25 17:48:34.000000 simulated-bifurcation-1.1.0/test/test_optimizer.py
--rw-rw-rw-   0        0        0     4463 2023-06-25 10:08:24.000000 simulated-bifurcation-1.1.0/test/test_stop_window.py
--rw-rw-rw-   0        0        0     3959 2023-06-25 17:41:12.000000 simulated-bifurcation-1.1.0/test/test_symplectic_integrator.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.418001 simulated-bifurcation-1.1.1/
+-rw-rw-rw-   0        0        0     1123 2023-04-30 10:03:26.000000 simulated-bifurcation-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9452 2023-06-25 19:12:59.419003 simulated-bifurcation-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8949 2023-06-25 19:07:14.000000 simulated-bifurcation-1.1.1/README.md
+-rw-rw-rw-   0        0        0      136 2023-06-25 19:12:59.421002 simulated-bifurcation-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-06-25 19:12:26.000000 simulated-bifurcation-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.340005 simulated-bifurcation-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.369026 simulated-bifurcation-1.1.1/src/simulated_bifurcation/
+-rw-rw-rw-   0        0        0       97 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/__init__.py
+-rw-rw-rw-   0        0        0     5250 2023-06-25 18:59:06.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/interface.py
+-rw-rw-rw-   0        0        0    10533 2023-06-25 18:58:05.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/ising.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.387003 simulated-bifurcation-1.1.1/src/simulated_bifurcation/karp/
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/karp/__init__.py
+-rw-rw-rw-   0        0        0     1537 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/karp/partitioning.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.400006 simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/
+-rw-rw-rw-   0        0        0       88 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/integer.py
+-rw-rw-rw-   0        0        0     1082 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/markowitz.py
+-rw-rw-rw-   0        0        0     3705 2023-06-25 18:30:47.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/qubo.py
+-rw-rw-rw-   0        0        0    13605 2023-06-25 18:54:34.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.381004 simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/
+-rw-rw-rw-   0        0        0     9452 2023-06-25 19:12:59.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-25 19:12:59.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:12:59.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-25 19:12:59.000000 simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 19:12:59.414003 simulated-bifurcation-1.1.1/test/
+-rw-rw-rw-   0        0        0     2676 2023-06-25 08:57:26.000000 simulated-bifurcation-1.1.1/test/test_ising.py
+-rw-rw-rw-   0        0        0      217 2023-06-25 17:52:32.000000 simulated-bifurcation-1.1.1/test/test_ising_interface.py
+-rw-rw-rw-   0        0        0     1393 2023-06-25 17:48:34.000000 simulated-bifurcation-1.1.1/test/test_optimizer.py
+-rw-rw-rw-   0        0        0     4463 2023-06-25 10:08:24.000000 simulated-bifurcation-1.1.1/test/test_stop_window.py
+-rw-rw-rw-   0        0        0     3959 2023-06-25 17:41:12.000000 simulated-bifurcation-1.1.1/test/test_symplectic_integrator.py
```

### Comparing `simulated-bifurcation-1.1.0/LICENSE` & `simulated-bifurcation-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/README.md` & `simulated-bifurcation-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/setup.py` & `simulated-bifurcation-1.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import setuptools
 
 
+with open("README.md", "r", encoding='utf-8') as readme:
+    long_description = readme.read()
+
 setuptools.setup(
     name="simulated-bifurcation",
-    version="1.1.0",
+    version="1.1.1",
     description="Efficient implementation of the quantum-inspired Simulated Bifurcation (SB) algorithm to solve Ising-like problems.",
     url="https://github.com/bqth29/simulated-bifurcation-algorithm",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.8"
 )
```

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/interface.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/interface.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/ising.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/ising.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/partitioning.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/karp/partitioning.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/integer.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/integer.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/markowitz.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/markowitz.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/qubo.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/models/qubo.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation/optimizer.py` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation/optimizer.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/SOURCES.txt` & `simulated-bifurcation-1.1.1/src/simulated_bifurcation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/test/test_ising.py` & `simulated-bifurcation-1.1.1/test/test_ising.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/test/test_optimizer.py` & `simulated-bifurcation-1.1.1/test/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/test/test_stop_window.py` & `simulated-bifurcation-1.1.1/test/test_stop_window.py`

 * *Files identical despite different names*

### Comparing `simulated-bifurcation-1.1.0/test/test_symplectic_integrator.py` & `simulated-bifurcation-1.1.1/test/test_symplectic_integrator.py`

 * *Files identical despite different names*

