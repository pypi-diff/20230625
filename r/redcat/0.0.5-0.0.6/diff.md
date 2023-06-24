# Comparing `tmp/redcat-0.0.5.tar.gz` & `tmp/redcat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.5.tar", max compression
+gzip compressed data, was "redcat-0.0.6.tar", max compression
```

## Comparing `redcat-0.0.5.tar` & `redcat-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1501 2023-05-27 20:07:39.776622 redcat-0.0.5/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-27 20:07:39.776622 redcat-0.0.5/README.md
--rw-r--r--   0        0        0     4407 2023-05-27 20:07:39.776622 redcat-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/__init__.py
--rw-r--r--   0        0        0    18034 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/base.py
--rw-r--r--   0        0        0    17391 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6733 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2428 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/comparators.py
--rw-r--r--   0        0        0        0 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/__init__.py
--rw-r--r--   0        0        0      315 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     4086 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/batching.py
--rw-r--r--   0        0        0     3728 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/joining.py
--rw-r--r--   0        0        0     2122 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0   140507 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/tensor.py
--rw-r--r--   0        0        0    52673 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    10148 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-06-24 23:40:47.361479 redcat-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2156 2023-06-24 23:40:47.361479 redcat-0.0.6/README.md
+-rw-r--r--   0        0        0     4330 2023-06-24 23:40:47.361479 redcat-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/__init__.py
+-rw-r--r--   0        0        0    18034 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/base.py
+-rw-r--r--   0        0        0    17391 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6733 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2769 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4109 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3764 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2158 2023-06-24 23:40:47.361479 redcat-0.0.6/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   140507 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/tensor.py
+-rw-r--r--   0        0        0    52673 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0     1128 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/format.py
+-rw-r--r--   0        0        0     1446 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/imports.py
+-rw-r--r--   0        0        0    10148 2023-06-24 23:40:47.365479 redcat-0.0.6/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 redcat-0.0.6/PKG-INFO
```

### Comparing `redcat-0.0.5/LICENSE` & `redcat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/README.md` & `redcat-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/pyproject.toml` & `redcat-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.5"
+version = "0.0.6"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
@@ -26,35 +26,29 @@
 
 packages = [
     { include = "redcat", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = "^0.0,>=0.0.7"
-numpy = "^1.24"
+coola = ">=0.0.12,<1.0"
+numpy = ">=1.24,<2.0"
 python = "^3.9"
-torch = "^2.0"
-polars = { version = "^0.17", optional = true }
-
-[tool.poetry.extras]
-all = [
-    "polars",
-]
+torch = ">=2.0.1,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
 coverage = { extras = ["toml"], version = "^7.2" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.3"
 pylint = "^2.17"
 pytest = "^7.3"
 pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = "^0.0,>=0.0.270"
+ruff = ">=0.0.275,<1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `redcat-0.0.5/src/redcat/base.py` & `redcat-0.0.6/src/redcat/base.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/batchdict.py` & `redcat-0.0.6/src/redcat/batchdict.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/batchlist.py` & `redcat-0.0.6/src/redcat/batchlist.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/datapipes/iter/batching.py` & `redcat-0.0.6/src/redcat/datapipes/iter/batching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 __all__ = ["MiniBatcherIterDataPipe"]
 
 import logging
 from collections.abc import Iterator
-from typing import TypeVar, Union
+from typing import TypeVar
 
 from coola.utils.format import str_indent
 from torch.utils.data import IterDataPipe
 from torch.utils.data.datapipes.iter import IterableWrapper
 
 from redcat.base import BaseBatch
 from redcat.utils.tensor import get_torch_generator
@@ -57,15 +59,15 @@
          tensor([4, 5], batch_dim=0),
          tensor([6, 7], batch_dim=0),
          tensor([8], batch_dim=0)]
     """
 
     def __init__(
         self,
-        datapipe_or_batch: Union[IterDataPipe[BaseBatch[T]], BaseBatch[T]],
+        datapipe_or_batch: IterDataPipe[BaseBatch[T]] | BaseBatch[T],
         batch_size: int,
         drop_last: bool = False,
         shuffle: bool = False,
         random_seed: int = 5513175564631803238,
     ) -> None:
         self._datapipe_or_batch = datapipe_or_batch
         self._batch_size = int(batch_size)
```

### Comparing `redcat-0.0.5/src/redcat/datapipes/iter/joining.py` & `redcat-0.0.6/src/redcat/datapipes/iter/joining.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = ["BatchExtenderIterDataPipe", "create_large_batch"]
 
 import logging
 from collections.abc import Iterator, Sequence
 from typing import TypeVar
 
 from coola.utils.format import str_indent
```

### Comparing `redcat-0.0.5/src/redcat/datapipes/iter/shuffling.py` & `redcat-0.0.6/src/redcat/datapipes/iter/shuffling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = ["BatchShufflerIterDataPipe"]
 
 import logging
 from collections.abc import Iterator
 from typing import TypeVar
 
 from coola.utils.format import str_indent
```

### Comparing `redcat-0.0.5/src/redcat/tensor.py` & `redcat-0.0.6/src/redcat/tensor.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/tensorseq.py` & `redcat-0.0.6/src/redcat/tensorseq.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/utils/format.py` & `redcat-0.0.6/src/redcat/utils/format.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/utils/imports.py` & `redcat-0.0.6/src/redcat/utils/imports.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/src/redcat/utils/tensor.py` & `redcat-0.0.6/src/redcat/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.5/PKG-INFO` & `redcat-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -17,19 +17,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: all
-Requires-Dist: coola (>=0.0.7,<0.1)
+Requires-Dist: coola (>=0.0.12,<1.0)
 Requires-Dist: numpy (>=1.24,<2.0)
-Requires-Dist: polars (>=0.17,<0.18) ; extra == "all"
-Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/durandtibo/redcat
 Description-Content-Type: text/markdown
 
 # redcat
 
 <p align="center">
     <a href="https://github.com/durandtibo/redcat/actions">
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.5 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.6 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries Provides-Extra: all Requires-Dist: coola
-(>=0.0.7,<0.1) Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: polars
-(>=0.17,<0.18) ; extra == "all" Requires-Dist: torch (>=2.0,<3.0) Project-URL:
+Development :: Libraries Requires-Dist: coola (>=0.0.12,<1.0) Requires-Dist:
+numpy (>=1.24,<2.0) Requires-Dist: torch (>=2.0.1,<3.0.0) Project-URL:
 Repository, https://github.com/durandtibo/redcat Description-Content-Type:
 text/markdown # redcat
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  0987ab26fe4d52025085/maintainability] [https://api.codeclimate.com/v1/badges/
                      0987ab26fe4d52025085/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
```

