# Comparing `tmp/django_choices_field-2.2.1.tar.gz` & `tmp/django_choices_field-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_choices_field-2.2.1.tar", max compression
+gzip compressed data, was "django_choices_field-2.2.2.tar", max compression
```

## Comparing `django_choices_field-2.2.1.tar` & `django_choices_field-2.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/LICENSE
--rw-r--r--   0        0        0     2822 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/README.md
--rw-r--r--   0        0        0      188 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/__init__.py
--rw-r--r--   0        0        0     5913 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/fields.py
--rw-r--r--   0        0        0     7193 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/fields.pyi
--rw-r--r--   0        0        0      625 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/types.py
--rw-r--r--   0        0        0     3264 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 django_choices_field-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/LICENSE
+-rw-r--r--   0        0        0     2822 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/README.md
+-rw-r--r--   0        0        0      188 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/django_choices_field/__init__.py
+-rw-r--r--   0        0        0     5913 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/django_choices_field/fields.py
+-rw-r--r--   0        0        0     7193 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/django_choices_field/fields.pyi
+-rw-r--r--   0        0        0      625 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/django_choices_field/types.py
+-rw-r--r--   0        0        0     3308 2023-06-25 15:50:54.516402 django_choices_field-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 django_choices_field-2.2.2/PKG-INFO
```

### Comparing `django_choices_field-2.2.1/LICENSE` & `django_choices_field-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.1/README.md` & `django_choices_field-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.1/django_choices_field/fields.py` & `django_choices_field-2.2.2/django_choices_field/fields.py`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.1/django_choices_field/fields.pyi` & `django_choices_field-2.2.2/django_choices_field/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.1/django_choices_field/types.py` & `django_choices_field-2.2.2/django_choices_field/types.py`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.1/pyproject.toml` & `django_choices_field-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-choices-field"
-version = "2.2.1"
+version = "2.2.2"
 description = "Django field that set/get django's new TextChoices/IntegerChoices enum."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bellini666/django-choices-field"
 repository = "https://github.com/bellini666/django-choices-field"
 documentation = "https://django-choices-field.readthedocs.io"
@@ -13,28 +13,29 @@
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
 ]
 packages = [{ include = "django_choices_field" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.7"
 django = ">=3.2"
 typing_extensions = ">=4.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 codecov = "^2.1.11"
 django = "^4.0"
@@ -42,15 +43,15 @@
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.2.0"
 ruff = "^0.0.274"
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ['py37']
 preview = true
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
@@ -117,15 +118,15 @@
   "TCH003",
   "PGH003",
   "PLR09",
   "PLR2004",
   "SLF001",
   "TRY003",
 ]
-target-version = "py38"
+target-version = "py37"
 exclude = [
   ".eggs",
   ".git",
   ".hg",
   ".mypy_cache",
   ".tox",
   ".venv",
@@ -138,15 +139,15 @@
 
 [tool.ruff.isort]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.pyright]
-pythonVersion = "3.8"
+pythonVersion = "3.7"
 useLibraryCodeForTypes = true
 venvPath = "."
 venv = ".venv"
 ignore = ["**/migrations"]
 reportCallInDefaultInitializer = "warning"
 reportMatchNotExhaustive = "warning"
 reportMissingSuperCall = "warning"
```

### Comparing `django_choices_field-2.2.1/PKG-INFO` & `django_choices_field-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: django-choices-field
-Version: 2.2.1
+Version: 2.2.2
 Summary: Django field that set/get django's new TextChoices/IntegerChoices enum.
 Home-page: https://github.com/bellini666/django-choices-field
 License: MIT
 Keywords: django,enum
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Project-URL: Documentation, https://django-choices-field.readthedocs.io
```

