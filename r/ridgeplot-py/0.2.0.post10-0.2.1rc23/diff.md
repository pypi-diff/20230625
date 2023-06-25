# Comparing `tmp/ridgeplot_py-0.2.0.post10.tar.gz` & `tmp/ridgeplot_py-0.2.1rc23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot_py-0.2.0.post10.tar", max compression
+gzip compressed data, was "ridgeplot_py-0.2.1rc23.tar", max compression
```

## Comparing `ridgeplot_py-0.2.0.post10.tar` & `ridgeplot_py-0.2.1rc23.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-10-25 14:03:44.842741 ridgeplot_py-0.2.0.post10/LICENSE
--rw-r--r--   0        0        0     2715 2022-10-30 22:21:13.486503 ridgeplot_py-0.2.0.post10/README.md
--rw-r--r--   0        0        0      938 2023-06-25 14:38:47.832981 ridgeplot_py-0.2.0.post10/pyproject.toml
--rw-r--r--   0        0        0       59 2022-10-25 14:03:44.843530 ridgeplot_py-0.2.0.post10/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8035 2022-10-27 22:31:49.168011 ridgeplot_py-0.2.0.post10/ridgeplot/colors.py
--rw-r--r--   0        0        0     3252 2022-11-16 05:25:43.303736 ridgeplot_py-0.2.0.post10/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      626 2022-10-27 21:37:34.106785 ridgeplot_py-0.2.0.post10/ridgeplot/stats.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.0.post10/setup.py
--rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.0.post10/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/README.md
+-rw-r--r--   0        0        0      949 2023-06-25 21:30:52.890171 ridgeplot_py-0.2.1rc23/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8035 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/ridgeplot/colors.py
+-rw-r--r--   0        0        0     3252 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      662 2023-06-25 21:30:24.074551 ridgeplot_py-0.2.1rc23/ridgeplot/stats.py
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.1rc23/setup.py
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.1rc23/PKG-INFO
```

### Comparing `ridgeplot_py-0.2.0.post10/LICENSE` & `ridgeplot_py-0.2.1rc23/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.0.post10/README.md` & `ridgeplot_py-0.2.1rc23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,7 +60,18 @@
 
 ![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)
 
 
 ## Example ##
 
 A [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!
+
+
+## Build on Apple silicon ##
+
+scipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):
+
+```
+brew install openblas
+export OPENBLAS="$(brew --prefix openblas)" 
+poetry install
+```
```

#### html2text {}

```diff
@@ -27,8 +27,11 @@
 data # the input data should be a dict of # - keys: group names for the
 distributions # - values: list of values data = {} for i in range(8): data
 ['data_{}'.format(i)] = np.random.randn(100) * (i+1) # make the plot fig =
 plt.figure() ax = fig.add_subplot(111) ridgeplot( ax, data, xlim=(-20,20),
 label_size=15 ) ``` ![img](https://raw.githubusercontent.com/wckdouglas/
 ridgeplot-py/main/img/ridgeplot.png) ## Example ## A [notebook](https://
 github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto
-is included in this repo!
+is included in this repo! ## Build on Apple silicon ## scipy may cause error
+and may be able to solved by the [this stackoverflow answer](https://
+stackoverflow.com/a/71764028): ``` brew install openblas export OPENBLAS="$
+(brew --prefix openblas)" poetry install ```
```

### Comparing `ridgeplot_py-0.2.0.post10/pyproject.toml` & `ridgeplot_py-0.2.1rc23/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ridgeplot-py"
-version = "0.2.0-post.10" # managed by poetry-dynamic-versioning
+version = "0.2.1-pre.23" # managed by poetry-dynamic-versioning
 description = "Plotting ridgeplots with matplotlib"
 authors = ["Douglas Wu <wckdouglas@gmail.com>"]
 license = "MIT"
 packages = [
     {"include" = "ridgeplot"}
 ]
 readme = "README.md"
@@ -22,14 +22,15 @@
 mypy = "^0.910"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 metadata= false
+bump = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.extras]
 dev = ["pytest", "pytest-cov", "mypy"]
```

### Comparing `ridgeplot_py-0.2.0.post10/ridgeplot/colors.py` & `ridgeplot_py-0.2.1rc23/ridgeplot/colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.0.post10/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.2.1rc23/ridgeplot/ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.0.post10/setup.py` & `ridgeplot_py-0.2.1rc23/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['matplotlib>=3.1.3,<4.0.0',
  'more-itertools>=8.9.0,<9.0.0',
  'numpy>=1.21.1,<2.0.0',
  'scipy>=1.4.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'ridgeplot-py',
-    'version': '0.2.0.post10',
+    'version': '0.2.1rc23',
     'description': 'Plotting ridgeplots with matplotlib',
-    'long_description': '# ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:\n\n<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a dict of\n# - keys: group names for the distributions\n# - values: list of values \ndata = {}\nfor i in range(8):\n    data[\'data_{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n    ax, \n    data, \n    xlim=(-20,20), \n    label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!\n',
+    'long_description': '# ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:\n\n<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a dict of\n# - keys: group names for the distributions\n# - values: list of values \ndata = {}\nfor i in range(8):\n    data[\'data_{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n    ax, \n    data, \n    xlim=(-20,20), \n    label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!\n\n\n## Build on Apple silicon ##\n\nscipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):\n\n```\nbrew install openblas\nexport OPENBLAS="$(brew --prefix openblas)" \npoetry install\n```\n',
     'author': 'Douglas Wu',
     'author_email': 'wckdouglas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['ridgeplot']
 package_data = \ {'': ['*']} install_requires = \ ['matplotlib>=3.1.3,<4.0.0',
 'more-itertools>=8.9.0,<9.0.0', 'numpy>=1.21.1,<2.0.0', 'scipy>=1.4.1,<2.0.0']
-setup_kwargs = { 'name': 'ridgeplot-py', 'version': '0.2.0.post10',
-'description': 'Plotting ridgeplots with matplotlib', 'long_description': '#
-ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/
-workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/
-actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/
-ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/
-gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/
-ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge]
-(https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
+setup_kwargs = { 'name': 'ridgeplot-py', 'version': '0.2.1rc23', 'description':
+'Plotting ridgeplots with matplotlib', 'long_description': '# ridgeplot-py
+#\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/
+ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/
+workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/
+branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/
+wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-
+py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://
+anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
 anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for
 plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/
 ) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is
 a great data visualization technique to compare distributions from multiple
 groups at the same time, and was first introduced in 2017 as joy plot:\n\n
      I hereby propose that we call these "joy plots" #rstats https://t.co/
      uuLGpQLAwY
@@ -33,12 +33,15 @@
 dict of\n# - keys: group names for the distributions\n# - values: list of
 values \ndata = {}\nfor i in range(8):\n data[\'data_{}\'.format(i)] =
 np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax =
 fig.add_subplot(111)\nridgeplot(\n ax, \n data, \n xlim=(-20,20), \n
 label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/
 ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https:/
 /github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick
-howto is included in this repo!\n', 'author': 'Douglas Wu', 'author_email':
-'wckdouglas@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+howto is included in this repo!\n\n\n## Build on Apple silicon ##\n\nscipy may
+cause error and may be able to solved by the [this stackoverflow answer](https:
+//stackoverflow.com/a/71764028):\n\n```\nbrew install openblas\nexport
+OPENBLAS="$(brew --prefix openblas)" \npoetry install\n```\n', 'author':
+'Douglas Wu', 'author_email': 'wckdouglas@gmail.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `ridgeplot_py-0.2.0.post10/PKG-INFO` & `ridgeplot_py-0.2.1rc23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ridgeplot-py
-Version: 0.2.0.post10
+Version: 0.2.1rc23
 Summary: Plotting ridgeplots with matplotlib
 License: MIT
 Author: Douglas Wu
 Author-email: wckdouglas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -83,7 +83,18 @@
 ![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)
 
 
 ## Example ##
 
 A [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!
 
+
+## Build on Apple silicon ##
+
+scipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):
+
+```
+brew install openblas
+export OPENBLAS="$(brew --prefix openblas)" 
+poetry install
+```
+
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.0.post10 Summary:
-Plotting ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-
-email: wckdouglas@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.1rc23 Summary: Plotting
+ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-email:
+wckdouglas@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: dev Requires-Dist: matplotlib
 (>=3.1.3,<4.0.0) Requires-Dist: more-itertools (>=8.9.0,<9.0.0) Requires-Dist:
 numpy (>=1.21.1,<2.0.0) Requires-Dist: scipy (>=1.4.1,<2.0.0) Description-
 Content-Type: text/markdown # ridgeplot-py # [![CI](https://github.com/
@@ -38,8 +38,11 @@
 data # the input data should be a dict of # - keys: group names for the
 distributions # - values: list of values data = {} for i in range(8): data
 ['data_{}'.format(i)] = np.random.randn(100) * (i+1) # make the plot fig =
 plt.figure() ax = fig.add_subplot(111) ridgeplot( ax, data, xlim=(-20,20),
 label_size=15 ) ``` ![img](https://raw.githubusercontent.com/wckdouglas/
 ridgeplot-py/main/img/ridgeplot.png) ## Example ## A [notebook](https://
 github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto
-is included in this repo!
+is included in this repo! ## Build on Apple silicon ## scipy may cause error
+and may be able to solved by the [this stackoverflow answer](https://
+stackoverflow.com/a/71764028): ``` brew install openblas export OPENBLAS="$
+(brew --prefix openblas)" poetry install ```
```

