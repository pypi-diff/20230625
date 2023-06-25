# Comparing `tmp/camel_converter-3.0.0.tar.gz` & `tmp/camel_converter-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_converter-3.0.0.tar", max compression
+gzip compressed data, was "camel_converter-3.0.1.tar", max compression
```

## Comparing `camel_converter-3.0.0.tar` & `camel_converter-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-11-27 01:07:21.884482 camel_converter-3.0.0/LICENSE
--rw-r--r--   0        0        0     4291 2022-11-27 01:07:21.884482 camel_converter-3.0.0/README.md
--rw-r--r--   0        0        0     4216 2022-11-27 01:07:21.884482 camel_converter-3.0.0/camel_converter/__init__.py
--rw-r--r--   0        0        0     1128 2022-11-27 01:07:21.884482 camel_converter-3.0.0/camel_converter/decorators.py
--rw-r--r--   0        0        0        0 2022-11-27 01:07:21.884482 camel_converter-3.0.0/camel_converter/py.typed
--rw-r--r--   0        0        0      648 2022-11-27 01:07:21.884482 camel_converter-3.0.0/camel_converter/pydantic_base.py
--rw-r--r--   0        0        0     1910 2022-11-27 01:07:21.884482 camel_converter-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 camel_converter-3.0.0/setup.py
--rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 camel_converter-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 12:57:35.391050 camel_converter-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4291 2023-06-25 12:57:35.391050 camel_converter-3.0.1/README.md
+-rw-r--r--   0        0        0     4216 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/__init__.py
+-rw-r--r--   0        0        0     1128 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/py.typed
+-rw-r--r--   0        0        0      648 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/pydantic_base.py
+-rw-r--r--   0        0        0     1860 2023-06-25 12:57:35.391050 camel_converter-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 camel_converter-3.0.1/PKG-INFO
```

### Comparing `camel_converter-3.0.0/LICENSE` & `camel_converter-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.0/README.md` & `camel_converter-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.0/camel_converter/__init__.py` & `camel_converter-3.0.1/camel_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.0/camel_converter/decorators.py` & `camel_converter-3.0.1/camel_converter/decorators.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.0/camel_converter/pydantic_base.py` & `camel_converter-3.0.1/camel_converter/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.0/setup.py` & `camel_converter-3.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,179 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: camel-converter
+Version: 3.0.1
+Summary: Converts a string from snake case to camel case or camel case to snake case
+Home-page: https://github.com/sanders41/camel-converter
+License: MIT
+Keywords: python,pydantic
+Author: Paul Sanders
+Author-email: psanders1@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Provides-Extra: pydantic
+Requires-Dist: pydantic (>=1.8.2) ; extra == "pydantic"
+Project-URL: Documentation, https://github.com/sanders41/camel-converter
+Project-URL: Repository, https://github.com/sanders41/camel-converter
+Description-Content-Type: text/markdown
 
-packages = \
-['camel_converter']
+# Camel Converter
 
-package_data = \
-{'': ['*']}
+[![CI Status](https://github.com/sanders41/camel-converter/workflows/CI/badge.svg?branch=main&event=push)](https://github.com/sanders41/camel-converter/actions?query=workflow%3CI+branch%3Amain+event%3Apush)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/camel-converter/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/camel-converter/main)
+[![Coverage](https://codecov.io/github/sanders41/camel-converter/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/camel-converter)
+[![PyPI version](https://badge.fury.io/py/camel-converter.svg)](https://badge.fury.io/py/camel-converter)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/camel-converter?color=5cc141)](https://github.com/sanders41/camel-converter)
 
-extras_require = \
-{'pydantic': ['pydantic>=1.8.2']}
-
-setup_kwargs = {
-    'name': 'camel-converter',
-    'version': '3.0.0',
-    'description': 'Converts a string from snake case to camel case or camel case to snake case',
-    'long_description': '# Camel Converter\n\n[![CI Status](https://github.com/sanders41/camel-converter/workflows/CI/badge.svg?branch=main&event=push)](https://github.com/sanders41/camel-converter/actions?query=workflow%3CI+branch%3Amain+event%3Apush)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/camel-converter/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/camel-converter/main)\n[![Coverage](https://codecov.io/github/sanders41/camel-converter/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/camel-converter)\n[![PyPI version](https://badge.fury.io/py/camel-converter.svg)](https://badge.fury.io/py/camel-converter)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/camel-converter?color=5cc141)](https://github.com/sanders41/camel-converter)\n\nIn JSON keys are frequently in camelCase format, while variable names in Python are typically\nsnake_case. The purpose of this pacakgae is to help convert between the two formats.\n\n## Usage\n\n- To convert from camel case to snake case:\n\n  ```py\n  from camel_converter import to_snake\n\n  snake = to_snake("myString")\n  ```\n\n  This will convert `myString` into `my_string`\n\n- To convert a dictonary\'s keys from camel case to snake case:\n\n  ```py\n  from camel_converter import dict_to_snake\n\n  snake = dict_to_snake({"myString": "val 1"})\n  ```\n\n  This will convert `{"myString": "val 1"}` into `{"my_string": "val 1"}`. Non-string keys will be\n  left unchanged.\n\n  This is also available as a decorator for functions that return a dictionary.\n\n  ```py\n  from camel_converter.decorators import dict_to_snake\n\n  @dict_to_snake\n  def my_func() -> dict[str, str]:\n      return {"myString": "val 1"}\n\n  snake = my_func()\n  ```\n\n  `my_func` will return `{"my_string": "val 1"}`. Non-string keys will be\n  left unchanged.\n\n- To convert from snake case to camel case:\n\n  ```py\n  from camel_converter import to_camel\n\n  camel = to_camel("my_string")\n  ```\n\n  This will convert `my_string` into `myString`\n\n- To convert from a dictionary\'s keys from snake case to camel case:\n\n  ```py\n  from camel_converter import dict_to_camel\n\n  camel = to_camel({"my_string": "val 1"})\n  ```\n\n  This will convert `{"my_string": "val 1"}` into `{"myString": "val 1"}` Non-string keys will be\n  left unchanged.\n\n  This is also available as a decorator for functions that return a dictionary.\n\n  ```py\n  from camel_converter.decorators import dict_to_camel\n\n  @dict_to_camel\n  def my_func() -> dict[str, str]:\n      return {"my_string": "val 1"}\n\n  camel = my_func()\n  ```\n\n  `my_func` will return `{"myString": "val 1"}`. Non-string keys will be\n  left unchanged.\n\n- To convert from snake to pascal case:\n\n  ```py\n  from camel_converter import to_pascal\n\n  pascal = to_pascal("my_string")\n  ```\n\n  This will convert `my_string` into `MyString`\n\n- To convert from a dictionary\'s keys from snake case to pascal case:\n\n  ```py\n  from camel_converter import dict_to_pascal\n\n  pascal = to_pascal({"my_string": "val 1"})\n  ```\n\n  This will convert `{"my_string": "val 1"}` into `{"MyString": "val 1"}` Non-string keys will be\n  left unchanged.\n\n  This is also available as a decorator for functions that return a dictionary.\n\n  ```py\n  from camel_converter.decorators import dict_to_pascal\n\n  @dict_to_pascal\n  def my_func() -> dict[str, str]:\n      return {"my_string": "val 1"}\n\n  pascal = my_func()\n  ```\n\n  `my_func` will return `{"MyString": "val 1"}`. Non-string keys will be\n  left unchanged.\n\n### Optional Extras\n\nAn optional extra is provided for [Pydantic](https://pydantic-docs.helpmanual.io/) that provides a\nbase class to automatically convert between snake case and camel case. To use this Pydantic class\ninstall camel converter with:\n\n```sh\npip install camel-converter[pydantic]\n```\n\nThen your Pydantic classes can inherit from CamelBase.\n\n```py\nfrom camel_converter.pydantic_base import CamelBase\n\n\nclass MyModel(CamelBase):\n    test_field: str\n\n\nmy_data = MyModel(**{"testField": "my value"})\nprint(my_data.test_field)\n```\n\nwill result in `my value` being printed.\n\nWith setting up your model in this way `myField` from the source, i.e. JSON data, will map to `my_field` in your model.\n\n## Contributing\n\nIf you are interesting in contributing to this project please see our [contributing guide](CONTRIBUTING.md)\n',
-    'author': 'Paul Sanders',
-    'author_email': 'psanders1@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sanders41/camel-converter',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+In JSON keys are frequently in camelCase format, while variable names in Python are typically
+snake_case. The purpose of this pacakgae is to help convert between the two formats.
 
+## Usage
+
+- To convert from camel case to snake case:
+
+  ```py
+  from camel_converter import to_snake
+
+  snake = to_snake("myString")
+  ```
+
+  This will convert `myString` into `my_string`
+
+- To convert a dictonary's keys from camel case to snake case:
+
+  ```py
+  from camel_converter import dict_to_snake
+
+  snake = dict_to_snake({"myString": "val 1"})
+  ```
+
+  This will convert `{"myString": "val 1"}` into `{"my_string": "val 1"}`. Non-string keys will be
+  left unchanged.
+
+  This is also available as a decorator for functions that return a dictionary.
+
+  ```py
+  from camel_converter.decorators import dict_to_snake
+
+  @dict_to_snake
+  def my_func() -> dict[str, str]:
+      return {"myString": "val 1"}
+
+  snake = my_func()
+  ```
+
+  `my_func` will return `{"my_string": "val 1"}`. Non-string keys will be
+  left unchanged.
+
+- To convert from snake case to camel case:
+
+  ```py
+  from camel_converter import to_camel
+
+  camel = to_camel("my_string")
+  ```
+
+  This will convert `my_string` into `myString`
+
+- To convert from a dictionary's keys from snake case to camel case:
+
+  ```py
+  from camel_converter import dict_to_camel
+
+  camel = to_camel({"my_string": "val 1"})
+  ```
+
+  This will convert `{"my_string": "val 1"}` into `{"myString": "val 1"}` Non-string keys will be
+  left unchanged.
+
+  This is also available as a decorator for functions that return a dictionary.
+
+  ```py
+  from camel_converter.decorators import dict_to_camel
+
+  @dict_to_camel
+  def my_func() -> dict[str, str]:
+      return {"my_string": "val 1"}
+
+  camel = my_func()
+  ```
+
+  `my_func` will return `{"myString": "val 1"}`. Non-string keys will be
+  left unchanged.
+
+- To convert from snake to pascal case:
+
+  ```py
+  from camel_converter import to_pascal
+
+  pascal = to_pascal("my_string")
+  ```
+
+  This will convert `my_string` into `MyString`
+
+- To convert from a dictionary's keys from snake case to pascal case:
+
+  ```py
+  from camel_converter import dict_to_pascal
+
+  pascal = to_pascal({"my_string": "val 1"})
+  ```
+
+  This will convert `{"my_string": "val 1"}` into `{"MyString": "val 1"}` Non-string keys will be
+  left unchanged.
+
+  This is also available as a decorator for functions that return a dictionary.
+
+  ```py
+  from camel_converter.decorators import dict_to_pascal
+
+  @dict_to_pascal
+  def my_func() -> dict[str, str]:
+      return {"my_string": "val 1"}
+
+  pascal = my_func()
+  ```
+
+  `my_func` will return `{"MyString": "val 1"}`. Non-string keys will be
+  left unchanged.
+
+### Optional Extras
+
+An optional extra is provided for [Pydantic](https://pydantic-docs.helpmanual.io/) that provides a
+base class to automatically convert between snake case and camel case. To use this Pydantic class
+install camel converter with:
+
+```sh
+pip install camel-converter[pydantic]
+```
+
+Then your Pydantic classes can inherit from CamelBase.
+
+```py
+from camel_converter.pydantic_base import CamelBase
+
+
+class MyModel(CamelBase):
+    test_field: str
+
+
+my_data = MyModel(**{"testField": "my value"})
+print(my_data.test_field)
+```
+
+will result in `my value` being printed.
+
+With setting up your model in this way `myField` from the source, i.e. JSON data, will map to `my_field` in your model.
+
+## Contributing
+
+If you are interesting in contributing to this project please see our [contributing guide](CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

