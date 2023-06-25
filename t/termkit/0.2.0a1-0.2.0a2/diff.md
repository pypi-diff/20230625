# Comparing `tmp/termkit-0.2.0a1.tar.gz` & `tmp/termkit-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termkit-0.2.0a1.tar", max compression
+gzip compressed data, was "termkit-0.2.0a2.tar", max compression
```

## Comparing `termkit-0.2.0a1.tar` & `termkit-0.2.0a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a1/README.md
--rw-r--r--   0        0        0      620 2023-06-21 20:44:44.495948 termkit-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a1/termkit/__init__.py
--rw-r--r--   0        0        0     6069 2023-06-21 20:43:42.512238 termkit-0.2.0a1/termkit/arguments.py
--rw-r--r--   0        0        0    10375 2023-06-21 20:03:14.257509 termkit-0.2.0a1/termkit/components.py
--rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a1/termkit/exceptions.py
--rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a1/termkit/formatters.py
--rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a1/termkit/groups.py
--rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a1/termkit/helpers.py
--rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a1/termkit/tests.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 termkit-0.2.0a1/setup.py
--rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 termkit-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a2/README.md
+-rw-r--r--   0        0        0      620 2023-06-25 21:18:51.732952 termkit-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a2/termkit/__init__.py
+-rw-r--r--   0        0        0     6069 2023-06-21 20:43:42.512238 termkit-0.2.0a2/termkit/arguments.py
+-rw-r--r--   0        0        0    10614 2023-06-25 09:23:37.771593 termkit-0.2.0a2/termkit/components.py
+-rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/exceptions.py
+-rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/formatters.py
+-rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/groups.py
+-rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a2/termkit/helpers.py
+-rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/tests.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 termkit-0.2.0a2/setup.py
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 termkit-0.2.0a2/PKG-INFO
```

### Comparing `termkit-0.2.0a1/LICENSE` & `termkit-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/README.md` & `termkit-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/pyproject.toml` & `termkit-0.2.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "termkit"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "Command Line Tools with ease"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `termkit-0.2.0a1/termkit/arguments.py` & `termkit-0.2.0a2/termkit/arguments.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/termkit/components.py` & `termkit-0.2.0a2/termkit/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,24 @@
     def callback(self):
         def _decorated_callable(callback: Callable):
             if inspect.isfunction(callback):
                 self._callback = callback
             else:
                 raise TermkitError(f"cannot set object of type '{type(callback).__name__}' as callback for Termkit application")
             return callback
+
         return _decorated_callable
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, argcomplete=False, *args, **kwargs):
         parser = TermkitParser(self)
+
+        if argcomplete:  # pragma: nocover
+            import argcomplete as _argcomplete
+            _argcomplete.autocomplete(parser)
+
         args = parser.parse_args()
 
         callbacks = [f for k, f in args.__dict__.items() if "__TERMKIT_CALLBACK_" in k]
 
         for callback in callbacks:
             callback(**get_callback_arguments(callback, args))
 
@@ -249,14 +255,15 @@
 
         if isinstance(group, ArgumentGroup):
             self._argument_groups[group] = super(self.__class__, self).add_argument_group(title=group.title, description=group.description)
 
         return self._argument_groups[group]
 
 
-def run(func_or_app: Union[Callable, Termkit]):
+def run(func_or_app: Union[Callable, Termkit],
+        argcomplete: bool = False):
     if inspect.isfunction(func_or_app):
-        Termkit(name=func_or_app.__name__, callback=func_or_app)()
+        Termkit(name=func_or_app.__name__, callback=func_or_app)(argcomplete=argcomplete)
     elif isinstance(func_or_app, Termkit):
-        func_or_app()
+        func_or_app(argcomplete=argcomplete)
     else:
         raise TermkitError(f"cannot run object of type '{type(func_or_app).__name__}'")
```

### Comparing `termkit-0.2.0a1/termkit/exceptions.py` & `termkit-0.2.0a2/termkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/termkit/formatters.py` & `termkit-0.2.0a2/termkit/formatters.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/termkit/groups.py` & `termkit-0.2.0a2/termkit/groups.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/termkit/helpers.py` & `termkit-0.2.0a2/termkit/helpers.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/termkit/tests.py` & `termkit-0.2.0a2/termkit/tests.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a1/setup.py` & `termkit-0.2.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['termkit']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'termkit',
-    'version': '0.2.0a1',
+    'version': '0.2.0a2',
     'description': 'Command Line Tools with ease',
     'long_description': '<p align="center">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner.png#gh-dark-mode-only" width="450">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner_light.png#gh-light-mode-only" width="450">\n</p>\n<div align="center">\n  <b><i>Command Line Tools with... ease.</i></b>\n<hr>\n\n[![Tests](https://github.com/thmahe/termkit/actions/workflows/tests.yml/badge.svg)](https://github.com/thmahe/termkit/actions/workflows/tests.yml)\n[![codecov](https://codecov.io/github/thmahe/termkit/branch/master/graph/badge.svg?token=o7UVrOsoq4)](https://codecov.io/github/thmahe/termkit)\n![PyPI](https://img.shields.io/pypi/v/termkit)\n![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20MacOS%20%7C%20Windows-lightgrey)\n\n</div>\n\n## Table of Contents\n\n- [Introduction](#introduction)\n- [Features](#features)\n- [Requirement](#requirement)\n- [Installation](#installation)\n- [Examples](#examples)\n- [Feedback](#feedback)\n- [Acknowledgments](#acknowledgments)\n\n## Introduction\n\nTermkit is a framework for building command line interface applications using functions \nand type hints [[PEP 484]](https://peps.python.org/pep-0484/). \n**Solely written using [Python Standard Library](https://docs.python.org/3/library/)** and will always be to ensure\nminimal dependency footprint within your project.\n\nIn few words, Termkit is designed to be the foundation of serious CLI tools.\n\n## Features\n\nA few of the things you can do with Termkit:\n\n* Build CLI from functional code\n* Create fast prototypes using implicit arguments\n* Helpers populated from docstrings\n* Named profile for pre-populated arguments\n* Autocompletion through [argcomplete](https://pypi.org/project/argcomplete/) module\n* Cross-platforms\n\n## Requirement\n* Python 3.7 or higher\n\n*Yes... that\'s about it !* \n\n### Compatibility matrix\n\n|          OS | Python 3.6 |     Python 3.7     |     Python 3.8     |     Python 3.9     |    Python 3.10     |    Python 3.11     |    Python 3.12    |\n|------------:|:----------:|:------------------:|:------------------:|:------------------:|:------------------:|:------------------:|:-----------------:|\n|   **Linux** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n|   **MacOS** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n| **Windows** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n\n\n## Installation\n\nTermkit is published as a [Python package](https://pypi.org/project/termkit) and can be installed with pip.\n\nOpen up a terminal and install Termkit with:\n```shell\npip install termkit\n```\n\n## Examples\n\n### Greeting application\n\n```python\n# greet.py\nimport termkit\n\ndef greet(name):\n    print(f\'Hello {name} !\')\n\nif __name__ == \'__main__\':\n    termkit.run(greet)\n```\n\n```\n$ python3 ./greet.py Thomas\nHello Thomas !\n```\n\n## Feedback\n\nFeel free to send me feedback by [raising an issue](https://github.com/thmahe/termkit/issues/new).\nFeature requests are always welcome.\n\n',
     'author': 'Thomas Mahé',
     'author_email': 'contact@tmahe.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `termkit-0.2.0a1/PKG-INFO` & `termkit-0.2.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termkit
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Command Line Tools with ease
 Author: Thomas Mahé
 Author-email: contact@tmahe.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

