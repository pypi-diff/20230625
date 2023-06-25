# Comparing `tmp/pytest-md-report-0.3.1.tar.gz` & `tmp/pytest-md-report-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-md-report-0.3.1.tar", last modified: Sun May 28 14:55:33 2023, max compression
+gzip compressed data, was "pytest-md-report-0.3.2.tar", last modified: Sun Jun 25 14:22:31 2023, max compression
```

## Comparing `pytest-md-report-0.3.1.tar` & `pytest-md-report-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    10153 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      764 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/pytest_md_report/
--rw-r--r--   0 toor      (1000) toor      (1000)      300 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4447 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16902 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/pytest_md_report.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      609 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-28 14:55:25.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       94 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       86 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2791 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1034 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/test_option.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5016 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      917 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    10153 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      801 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/pytest_md_report/
+-rw-r--r--   0 toor      (1000) toor      (1000)      300 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4447 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16816 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/pytest_md_report/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/pytest_md_report.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      609 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 14:21:55.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       94 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-06-25 14:22:31.000000 pytest-md-report-0.3.2/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       86 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2791 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 14:22:31.824814 pytest-md-report-0.3.2/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       30 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/conftest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1034 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/test_option.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5016 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tests/test_plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      857 2023-06-25 14:21:37.000000 pytest-md-report-0.3.2/tox.ini
```

### Comparing `pytest-md-report-0.3.1/LICENSE` & `pytest-md-report-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/PKG-INFO` & `pytest-md-report-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.1
+Version: 0.3.2
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
```

### Comparing `pytest-md-report-0.3.1/README.rst` & `pytest-md-report-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/pyproject.toml` & `pytest-md-report-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
```

### Comparing `pytest-md-report-0.3.1/pytest_md_report/_const.py` & `pytest-md-report-0.3.2/pytest_md_report/_const.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/pytest_md_report/plugin.py` & `pytest-md-report-0.3.2/pytest_md_report/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pytablewriter.writer import AbstractTableWriter
 from typepy import Bool, Integer, StrictLevel
 from typepy.error import TypeConversionError
 
 from ._const import BGColor, ColorPolicy, Default, FGColor, Header, HelpMsg, Option, ZerosRender
 
 
-def zero_to_nullstr(value) -> str:
+def zero_to_nullstr(value: Any) -> Any:
     if value == 0:
         return ""
 
     return value
 
 
 def pytest_addoption(parser):
@@ -150,15 +150,15 @@
     if make_report is None:
         return False
 
     return make_report
 
 
 def _is_ci() -> bool:
-    # most of the CI services will be set CI environment to 'true'
+    # many CI services will set the CI environment variable to 'true'
     CI = os.environ.get("CI")
     if not CI:
         return False
 
     return CI.lower() == "true"
 
 
@@ -172,15 +172,15 @@
     APPVEYOR = os.environ.get("APPVEYOR")
     if not APPVEYOR:
         return False
 
     return APPVEYOR.lower() == "true"
 
 
-def _to_int(value) -> Optional[int]:
+def _to_int(value: Any) -> Optional[int]:
     try:
         return Integer(value, strict_level=StrictLevel.MIN).convert()
     except TypeConversionError:
         return None
 
 
 def retrieve_verbosity_level(config: Config) -> int:
@@ -323,15 +323,15 @@
         else:
             fg_color = self.__color_map[FGColor.GRAYOUT] if self.__is_grayout else base_color
             bg_color = BGColor.ODD_ROW if self.__report_color == ColorPolicy.AUTO else None
 
         return (fg_color, bg_color)
 
 
-def style_filter(cell: Cell, **kwargs: Dict[str, Any]) -> Optional[Style]:
+def style_filter(cell: Cell, **kwargs: Any) -> Optional[Style]:
     writer = cast(AbstractTableWriter, kwargs["writer"])
     report_color = cast(str, kwargs["report_color"])
     color_map = kwargs["color_map"]
     num_rows = cast(int, kwargs["num_rows"])
     fg_color = None
     bg_color = None
 
@@ -452,24 +452,22 @@
     matrix = [
         list(key) + [results.get(key, 0) for key in outcomes] + [sum(results.values())]
         for key, results in results_per_testfunc.items()
     ]
     if verbosity_level == 0:
         writer.headers = [Header.FILEPATH] + outcomes + [Header.SUBTOTAL]
         matrix.append(
-            ["TOTAL"]
-            + [total_stats.get(key, 0) for key in outcomes]  # type: ignore
-            + [sum(total_stats.values())]  # type: ignore
+            ["TOTAL"] + [total_stats.get(key, 0) for key in outcomes] + [sum(total_stats.values())]
         )
     elif verbosity_level >= 1:
         writer.headers = [Header.FILEPATH, Header.TESTFUNC] + outcomes + [Header.SUBTOTAL]
         matrix.append(
             ["TOTAL", ""]
-            + [total_stats.get(key, 0) for key in outcomes]  # type: ignore
-            + [sum(total_stats.values())]  # type: ignore
+            + [total_stats.get(key, 0) for key in outcomes]
+            + [sum(total_stats.values())]
         )
 
     writer.margin = retrieve_report_margin(config)
     writer.value_matrix = matrix
 
     report_color = retrieve_report_color(config)
     if report_color != ColorPolicy.NEVER:
```

### Comparing `pytest-md-report-0.3.1/pytest_md_report.egg-info/PKG-INFO` & `pytest-md-report-0.3.2/pytest_md_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.1
+Version: 0.3.2
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
```

### Comparing `pytest-md-report-0.3.1/pytest_md_report.egg-info/SOURCES.txt` & `pytest-md-report-0.3.2/pytest_md_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/setup.py` & `pytest-md-report-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/tests/test_option.py` & `pytest-md-report-0.3.2/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/tests/test_plugin.py` & `pytest-md-report-0.3.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.1/tox.ini` & `pytest-md-report-0.3.2/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 extras =
     test
 commands =
     pytest tests {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -42,11 +42,10 @@
 [testenv:lint]
 skip_install = true
 deps =
     codespell
     mypy>=1
     pylama>=8.4.1
 commands =
-    python setup.py check
     mypy pytest_md_report setup.py
     pylama
     - codespell pytest_md_report examples tests -q 2 --check-filenames
```

