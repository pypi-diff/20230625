# Comparing `tmp/autonomy_dev-0.1.6.tar.gz` & `tmp/autonomy_dev-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.6.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.7.tar", max compression
```

## Comparing `autonomy_dev-0.1.6.tar` & `autonomy_dev-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0      578 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/LICENSE
--rw-r--r--   0        0        0      368 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/__init__.py
--rw-r--r--   0        0        0     3151 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/cli.py
--rw-r--r--   0        0        0     2822 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/cli_executor.py
--rw-r--r--   0        0        0      301 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/constants.py
--rw-r--r--   0        0        0      642 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      464 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/test.py
--rw-r--r--   0        0        0     1083 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/utils.py
--rw-r--r--   0        0        0     2518 2023-06-18 14:35:10.774490 autonomy_dev-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-06-18 14:35:10.774490 autonomy_dev-0.1.6/tests/test_cli.py
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 autonomy_dev-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-06-25 13:59:32.323627 autonomy_dev-0.1.7/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-25 13:59:32.323627 autonomy_dev-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 13:59:32.323627 autonomy_dev-0.1.7/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2454 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     4303 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     1890 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     1984 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     1457 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      369 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/constants.py
+-rw-r--r--   0        0        0      173 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      642 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0     2027 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/fmt.py
+-rw-r--r--   0        0        0      464 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/test.py
+-rw-r--r--   0        0        0     1585 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/auto_dev/utils.py
+-rw-r--r--   0        0        0     2509 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1634 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1484 2023-06-25 13:59:32.327627 autonomy_dev-0.1.7/tests/test_cli.py
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 autonomy_dev-0.1.7/PKG-INFO
```

### Comparing `autonomy_dev-0.1.6/LICENSE` & `autonomy_dev-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.6/auto_dev/cli_executor.py` & `autonomy_dev-0.1.7/auto_dev/cli_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,15 @@
     def execute(self, stream=False, verbose: bool = True):
         """Execute the command."""
         if stream:
             return self._execute_stream(verbose)
         logger.debug(f"Executing command:\n\"\"\n{' '.join(self.command)}\n\"\"")
         try:
             result = subprocess.run(
-                self.command,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                cwd=self.cwd, check=False,
-                env=os.environ
+                self.command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=self.cwd, check=False, env=os.environ
             )
             if verbose:
                 if len(result.stdout) > 0:
                     logger.info(result.stdout.decode("utf-8"))
                 if len(result.stderr) > 0:
                     logger.error(result.stderr.decode("utf-8"))
```

### Comparing `autonomy_dev-0.1.6/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.7/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.6/auto_dev/utils.py` & `autonomy_dev-0.1.7/auto_dev/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Utilities for auto_dev.
 """
 import json
 import logging
+from functools import reduce
+from glob import glob
 from pathlib import Path
+from typing import Optional
 
 from rich.logging import RichHandler
 
 from .constants import AUTONOMY_PACKAGES_FILE, DEFAULT_ENCODING
 
 
-def get_logger(name=__name__):
+def get_logger(name=__name__, log_level="INFO"):
     """Get the logger."""
     msg_format = "%(message)s"
     handler = RichHandler(
         rich_tracebacks=True,
         markup=True,
     )
     logging.basicConfig(level="NOTSET", format=msg_format, datefmt="[%X]", handlers=[handler])
 
     log = logging.getLogger(name)
+    log.setLevel(log_level)
     return log
 
 
 def get_packages():
     """Get the packages file."""
     with open(AUTONOMY_PACKAGES_FILE, "r", encoding=DEFAULT_ENCODING) as file:
         packages = json.load(file)
@@ -32,7 +36,15 @@
     for package in dev_packages:
         component_type, author, component_name, _ = package.split("/")
         package_path = Path(f"packages/{author}/{component_type}s/{component_name}")
         if not package_path.exists():
             raise FileNotFoundError(f"Package {package} does not exist")
         results.append(package_path)
     return results
+
+
+def get_paths(path=Optional[str]):
+    """Get the paths."""
+    if not path and not Path(AUTONOMY_PACKAGES_FILE).exists():
+        raise FileNotFoundError("No path was provided and no default packages file found")
+    packages = get_packages() if not path else [path]
+    return reduce(lambda x, y: x + y, [glob(f"{package}/**/*py", recursive=True) for package in packages])
```

### Comparing `autonomy_dev-0.1.6/pyproject.toml` & `autonomy_dev-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.6"
+version = "0.1.7"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "auto_dev" },
     { include = "tests", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.2,<4.0"
+python = ">=3.7,<3.11"
 click = ">=8.0.2"
 black = "^22.6.0"
-isort = "^5.10.1"
 mypy = "^0.971"
 pytest-cov = "^3.0.0"
 tox = "^3.25.1"
 pip = "^22.2.2"
 mkdocs = "^1.3.1"
 mkdocs-include-markdown-plugin = "^3.6.1"
 mkdocs-material = "^8.4.0"
@@ -44,15 +43,16 @@
 bump2version = "^1.0.1"
 yamllint = "^1.27.1"
 GitPython = "^3.1.27"
 pylama = {extras = ["all"], version = "^8.4.1"}
 rich-click = "^1.5.2"
 install = "^1.3.5"
 mkdocstrings-python = "^0.10.0"
-pylint = "^2.17.4"
+isort = "~5"
+pylint = "~2"
 
 [tool.poetry.dev-dependencies]
 
 
 [tool.poetry.extras]
 all = [
     "pytest",
```

### Comparing `autonomy_dev-0.1.6/PKG-INFO` & `autonomy_dev-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
-Requires-Python: >=3.7.2,<4.0
+Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: click (>=8.0.2)
 Requires-Dist: install (>=1.3.5,<2.0.0)
-Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "all"
+Requires-Dist: isort (>=5,<6) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
 Requires-Dist: mkdocstrings-python (>=0.10.0,<0.11.0)
 Requires-Dist: mypy (>=0.971,<0.972) ; extra == "all"
 Requires-Dist: pip (>=22.2.2,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pylama[all] (>=8.4.1,<9.0.0) ; extra == "all"
-Requires-Dist: pylint (>=2.17.4,<3.0.0) ; extra == "all"
+Requires-Dist: pylint (>=2,<3) ; extra == "all"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "all"
 Requires-Dist: rich-click (>=1.5.2,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.25.1,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=4.0.1,<5.0.0) ; extra == "dev"
 Requires-Dist: yamllint (>=1.27.1,<2.0.0)
 Description-Content-Type: text/markdown
```

