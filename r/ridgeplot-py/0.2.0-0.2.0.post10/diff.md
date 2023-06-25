# Comparing `tmp/ridgeplot-py-0.2.0.tar.gz` & `tmp/ridgeplot_py-0.2.0.post10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot-py-0.2.0.tar", max compression
+gzip compressed data, was "ridgeplot_py-0.2.0.post10.tar", max compression
```

## Comparing `ridgeplot-py-0.2.0.tar` & `ridgeplot_py-0.2.0.post10.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-10-25 15:48:46.308957 ridgeplot-py-0.2.0/LICENSE
--rw-r--r--   0        0        0     2593 2022-10-27 21:40:18.109509 ridgeplot-py-0.2.0/README.md
--rw-r--r--   0        0        0      757 2022-10-27 21:58:03.009608 ridgeplot-py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       59 2022-10-25 15:48:46.308957 ridgeplot-py-0.2.0/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8035 2022-10-27 22:01:34.062214 ridgeplot-py-0.2.0/ridgeplot/colors.py
--rw-r--r--   0        0        0     3252 2022-10-27 21:40:18.113509 ridgeplot-py-0.2.0/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      626 2022-10-27 21:40:18.113509 ridgeplot-py-0.2.0/ridgeplot/stats.py
--rw-r--r--   0        0        0     3357 2022-10-27 22:06:16.955390 ridgeplot-py-0.2.0/setup.py
--rw-r--r--   0        0        0     3267 2022-10-27 22:06:16.956174 ridgeplot-py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-25 14:03:44.842741 ridgeplot_py-0.2.0.post10/LICENSE
+-rw-r--r--   0        0        0     2715 2022-10-30 22:21:13.486503 ridgeplot_py-0.2.0.post10/README.md
+-rw-r--r--   0        0        0      938 2023-06-25 14:38:47.832981 ridgeplot_py-0.2.0.post10/pyproject.toml
+-rw-r--r--   0        0        0       59 2022-10-25 14:03:44.843530 ridgeplot_py-0.2.0.post10/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8035 2022-10-27 22:31:49.168011 ridgeplot_py-0.2.0.post10/ridgeplot/colors.py
+-rw-r--r--   0        0        0     3252 2022-11-16 05:25:43.303736 ridgeplot_py-0.2.0.post10/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      626 2022-10-27 21:37:34.106785 ridgeplot_py-0.2.0.post10/ridgeplot/stats.py
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.0.post10/setup.py
+-rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.0.post10/PKG-INFO
```

### Comparing `ridgeplot-py-0.2.0/LICENSE` & `ridgeplot_py-0.2.0.post10/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot-py-0.2.0/README.md` & `ridgeplot_py-0.2.0.post10/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 
 ```bash
 git clone git@github.com:wckdouglas/ridgeplot-py.git
 cd ridgeplot-py
 python setup.py install 
 ```
 
+or via conda:
+
+```bash
+conda install -c conda-forge ridgeplot-py
+```
+
+or via pypi:
+
+```bash
+pip install ridgeplot-py
+```
+
 ## Usage ##
 
 ```python
 from ridgeplot import ridgeplot
 from ridgeplot.colors import ColorEncoder, ColorPalette
 import numpy as np
 import matplotlib.pyplot as plt
```

#### html2text {}

```diff
@@ -16,17 +16,19 @@
 [ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to
 produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder]
 (https://github.com/wckdouglas/ridgeplot-py/blob/
 0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with
 scikit-learn syntax for manipulating color annotations in a consistent way
 [through out manuscripts or presentations]. ## Install ## ```bash git clone
 git@github.com:wckdouglas/ridgeplot-py.git cd ridgeplot-py python setup.py
-install ``` ## Usage ## ```python from ridgeplot import ridgeplot from
-ridgeplot.colors import ColorEncoder, ColorPalette import numpy as np import
-matplotlib.pyplot as plt # mocking some data # the input data should be a dict
-of # - keys: group names for the distributions # - values: list of values data
-= {} for i in range(8): data['data_{}'.format(i)] = np.random.randn(100) *
-(i+1) # make the plot fig = plt.figure() ax = fig.add_subplot(111) ridgeplot
-( ax, data, xlim=(-20,20), label_size=15 ) ``` ![img](https://
-raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png) ##
-Example ## A [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/
-Example.ipynb) showing quick howto is included in this repo!
+install ``` or via conda: ```bash conda install -c conda-forge ridgeplot-py ```
+or via pypi: ```bash pip install ridgeplot-py ``` ## Usage ## ```python from
+ridgeplot import ridgeplot from ridgeplot.colors import ColorEncoder,
+ColorPalette import numpy as np import matplotlib.pyplot as plt # mocking some
+data # the input data should be a dict of # - keys: group names for the
+distributions # - values: list of values data = {} for i in range(8): data
+['data_{}'.format(i)] = np.random.randn(100) * (i+1) # make the plot fig =
+plt.figure() ax = fig.add_subplot(111) ridgeplot( ax, data, xlim=(-20,20),
+label_size=15 ) ``` ![img](https://raw.githubusercontent.com/wckdouglas/
+ridgeplot-py/main/img/ridgeplot.png) ## Example ## A [notebook](https://
+github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto
+is included in this repo!
```

### Comparing `ridgeplot-py-0.2.0/pyproject.toml` & `ridgeplot_py-0.2.0.post10/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ridgeplot-py"
-version = "0.2.0"
+version = "0.2.0-post.10" # managed by poetry-dynamic-versioning
 description = "Plotting ridgeplots with matplotlib"
 authors = ["Douglas Wu <wckdouglas@gmail.com>"]
 license = "MIT"
 packages = [
     {"include" = "ridgeplot"}
 ]
 readme = "README.md"
@@ -17,23 +17,30 @@
 numpy = "^1.21.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
 mypy = "^0.910"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+metadata= false
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.extras]
 dev = ["pytest", "pytest-cov", "mypy"]
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
 
 [[tool.mypy.overrides]]
 module = [
     "matplotlib.*",
     "scipy.*"
 ]
 ignore_missing_imports = true
+
```

### Comparing `ridgeplot-py-0.2.0/ridgeplot/colors.py` & `ridgeplot_py-0.2.0.post10/ridgeplot/colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot-py-0.2.0/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.2.0.post10/ridgeplot/ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot-py-0.2.0/ridgeplot/stats.py` & `ridgeplot_py-0.2.0.post10/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot-py-0.2.0/setup.py` & `ridgeplot_py-0.2.0.post10/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['matplotlib>=3.1.3,<4.0.0',
  'more-itertools>=8.9.0,<9.0.0',
  'numpy>=1.21.1,<2.0.0',
  'scipy>=1.4.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'ridgeplot-py',
-    'version': '0.2.0',
+    'version': '0.2.0.post10',
     'description': 'Plotting ridgeplots with matplotlib',
-    'long_description': '# ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:\n\n<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython setup.py install \n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a dict of\n# - keys: group names for the distributions\n# - values: list of values \ndata = {}\nfor i in range(8):\n    data[\'data_{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n    ax, \n    data, \n    xlim=(-20,20), \n    label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!\n',
+    'long_description': '# ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:\n\n<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a dict of\n# - keys: group names for the distributions\n# - values: list of values \ndata = {}\nfor i in range(8):\n    data[\'data_{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n    ax, \n    data, \n    xlim=(-20,20), \n    label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!\n',
     'author': 'Douglas Wu',
     'author_email': 'wckdouglas@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['ridgeplot']
 package_data = \ {'': ['*']} install_requires = \ ['matplotlib>=3.1.3,<4.0.0',
 'more-itertools>=8.9.0,<9.0.0', 'numpy>=1.21.1,<2.0.0', 'scipy>=1.4.1,<2.0.0']
-setup_kwargs = { 'name': 'ridgeplot-py', 'version': '0.2.0', 'description':
-'Plotting ridgeplots with matplotlib', 'long_description': '# ridgeplot-py
-#\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/
-ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/
-workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/
-branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/
-wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-
-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://
-anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
+setup_kwargs = { 'name': 'ridgeplot-py', 'version': '0.2.0.post10',
+'description': 'Plotting ridgeplots with matplotlib', 'long_description': '#
+ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/
+workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/
+actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/
+ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/
+gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/
+ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge]
+(https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
 anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for
 plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/
 ) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is
 a great data visualization technique to compare distributions from multiple
 groups at the same time, and was first introduced in 2017 as joy plot:\n\n
      I hereby propose that we call these "joy plots" #rstats https://t.co/
      uuLGpQLAwY
@@ -21,22 +21,24 @@
 \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple
 API to produce matplotlib-compatible ridgeplots, as well as a handy
 [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/
 0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with
 scikit-learn syntax for manipulating color annotations in a consistent way
 [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit
 clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython
-setup.py install \n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import
-ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport
-numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the
-input data should be a dict of\n# - keys: group names for the distributions\n#
-- values: list of values \ndata = {}\nfor i in range(8):\n data[\'data_
-{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig =
-plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n ax, \n data, \n xlim=(-
-20,20), \n label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/
-wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA
-[notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb)
-showing quick howto is included in this repo!\n', 'author': 'Douglas Wu',
-'author_email': 'wckdouglas@gmail.com', 'maintainer': None, 'maintainer_email':
-None, 'url': None, 'packages': packages, 'package_data': package_data,
+setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-
+forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-
+py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom
+ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport
+matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a
+dict of\n# - keys: group names for the distributions\n# - values: list of
+values \ndata = {}\nfor i in range(8):\n data[\'data_{}\'.format(i)] =
+np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax =
+fig.add_subplot(111)\nridgeplot(\n ax, \n data, \n xlim=(-20,20), \n
+label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/
+ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https:/
+/github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick
+howto is included in this repo!\n', 'author': 'Douglas Wu', 'author_email':
+'wckdouglas@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'None', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `ridgeplot-py-0.2.0/PKG-INFO` & `ridgeplot_py-0.2.0.post10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: ridgeplot-py
-Version: 0.2.0
+Version: 0.2.0.post10
 Summary: Plotting ridgeplots with matplotlib
 License: MIT
 Author: Douglas Wu
 Author-email: wckdouglas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Requires-Dist: matplotlib (>=3.1.3,<4.0.0)
 Requires-Dist: more-itertools (>=8.9.0,<9.0.0)
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Description-Content-Type: text/markdown
 
@@ -35,14 +37,26 @@
 
 ```bash
 git clone git@github.com:wckdouglas/ridgeplot-py.git
 cd ridgeplot-py
 python setup.py install 
 ```
 
+or via conda:
+
+```bash
+conda install -c conda-forge ridgeplot-py
+```
+
+or via pypi:
+
+```bash
+pip install ridgeplot-py
+```
+
 ## Usage ##
 
 ```python
 from ridgeplot import ridgeplot
 from ridgeplot.colors import ColorEncoder, ColorPalette
 import numpy as np
 import matplotlib.pyplot as plt
```

#### html2text {}

```diff
@@ -1,41 +1,45 @@
-Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.0 Summary: Plotting
-ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-email:
-wckdouglas@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.0.post10 Summary:
+Plotting ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-
+email: wckdouglas@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: dev Requires-Dist: matplotlib (>=3.1.3,<4.0.0) Requires-Dist:
-more-itertools (>=8.9.0,<9.0.0) Requires-Dist: numpy (>=1.21.1,<2.0.0)
-Requires-Dist: scipy (>=1.4.1,<2.0.0) Description-Content-Type: text/markdown #
-ridgeplot-py # [![CI](https://github.com/wckdouglas/ridgeplot-py/actions/
-workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/
-actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/
-ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/
-gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/
-ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge]
-(https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
-anaconda.org/conda-forge/ridgeplot-py) This is a simple module for plotting
-[ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the
-[scipy ecosystem](https://www.scipy.org/about.html). Ridgeplot is a great data
-visualization technique to compare distributions from multiple groups at the
-same time, and was first introduced in 2017 as joy plot:
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: dev Requires-Dist: matplotlib
+(>=3.1.3,<4.0.0) Requires-Dist: more-itertools (>=8.9.0,<9.0.0) Requires-Dist:
+numpy (>=1.21.1,<2.0.0) Requires-Dist: scipy (>=1.4.1,<2.0.0) Description-
+Content-Type: text/markdown # ridgeplot-py # [![CI](https://github.com/
+wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://
+github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
+(https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/
+badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [!
+[PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://
+badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-
+forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/
+ridgeplot-py) This is a simple module for plotting [ridgeplot](https://
+clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem]
+(https://www.scipy.org/about.html). Ridgeplot is a great data visualization
+technique to compare distributions from multiple groups at the same time, and
+was first introduced in 2017 as joy plot:
      I hereby propose that we call these "joy plots" #rstats https://t.co/
      uuLGpQLAwY
      — Jenny Bryan (@JennyBryan) April_25,_2017
 [ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to
 produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder]
 (https://github.com/wckdouglas/ridgeplot-py/blob/
 0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with
 scikit-learn syntax for manipulating color annotations in a consistent way
 [through out manuscripts or presentations]. ## Install ## ```bash git clone
 git@github.com:wckdouglas/ridgeplot-py.git cd ridgeplot-py python setup.py
-install ``` ## Usage ## ```python from ridgeplot import ridgeplot from
-ridgeplot.colors import ColorEncoder, ColorPalette import numpy as np import
-matplotlib.pyplot as plt # mocking some data # the input data should be a dict
-of # - keys: group names for the distributions # - values: list of values data
-= {} for i in range(8): data['data_{}'.format(i)] = np.random.randn(100) *
-(i+1) # make the plot fig = plt.figure() ax = fig.add_subplot(111) ridgeplot
-( ax, data, xlim=(-20,20), label_size=15 ) ``` ![img](https://
-raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png) ##
-Example ## A [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/
-Example.ipynb) showing quick howto is included in this repo!
+install ``` or via conda: ```bash conda install -c conda-forge ridgeplot-py ```
+or via pypi: ```bash pip install ridgeplot-py ``` ## Usage ## ```python from
+ridgeplot import ridgeplot from ridgeplot.colors import ColorEncoder,
+ColorPalette import numpy as np import matplotlib.pyplot as plt # mocking some
+data # the input data should be a dict of # - keys: group names for the
+distributions # - values: list of values data = {} for i in range(8): data
+['data_{}'.format(i)] = np.random.randn(100) * (i+1) # make the plot fig =
+plt.figure() ax = fig.add_subplot(111) ridgeplot( ax, data, xlim=(-20,20),
+label_size=15 ) ``` ![img](https://raw.githubusercontent.com/wckdouglas/
+ridgeplot-py/main/img/ridgeplot.png) ## Example ## A [notebook](https://
+github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto
+is included in this repo!
```

