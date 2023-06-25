# Comparing `tmp/monstermash-1.0.1.tar.gz` & `tmp/monstermash-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.0.1.tar", max compression
+gzip compressed data, was "monstermash-1.1.0.tar", max compression
```

## Comparing `monstermash-1.0.1.tar` & `monstermash-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1366 2023-06-25 04:08:12.643755 monstermash-1.0.1/README.md
--rw-r--r--   0        0        0     1055 2023-06-25 04:08:12.643755 monstermash-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/__init__.py
--rw-r--r--   0        0        0     1646 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1772 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/crypt.py
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1366 2023-06-25 04:39:34.307284 monstermash-1.1.0/README.md
+-rw-r--r--   0        0        0     1080 2023-06-25 04:39:34.311284 monstermash-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     1646 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1772 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/crypt.py
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 monstermash-1.1.0/PKG-INFO
```

### Comparing `monstermash-1.0.1/README.md` & `monstermash-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.0.1
+> 1️⃣ version: 1.1.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-1.0.1/pyproject.toml` & `monstermash-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "monstermash"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">=3.8.1,<3.12"
 pynacl = "^1.5.0"
 click = "^8.1.3"
 pydantic = "^1.10.7"
 questionary = "^1.10.0"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -35,14 +35,15 @@
 mkautodoc = "^0.2.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-dotenv = "^0.5.2"
 pytest-cov = "^4.0.0"
+scipy = "^1.10.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 monstermash = { callable = "monstermash.__main__:main"}
```

### Comparing `monstermash-1.0.1/src/monstermash/__main__.py` & `monstermash-1.1.0/src/monstermash/__main__.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.0.1/src/monstermash/crypt.py` & `monstermash-1.1.0/src/monstermash/crypt.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.0.1/PKG-INFO` & `monstermash-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.0.1
+> 1️⃣ version: 1.1.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

