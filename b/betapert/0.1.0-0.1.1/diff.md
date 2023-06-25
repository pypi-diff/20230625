# Comparing `tmp/betapert-0.1.0.tar.gz` & `tmp/betapert-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betapert-0.1.0.tar", max compression
+gzip compressed data, was "betapert-0.1.1.tar", max compression
```

## Comparing `betapert-0.1.0.tar` & `betapert-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1361 2023-06-25 14:28:43.511417 betapert-0.1.0/README.md
--rw-r--r--   0        0        0     2709 2023-06-25 14:04:25.518999 betapert-0.1.0/betapert/__init__.py
--rw-r--r--   0        0        0     2814 2023-06-25 14:04:25.514803 betapert-0.1.0/betapert/funcs.py
--rw-r--r--   0        0        0      833 2023-06-25 13:39:09.923808 betapert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 22:47:37.319709 betapert-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1110 2023-06-25 14:04:25.512858 betapert-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1972 2023-06-25 13:03:16.467533 betapert-0.1.0/tests/test_frozen.py
--rw-r--r--   0        0        0      864 2023-06-25 14:04:25.517734 betapert-0.1.0/tests/test_generalization.py
--rw-r--r--   0        0        0     3790 2023-06-25 13:55:10.358243 betapert-0.1.0/tests/test_mpert_parametrized.py
--rw-r--r--   0        0        0     1487 2023-06-25 14:04:25.516401 betapert-0.1.0/tests/test_special_cases.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 betapert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1403 2023-06-25 14:44:22.591085 betapert-0.1.1/README.md
+-rw-r--r--   0        0        0     2709 2023-06-25 14:04:25.518999 betapert-0.1.1/betapert/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-25 14:04:25.514803 betapert-0.1.1/betapert/funcs.py
+-rw-r--r--   0        0        0      833 2023-06-25 14:45:53.987823 betapert-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 22:47:37.319709 betapert-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1110 2023-06-25 14:04:25.512858 betapert-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1972 2023-06-25 13:03:16.467533 betapert-0.1.1/tests/test_frozen.py
+-rw-r--r--   0        0        0      864 2023-06-25 14:04:25.517734 betapert-0.1.1/tests/test_generalization.py
+-rw-r--r--   0        0        0     3790 2023-06-25 13:55:10.358243 betapert-0.1.1/tests/test_mpert_parametrized.py
+-rw-r--r--   0        0        0     1487 2023-06-25 14:04:25.516401 betapert-0.1.1/tests/test_special_cases.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 betapert-0.1.1/PKG-INFO
```

### Comparing `betapert-0.1.0/README.md` & `betapert-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 pert.pdf(50, mini=10, mode=30, maxi=90)
 pert.cdf(50, mini=10, mode=30, maxi=90)
 pert.mean(mini=10, mode=30, maxi=90)
 pert.rvs(mini=10, mode=30, maxi=90, size=10)
 
 # The modified PERT distribution is also available.
 # A PERT distribution corresponds to `lambd=4`.
-# Note that you cannot call `mpert` without specifying `lambd`. 
-# Two distributions are needed due to a limitation in SciPy.
+# Note that you cannot call `mpert` without specifying `lambd`
+# (`pert` and `mpert` must have different signatures since SciPy does
+# not support optional shape parameters).
 mdist = mpert(10, 30, 90, lambd=2)
 
-# Values less than `lambd=4` have the effect of flattening the density curve
-#      6%                  >  1.5%
+# Values of `lambd<4` have the effect of flattening the density curve
+#       6%                 >  1.5%
 assert (1 - mdist.cdf(80)) > (1 - dist.cdf(80))
 ```
```

### Comparing `betapert-0.1.0/betapert/__init__.py` & `betapert-0.1.1/betapert/__init__.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/betapert/funcs.py` & `betapert-0.1.1/betapert/funcs.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/pyproject.toml` & `betapert-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "betapert"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/tadamcz/betapert"
 description = "Top-level package for beta-PERT distribution."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `betapert-0.1.0/tests/conftest.py` & `betapert-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/tests/test_frozen.py` & `betapert-0.1.1/tests/test_frozen.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/tests/test_generalization.py` & `betapert-0.1.1/tests/test_generalization.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/tests/test_mpert_parametrized.py` & `betapert-0.1.1/tests/test_mpert_parametrized.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/tests/test_special_cases.py` & `betapert-0.1.1/tests/test_special_cases.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.0/PKG-INFO` & `betapert-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betapert
-Version: 0.1.0
+Version: 0.1.1
 Summary: Top-level package for beta-PERT distribution.
 Home-page: https://github.com/tadamcz/betapert
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,16 @@
 pert.pdf(50, mini=10, mode=30, maxi=90)
 pert.cdf(50, mini=10, mode=30, maxi=90)
 pert.mean(mini=10, mode=30, maxi=90)
 pert.rvs(mini=10, mode=30, maxi=90, size=10)
 
 # The modified PERT distribution is also available.
 # A PERT distribution corresponds to `lambd=4`.
-# Note that you cannot call `mpert` without specifying `lambd`. 
-# Two distributions are needed due to a limitation in SciPy.
+# Note that you cannot call `mpert` without specifying `lambd`
+# (`pert` and `mpert` must have different signatures since SciPy does
+# not support optional shape parameters).
 mdist = mpert(10, 30, 90, lambd=2)
 
-# Values less than `lambd=4` have the effect of flattening the density curve
-#      6%                  >  1.5%
+# Values of `lambd<4` have the effect of flattening the density curve
+#       6%                 >  1.5%
 assert (1 - mdist.cdf(80)) > (1 - dist.cdf(80))
 ```
```

