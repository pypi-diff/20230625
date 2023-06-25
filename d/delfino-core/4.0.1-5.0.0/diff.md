# Comparing `tmp/delfino_core-4.0.1.tar.gz` & `tmp/delfino_core-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino_core-4.0.1.tar", max compression
+gzip compressed data, was "delfino_core-5.0.0.tar", max compression
```

## Comparing `delfino_core-4.0.1.tar` & `delfino_core-5.0.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1078 2022-12-29 20:35:10.986732 delfino_core-4.0.1/LICENSE.md
--rw-r--r--   0        0        0     5291 2022-12-29 20:35:10.986732 delfino_core-4.0.1/README.md
--rw-r--r--   0        0        0     4204 2022-12-29 20:35:10.986732 delfino_core-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/__init__.py
--rw-r--r--   0        0        0      293 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/backports.py
--rw-r--r--   0        0        0        0 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/__init__.py
--rw-r--r--   0        0        0     9055 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/dependencies_update.py
--rw-r--r--   0        0        0     2738 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/format.py
--rw-r--r--   0        0        0     6681 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/lint.py
--rw-r--r--   0        0        0     3471 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/switch_python_version.py
--rw-r--r--   0        0        0     7883 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/test.py
--rw-r--r--   0        0        0     3392 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/typecheck.py
--rw-r--r--   0        0        0      748 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/commands/verify_all.py
--rw-r--r--   0        0        0      904 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/config.py
--rw-r--r--   0        0        0     1720 2022-12-29 20:35:10.990732 delfino_core-4.0.1/src/delfino_core/utils.py
--rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 delfino_core-4.0.1/setup.py
--rw-r--r--   0        0        0     7717 1970-01-01 00:00:00.000000 delfino_core-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-25 11:49:06.204935 delfino_core-5.0.0/LICENSE.md
+-rw-r--r--   0        0        0     5291 2023-06-25 11:49:06.204935 delfino_core-5.0.0/README.md
+-rw-r--r--   0        0        0     4197 2023-06-25 11:49:06.204935 delfino_core-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/backports.py
+-rw-r--r--   0        0        0        0 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/__init__.py
+-rw-r--r--   0        0        0     9055 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/dependencies_update.py
+-rw-r--r--   0        0        0     2737 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/format.py
+-rw-r--r--   0        0        0     6681 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/lint.py
+-rw-r--r--   0        0        0     3471 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/switch_python_version.py
+-rw-r--r--   0        0        0     7883 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/test.py
+-rw-r--r--   0        0        0     3392 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/typecheck.py
+-rw-r--r--   0        0        0      748 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/commands/verify_all.py
+-rw-r--r--   0        0        0      904 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/config.py
+-rw-r--r--   0        0        0     1720 2023-06-25 11:49:06.204935 delfino_core-5.0.0/src/delfino_core/utils.py
+-rw-r--r--   0        0        0     7463 1970-01-01 00:00:00.000000 delfino_core-5.0.0/PKG-INFO
```

### Comparing `delfino_core-4.0.1/LICENSE.md` & `delfino_core-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/README.md` & `delfino_core-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/pyproject.toml` & `delfino_core-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="delfino-core"
-version="4.0.1"
+version="5.0.0"
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 description="Delfino core plugin"
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino-core"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 delfino = ">=0.29.0"
 
 black = {version = "*", optional = true}
 isort = {version = "*", optional = true}
 pre-commit = {version = "*", optional = true}
 pytest = {version = "*", optional = true}
 coverage = {version = "*", optional = true}
@@ -44,23 +44,23 @@
 # https://python-poetry.org/docs/pyproject/#plugins
 [tool.poetry.plugins]
 
 [tool.poetry.plugins."delfino.plugin"]
 "delfino-core" = "delfino_core.commands"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.6"
-isort = "^5.9.3"
+black = "^23.3"
+isort = "^5.9"
 coverage = "^7.0"
 pylint = "^2.11"
-mypy = "^0.991"
+mypy = "^1.4"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
-pre-commit = "^2.15"
+pre-commit = "^3.3"
 pycodestyle = "^2.8"
 pydocstyle = "^6.1"
 shellingham = "^1.4"
 psutil = "^5.9.4"
 types-termcolor = "*"
 types-toml = "^0.10.8.1"
 types-psutil = "^5.9.5.5"
```

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/dependencies_update.py` & `delfino_core-5.0.0/src/delfino_core/commands/dependencies_update.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/format.py` & `delfino_core-5.0.0/src/delfino_core/commands/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from delfino.validation import assert_pip_package_installed
 
 from delfino_core.config import CorePluginConfig, pass_plugin_app_context
 
 
 def _check_result(app_context: AppContext[CorePluginConfig], result: CompletedProcess, check: bool, msg: str):
     if result.returncode == 1 and check:
-
         msg_lines = [
             f"{msg} before commit. Try following:",
             f" * Run formatter manually with `{run_command_example(run_format, app_context)}` before committing code.",
         ]
         if not app_context.plugin_config.disable_pre_commit:
             msg_lines.insert(1, " * Enable pre-commit hook by running `pre-commit install` in the repository.")
```

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/lint.py` & `delfino_core-5.0.0/src/delfino_core/commands/lint.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/switch_python_version.py` & `delfino_core-5.0.0/src/delfino_core/commands/switch_python_version.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/test.py` & `delfino_core-5.0.0/src/delfino_core/commands/test.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/typecheck.py` & `delfino_core-5.0.0/src/delfino_core/commands/typecheck.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/commands/verify_all.py` & `delfino_core-5.0.0/src/delfino_core/commands/verify_all.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/config.py` & `delfino_core-5.0.0/src/delfino_core/config.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/src/delfino_core/utils.py` & `delfino_core-5.0.0/src/delfino_core/utils.py`

 * *Files identical despite different names*

### Comparing `delfino_core-4.0.1/setup.py` & `delfino_core-5.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,179 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: delfino-core
+Version: 5.0.0
+Summary: Delfino core plugin
+Home-page: https://github.com/radeklat/delfino-core
+License: MIT
+Author: Radek Lát
+Author-email: radek.lat@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Provides-Extra: all
+Provides-Extra: dependencies-update
+Provides-Extra: format
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: typecheck
+Provides-Extra: verify-all
+Requires-Dist: black ; extra == "all" or extra == "verify-all" or extra == "format"
+Requires-Dist: coverage ; extra == "all" or extra == "verify-all" or extra == "test"
+Requires-Dist: delfino (>=0.29.0)
+Requires-Dist: gitpython ; extra == "all" or extra == "dependencies-update"
+Requires-Dist: isort ; extra == "all" or extra == "verify-all" or extra == "format"
+Requires-Dist: mypy ; extra == "all" or extra == "verify-all" or extra == "typecheck"
+Requires-Dist: pre-commit ; extra == "all" or extra == "verify-all" or extra == "format"
+Requires-Dist: psutil ; extra == "all" or extra == "verify-all" or extra == "lint"
+Requires-Dist: pycodestyle ; extra == "all" or extra == "verify-all" or extra == "lint"
+Requires-Dist: pydocstyle ; extra == "all" or extra == "verify-all" or extra == "lint"
+Requires-Dist: pylint ; extra == "all" or extra == "verify-all" or extra == "lint"
+Requires-Dist: pytest ; extra == "all" or extra == "verify-all" or extra == "test"
+Requires-Dist: pytest-cov ; extra == "all" or extra == "verify-all" or extra == "test"
+Requires-Dist: shellingham
+Description-Content-Type: text/markdown
+
+<h1 align="center" style="border-bottom: none;"> 🔌&nbsp;&nbsp;Delfino Core&nbsp;&nbsp; 🔌</h1>
+<h3 align="center">A <a href="https://github.com/radeklat/delfino">Delfino</a> plugin with core functionality.</h3>
+
+<p align="center">
+    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino-core?branch=main">
+        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino-core">
+    </a>
+    <a href="https://app.codecov.io/gh/radeklat/delfino-core/">
+        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino-core">
+    </a>
+    <a href="https://github.com/radeklat/delfino-core/tags">
+        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino-core">
+    </a>
+    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2022">
+    <a href="https://github.com/radeklat/delfino-core/commits/main">
+        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino-core">
+    </a>
+    <a href="https://www.python.org/doc/versions/">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino-core">
+    </a>
+    <a href="https://pypistats.org/packages/delfino-core">
+        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino-core">
+    </a>
+</p>
+
+# Commands
+  
+| Command               | Description                                         |
+|-----------------------|-----------------------------------------------------|
+| coverage-open         | Open coverage results in default browser.           |
+| coverage-report       | Analyse coverage and generate a term/HTML report.   |
+| dependencies-update   | Manages the process of updating dependencies.       |
+| format                | Runs black code formatter and isort on source code. |
+| lint                  | Run linting on the entire code base.                |
+| lint-pycodestyle      | Run PEP8 checking on code.                          |
+| lint-pydocstyle       | Run docstring linting on source code.               |
+| lint-pylint           | Run pylint on code.                                 |
+| switch-python-version | Switches Python venv to a different Python version. |
+| test-all              | Run all tests, and generate coverage report.        |
+| test-integration      | Run integration tests.                              |
+| test-unit             | Run unit tests.                                     |
+| typecheck             | Run type checking on source code.                   |
+| verify-all            | Runs all verification commands.                     |
+
+# Installation
+
+- pip: `pip install delfino-core`
+- Poetry: `poetry add -D delfino-core`
+- Pipenv: `pipenv install -d delfino-core`
+
+## Optional dependencies
+
+Each project may use different sub-set of [commands](#commands). Therefore, dependencies of all commands are optional and checked only when the command is executed.
+
+Using `[all]` installs all the [optional dependencies](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) used by all the commands. If you want only a sub-set of those dependencies, there are finer-grained groups available:
+
+- For individual commands (matches the command names):
+  - `typecheck`
+  - `format`
+  - `dependencies-update`
+- For groups of commands:
+  - `test` - for testing and coverage commands
+  - `lint` - for all the linting commands
+- For groups of groups:
+  - `verify-all` - same as `[typecheck,format,test,lint]`
+  - `all` - all optional packages
+
+# Configuration
+
+Delfino doesn't load any plugins by default. To enable this plugin, add the following config into `pyproject.toml`:
+
+```toml
+[tool.delfino.plugins.delfino-core]
+
+```
+
+## Plugin configuration
+
+This plugin has several options. All the values are optional and defaults are shown below: 
+
+```toml
+[tool.delfino.plugins.delfino-core]
+# Source files - may have different rules than tests (usually stricter)
+sources_directory = "src"
+
+# Test files
+tests_directory = "tests"
+
+# Where to store reports generated by various tools
+reports_directory = "reports"
+
+# Types of tests you have nested under the `tests_directory`. Will be executed in given order.
+test_types = ["unit", "integration"]
+
+# One or more module to wrap `pytest` in, executing it as `python -m <MODULE> pytest ...`
+pytest_modules = []
+
+# Commands to run as a quality gate in given order.
+verify_commands = ["format", "lint", "typecheck", "test-all"]
+
+# Do not install pre-commit if this is set to true.
+disable_pre_commit = false
+```
+
+## Commands configuration
+
+Several commands have their own configuration as well:
+
+```toml
+[tool.delfino.plugins.delfino-core.typecheck]
+# One or more directories where type hint will be required. By default they are optional.
+strict_directories = []  
+```
+
+# Usage
+
+Run `delfino --help`.
+
+# Development
+
+To develop against editable `delfino` sources:
+
+1. Make sure `delfino` sources are next to this plugin:
+    ```shell
+    cd ..
+    git clone https://github.com/radeklat/delfino.git
+    ```
+2. Install `delfino` as editable package:
+    ```shell
+    pip install -e ../delfino
+    ```
+   Note that poetry will reset this to the released package when you install/update anything.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['delfino_core', 'delfino_core.commands']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['delfino>=0.29.0']
-
-extras_require = \
-{'all': ['black',
-         'isort',
-         'pre-commit',
-         'pytest',
-         'coverage',
-         'pytest-cov',
-         'mypy',
-         'pylint',
-         'pycodestyle',
-         'pydocstyle',
-         'gitpython',
-         'psutil'],
- 'dependencies-update': ['gitpython'],
- 'format': ['black', 'isort', 'pre-commit'],
- 'lint': ['pylint', 'pycodestyle', 'pydocstyle', 'psutil'],
- 'test': ['pytest', 'coverage', 'pytest-cov'],
- 'typecheck': ['mypy'],
- 'verify-all': ['black',
-                'isort',
-                'pre-commit',
-                'pytest',
-                'coverage',
-                'pytest-cov',
-                'mypy',
-                'pylint',
-                'pycodestyle',
-                'pydocstyle',
-                'psutil']}
-
-entry_points = \
-{'delfino.plugin': ['delfino-core = delfino_core.commands']}
-
-setup_kwargs = {
-    'name': 'delfino-core',
-    'version': '4.0.1',
-    'description': 'Delfino core plugin',
-    'long_description': '<h1 align="center" style="border-bottom: none;"> 🔌&nbsp;&nbsp;Delfino Core&nbsp;&nbsp; 🔌</h1>\n<h3 align="center">A <a href="https://github.com/radeklat/delfino">Delfino</a> plugin with core functionality.</h3>\n\n<p align="center">\n    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino-core?branch=main">\n        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino-core">\n    </a>\n    <a href="https://app.codecov.io/gh/radeklat/delfino-core/">\n        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino-core">\n    </a>\n    <a href="https://github.com/radeklat/delfino-core/tags">\n        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino-core">\n    </a>\n    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2022">\n    <a href="https://github.com/radeklat/delfino-core/commits/main">\n        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino-core">\n    </a>\n    <a href="https://www.python.org/doc/versions/">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino-core">\n    </a>\n    <a href="https://pypistats.org/packages/delfino-core">\n        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino-core">\n    </a>\n</p>\n\n# Commands\n  \n| Command               | Description                                         |\n|-----------------------|-----------------------------------------------------|\n| coverage-open         | Open coverage results in default browser.           |\n| coverage-report       | Analyse coverage and generate a term/HTML report.   |\n| dependencies-update   | Manages the process of updating dependencies.       |\n| format                | Runs black code formatter and isort on source code. |\n| lint                  | Run linting on the entire code base.                |\n| lint-pycodestyle      | Run PEP8 checking on code.                          |\n| lint-pydocstyle       | Run docstring linting on source code.               |\n| lint-pylint           | Run pylint on code.                                 |\n| switch-python-version | Switches Python venv to a different Python version. |\n| test-all              | Run all tests, and generate coverage report.        |\n| test-integration      | Run integration tests.                              |\n| test-unit             | Run unit tests.                                     |\n| typecheck             | Run type checking on source code.                   |\n| verify-all            | Runs all verification commands.                     |\n\n# Installation\n\n- pip: `pip install delfino-core`\n- Poetry: `poetry add -D delfino-core`\n- Pipenv: `pipenv install -d delfino-core`\n\n## Optional dependencies\n\nEach project may use different sub-set of [commands](#commands). Therefore, dependencies of all commands are optional and checked only when the command is executed.\n\nUsing `[all]` installs all the [optional dependencies](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) used by all the commands. If you want only a sub-set of those dependencies, there are finer-grained groups available:\n\n- For individual commands (matches the command names):\n  - `typecheck`\n  - `format`\n  - `dependencies-update`\n- For groups of commands:\n  - `test` - for testing and coverage commands\n  - `lint` - for all the linting commands\n- For groups of groups:\n  - `verify-all` - same as `[typecheck,format,test,lint]`\n  - `all` - all optional packages\n\n# Configuration\n\nDelfino doesn\'t load any plugins by default. To enable this plugin, add the following config into `pyproject.toml`:\n\n```toml\n[tool.delfino.plugins.delfino-core]\n\n```\n\n## Plugin configuration\n\nThis plugin has several options. All the values are optional and defaults are shown below: \n\n```toml\n[tool.delfino.plugins.delfino-core]\n# Source files - may have different rules than tests (usually stricter)\nsources_directory = "src"\n\n# Test files\ntests_directory = "tests"\n\n# Where to store reports generated by various tools\nreports_directory = "reports"\n\n# Types of tests you have nested under the `tests_directory`. Will be executed in given order.\ntest_types = ["unit", "integration"]\n\n# One or more module to wrap `pytest` in, executing it as `python -m <MODULE> pytest ...`\npytest_modules = []\n\n# Commands to run as a quality gate in given order.\nverify_commands = ["format", "lint", "typecheck", "test-all"]\n\n# Do not install pre-commit if this is set to true.\ndisable_pre_commit = false\n```\n\n## Commands configuration\n\nSeveral commands have their own configuration as well:\n\n```toml\n[tool.delfino.plugins.delfino-core.typecheck]\n# One or more directories where type hint will be required. By default they are optional.\nstrict_directories = []  \n```\n\n# Usage\n\nRun `delfino --help`.\n\n# Development\n\nTo develop against editable `delfino` sources:\n\n1. Make sure `delfino` sources are next to this plugin:\n    ```shell\n    cd ..\n    git clone https://github.com/radeklat/delfino.git\n    ```\n2. Install `delfino` as editable package:\n    ```shell\n    pip install -e ../delfino\n    ```\n   Note that poetry will reset this to the released package when you install/update anything.\n',
-    'author': 'Radek Lát',
-    'author_email': 'radek.lat@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/radeklat/delfino-core',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,74 +1,78 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['delfino_core', 'delfino_core.commands'] package_data = \
-{'': ['*']} install_requires = \ ['delfino>=0.29.0'] extras_require = \ {'all':
-['black', 'isort', 'pre-commit', 'pytest', 'coverage', 'pytest-cov', 'mypy',
-'pylint', 'pycodestyle', 'pydocstyle', 'gitpython', 'psutil'], 'dependencies-
-update': ['gitpython'], 'format': ['black', 'isort', 'pre-commit'], 'lint':
-['pylint', 'pycodestyle', 'pydocstyle', 'psutil'], 'test': ['pytest',
-'coverage', 'pytest-cov'], 'typecheck': ['mypy'], 'verify-all': ['black',
-'isort', 'pre-commit', 'pytest', 'coverage', 'pytest-cov', 'mypy', 'pylint',
-'pycodestyle', 'pydocstyle', 'psutil']} entry_points = \ {'delfino.plugin':
-['delfino-core = delfino_core.commands']} setup_kwargs = { 'name': 'delfino-
-core', 'version': '4.0.1', 'description': 'Delfino core plugin',
-'long_description': '
+Metadata-Version: 2.1 Name: delfino-core Version: 5.0.0 Summary: Delfino core
+plugin Home-page: https://github.com/radeklat/delfino-core License: MIT Author:
+Radek LÃ¡t Author-email: radek.lat@gmail.com Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7 Classifier: Topic :: Software
+Development Classifier: Topic :: Utilities Provides-Extra: all Provides-Extra:
+dependencies-update Provides-Extra: format Provides-Extra: lint Provides-Extra:
+test Provides-Extra: typecheck Provides-Extra: verify-all Requires-Dist: black
+; extra == "all" or extra == "verify-all" or extra == "format" Requires-Dist:
+coverage ; extra == "all" or extra == "verify-all" or extra == "test" Requires-
+Dist: delfino (>=0.29.0) Requires-Dist: gitpython ; extra == "all" or extra ==
+"dependencies-update" Requires-Dist: isort ; extra == "all" or extra ==
+"verify-all" or extra == "format" Requires-Dist: mypy ; extra == "all" or extra
+== "verify-all" or extra == "typecheck" Requires-Dist: pre-commit ; extra ==
+"all" or extra == "verify-all" or extra == "format" Requires-Dist: psutil ;
+extra == "all" or extra == "verify-all" or extra == "lint" Requires-Dist:
+pycodestyle ; extra == "all" or extra == "verify-all" or extra == "lint"
+Requires-Dist: pydocstyle ; extra == "all" or extra == "verify-all" or extra ==
+"lint" Requires-Dist: pylint ; extra == "all" or extra == "verify-all" or extra
+== "lint" Requires-Dist: pytest ; extra == "all" or extra == "verify-all" or
+extra == "test" Requires-Dist: pytest-cov ; extra == "all" or extra == "verify-
+all" or extra == "test" Requires-Dist: shellingham Description-Content-Type:
+text/markdown
                     ****** ð  Delfino Core   ð ******
-\n
               **** A Delfino plugin with core functionality. ****
-\n\n
-  \n \n_[CircleCI]\n\n \n_[Codecov]\n\n \n_[GitHub_tag_(latest_SemVer)]\n\n
-[Maintenance]\n \n_[GitHub_last_commit]\n\n \n_[PyPI_-_Python_Version]\n\n \n_
-                                [Downloads]\n\n
-\n\n# Commands\n \n| Command | Description |\n|-----------------------|--------
----------------------------------------------|\n| coverage-open | Open coverage
-results in default browser. |\n| coverage-report | Analyse coverage and
-generate a term/HTML report. |\n| dependencies-update | Manages the process of
-updating dependencies. |\n| format | Runs black code formatter and isort on
-source code. |\n| lint | Run linting on the entire code base. |\n| lint-
-pycodestyle | Run PEP8 checking on code. |\n| lint-pydocstyle | Run docstring
-linting on source code. |\n| lint-pylint | Run pylint on code. |\n| switch-
-python-version | Switches Python venv to a different Python version. |\n| test-
-all | Run all tests, and generate coverage report. |\n| test-integration | Run
-integration tests. |\n| test-unit | Run unit tests. |\n| typecheck | Run type
-checking on source code. |\n| verify-all | Runs all verification commands.
-|\n\n# Installation\n\n- pip: `pip install delfino-core`\n- Poetry: `poetry add
--D delfino-core`\n- Pipenv: `pipenv install -d delfino-core`\n\n## Optional
-dependencies\n\nEach project may use different sub-set of [commands]
-(#commands). Therefore, dependencies of all commands are optional and checked
-only when the command is executed.\n\nUsing `[all]` installs all the [optional
-dependencies](https://setuptools.pypa.io/en/latest/userguide/
+ [CircleCI] [Codecov] [GitHub_tag_(latest_SemVer)] [Maintenance] [GitHub_last
+                  commit] [PyPI_-_Python_Version] [Downloads]
+# Commands | Command | Description | |-----------------------|-----------------
+------------------------------------| | coverage-open | Open coverage results
+in default browser. | | coverage-report | Analyse coverage and generate a term/
+HTML report. | | dependencies-update | Manages the process of updating
+dependencies. | | format | Runs black code formatter and isort on source code.
+| | lint | Run linting on the entire code base. | | lint-pycodestyle | Run PEP8
+checking on code. | | lint-pydocstyle | Run docstring linting on source code. |
+| lint-pylint | Run pylint on code. | | switch-python-version | Switches Python
+venv to a different Python version. | | test-all | Run all tests, and generate
+coverage report. | | test-integration | Run integration tests. | | test-unit |
+Run unit tests. | | typecheck | Run type checking on source code. | | verify-
+all | Runs all verification commands. | # Installation - pip: `pip install
+delfino-core` - Poetry: `poetry add -D delfino-core` - Pipenv: `pipenv install
+-d delfino-core` ## Optional dependencies Each project may use different sub-
+set of [commands](#commands). Therefore, dependencies of all commands are
+optional and checked only when the command is executed. Using `[all]` installs
+all the [optional dependencies](https://setuptools.pypa.io/en/latest/userguide/
 dependency_management.html#optional-dependencies) used by all the commands. If
 you want only a sub-set of those dependencies, there are finer-grained groups
-available:\n\n- For individual commands (matches the command names):\n -
-`typecheck`\n - `format`\n - `dependencies-update`\n- For groups of commands:\n
-- `test` - for testing and coverage commands\n - `lint` - for all the linting
-commands\n- For groups of groups:\n - `verify-all` - same as `
-[typecheck,format,test,lint]`\n - `all` - all optional packages\n\n#
-Configuration\n\nDelfino doesn\'t load any plugins by default. To enable this
-plugin, add the following config into `pyproject.toml`:\n\n```toml\n
-[tool.delfino.plugins.delfino-core]\n\n```\n\n## Plugin configuration\n\nThis
-plugin has several options. All the values are optional and defaults are shown
-below: \n\n```toml\n[tool.delfino.plugins.delfino-core]\n# Source files - may
-have different rules than tests (usually stricter)\nsources_directory =
-"src"\n\n# Test files\ntests_directory = "tests"\n\n# Where to store reports
-generated by various tools\nreports_directory = "reports"\n\n# Types of tests
-you have nested under the `tests_directory`. Will be executed in given
-order.\ntest_types = ["unit", "integration"]\n\n# One or more module to wrap
-`pytest` in, executing it as `python -m  pytest ...`\npytest_modules = []\n\n#
-Commands to run as a quality gate in given order.\nverify_commands = ["format",
-"lint", "typecheck", "test-all"]\n\n# Do not install pre-commit if this is set
-to true.\ndisable_pre_commit = false\n```\n\n## Commands
-configuration\n\nSeveral commands have their own configuration as well:
-\n\n```toml\n[tool.delfino.plugins.delfino-core.typecheck]\n# One or more
-directories where type hint will be required. By default they are
-optional.\nstrict_directories = [] \n```\n\n# Usage\n\nRun `delfino --
-help`.\n\n# Development\n\nTo develop against editable `delfino` sources:\n\n1.
-Make sure `delfino` sources are next to this plugin:\n ```shell\n cd ..\n git
-clone https://github.com/radeklat/delfino.git\n ```\n2. Install `delfino` as
-editable package:\n ```shell\n pip install -e ../delfino\n ```\n Note that
-poetry will reset this to the released package when you install/update
-anything.\n', 'author': 'Radek LÃ¡t', 'author_email': 'radek.lat@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-radeklat/delfino-core', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'entry_points': entry_points,
-'python_requires': '>=3.7.2,<4.0.0', } setup(**setup_kwargs)
+available: - For individual commands (matches the command names): - `typecheck`
+- `format` - `dependencies-update` - For groups of commands: - `test` - for
+testing and coverage commands - `lint` - for all the linting commands - For
+groups of groups: - `verify-all` - same as `[typecheck,format,test,lint]` -
+`all` - all optional packages # Configuration Delfino doesn't load any plugins
+by default. To enable this plugin, add the following config into
+`pyproject.toml`: ```toml [tool.delfino.plugins.delfino-core] ``` ## Plugin
+configuration This plugin has several options. All the values are optional and
+defaults are shown below: ```toml [tool.delfino.plugins.delfino-core] # Source
+files - may have different rules than tests (usually stricter)
+sources_directory = "src" # Test files tests_directory = "tests" # Where to
+store reports generated by various tools reports_directory = "reports" # Types
+of tests you have nested under the `tests_directory`. Will be executed in given
+order. test_types = ["unit", "integration"] # One or more module to wrap
+`pytest` in, executing it as `python -m  pytest ...` pytest_modules = [] #
+Commands to run as a quality gate in given order. verify_commands = ["format",
+"lint", "typecheck", "test-all"] # Do not install pre-commit if this is set to
+true. disable_pre_commit = false ``` ## Commands configuration Several commands
+have their own configuration as well: ```toml [tool.delfino.plugins.delfino-
+core.typecheck] # One or more directories where type hint will be required. By
+default they are optional. strict_directories = [] ``` # Usage Run `delfino --
+help`. # Development To develop against editable `delfino` sources: 1. Make
+sure `delfino` sources are next to this plugin: ```shell cd .. git clone https:
+//github.com/radeklat/delfino.git ``` 2. Install `delfino` as editable package:
+```shell pip install -e ../delfino ``` Note that poetry will reset this to the
+released package when you install/update anything.
```

