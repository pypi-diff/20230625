# Comparing `tmp/constrainedlr-0.1.2.tar.gz` & `tmp/constrainedlr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.1.2.tar", last modified: Sat Jun 24 14:16:17 2023, max compression
+gzip compressed data, was "constrainedlr-0.1.3.tar", last modified: Sun Jun 25 10:25:10 2023, max compression
```

## Comparing `constrainedlr-0.1.2.tar` & `constrainedlr-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.334225 constrainedlr-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/LICENCE
--rw-rw-rw-   0        0        0     2610 2023-06-24 14:16:17.333225 constrainedlr-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/README.md
--rw-rw-rw-   0        0        0     1324 2023-06-24 14:14:38.000000 constrainedlr-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 14:16:17.335236 constrainedlr-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.212226 constrainedlr-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.247226 constrainedlr-0.1.2/src/constrainedlr/
--rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/src/constrainedlr/__init__.py
--rw-rw-rw-   0        0        0     7671 2023-06-24 13:55:44.000000 constrainedlr-0.1.2/src/constrainedlr/model.py
--rw-rw-rw-   0        0        0     2727 2023-06-24 13:57:55.000000 constrainedlr-0.1.2/src/constrainedlr/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.321245 constrainedlr-0.1.2/src/constrainedlr.egg-info/
--rw-rw-rw-   0        0        0     2610 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.329247 constrainedlr-0.1.2/tests/
--rw-rw-rw-   0        0        0     4887 2023-06-24 13:53:15.000000 constrainedlr-0.1.2/tests/test_fit.py
+drwxrwxrwx   0        0        0        0 2023-06-25 10:25:10.641239 constrainedlr-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0     2610 2023-06-25 10:25:10.639237 constrainedlr-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-06-21 18:38:31.000000 constrainedlr-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1324 2023-06-25 10:23:18.000000 constrainedlr-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 10:25:10.642240 constrainedlr-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 10:25:10.535239 constrainedlr-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 10:25:10.591237 constrainedlr-0.1.3/src/constrainedlr/
+-rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.3/src/constrainedlr/__init__.py
+-rw-rw-rw-   0        0        0     7871 2023-06-25 10:23:12.000000 constrainedlr-0.1.3/src/constrainedlr/model.py
+-rw-rw-rw-   0        0        0     3742 2023-06-25 10:23:12.000000 constrainedlr-0.1.3/src/constrainedlr/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-25 10:25:10.631287 constrainedlr-0.1.3/src/constrainedlr.egg-info/
+-rw-rw-rw-   0        0        0     2610 2023-06-25 10:25:10.000000 constrainedlr-0.1.3/src/constrainedlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-25 10:25:10.000000 constrainedlr-0.1.3/src/constrainedlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 10:25:10.000000 constrainedlr-0.1.3/src/constrainedlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-25 10:25:10.000000 constrainedlr-0.1.3/src/constrainedlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 10:25:10.000000 constrainedlr-0.1.3/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 10:25:10.635239 constrainedlr-0.1.3/tests/
+-rw-rw-rw-   0        0        0     5800 2023-06-25 10:23:12.000000 constrainedlr-0.1.3/tests/test_fit.py
```

### Comparing `constrainedlr-0.1.2/LICENCE` & `constrainedlr-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.2/PKG-INFO` & `constrainedlr-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.2 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.3 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 constrainedlr Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `constrainedlr-0.1.2/README.md` & `constrainedlr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.2/pyproject.toml` & `constrainedlr-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.1.2'
+version = '0.1.3'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `constrainedlr-0.1.2/src/constrainedlr/model.py` & `constrainedlr-0.1.3/src/constrainedlr/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import numpy as np
 import pandas as pd
 from cvxopt import matrix, solvers
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 
-from .validation import validate_coefficients_sign_constraints, validate_coefficients_range_constraints
+from .validation import (
+    validate_coefficients_sign_constraints,
+    validate_coefficients_range_constraints,
+    validate_intercept_sign_constraint,
+)
 
 
 class ConstrainedLinearRegression(BaseEstimator, RegressorMixin):
     def __init__(self, fit_intercept: bool = True, alpha: float = 0.0):
         """
         Least squares Linear Regression with optional constraints on its coefficients/weights.
 
@@ -41,15 +45,15 @@
     def fit(
         self,
         X: Union[np.ndarray, pd.DataFrame],
         y: np.ndarray,
         sample_weight: np.ndarray = None,
         coefficients_sign_constraints: dict = {},
         coefficients_range_constraints: dict = {},
-        intercept_sign_constraint: int = 0,
+        intercept_sign_constraint: Union[int, str] = 0,
         coefficients_sum_constraint: float = None,
     ) -> "ConstrainedLinearRegression":
         """
         Fit linear model with constraints.
 
         Args:
             X:
@@ -79,15 +83,16 @@
             coefficients_sum_constraint:
                 Constraints the sum of all coefficients plus intercept (if present).
 
         Returns:
             Fitted Estimator.
         """
         X, y = check_X_y(X, y)
-        validate_coefficients_sign_constraints(coefficients_sign_constraints, X)
+        coefficients_sign_constraints = validate_coefficients_sign_constraints(coefficients_sign_constraints, X)
+        intercept_sign_constraint = validate_intercept_sign_constraint(intercept_sign_constraint)
         validate_coefficients_range_constraints(coefficients_range_constraints, X)
 
         if len(coefficients_sign_constraints) > 0 and len(coefficients_range_constraints) > 0:
             raise ValueError(
                 "Only one of `features_sign_constraints` or `coefficients_range_constraints` can be provided."
             )
```

### Comparing `constrainedlr-0.1.2/src/constrainedlr/validation.py` & `constrainedlr-0.1.3/src/constrainedlr/validation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,53 @@
-def validate_coefficients_sign_constraints(coefficients_sign_constraints: dict, X) -> None:
+from typing import Union
+
+
+def validate_coefficients_sign_constraints(coefficients_sign_constraints: dict, X) -> dict:
     if type(coefficients_sign_constraints) != dict:
         raise ValueError("coefficients_sign_constraints must be of type dict")
 
     if len(coefficients_sign_constraints) > 0:
         coef_indices = list(coefficients_sign_constraints.keys())
         if any([type(ci) != int for ci in coef_indices]):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
         if (min(coef_indices) < 0) or (max(coef_indices) >= X.shape[1]):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
 
-        if len(set(coefficients_sign_constraints.values()) - {-1, 0, 1}) > 0:
+        if len(set(coefficients_sign_constraints.values()) - {-1, 0, 1, "positive", "negative"}) > 0:
             raise ValueError(
-                "Values of coefficients_sign_constraints must be 0, -1, or 1, for no sign constraint, "
-                "negative sign constraint, or positive sign constraint respectively"
+                "Values of coefficients_sign_constraints must be 0 (no sign constraint), 'positive' or 1 (positive sign constraint), "
+                "'negative' or -1 (negative sign constraint)"
             )
 
+        # Replace "positive" with 1, "negative" with -1 for compatibility with the optimizer
+        coefficients_sign_constraints = {
+            k: 1 if v == "positive" else -1 if v == "negative" else v for k, v in coefficients_sign_constraints.items()
+        }
+    return coefficients_sign_constraints
+
+
+def validate_intercept_sign_constraint(intercept_sign_constraint: Union[int, str]) -> int:
+    if intercept_sign_constraint not in [-1, 0, 1, "positive", "negative"]:
+        raise ValueError(
+            "intercept_sign_constraint must be 0 (no sign constraint), 'positive' or 1 (positive sign constraint), "
+            "'negative' or -1 (negative sign constraint)"
+        )
+    intercept_sign_constraint = (
+        1
+        if intercept_sign_constraint == "positive"
+        else -1
+        if intercept_sign_constraint == "negative"
+        else intercept_sign_constraint
+    )
+    return intercept_sign_constraint
+
 
 def validate_coefficients_range_constraints(coefficients_range_constraints: dict, X) -> None:
     if type(coefficients_range_constraints) != dict:
         raise ValueError("coefficients_range_constraints must be of type dict")
 
     if len(coefficients_range_constraints) > 0:
         coef_indices = list(coefficients_range_constraints.keys())
```

### Comparing `constrainedlr-0.1.2/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.1.3/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.2 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.3 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 constrainedlr Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `constrainedlr-0.1.2/tests/test_fit.py` & `constrainedlr-0.1.3/tests/test_fit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sys
+import random
 
 import numpy as np
 import pandas as pd
 from sklearn.datasets import load_diabetes
 from sklearn.linear_model import LinearRegression, Ridge
-
+import pytest
 from constrainedlr.model import ConstrainedLinearRegression
 
 atol = 1e-5
 
 dataset = load_diabetes()
 X = dataset["data"]
 y = dataset["target"]
@@ -51,30 +51,51 @@
 
 
 def test_feature_signs():
     clr = ConstrainedLinearRegression(fit_intercept=True)
 
     # Perform multiple tests since signs are produced randomly
     np.random.seed(0)
-    for _ in range(10):
-        signs = np.random.choice([-1, 1], size=X.shape[1])
+    for _ in range(30):
+        signs = random.choices([-1, 1, "positive", "negative"], k=X.shape[1])
         features_sign_constraints = dict(zip(list(range(X.shape[1])), signs))
         clr.fit(X, y, coefficients_sign_constraints=features_sign_constraints)
 
-        assert np.all(np.sign(clr.coef_) == signs)
+        # if coefficients multipled with imposed signs are all positive (or approximately positive) then pass the test
+        signs_numeric = np.array([1 if s == "positive" else -1 if s == "negative" else s for s in signs])
+        assert np.all(clr.coef_ * signs_numeric > -atol)
 
 
 def test_intercept_sign():
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y, intercept_sign_constraint=1)
     assert clr.intercept_ > 0
 
     clr.fit(X, y, intercept_sign_constraint=-1)
     assert clr.intercept_ < 0
 
+    clr.fit(X, y, intercept_sign_constraint="positive")
+    assert clr.intercept_ > 0
+
+    clr.fit(X, y, intercept_sign_constraint="negative")
+    assert clr.intercept_ < 0
+
+    # Check the below runs without raising any exceptions
+    try:
+        clr.fit(X, y, intercept_sign_constraint=0)
+        clr.fit(X, y)
+    except Exception as exception:
+        assert False
+
+    # Check if exception is raised when an invalid value is given
+    with pytest.raises(ValueError):
+        clr.fit(X, y, intercept_sign_constraint="invalid value")
+    with pytest.raises(ValueError):
+        clr.fit(X, y, intercept_sign_constraint=2)
+
 
 def test_features_sum():
     clr = ConstrainedLinearRegression(fit_intercept=True)
     features_sum_constraint_equal = 15
     clr.fit(X, y, coefficients_sum_constraint=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum() + clr.intercept_
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
```

