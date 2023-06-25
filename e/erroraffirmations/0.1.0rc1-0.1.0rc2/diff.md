# Comparing `tmp/erroraffirmations-0.1.0rc1.tar.gz` & `tmp/erroraffirmations-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erroraffirmations-0.1.0rc1.tar", last modified: Sun Jun 25 11:50:16 2023, max compression
+gzip compressed data, was "erroraffirmations-0.1.0rc2.tar", last modified: Sun Jun 25 17:17:30 2023, max compression
```

## Comparing `erroraffirmations-0.1.0rc1.tar` & `erroraffirmations-0.1.0rc2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/affirmations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/erroraffirmations/data/affirmations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:50:16.000000 erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:50:16.784262 erroraffirmations-0.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-25 11:50:08.000000 erroraffirmations-0.1.0rc1/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:17:30.478293 erroraffirmations-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-25 17:17:30.478293 erroraffirmations-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:17:30.474293 erroraffirmations-0.1.0rc2/erroraffirmations/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/erroraffirmations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/erroraffirmations/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/erroraffirmations/affirmations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:17:30.478293 erroraffirmations-0.1.0rc2/erroraffirmations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/erroraffirmations/data/affirmations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:17:30.478293 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:17:30.000000 erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-25 17:17:30.482293 erroraffirmations-0.1.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:17:30.478293 erroraffirmations-0.1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-25 17:17:17.000000 erroraffirmations-0.1.0rc2/tests/test_interface.py
```

### Comparing `erroraffirmations-0.1.0rc1/LICENSE` & `erroraffirmations-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc1/PKG-INFO` & `erroraffirmations-0.1.0rc2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroraffirmations
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Affirmative error messages for Python
 Author-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 Maintainer-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Gessey-Jones
         
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/ThomasGesseyJones/ErrorAffirmations
 Project-URL: Bug Tracker, https://github.com/ThomasGesseyJones/ErrorAffirmations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Bug Tracking
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
@@ -43,16 +43,17 @@
 ========================================================
 
 Introduction
 ------------
 
 :ErrorAffirmations: Affirmative error messages for Python
 :Author: Thomas Gessey-Jones
-:Version: 0.1.0-rc.1
+:Version: 0.1.0-rc.2
 :Homepage: https://github.com/ThomasGesseyJones/ErrorAffirmations
+:Documentation: https://erroraffirmations.readthedocs.io
 
 .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Python version
 .. image:: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml
    :alt: Testing Status
@@ -62,17 +63,69 @@
 .. image:: https://readthedocs.org/projects/erroraffirmations/badge/?version=latest
    :target: https://erroraffirmations.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE
    :alt: License information
 
+``ErrorAffirmations`` is a Python package that appends affirmations to
+to help you feel better about your errors.
+
+Quickstart
+----------
+
+First install ``ErrorAffirmations``:
+
+.. code:: bash
+
+   pip install erroraffirmations
+
+Then import the ``erroraffirmations`` module:
+
+.. code:: python
+
+   import erroraffirmations
+
+and your ready to go! All errors will now be appended with an affirmation.
+
+
+Features
+--------
+
+Currently, ``ErrorAffirmations`` has the following features:
+
+- Appends affirmations to all errors
+- Allows you to add your own affirmations and remove existing affirmations
+- Allows you to enable/disable the adding of affirmations
+- Utilities to load affirmations from a file
+- A set of default affirmations to keep you motivated
+
+
+Requirements
+------------
+
+``ErrorAffirmations`` requires Python 3.7 or higher. It has no
+required dependencies.
+
+For documentation generation you will need:
+
+- Sphinx
+- sphinx-rtd-theme
+- numpydoc
+
+Testing requires:
+
+- pytest
+- pytest-cov
+- flake8
+- pydocstyle
+- pre-commit
+- packaging
+
 
-``ErrorAffirmations`` is a Python library that provides affirmative error messages, to help you feel better about your
-errors.
 
 Installation
 ------------
 
 ``ErrorAffirmations`` can be  directly installed via pip:
 
 .. code:: bash
@@ -112,71 +165,54 @@
       File "basic_usage.py", line 3, in <module>
         raise Exception('Something went wrong')
     Exception: Something went wrong
 
     Remember, every error you encounter is an opportunity for growth and learning. You're capable of overcoming this challenge!
 
 
-You can also access the affirmations list directly, to add your own affirmations:
-
-.. code:: python
-
-    from erroraffirmations import add_affirmation, get_affirmations, \
-    clear_affirmations
-
-    # Show part of the current list of affirmations
-    for affirmation in list(get_affirmations())[:5]:
-        print(affirmation)
-    print("\n")
-
-    # Remove all existing affirmations
-    clear_affirmations()
-
-    # Add your own affirmations
-    add_affirmation("You are doing great!")
+Code snippets demonstrating the advanced usage of ``ErrorAffirmations`` can be
+found in the `examples <https://github.com/ThomasGesseyJones/ErrorAffirmations/tree/main/examples>`__ directory.
 
-    # Show new list of affirmations
-    print(get_affirmations())
-    print("\n")
 
-    # Let us see it in action
-    raise ValueError("1 + 1 is not equal to 3")
+Documentation
+-------------
 
+The documentation for ``ErrorAffirmations`` can be found at
+`erroraffirmations.readthedocs.io <https://erroraffirmations.readthedocs.io/en/latest/>`__.
 
-.. code::
+To build the documentation locally, you will need to install the
+documentation dependencies:
 
-    The best programmers encounter errors regularly. It's a sign that you're exploring new territory and pushing your limits.
-    Mistakes are an essential part of the learning process. You're getting closer to the solution with each error you encounter.
-    The fact that you're facing this challenge head-on shows your determination and dedication. You've got this!
-    Take a moment to step back, breathe, and approach the problem from a different angle. A fresh perspective can lead to breakthroughs.
-    Remember, every error you encounter is an opportunity for growth and learning. You're capable of overcoming this challenge!
-
-
-    {'You are doing great!'}
-
-
-    Traceback (most recent call last):
-      File "/home/thomas/Documents/Pet_Projects/ErrorAffirmations/examples/editing_affirmations.py", line 22, in <module>
-        raise ValueError("1 + 1 is not equal to 3")
-    ValueError: 1 + 1 is not equal to 3
+.. code:: bash
 
-    You are doing great!
+   python -m pip install ".[docs]"
 
-    Process finished with exit code 1
+Then you can build the documentation:
 
+.. code:: bash
 
-Code snippets demonstrating the usage of ``ErrorAffirmations`` can be found in the ``examples`` directory.
+   cd docs
+   make html
 
+The documentation will be built in the ``docs/build`` directory.
+Open ``docs/build/html/index.html`` in your browser to view the documentation.
 
 License
 -------
 
-``ErrorAffirmations`` is licensed under the MIT license. See the ``LICENSE`` file for more details.
+``ErrorAffirmations`` is licensed under the MIT license. See the
+`LICENSE <https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE>`__
+file for more details.
 
 
 Contributing
 ------------
 
 Contributions are always welcome and greatly appreciated.
 
 - You can `open an issue <https://github.com/ThomasGesseyJones/ErrorAffirmations/issues>`__ to report bugs or to propose new features.
-- Or fork the repository, make your changes, and submit a pull request
+- Or fork the `repository <https://github.com/ThomasGesseyJones/ErrorAffirmations>`__, make your changes, and submit a `pull request <https://github.com/ThomasGesseyJones/ErrorAffirmations/pulls>`__.
+
+If it is your
+first time contributing to ``ErrorAffirmations``, please read the
+`contributing guidelines <https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/.github/CONTRIBUTING.md>`__
+before making a pull request.
```

### Comparing `erroraffirmations-0.1.0rc1/erroraffirmations/affirmations.py` & `erroraffirmations-0.1.0rc2/erroraffirmations/affirmations.py`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc1/erroraffirmations/data/affirmations.txt` & `erroraffirmations-0.1.0rc2/erroraffirmations/data/affirmations.txt`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc1/erroraffirmations.egg-info/PKG-INFO` & `erroraffirmations-0.1.0rc2/erroraffirmations.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroraffirmations
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Affirmative error messages for Python
 Author-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 Maintainer-email: Thomas Gessey-Jones <thomasgesseyjones@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Gessey-Jones
         
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/ThomasGesseyJones/ErrorAffirmations
 Project-URL: Bug Tracker, https://github.com/ThomasGesseyJones/ErrorAffirmations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Bug Tracking
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
@@ -43,16 +43,17 @@
 ========================================================
 
 Introduction
 ------------
 
 :ErrorAffirmations: Affirmative error messages for Python
 :Author: Thomas Gessey-Jones
-:Version: 0.1.0-rc.1
+:Version: 0.1.0-rc.2
 :Homepage: https://github.com/ThomasGesseyJones/ErrorAffirmations
+:Documentation: https://erroraffirmations.readthedocs.io
 
 .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Python version
 .. image:: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/actions/workflows/CI.yaml
    :alt: Testing Status
@@ -62,17 +63,69 @@
 .. image:: https://readthedocs.org/projects/erroraffirmations/badge/?version=latest
    :target: https://erroraffirmations.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE
    :alt: License information
 
+``ErrorAffirmations`` is a Python package that appends affirmations to
+to help you feel better about your errors.
+
+Quickstart
+----------
+
+First install ``ErrorAffirmations``:
+
+.. code:: bash
+
+   pip install erroraffirmations
+
+Then import the ``erroraffirmations`` module:
+
+.. code:: python
+
+   import erroraffirmations
+
+and your ready to go! All errors will now be appended with an affirmation.
+
+
+Features
+--------
+
+Currently, ``ErrorAffirmations`` has the following features:
+
+- Appends affirmations to all errors
+- Allows you to add your own affirmations and remove existing affirmations
+- Allows you to enable/disable the adding of affirmations
+- Utilities to load affirmations from a file
+- A set of default affirmations to keep you motivated
+
+
+Requirements
+------------
+
+``ErrorAffirmations`` requires Python 3.7 or higher. It has no
+required dependencies.
+
+For documentation generation you will need:
+
+- Sphinx
+- sphinx-rtd-theme
+- numpydoc
+
+Testing requires:
+
+- pytest
+- pytest-cov
+- flake8
+- pydocstyle
+- pre-commit
+- packaging
+
 
-``ErrorAffirmations`` is a Python library that provides affirmative error messages, to help you feel better about your
-errors.
 
 Installation
 ------------
 
 ``ErrorAffirmations`` can be  directly installed via pip:
 
 .. code:: bash
@@ -112,71 +165,54 @@
       File "basic_usage.py", line 3, in <module>
         raise Exception('Something went wrong')
     Exception: Something went wrong
 
     Remember, every error you encounter is an opportunity for growth and learning. You're capable of overcoming this challenge!
 
 
-You can also access the affirmations list directly, to add your own affirmations:
-
-.. code:: python
-
-    from erroraffirmations import add_affirmation, get_affirmations, \
-    clear_affirmations
-
-    # Show part of the current list of affirmations
-    for affirmation in list(get_affirmations())[:5]:
-        print(affirmation)
-    print("\n")
-
-    # Remove all existing affirmations
-    clear_affirmations()
-
-    # Add your own affirmations
-    add_affirmation("You are doing great!")
+Code snippets demonstrating the advanced usage of ``ErrorAffirmations`` can be
+found in the `examples <https://github.com/ThomasGesseyJones/ErrorAffirmations/tree/main/examples>`__ directory.
 
-    # Show new list of affirmations
-    print(get_affirmations())
-    print("\n")
 
-    # Let us see it in action
-    raise ValueError("1 + 1 is not equal to 3")
+Documentation
+-------------
 
+The documentation for ``ErrorAffirmations`` can be found at
+`erroraffirmations.readthedocs.io <https://erroraffirmations.readthedocs.io/en/latest/>`__.
 
-.. code::
+To build the documentation locally, you will need to install the
+documentation dependencies:
 
-    The best programmers encounter errors regularly. It's a sign that you're exploring new territory and pushing your limits.
-    Mistakes are an essential part of the learning process. You're getting closer to the solution with each error you encounter.
-    The fact that you're facing this challenge head-on shows your determination and dedication. You've got this!
-    Take a moment to step back, breathe, and approach the problem from a different angle. A fresh perspective can lead to breakthroughs.
-    Remember, every error you encounter is an opportunity for growth and learning. You're capable of overcoming this challenge!
-
-
-    {'You are doing great!'}
-
-
-    Traceback (most recent call last):
-      File "/home/thomas/Documents/Pet_Projects/ErrorAffirmations/examples/editing_affirmations.py", line 22, in <module>
-        raise ValueError("1 + 1 is not equal to 3")
-    ValueError: 1 + 1 is not equal to 3
+.. code:: bash
 
-    You are doing great!
+   python -m pip install ".[docs]"
 
-    Process finished with exit code 1
+Then you can build the documentation:
 
+.. code:: bash
 
-Code snippets demonstrating the usage of ``ErrorAffirmations`` can be found in the ``examples`` directory.
+   cd docs
+   make html
 
+The documentation will be built in the ``docs/build`` directory.
+Open ``docs/build/html/index.html`` in your browser to view the documentation.
 
 License
 -------
 
-``ErrorAffirmations`` is licensed under the MIT license. See the ``LICENSE`` file for more details.
+``ErrorAffirmations`` is licensed under the MIT license. See the
+`LICENSE <https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/LICENSE>`__
+file for more details.
 
 
 Contributing
 ------------
 
 Contributions are always welcome and greatly appreciated.
 
 - You can `open an issue <https://github.com/ThomasGesseyJones/ErrorAffirmations/issues>`__ to report bugs or to propose new features.
-- Or fork the repository, make your changes, and submit a pull request
+- Or fork the `repository <https://github.com/ThomasGesseyJones/ErrorAffirmations>`__, make your changes, and submit a `pull request <https://github.com/ThomasGesseyJones/ErrorAffirmations/pulls>`__.
+
+If it is your
+first time contributing to ``ErrorAffirmations``, please read the
+`contributing guidelines <https://github.com/ThomasGesseyJones/ErrorAffirmations/blob/main/.github/CONTRIBUTING.md>`__
+before making a pull request.
```

### Comparing `erroraffirmations-0.1.0rc1/pyproject.toml` & `erroraffirmations-0.1.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "Affirmative error messages for Python"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Topic :: Software Development :: Bug Tracking"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ThomasGesseyJones/ErrorAffirmations"
 "Bug Tracker" = "https://github.com/ThomasGesseyJones/ErrorAffirmations/issues"
```

### Comparing `erroraffirmations-0.1.0rc1/tests/test_examples.py` & `erroraffirmations-0.1.0rc2/tests/test_examples.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 """Test the example scripts."""
 
 import sys
+from erroraffirmations import enable_affirmations
 from pathlib import Path
 sys.path.append(str(Path(__file__).parent.parent.joinpath('examples')))
 
 
 # Run each example script
-def test_basic_usage_example():
-    """Test that basic_usage.py runs with expected Exception."""
+def test_quick_start_example():
+    """Test that quick_start.py runs with expected Exception."""
     try:
-        import basic_usage  # noqa: F401
+        import quick_start  # noqa: F401
     except Exception as e:
         assert isinstance(e, Exception)
         assert str(e) == 'Something went wrong'
 
 
 def test_editing_affirmations_example():
     """Test that editing_affirmations.py runs with expected Exception."""
     try:
         import editing_affirmations  # noqa: F401
     except ValueError as e:
         assert isinstance(e, ValueError)
         assert str(e) == "1 + 1 is not equal to 3"
 
 
+def test_loading_affirmations_example():
+    """Test that loading_affirmations.py runs with expected Exception."""
+    try:
+        import loading_affirmations  # noqa: F401
+    except ZeroDivisionError as e:
+        assert isinstance(e, ZeroDivisionError)
+
+
+def test_disabling_affirmations_example():
+    """Test that disabling_affirmations.py runs with expected Exception."""
+    try:
+        import disabling_affirmations  # noqa: F401
+    except TypeError as e:
+        assert isinstance(e, TypeError)
+        assert str(e) == "Boring regular error message"
+
+    # Renable affirmations for other tests
+    enable_affirmations()
+
+
 def test_empty_affirmations_examples():
     """Test that empty_affirmations.py runs with expected Exception."""
     try:
         import empty_affirmations  # noqa: F401
     except ValueError as e:
         assert isinstance(e, ValueError)
         assert str(e) == "A normal error message"
```

### Comparing `erroraffirmations-0.1.0rc1/tests/test_functionality.py` & `erroraffirmations-0.1.0rc2/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `erroraffirmations-0.1.0rc1/tests/test_interface.py` & `erroraffirmations-0.1.0rc2/tests/test_interface.py`

 * *Files identical despite different names*

