# Comparing `tmp/svgtrace-2023.0.1.tar.gz` & `tmp/svgtrace-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgtrace-2023.0.1.tar", max compression
+gzip compressed data, was "svgtrace-2023.1.tar", max compression
```

## Comparing `svgtrace-2023.0.1.tar` & `svgtrace-2023.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-01-01 17:54:48.005567 svgtrace-2023.0.1/LICENSE.md
--rw-r--r--   0        0        0     1977 2023-03-12 17:33:40.226362 svgtrace-2023.0.1/pyproject.toml
--rw-r--r--   0        0        0     8012 2023-01-08 21:31:08.611722 svgtrace-2023.0.1/README.md
--rw-r--r--   0        0        0     1767 2023-03-12 17:32:59.343994 svgtrace-2023.0.1/svgtrace/__init__.py
--rw-r--r--   0        0        0      290 2023-01-01 17:54:48.005567 svgtrace-2023.0.1/svgtrace/imagetracer.html
--rw-r--r--   0        0        0    49433 2023-01-01 17:54:48.005567 svgtrace-2023.0.1/svgtrace/imagetracer.js
--rw-r--r--   0        0        0     9055 1970-01-01 00:00:00.000000 svgtrace-2023.0.1/setup.py
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 svgtrace-2023.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-01-01 17:54:48.005567 svgtrace-2023.1/LICENSE.md
+-rw-r--r--   0        0        0     2045 2023-06-25 21:43:06.883804 svgtrace-2023.1/pyproject.toml
+-rw-r--r--   0        0        0     7294 2023-06-25 21:20:38.123888 svgtrace-2023.1/README.md
+-rw-r--r--   0        0        0     3958 2023-06-25 21:38:04.050644 svgtrace-2023.1/svgtrace/__init__.py
+-rw-r--r--   0        0        0      290 2023-01-01 17:54:48.005567 svgtrace-2023.1/svgtrace/imagetracer.html
+-rw-r--r--   0        0        0    49433 2023-01-01 17:54:48.005567 svgtrace-2023.1/svgtrace/imagetracer.js
+-rw-r--r--   0        0        0     8374 1970-01-01 00:00:00.000000 svgtrace-2023.1/setup.py
+-rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 svgtrace-2023.1/PKG-INFO
```

### Comparing `svgtrace-2023.0.1/LICENSE.md` & `svgtrace-2023.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svgtrace-2023.0.1/pyproject.toml` & `svgtrace-2023.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svgtrace"
-version = "2023.0.1"
+version = "2023.1"
 license = "mit"
 description = "Leverage playwright and the imagetrace.js library to trace a bitmap to svg in python"
 authors = ["FredHappyface"]
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Developers",
 	"Intended Audience :: Education",
@@ -17,17 +17,20 @@
 ]
 homepage = "https://github.com/FHPythonUtils/SvgTrace"
 repository = "https://github.com/FHPythonUtils/SvgTrace"
 documentation = "https://github.com/FHPythonUtils/SvgTrace/blob/master/README.md"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-playwright = "<2,>=1.29.1"
+python = "^3.9"
+playwright = "<2,>=1.35.0"
 install-playwright = "<2,>=0.0.0"
+scikit-image = "<2,>=0.21.0"
+pillow = "<10,>=9.5.0"
+numpy = "<2,>=1.25.0"
 
 [tool.poetry.group.dev.dependencies]
 nocairosvg = "^2023"
 pytest = "^7.1.1"
 pylint = "^2.13.5"
 handsdown = "^1.1.0"
 coverage = "^6.3.2"
@@ -69,15 +72,14 @@
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 env_list =
 	py311
 	py310
 	py39
-	py38
 
 [testenv]
 deps =
 	nocairosvg
 	pytest
 	imgcompare
 commands = pytest tests
```

### Comparing `svgtrace-2023.0.1/README.md` & `svgtrace-2023.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # SvgTrace
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
 Leverage playwright and the imagetrace.js library to trace a bitmap to SVG in
 python
 
-- [Example](#example)
 - [Documentation](#documentation)
 - [Install With PIP](#install-with-pip)
 - [Language information](#language-information)
 	- [Built for](#built-for)
 - [Install Python on Windows](#install-python-on-windows)
 	- [Chocolatey](#chocolatey)
 	- [Windows - Python.org](#windows---pythonorg)
@@ -45,53 +44,21 @@
 	- [Changelog](#changelog)
 	- [Code of Conduct](#code-of-conduct)
 	- [Contributing](#contributing)
 	- [Security](#security)
 	- [Support](#support)
 	- [Rationale](#rationale)
 
-## Example
-
-Convert the following files:
-<div>
-<img src="tests/data/logo-bw.png" alt="Screenshot 1" width="300">
-<img src="tests/data/logo.png" alt="Screenshot 2" width="300">
-</div>
-
-```python
-"""Test the image tracer."""
-from pathlib import Path
-
-from svgtrace import trace
-
-THISDIR = str(Path(__file__).resolve().parent)
-logoFile = f"{THISDIR}/data/logo"
-
-Path(f"{logoFile}-bw.svg").write_text(trace(f"{logoFile}-bw.png", True), encoding="utf-8")
-
-Path(f"{logoFile}.svg").write_text(trace(f"{logoFile}.png"), encoding="utf-8")
-
-```
-
-Output
-
-<div>
-<img src="tests/data/logo-bw.svg" alt="Screenshot 1" width="300">
-<img src="tests/data/logo.svg" alt="Screenshot 2" width="300">
-</div>
-
 ## Documentation
 
 A high-level overview of how the documentation is organized organized will help you know
 where to look for certain things:
 
-<!--
 - [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
   started using the software. Start here if you’re new.
--->
 - The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
   machinery. This documentation describes how to use the classes and functions at a lower level
   and assume that you have a good high-level understanding of the software.
 <!--
 - The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
   may have.
 -->
```

### Comparing `svgtrace-2023.0.1/svgtrace/imagetracer.js` & `svgtrace-2023.1/svgtrace/imagetracer.js`

 * *Files identical despite different names*

### Comparing `svgtrace-2023.0.1/setup.py` & `svgtrace-2023.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 packages = \
 ['svgtrace']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['install-playwright>=0.0.0,<2', 'playwright>=1.29.1,<2']
+['install-playwright>=0.0.0,<2',
+ 'numpy>=1.25.0,<2',
+ 'pillow>=9.5.0,<10',
+ 'playwright>=1.35.0,<2',
+ 'scikit-image>=0.21.0,<2']
 
 setup_kwargs = {
     'name': 'svgtrace',
-    'version': '2023.0.1',
+    'version': '2023.1',
     'description': 'Leverage playwright and the imagetrace.js library to trace a bitmap to svg in python',
-    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/svgtrace.svg?style=for-the-badge)](https://pypistats.org/packages/svgtrace)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsvgtrace)](https://pepy.tech/project/svgtrace)\n[![PyPI Version](https://img.shields.io/pypi/v/svgtrace.svg?style=for-the-badge)](https://pypi.org/project/svgtrace)\n\n<!-- omit in toc -->\n# SvgTrace\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nLeverage playwright and the imagetrace.js library to trace a bitmap to SVG in\npython\n\n- [Example](#example)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Example\n\nConvert the following files:\n<div>\n<img src="tests/data/logo-bw.png" alt="Screenshot 1" width="300">\n<img src="tests/data/logo.png" alt="Screenshot 2" width="300">\n</div>\n\n```python\n"""Test the image tracer."""\nfrom pathlib import Path\n\nfrom svgtrace import trace\n\nTHISDIR = str(Path(__file__).resolve().parent)\nlogoFile = f"{THISDIR}/data/logo"\n\nPath(f"{logoFile}-bw.svg").write_text(trace(f"{logoFile}-bw.png", True), encoding="utf-8")\n\nPath(f"{logoFile}.svg").write_text(trace(f"{logoFile}.png"), encoding="utf-8")\n\n```\n\nOutput\n\n<div>\n<img src="tests/data/logo-bw.svg" alt="Screenshot 1" width="300">\n<img src="tests/data/logo.svg" alt="Screenshot 2" width="300">\n</div>\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install svgtrace\n```\n\nHead to https://pypi.org/project/svgtrace/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SvgTrace\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
+    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/svgtrace.svg?style=for-the-badge)](https://pypistats.org/packages/svgtrace)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsvgtrace)](https://pepy.tech/project/svgtrace)\n[![PyPI Version](https://img.shields.io/pypi/v/svgtrace.svg?style=for-the-badge)](https://pypi.org/project/svgtrace)\n\n<!-- omit in toc -->\n# SvgTrace\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nLeverage playwright and the imagetrace.js library to trace a bitmap to SVG in\npython\n\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install svgtrace\n```\n\nHead to https://pypi.org/project/svgtrace/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SvgTrace\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/SvgTrace',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `svgtrace-2023.0.1/PKG-INFO` & `svgtrace-2023.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: svgtrace
-Version: 2023.0.1
+Version: 2023.1
 Summary: Leverage playwright and the imagetrace.js library to trace a bitmap to svg in python
 Home-page: https://github.com/FHPythonUtils/SvgTrace
 License: MIT
 Author: FredHappyface
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: install-playwright (>=0.0.0,<2)
-Requires-Dist: playwright (>=1.29.1,<2)
+Requires-Dist: numpy (>=1.25.0,<2)
+Requires-Dist: pillow (>=9.5.0,<10)
+Requires-Dist: playwright (>=1.35.0,<2)
+Requires-Dist: scikit-image (>=0.21.0,<2)
 Project-URL: Documentation, https://github.com/FHPythonUtils/SvgTrace/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/SvgTrace
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)
 [![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../)
 [![Issues](https://img.shields.io/github/issues/FHPythonUtils/SvgTrace.svg?style=for-the-badge)](../../issues)
@@ -41,15 +43,14 @@
 # SvgTrace
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
 Leverage playwright and the imagetrace.js library to trace a bitmap to SVG in
 python
 
-- [Example](#example)
 - [Documentation](#documentation)
 - [Install With PIP](#install-with-pip)
 - [Language information](#language-information)
 	- [Built for](#built-for)
 - [Install Python on Windows](#install-python-on-windows)
 	- [Chocolatey](#chocolatey)
 	- [Windows - Python.org](#windows---pythonorg)
@@ -74,53 +75,21 @@
 	- [Changelog](#changelog)
 	- [Code of Conduct](#code-of-conduct)
 	- [Contributing](#contributing)
 	- [Security](#security)
 	- [Support](#support)
 	- [Rationale](#rationale)
 
-## Example
-
-Convert the following files:
-<div>
-<img src="tests/data/logo-bw.png" alt="Screenshot 1" width="300">
-<img src="tests/data/logo.png" alt="Screenshot 2" width="300">
-</div>
-
-```python
-"""Test the image tracer."""
-from pathlib import Path
-
-from svgtrace import trace
-
-THISDIR = str(Path(__file__).resolve().parent)
-logoFile = f"{THISDIR}/data/logo"
-
-Path(f"{logoFile}-bw.svg").write_text(trace(f"{logoFile}-bw.png", True), encoding="utf-8")
-
-Path(f"{logoFile}.svg").write_text(trace(f"{logoFile}.png"), encoding="utf-8")
-
-```
-
-Output
-
-<div>
-<img src="tests/data/logo-bw.svg" alt="Screenshot 1" width="300">
-<img src="tests/data/logo.svg" alt="Screenshot 2" width="300">
-</div>
-
 ## Documentation
 
 A high-level overview of how the documentation is organized organized will help you know
 where to look for certain things:
 
-<!--
 - [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
   started using the software. Start here if you’re new.
--->
 - The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
   machinery. This documentation describes how to use the classes and functions at a lower level
   and assume that you have a good high-level understanding of the software.
 <!--
 - The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
   may have.
 -->
```

