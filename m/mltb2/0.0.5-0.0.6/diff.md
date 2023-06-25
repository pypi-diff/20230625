# Comparing `tmp/mltb2-0.0.5.tar.gz` & `tmp/mltb2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltb2-0.0.5.tar", last modified: Sun Jun 11 10:23:10 2023, max compression
+gzip compressed data, was "dist/mltb2-0.0.6.tar", last modified: Sun Jun 25 05:59:46 2023, max compression
```

## Comparing `mltb2-0.0.5.tar` & `mltb2-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-11 10:23:00.000000 mltb2-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 10:23:00.000000 mltb2-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-11 10:23:10.000000 mltb2-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-11 10:23:00.000000 mltb2-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-11 10:23:00.000000 mltb2-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-11 10:23:10.000000 mltb2-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-11 10:23:00.000000 mltb2-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 05:59:34.000000 mltb2-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-25 05:59:34.000000 mltb2-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-25 05:59:46.000000 mltb2-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-25 05:59:34.000000 mltb2-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-25 05:59:34.000000 mltb2-0.0.6/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 05:59:46.000000 mltb2-0.0.6/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-25 05:59:34.000000 mltb2-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-25 05:59:46.000000 mltb2-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-25 05:59:34.000000 mltb2-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:46.000000 mltb2-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-25 05:59:34.000000 mltb2-0.0.6/tests/test_transformers.py
```

### Comparing `mltb2-0.0.5/LICENSE` & `mltb2-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/PKG-INFO` & `mltb2-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -26,16 +26,23 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: checking
+Provides-Extra: files
+Provides-Extra: fasttext
+Provides-Extra: optuna
+Provides-Extra: plot
+Provides-Extra: somajo
+Provides-Extra: transformers
+Provides-Extra: somajo_transformers
 Provides-Extra: optional
+Provides-Extra: checking
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
 
 # Machine Learning Toolbox 2 - MLTB2
 
@@ -84,14 +91,16 @@
 
 Some optional dependencies might be necessary. You can install all of them with:
 
 ```bash
 pip install mltb2[optional]
 ```
 
+If you don't want to install all dependencies, see the description of the individual modules.
+
 ## Licensing
 
 Copyright (c) 2023 Philip May\
 Copyright (c) 2023 Philip May, Deutsche Telekom AG
 
 Licensed under the **MIT License** (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License by reviewing the file
```

### Comparing `mltb2-0.0.5/README.md` & `mltb2-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 Some optional dependencies might be necessary. You can install all of them with:
 
 ```bash
 pip install mltb2[optional]
 ```
 
+If you don't want to install all dependencies, see the description of the individual modules.
+
 ## Licensing
 
 Copyright (c) 2023 Philip May\
 Copyright (c) 2023 Philip May, Deutsche Telekom AG
 
 Licensed under the **MIT License** (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License by reviewing the file
```

### Comparing `mltb2-0.0.5/mltb2/fasttext.py` & `mltb2-0.0.6/mltb2/fasttext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """fastText specific functionality.
 
 This module is based on `fastText <https://fasttext.cc/docs/en/support.html>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[fasttext]``
 """
 
 import os
 from dataclasses import dataclass, field
 
 import fasttext
 from fasttext.FastText import _FastText
```

### Comparing `mltb2-0.0.5/mltb2/files.py` & `mltb2-0.0.6/mltb2/files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""File utils."""
+"""File utils.
+
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[files]``
+"""
 
 
 import os
 from typing import Optional
 
 from platformdirs import user_data_dir
 from sklearn.datasets._base import RemoteFileMetadata, _fetch_remote
```

### Comparing `mltb2-0.0.5/mltb2/optuna.py` & `mltb2-0.0.6/mltb2/optuna.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2021 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """Optuna specific functionality.
 
 This module is based on `Optuna <https://optuna.readthedocs.io/en/stable/>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[optuna]``
 """
 
 
 import logging
 
 import numpy as np
 import optuna
```

### Comparing `mltb2-0.0.5/mltb2/plot.py` & `mltb2-0.0.6/mltb2/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2018 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """A collection of plot tools.
 
 This module is based on `Matplotlib <https://matplotlib.org/>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[plot]``
 """
 
 from typing import Optional
 
 import matplotlib.pyplot as plt
```

### Comparing `mltb2-0.0.5/mltb2/somajo.py` & `mltb2-0.0.6/mltb2/somajo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """SoMaJo specific functionality.
 
 This module is based on `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[somajo]``
 """
 
 
 from dataclasses import dataclass, field
 from typing import List, Set
 
 from somajo import SoMaJo
```

### Comparing `mltb2-0.0.5/mltb2/somajo_transformers.py` & `mltb2-0.0.6/mltb2/somajo_transformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # which is available at https://opensource.org/licenses/MIT
 
 """Hugging Face Transformers and SoMaJo specific functionality.
 
 This module is based on
 `Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_ and
 `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[somajo_transformers]``
 """
 
 
 from dataclasses import dataclass
 from typing import List
 
 from tqdm import tqdm
```

### Comparing `mltb2-0.0.5/mltb2/transformers.py` & `mltb2-0.0.6/mltb2/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """Hugging Face Transformers specific functionality.
 
 This module is based on
 `Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_.
+Use pip to install the necessary dependencies for this module:
+``pip install mltb2[transformers]``
 """
 
 import os
 from dataclasses import dataclass, field
 from typing import Iterable, List, Union
 
 import sklearn
```

### Comparing `mltb2-0.0.5/mltb2.egg-info/PKG-INFO` & `mltb2-0.0.6/mltb2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -26,16 +26,23 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: checking
+Provides-Extra: files
+Provides-Extra: fasttext
+Provides-Extra: optuna
+Provides-Extra: plot
+Provides-Extra: somajo
+Provides-Extra: transformers
+Provides-Extra: somajo_transformers
 Provides-Extra: optional
+Provides-Extra: checking
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
 
 # Machine Learning Toolbox 2 - MLTB2
 
@@ -84,14 +91,16 @@
 
 Some optional dependencies might be necessary. You can install all of them with:
 
 ```bash
 pip install mltb2[optional]
 ```
 
+If you don't want to install all dependencies, see the description of the individual modules.
+
 ## Licensing
 
 Copyright (c) 2023 Philip May\
 Copyright (c) 2023 Philip May, Deutsche Telekom AG
 
 Licensed under the **MIT License** (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License by reviewing the file
```

### Comparing `mltb2-0.0.5/mltb2.egg-info/SOURCES.txt` & `mltb2-0.0.6/mltb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/pyproject.toml` & `mltb2-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_fasttext.py` & `mltb2-0.0.6/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_files.py` & `mltb2-0.0.6/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_optuna.py` & `mltb2-0.0.6/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_somajo.py` & `mltb2-0.0.6/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_somajo_transformers.py` & `mltb2-0.0.6/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.5/tests/test_transformers.py` & `mltb2-0.0.6/tests/test_transformers.py`

 * *Files identical despite different names*

