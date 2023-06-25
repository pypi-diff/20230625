# Comparing `tmp/autofeat-2.1.0.tar.gz` & `tmp/autofeat-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofeat-2.1.0.tar", last modified: Sun May 14 13:57:49 2023, max compression
+gzip compressed data, was "autofeat-2.1.1.tar", last modified: Sun Jun 25 19:03:51 2023, max compression
```

## Comparing `autofeat-2.1.0.tar` & `autofeat-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.979966 autofeat-2.1.0/
--rw-r--r--   0 franzi     (501) staff       (20)     1057 2016-11-03 21:17:21.000000 autofeat-2.1.0/LICENSE
--rw-r--r--   0 franzi     (501) staff       (20)       16 2017-09-06 12:18:36.000000 autofeat-2.1.0/MANIFEST.in
--rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-05-14 13:57:49.979277 autofeat-2.1.0/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)     5190 2023-05-13 14:02:00.000000 autofeat-2.1.0/README.md
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.975979 autofeat-2.1.0/autofeat/
--rw-r--r--   0 franzi     (501) staff       (20)      282 2023-05-13 16:16:16.000000 autofeat-2.1.0/autofeat/__init__.py
--rw-r--r--   0 franzi     (501) staff       (20)    28687 2023-05-14 13:13:41.000000 autofeat-2.1.0/autofeat/autofeat.py
--rw-r--r--   0 franzi     (501) staff       (20)    12858 2023-05-13 15:58:07.000000 autofeat-2.1.0/autofeat/autofeatlight.py
--rw-r--r--   0 franzi     (501) staff       (20)    19859 2023-05-13 15:57:45.000000 autofeat-2.1.0/autofeat/feateng.py
--rw-r--r--   0 franzi     (501) staff       (20)    17833 2023-05-13 16:01:10.000000 autofeat-2.1.0/autofeat/featsel.py
--rw-r--r--   0 franzi     (501) staff       (20)      831 2023-05-13 14:15:17.000000 autofeat-2.1.0/autofeat/nb_utils.py
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.978549 autofeat-2.1.0/autofeat.egg-info/
--rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)      332 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/SOURCES.txt
--rw-r--r--   0 franzi     (501) staff       (20)        1 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/dependency_links.txt
--rw-r--r--   0 franzi     (501) staff       (20)       72 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/requires.txt
--rw-r--r--   0 franzi     (501) staff       (20)        9 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/top_level.txt
--rw-r--r--   0 franzi     (501) staff       (20)      891 2023-05-14 13:54:25.000000 autofeat-2.1.0/pyproject.toml
--rw-r--r--   0 franzi     (501) staff       (20)       38 2023-05-14 13:57:49.980135 autofeat-2.1.0/setup.cfg
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.533599 autofeat-2.1.1/
+-rw-r--r--   0 franzi     (501) staff       (20)     1057 2016-11-03 21:17:21.000000 autofeat-2.1.1/LICENSE
+-rw-r--r--   0 franzi     (501) staff       (20)       16 2017-09-06 12:18:36.000000 autofeat-2.1.1/MANIFEST.in
+-rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-06-25 19:03:51.533086 autofeat-2.1.1/PKG-INFO
+-rw-r--r--   0 franzi     (501) staff       (20)     5190 2023-05-13 14:02:00.000000 autofeat-2.1.1/README.md
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.530579 autofeat-2.1.1/autofeat/
+-rw-r--r--   0 franzi     (501) staff       (20)      282 2023-06-25 19:01:09.000000 autofeat-2.1.1/autofeat/__init__.py
+-rw-r--r--   0 franzi     (501) staff       (20)    28722 2023-06-25 19:00:12.000000 autofeat-2.1.1/autofeat/autofeat.py
+-rw-r--r--   0 franzi     (501) staff       (20)    12893 2023-06-25 19:00:16.000000 autofeat-2.1.1/autofeat/autofeatlight.py
+-rw-r--r--   0 franzi     (501) staff       (20)    19894 2023-06-25 19:00:41.000000 autofeat-2.1.1/autofeat/feateng.py
+-rw-r--r--   0 franzi     (501) staff       (20)    17868 2023-06-25 19:00:36.000000 autofeat-2.1.1/autofeat/featsel.py
+-rw-r--r--   0 franzi     (501) staff       (20)      866 2023-06-25 19:00:30.000000 autofeat-2.1.1/autofeat/nb_utils.py
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.532288 autofeat-2.1.1/autofeat.egg-info/
+-rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/PKG-INFO
+-rw-r--r--   0 franzi     (501) staff       (20)      332 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/SOURCES.txt
+-rw-r--r--   0 franzi     (501) staff       (20)        1 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/dependency_links.txt
+-rw-r--r--   0 franzi     (501) staff       (20)       72 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/requires.txt
+-rw-r--r--   0 franzi     (501) staff       (20)        9 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/top_level.txt
+-rw-r--r--   0 franzi     (501) staff       (20)      891 2023-06-25 19:03:28.000000 autofeat-2.1.1/pyproject.toml
+-rw-r--r--   0 franzi     (501) staff       (20)       38 2023-06-25 19:03:51.533810 autofeat-2.1.1/setup.cfg
```

### Comparing `autofeat-2.1.0/LICENSE` & `autofeat-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autofeat-2.1.0/PKG-INFO` & `autofeat-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofeat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Automatic Feature Engineering and Selection Linear Prediction Model
 Author-email: Franziska Horn <cod3licious@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/cod3licious/autofeat
 Keywords: automl,feature engineering,feature selection,linear model
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `autofeat` library
 ### Linear Prediction Models with Automated Feature Engineering and Selection
 
 This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
```

### Comparing `autofeat-2.1.0/README.md` & `autofeat-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autofeat-2.1.0/autofeat/autofeat.py` & `autofeat-2.1.1/autofeat/autofeat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
+from __future__ import annotations
 import warnings
 import numba as nb
 import numpy as np
 import pandas as pd
 import sklearn.linear_model as lm
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.base import BaseEstimator, RegressorMixin, ClassifierMixin
```

### Comparing `autofeat-2.1.0/autofeat/autofeatlight.py` & `autofeat-2.1.1/autofeat/autofeatlight.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
+from __future__ import annotations
 import sys
 import numpy as np
 import pandas as pd
 from collections import defaultdict
 from typing import Tuple
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_array, check_is_fitted
```

### Comparing `autofeat-2.1.0/autofeat/feateng.py` & `autofeat-2.1.1/autofeat/feateng.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
+from __future__ import annotations
 import re
 import operator as op
 from functools import reduce
 from itertools import combinations, product
 from typing import Callable, Tuple
 
 import numba as nb
```

### Comparing `autofeat-2.1.0/autofeat/featsel.py` & `autofeat-2.1.1/autofeat/featsel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
+from __future__ import annotations
 import warnings
 import numpy as np
 import pandas as pd
 from collections import Counter
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
```

### Comparing `autofeat-2.1.0/autofeat/nb_utils.py` & `autofeat-2.1.1/autofeat/nb_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Author: Jeethu Rao <jboloor@acm.org>
 # License: MIT
 
+from __future__ import annotations
 import numba as nb
 import numpy as np
 
 
 @nb.njit(inline="always")
 def nb_apply_along_axis(func1d, axis, arr):
     assert arr.ndim == 2
```

### Comparing `autofeat-2.1.0/autofeat.egg-info/PKG-INFO` & `autofeat-2.1.1/autofeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofeat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Automatic Feature Engineering and Selection Linear Prediction Model
 Author-email: Franziska Horn <cod3licious@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/cod3licious/autofeat
 Keywords: automl,feature engineering,feature selection,linear model
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `autofeat` library
 ### Linear Prediction Models with Automated Feature Engineering and Selection
 
 This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
```

### Comparing `autofeat-2.1.0/pyproject.toml` & `autofeat-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autofeat"
-version = "2.1.0"
+version = "2.1.1"
 description = "Automatic Feature Engineering and Selection Linear Prediction Model"
 readme = "README.md"
 authors = [{ name = "Franziska Horn", email = "cod3licious@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -26,11 +26,11 @@
     "numba",
     "pandas>=0.24.0",
     "sympy>=1.7.1",
     "scikit-learn>=1.2.0",
     "joblib",
     "pint",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/cod3licious/autofeat"
```

