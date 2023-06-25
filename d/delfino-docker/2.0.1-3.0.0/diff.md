# Comparing `tmp/delfino_docker-2.0.1.tar.gz` & `tmp/delfino_docker-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino_docker-2.0.1.tar", max compression
+gzip compressed data, was "delfino_docker-3.0.0.tar", max compression
```

## Comparing `delfino_docker-2.0.1.tar` & `delfino_docker-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-12-30 12:07:03.497378 delfino_docker-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     3154 2022-12-30 12:07:03.497378 delfino_docker-2.0.1/README.md
--rw-r--r--   0        0        0     3025 2022-12-30 12:07:03.497378 delfino_docker-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5461 2022-12-30 12:07:03.497378 delfino_docker-2.0.1/src/delfino_docker/__init__.py
--rw-r--r--   0        0        0      509 2022-12-30 12:07:03.497378 delfino_docker-2.0.1/src/delfino_docker/config.py
--rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 delfino_docker-2.0.1/setup.py
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 delfino_docker-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-25 13:52:53.229104 delfino_docker-3.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3154 2023-06-25 13:52:53.229104 delfino_docker-3.0.0/README.md
+-rw-r--r--   0        0        0     2948 2023-06-25 13:52:53.233104 delfino_docker-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5461 2023-06-25 13:52:53.233104 delfino_docker-3.0.0/src/delfino_docker/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-25 13:52:53.233104 delfino_docker-3.0.0/src/delfino_docker/config.py
+-rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 delfino_docker-3.0.0/PKG-INFO
```

### Comparing `delfino_docker-2.0.1/LICENSE.md` & `delfino_docker-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `delfino_docker-2.0.1/README.md` & `delfino_docker-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `delfino_docker-2.0.1/pyproject.toml` & `delfino_docker-3.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="delfino-docker"
-version="2.0.1"
+version="3.0.0"
 authors = ["Radek Lat <radek.lat@gmail.com>"]
 description="A delfino plugin with helper scripts for working with docker."
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino-docker"
 
 # https://pypi.org/classifiers/
@@ -12,49 +12,49 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.2,<=3.11"
-delfino = "^1.1.0"
-packaging = "^22.0"
+python = "^3.8"
+delfino = "^2.0"
+packaging = "^23.0"
 
 [tool.poetry.plugins]
 
 [tool.poetry.plugins."delfino.plugin"]
 "delfino-docker" = "delfino_docker"
 
 [tool.poetry.group.dev.dependencies]
 types-toml = "*"
-delfino-core = {extras = ["verify-all"], version = "^3.10.0"}
+delfino-core = {extras = ["verify-all"], version = "^5.1"}
+gitpython = "^3.1"
 
 [tool.isort]
 # Setting compatible with black. See https://black.readthedocs.io/en/stable/compatible_configs.html
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 120
 
 [tool.black]
 line-length = 120
-target-version = ['py37']
+target-version = ['py38']
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -107,8 +107,7 @@
     "D202",  # "No blank lines allowed after function docstring" is false positive caused by black formatter.
     "D204",  # "1 blank line required after class docstring"
     "D401",  # "First line should be in imperative mood"
     "D413",  # "Missing blank line after last section"
 ]
 
 [tool.delfino.plugins.delfino-core]
-disable_commands = ["build-docker"]
```

### Comparing `delfino_docker-2.0.1/src/delfino_docker/__init__.py` & `delfino_docker-3.0.0/src/delfino_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `delfino_docker-2.0.1/setup.py` & `delfino_docker-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: delfino-docker
+Version: 3.0.0
+Summary: A delfino plugin with helper scripts for working with docker.
+Home-page: https://github.com/radeklat/delfino-docker
+License: MIT
+Author: Radek Lat
+Author-email: radek.lat@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
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
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: delfino (>=2.0,<3.0)
+Requires-Dist: packaging (>=23.0,<24.0)
+Description-Content-Type: text/markdown
+
+<h1 align="center" style="border-bottom: none;"> 🔌&nbsp;&nbsp;Delfino Docker&nbsp;&nbsp; 🔌</h1>
+<h3 align="center">A delfino plugin with helper scripts for working with docker.</h3>
+
+<p align="center">
+    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino-docker?branch=main">
+        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino-docker">
+    </a>
+    <a href="https://app.codecov.io/gh/radeklat/delfino-docker/">
+        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino-docker">
+    </a>
+    <a href="https://github.com/radeklat/delfino-docker/tags">
+        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino-docker">
+    </a>
+    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2022">
+    <a href="https://github.com/radeklat/delfino-docker/commits/main">
+        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino-docker">
+    </a>
+    <a href="https://www.python.org/doc/versions/">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino-docker">
+    </a>
+    <a href="https://pypistats.org/packages/delfino-docker">
+        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino-docker">
+    </a>
+</p>
+
+# Commands
+  
+| Command      | Description                                                                              |
+|--------------|------------------------------------------------------------------------------------------|
+| docker-build | Runs a `docker build` command for multiple platforms and pushes to dockerhub at the end. |
+
+# Installation
+
+- pip: `pip install delfino-docker`
+- Poetry: `poetry add -D delfino-docker`
+- Pipenv: `pipenv install -d delfino-docker`
+
+<!-- PUT DEPENDENCIES OF INDIVIDUAL COMMANDS AS EXTRAS -->
+<!--
+## Optional dependencies
+
+Each project may use different sub-set of [commands](#commands). Therefore, dependencies of all commands are optional and checked only when the command is executed.
+
+Using `[all]` installs all the [optional dependencies](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) used by all the commands. If you want only a sub-set of those dependencies, there are finer-grained groups available:
+
+- `demo`
+-->
+
+# Configuration
+
+Delfino doesn't load any plugins by default. To enable this plugin, add the following config into `pyproject.toml`:
+
+```toml
+[tool.delfino.plugins.delfino-docker]
+
+```
+
+<!-- PLUGIN MAY NEED CONFIGURATION -->
+<!--
+## Plugin configuration
+
+This plugin has several options. All the values are optional and defaults are shown below: 
+
+```toml
+[tool.delfino.plugins.delfino-docker]
+# Config option description
+config_option_name = "default value"
+```
+-->
+
+## Commands configuration
+
+```toml
+[tool.delfino.plugins.delfino-docker.docker-build]
+# User name for logging in into dockerhub
+dockerhub_username = ""
+
+# Platforms to build with dockerx
+build_for_platforms = [
+    "linux/arm/v7",
+    "linux/arm64",
+    "linux/amd64",
+]
+```
 
-package_dir = \
-{'': 'src'}
+# Usage
 
-packages = \
-['delfino_docker']
+Run `delfino --help`.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['delfino>=1.1.0,<2.0.0', 'packaging>=22.0,<23.0']
-
-entry_points = \
-{'delfino.plugin': ['delfino-docker = delfino_docker']}
-
-setup_kwargs = {
-    'name': 'delfino-docker',
-    'version': '2.0.1',
-    'description': 'A delfino plugin with helper scripts for working with docker.',
-    'long_description': '<h1 align="center" style="border-bottom: none;"> 🔌&nbsp;&nbsp;Delfino Docker&nbsp;&nbsp; 🔌</h1>\n<h3 align="center">A delfino plugin with helper scripts for working with docker.</h3>\n\n<p align="center">\n    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino-docker?branch=main">\n        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino-docker">\n    </a>\n    <a href="https://app.codecov.io/gh/radeklat/delfino-docker/">\n        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino-docker">\n    </a>\n    <a href="https://github.com/radeklat/delfino-docker/tags">\n        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino-docker">\n    </a>\n    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2022">\n    <a href="https://github.com/radeklat/delfino-docker/commits/main">\n        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino-docker">\n    </a>\n    <a href="https://www.python.org/doc/versions/">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino-docker">\n    </a>\n    <a href="https://pypistats.org/packages/delfino-docker">\n        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino-docker">\n    </a>\n</p>\n\n# Commands\n  \n| Command      | Description                                                                              |\n|--------------|------------------------------------------------------------------------------------------|\n| docker-build | Runs a `docker build` command for multiple platforms and pushes to dockerhub at the end. |\n\n# Installation\n\n- pip: `pip install delfino-docker`\n- Poetry: `poetry add -D delfino-docker`\n- Pipenv: `pipenv install -d delfino-docker`\n\n<!-- PUT DEPENDENCIES OF INDIVIDUAL COMMANDS AS EXTRAS -->\n<!--\n## Optional dependencies\n\nEach project may use different sub-set of [commands](#commands). Therefore, dependencies of all commands are optional and checked only when the command is executed.\n\nUsing `[all]` installs all the [optional dependencies](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) used by all the commands. If you want only a sub-set of those dependencies, there are finer-grained groups available:\n\n- `demo`\n-->\n\n# Configuration\n\nDelfino doesn\'t load any plugins by default. To enable this plugin, add the following config into `pyproject.toml`:\n\n```toml\n[tool.delfino.plugins.delfino-docker]\n\n```\n\n<!-- PLUGIN MAY NEED CONFIGURATION -->\n<!--\n## Plugin configuration\n\nThis plugin has several options. All the values are optional and defaults are shown below: \n\n```toml\n[tool.delfino.plugins.delfino-docker]\n# Config option description\nconfig_option_name = "default value"\n```\n-->\n\n## Commands configuration\n\n```toml\n[tool.delfino.plugins.delfino-docker.docker-build]\n# User name for logging in into dockerhub\ndockerhub_username = ""\n\n# Platforms to build with dockerx\nbuild_for_platforms = [\n    "linux/arm/v7",\n    "linux/arm64",\n    "linux/amd64",\n]\n```\n\n# Usage\n\nRun `delfino --help`.\n',
-    'author': 'Radek Lat',
-    'author_email': 'radek.lat@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/radeklat/delfino-docker',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<=3.11',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['delfino_docker'] package_data = \ {'': ['*']}
-install_requires = \ ['delfino>=1.1.0,<2.0.0', 'packaging>=22.0,<23.0']
-entry_points = \ {'delfino.plugin': ['delfino-docker = delfino_docker']}
-setup_kwargs = { 'name': 'delfino-docker', 'version': '2.0.1', 'description':
-'A delfino plugin with helper scripts for working with docker.',
-'long_description': '
+Metadata-Version: 2.1 Name: delfino-docker Version: 3.0.0 Summary: A delfino
+plugin with helper scripts for working with docker. Home-page: https://
+github.com/radeklat/delfino-docker License: MIT Author: Radek Lat Author-email:
+radek.lat@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
+:: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development Classifier: Topic :: Utilities Requires-Dist: delfino
+(>=2.0,<3.0) Requires-Dist: packaging (>=23.0,<24.0) Description-Content-Type:
+text/markdown
                    ****** ð  Delfino Docker   ð ******
-\n
     **** A delfino plugin with helper scripts for working with docker. ****
-\n\n
-  \n \n_[CircleCI]\n\n \n_[Codecov]\n\n \n_[GitHub_tag_(latest_SemVer)]\n\n
-[Maintenance]\n \n_[GitHub_last_commit]\n\n \n_[PyPI_-_Python_Version]\n\n \n_
-                                [Downloads]\n\n
-\n\n# Commands\n \n| Command | Description |\n|--------------|-----------------
--------------------------------------------------------------------------|\n|
-docker-build | Runs a `docker build` command for multiple platforms and pushes
-to dockerhub at the end. |\n\n# Installation\n\n- pip: `pip install delfino-
-docker`\n- Poetry: `poetry add -D delfino-docker`\n- Pipenv: `pipenv install -
-d delfino-docker`\n\n\n\n\n# Configuration\n\nDelfino doesn\'t load any plugins
-by default. To enable this plugin, add the following config into
-`pyproject.toml`:\n\n```toml\n[tool.delfino.plugins.delfino-
-docker]\n\n```\n\n\n\n\n## Commands configuration\n\n```toml\n
-[tool.delfino.plugins.delfino-docker.docker-build]\n# User name for logging in
-into dockerhub\ndockerhub_username = ""\n\n# Platforms to build with
-dockerx\nbuild_for_platforms = [\n "linux/arm/v7",\n "linux/arm64",\n "linux/
-amd64",\n]\n```\n\n# Usage\n\nRun `delfino --help`.\n', 'author': 'Radek Lat',
-'author_email': 'radek.lat@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/radeklat/delfino-
-docker', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.7.2,<=3.11', } setup(**setup_kwargs)
+ [CircleCI] [Codecov] [GitHub_tag_(latest_SemVer)] [Maintenance] [GitHub_last
+                  commit] [PyPI_-_Python_Version] [Downloads]
+# Commands | Command | Description | |--------------|--------------------------
+----------------------------------------------------------------| | docker-
+build | Runs a `docker build` command for multiple platforms and pushes to
+dockerhub at the end. | # Installation - pip: `pip install delfino-docker` -
+Poetry: `poetry add -D delfino-docker` - Pipenv: `pipenv install -d delfino-
+docker`   # Configuration Delfino doesn't load any plugins by default. To
+enable this plugin, add the following config into `pyproject.toml`: ```toml
+[tool.delfino.plugins.delfino-docker] ```   ## Commands configuration ```toml
+[tool.delfino.plugins.delfino-docker.docker-build] # User name for logging in
+into dockerhub dockerhub_username = "" # Platforms to build with dockerx
+build_for_platforms = [ "linux/arm/v7", "linux/arm64", "linux/amd64", ] ``` #
+Usage Run `delfino --help`.
```

