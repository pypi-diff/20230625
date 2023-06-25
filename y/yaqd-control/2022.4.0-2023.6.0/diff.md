# Comparing `tmp/yaqd-control-2022.4.0.tar.gz` & `tmp/yaqd_control-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqd-control-2022.4.0.tar", last modified: Mon Apr 25 20:32:52 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `yaqd-control-2022.4.0.tar` & `yaqd_control-2023.6.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1344 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/.gitignore
--rw-r--r--   0        0        0      808 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       34 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/.gitlab/CODEOWNERS
--rw-r--r--   0        0        0      363 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2822 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     7651 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/LICENSE
--rw-r--r--   0        0        0      700 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/README.md
--rw-r--r--   0        0        0     8706 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/docs/index.html
--rw-r--r--   0        0        0      737 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/docs/style.css
--rw-r--r--   0        0        0     1333 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/pyproject.toml
--rw-r--r--   0        0        0     1846 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/tests/test_get_executable_path_windows.py
--rw-r--r--   0        0        0       42 2022-04-25 20:32:21.602275 yaqd-control-2022.4.0/tests/test_smoke.py
--rw-r--r--   0        0        0       10 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/VERSION
--rw-r--r--   0        0        0      317 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/__init__.py
--rw-r--r--   0        0        0     6009 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/__main__.py
--rw-r--r--   0        0        0      493 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/__version__.py
--rw-r--r--   0        0        0     1727 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_cache.py
--rw-r--r--   0        0        0      458 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_daemon_data.py
--rw-r--r--   0        0        0     7615 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_enablement.py
--rw-r--r--   0        0        0     1658 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_list.py
--rw-r--r--   0        0        0     1725 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_scan.py
--rw-r--r--   0        0        0     1871 2022-04-25 20:32:21.603274 yaqd-control-2022.4.0/yaqd_control/_status.py
--rw-r--r--   0        0        0   368640 2022-04-25 20:32:21.606275 yaqd-control-2022.4.0/yaqd_control/bin/nssm.exe
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 yaqd-control-2022.4.0/PKG-INFO
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/docs/CNAME
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/docs/index.html
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/docs/style.css
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/tests/test_get_executable_path_windows.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/tests/test_smoke.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/__init__.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/__main__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/__version__.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_cache.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_daemon_data.py
+-rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_enablement.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_list.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_scan.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/_status.py
+-rw-r--r--   0        0        0   368640 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/yaqd_control/bin/nssm.exe
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/LICENSE
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/README.md
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 yaqd_control-2023.6.0/PKG-INFO
```

### Comparing `yaqd-control-2022.4.0/.gitignore` & `yaqd_control-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/.gitlab-ci.yml` & `yaqd_control-2023.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/CHANGELOG.md` & `yaqd_control-2023.6.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0]
+
+### Changed
+- Upgraded appdirs to platformdirs
+- Warn for unexpected characters in daemon names
+- Switch to hatchling
+
+### Added
+- Timeout for scan, including handling of scanning non-yaq ports
+
 ### [2022.4.0]
 
 ### Fixed
 - fixed bug where edit-config did not correctly call certain `%EDITOR%`s on Windows
 
 ### [2021.10.0]
 
@@ -84,15 +94,16 @@
 - manifest file: license actually distributed
 
 ## [0.1.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://gitlab.com/yaq/yaqd-control/-/compare/v2022.4.0...main
+[Unreleased]: https://gitlab.com/yaq/yaqd-control/-/compare/v2023.6.0...main
+[2023.6.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2022.4.0...v2023.6.0
 [2022.4.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2021.10.0...v2022.4.0
 [2021.10.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2021.5.0...v2021.10.0
 [2021.5.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2020.10.0...v2021.5.0
 [2020.10.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2020.07.0...v2020.10.0
 [2020.07.1]: https://gitlab.com/yaq/yaqd-control/-/compare/v2020.07.0...v2020.07.1
 [2020.07.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2020.06.0...v2020.07.0
 [2020.06.0]: https://gitlab.com/yaq/yaqd-control/-/compare/v2020.05.0...v2020.06.0
```

### Comparing `yaqd-control-2022.4.0/LICENSE` & `yaqd_control-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/docs/index.html` & `yaqd_control-2023.6.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/docs/style.css` & `yaqd_control-2023.6.0/docs/style.css`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/tests/test_get_executable_path_windows.py` & `yaqd_control-2023.6.0/tests/test_get_executable_path_windows.py`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/yaqd_control/__main__.py` & `yaqd_control-2023.6.0/yaqd_control/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import os
 import pathlib
 import subprocess
 import sys
 
-import appdirs  # type: ignore
+import platformdirs  # type: ignore
 import click
 
 from .__version__ import __version__
 from ._cache import add_config, clear_cache, read_daemon_cache
 from ._enablement import enable, disable, start, stop, reload, restart
 from ._scan import scan
 from ._status import status
@@ -66,31 +66,29 @@
     if not debug:
         sys.tracebacklimit = 0
     for k in kind:
         try:
             dd = next(d for d in read_daemon_cache() if d.kind == k)
             config_filepath = pathlib.Path(dd.config_filepath)
         except:
-            config_filepath = (
-                pathlib.Path(appdirs.user_config_dir("yaqd", "yaq")) / k / "config.toml"
-            )
+            config_filepath = platformdirs.user_config_path("yaqd", "yaq") / k / "config.toml"
         config_filepath.parent.mkdir(parents=True, exist_ok=True)
         while True:
             if sys.platform.startswith("win32"):
                 config_filepath = str(config_filepath)
                 import shutil
+
                 editor = shutil.which(os.environ.get("EDITOR", "notepad.exe"))
                 subprocess.run([editor, config_filepath])
             else:
                 subprocess.run([os.environ.get("EDITOR", "vi"), config_filepath])
             try:
                 add_config(config_filepath)
                 break
             except Exception:
-
                 if not click.confirm(
                     "Error updating cache. Would you like to re-edit the config?",
                     default=True,
                 ):
                     break
```

### Comparing `yaqd-control-2022.4.0/yaqd_control/_cache.py` & `yaqd_control-2023.6.0/yaqd_control/_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 __all__ = ["read_daemon_cache", "write_daemon_cache"]
 
 
 import pathlib
-import appdirs  # type: ignore
+import re
+import warnings
+
+import platformdirs
 import toml
 from ._daemon_data import DaemonData
 
 
 daemon_cache_path = (
-    pathlib.Path(appdirs.user_cache_dir(appname="yaqd-control", appauthor="yaq"))
-    / "daemon-cache.toml"
+    platformdirs.user_cache_path(appname="yaqd-control", appauthor="yaq") / "daemon-cache.toml"
 )
 
 daemon_cache_path.parent.mkdir(parents=True, exist_ok=True)
 
 
 # TODO: consider adding lockfile for cache
 
@@ -58,17 +60,25 @@
 def add_config(filepath):
     filepath = pathlib.Path(filepath).absolute()
     with open(filepath, "r") as f:
         dic = toml.load(f)
     kind = filepath.parent.name
     if kind.startswith("yaqd-"):
         kind = kind[5:]
+    ident = re.compile("^[a-zA-z_][a-zA-Z0-9_]*$")
     for k, v in dic.items():
         if k in ("enable", "shared-settings"):
             continue
+        if ident.match(k) is None:
+            warnings.warn(
+                f"Daemon named {k!r} may have incompatibilities with external systems"
+                "such as happi. Using a name which consists of only alphanumeric ASCII"
+                "characters or '_' (and not starting with a number) is recommended."
+            )
+
         dd = DaemonData(
             kind=kind,
             host="127.0.0.1",
             port=v["port"],
             name=k,
             config_filepath=str(filepath),
         )
```

### Comparing `yaqd-control-2022.4.0/yaqd_control/_enablement.py` & `yaqd_control-2023.6.0/yaqd_control/_enablement.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import getpass
 import pathlib
 import subprocess
 import sys
 import tempfile
 
-import appdirs  # type: ignore
+import platformdirs  # type: ignore
 
 from ._cache import add_config, read_daemon_cache
 from enum import Enum
 
 # Linux
 service_template = """
 [Unit]
@@ -219,15 +219,15 @@
 
 def _get_config_path(kind: str):
     known_daemons = read_daemon_cache()
     try:
         daemon_data = next(d for d in known_daemons if d.kind == kind)
         config_path = daemon_data.config_filepath
     except:
-        config_path = pathlib.Path(appdirs.user_config_dir("yaqd", "yaq")) / kind / "config.toml"
+        config_path = platformdirs.user_config_path("yaqd", "yaq") / kind / "config.toml"
         add_config(config_path)
     return config_path
 
 
 def _run_nssm_exe_by_action(action: Action, kind: str, check: bool = False, *additional_args):
     command = [nssm_exe, action, yaq_kind_template.format(kind=kind)]
     for arg in additional_args:
```

### Comparing `yaqd-control-2022.4.0/yaqd_control/_list.py` & `yaqd_control-2023.6.0/yaqd_control/_list.py`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/yaqd_control/_scan.py` & `yaqd_control-2023.6.0/yaqd_control/_scan.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,26 @@
         if dd.host == host:
             old_ports[dd.port] = dd
     #
     print(f"scanning host {host} from {start} to {stop}...")
     for i in range(start, stop + 1):
         kwargs = dict()
         try:
-            c = yaqc.Client(host=host, port=i)
+            c = yaqc.Client(host=host, port=i, timeout=0.1)
             kwargs["host"] = host
             kwargs["port"] = i
             kwargs["kind"] = c.id()["kind"]
             kwargs["name"] = c.id()["name"]
             kwargs["config_filepath"] = c.get_config_filepath()
             kwargs["make"] = c.id()["make"]
             kwargs["model"] = c.id()["model"]
             kwargs["serial"] = c.id()["serial"]
         except Exception as e:
+            if isinstance(e, socket.timeout):
+                print(f"...port {i} is open but does not appear to be a yaq daemon")
             if i in old_ports.keys():
                 kind = old_ports[i].kind
                 name = old_ports[i].name
                 print(f"...known daemon {kind}:{name} on port {i} not responding")
             continue
         # format result
         dd = DaemonData(**kwargs)
```

### Comparing `yaqd-control-2022.4.0/yaqd_control/_status.py` & `yaqd_control-2023.6.0/yaqd_control/_status.py`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/yaqd_control/bin/nssm.exe` & `yaqd_control-2023.6.0/yaqd_control/bin/nssm.exe`

 * *Files identical despite different names*

### Comparing `yaqd-control-2022.4.0/PKG-INFO` & `yaqd_control-2023.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 Metadata-Version: 2.1
 Name: yaqd-control
-Version: 2022.4.0
-Summary: Command line tools for inspecting and controlling yaq daemons.
-Home-page: https://yaq.fyi
+Version: 2023.6.0
+Project-URL: Home page, https://yaq.fyi
+Project-URL: Source, https://github.com/yaq-project/yaqd-control
+Project-URL: Documentation, https://control.yaq.fyi
+Project-URL: Issues, https://github.com/yaq-project/yaqd-control/issues
 Author: yaq developers
-Author-email: git@ksunden.space
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 2 - Pre-Alpha
+License-Expression: LGPL-3.0-only
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: appdirs
-Requires-Dist: toml>=0.10.2
+Requires-Python: >=3.7
 Requires-Dist: click
+Requires-Dist: platformdirs
 Requires-Dist: prettytable!=1.0.0
 Requires-Dist: rich
-Requires-Dist: yaqc
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: pytest ; extra == "tests"
-Requires-Dist: pytest-subprocess ; extra == "tests"
-Requires-Dist: types-toml ; extra == "tests"
-Requires-Dist: types-click ; extra == "tests"
-Project-URL: Documentation, https://control.yaq.fyi
-Project-URL: Issues, https://gitlab.com/yaq/yaqd-control/issues
-Project-URL: Source, https://gitlab.com/yaq/yaqd-control
+Requires-Dist: toml>=0.10.2
+Requires-Dist: yaqc>=2023.6.0
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-subprocess; extra == 'tests'
+Requires-Dist: types-click; extra == 'tests'
+Requires-Dist: types-toml; extra == 'tests'
+Description-Content-Type: text/markdown
 
 # yaqd-control
 
 [![PyPI](https://img.shields.io/pypi/v/yaqd-control)](https://pypi.org/project/yaqd-control)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/yaqd-control)](https://anaconda.org/conda-forge/yaqd-control)
 [![yaq](https://img.shields.io/badge/framework-yaq-orange)](https://yaq.fyi/)
 [![black](https://img.shields.io/badge/code--style-black-black)](https://black.readthedocs.io/)
 [![ver](https://img.shields.io/badge/calver-YYYY.0M.MICRO-blue)](https://calver.org/)
-[![log](https://img.shields.io/badge/change-log-informational)](https://gitlab.com/yaq/yaqd-control/-/blob/main/CHANGELOG.md)
+[![log](https://img.shields.io/badge/change-log-informational)](https://github.com/yaq-project/yaqd-control/blob/main/CHANGELOG.md#changelog)
 
 Command line tools for inspecting and controlling yaq daemons.
 https://control.yaq.fyi/
 
+## package maintainers
+
+- [Blaise Thompson](https://github.com/untzag)
+- [Kyle Sunden](https://github.com/ksunden)
```

