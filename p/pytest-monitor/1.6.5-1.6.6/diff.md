# Comparing `tmp/pytest-monitor-1.6.5.tar.gz` & `tmp/pytest-monitor-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-monitor-1.6.5.tar", last modified: Sat Oct 22 13:48:22 2022, max compression
+gzip compressed data, was "pytest-monitor-1.6.6.tar", last modified: Sun Jun 25 16:01:17 2023, max compression
```

## Comparing `pytest-monitor-1.6.5.tar` & `pytest-monitor-1.6.6.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-22 13:48:22.054742 pytest-monitor-1.6.5/
--rw-r--r--   0 root         (0) root         (0)      196 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1091 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13211 2022-10-22 13:48:22.054742 pytest-monitor-1.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11971 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-22 13:48:22.054742 pytest-monitor-1.6.5/pytest_monitor/
--rw-r--r--   0 root         (0) root         (0)       57 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/pytest_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4074 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/pytest_monitor/handler.py
--rw-r--r--   0 root         (0) root         (0)    12046 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/pytest_monitor/pytest_monitor.py
--rw-r--r--   0 root         (0) root         (0)     6706 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/pytest_monitor/session.py
--rw-r--r--   0 root         (0) root         (0)     5651 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/pytest_monitor/sys_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-22 13:48:22.054742 pytest-monitor-1.6.5/pytest_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13211 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       58 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-10-22 13:48:22.000000 pytest-monitor-1.6.5/pytest_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-22 13:48:22.054742 pytest-monitor-1.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2022-10-22 13:47:45.000000 pytest-monitor-1.6.5/setup.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-06-25 16:01:17.995260 pytest-monitor-1.6.6/
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)      196 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/AUTHORS
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     1091 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/LICENSE
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       97 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/MANIFEST.in
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    13201 2023-06-25 16:01:17.995260 pytest-monitor-1.6.6/PKG-INFO
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    11962 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/README.rst
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-06-25 16:01:17.991260 pytest-monitor-1.6.6/pytest_monitor/
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       57 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/pytest_monitor/__init__.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     4074 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/pytest_monitor/handler.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    12046 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/pytest_monitor/pytest_monitor.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     6706 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/pytest_monitor/session.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     5651 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/pytest_monitor/sys_utils.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-06-25 16:01:17.991260 pytest-monitor-1.6.6/pytest_monitor.egg-info/
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    13201 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)      529 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)        1 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       51 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       58 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/requires.txt
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       15 2023-06-25 16:01:17.000000 pytest-monitor-1.6.6/pytest_monitor.egg-info/top_level.txt
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)       38 2023-06-25 16:01:17.995260 pytest-monitor-1.6.6/setup.cfg
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     2364 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/setup.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-06-25 16:01:17.995260 pytest-monitor-1.6.6/tests/
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    11515 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/tests/test_monitor.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     4627 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/tests/test_monitor_component.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     4999 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/tests/test_monitor_context.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)    12271 2023-06-25 16:00:31.000000 pytest-monitor-1.6.6/tests/test_monitor_in_ci.py
```

### Comparing `pytest-monitor-1.6.5/LICENSE` & `pytest-monitor-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-monitor-1.6.5/PKG-INFO` & `pytest-monitor-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-monitor
-Version: 1.6.5
+Version: 1.6.6
 Summary: Pytest plugin for analyzing resource usage.
 Home-page: https://pytest-monitor.readthedocs.io/
 Author: Jean-Sébastien Dieu
 Author-email: jean-sebastien.dieu@cfm.fr
 Maintainer: Jean-Sébastien Dieu
 Maintainer-email: jean-sebastien.dieu@cfm.fr
 License: MIT
@@ -176,15 +176,15 @@
 ------
 
 If you encounter any problem, please `file an issue`_ along with a detailed description.
 
 Author
 ------
 
-The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jean-sebastien.dieu@cfm.fr.
+The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jdieu@salsify.fr.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
```

### Comparing `pytest-monitor-1.6.5/README.rst` & `pytest-monitor-1.6.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 ------
 
 If you encounter any problem, please `file an issue`_ along with a detailed description.
 
 Author
 ------
 
-The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jean-sebastien.dieu@cfm.fr.
+The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jdieu@salsify.fr.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
@@ -165,8 +165,8 @@
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/CFMTech/pytest-monitor/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
 .. _`monitor-server-api`: : https://github.com/CFMTech/monitor-server-api
-.. _`pytest-monitor-backend`: https://github.com/dremdem/pytest-monitor-backend
+.. _`pytest-monitor-backend`: https://github.com/dremdem/pytest-monitor-backend
```

### Comparing `pytest-monitor-1.6.5/pytest_monitor/handler.py` & `pytest-monitor-1.6.6/pytest_monitor/handler.py`

 * *Files identical despite different names*

### Comparing `pytest-monitor-1.6.5/pytest_monitor/pytest_monitor.py` & `pytest-monitor-1.6.6/pytest_monitor/pytest_monitor.py`

 * *Files identical despite different names*

### Comparing `pytest-monitor-1.6.5/pytest_monitor/session.py` & `pytest-monitor-1.6.6/pytest_monitor/session.py`

 * *Files identical despite different names*

### Comparing `pytest-monitor-1.6.5/pytest_monitor/sys_utils.py` & `pytest-monitor-1.6.6/pytest_monitor/sys_utils.py`

 * *Files identical despite different names*

### Comparing `pytest-monitor-1.6.5/pytest_monitor.egg-info/PKG-INFO` & `pytest-monitor-1.6.6/pytest_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-monitor
-Version: 1.6.5
+Version: 1.6.6
 Summary: Pytest plugin for analyzing resource usage.
 Home-page: https://pytest-monitor.readthedocs.io/
 Author: Jean-Sébastien Dieu
 Author-email: jean-sebastien.dieu@cfm.fr
 Maintainer: Jean-Sébastien Dieu
 Maintainer-email: jean-sebastien.dieu@cfm.fr
 License: MIT
@@ -176,15 +176,15 @@
 ------
 
 If you encounter any problem, please `file an issue`_ along with a detailed description.
 
 Author
 ------
 
-The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jean-sebastien.dieu@cfm.fr.
+The main author of `pytest-monitor` is Jean-Sébastien Dieu, who can be reached at jdieu@salsify.fr.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
```

### Comparing `pytest-monitor-1.6.5/setup.py` & `pytest-monitor-1.6.6/setup.py`

 * *Files identical despite different names*

