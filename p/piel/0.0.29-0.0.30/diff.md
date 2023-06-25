# Comparing `tmp/piel-0.0.29.tar.gz` & `tmp/piel-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.29.tar", last modified: Wed Jun 21 15:17:29 2023, max compression
+gzip compressed data, was "piel-0.0.30.tar", last modified: Sun Jun 25 21:43:52 2023, max compression
```

## Comparing `piel-0.0.29.tar` & `piel-0.0.30.tar`

### file list

```diff
@@ -1,85 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 15:17:08.000000 piel-0.0.29/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-21 15:17:08.000000 piel-0.0.29/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 15:17:08.000000 piel-0.0.29/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 15:17:08.000000 piel-0.0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 15:17:08.000000 piel-0.0.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-21 15:17:29.394924 piel-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-21 15:17:08.000000 piel-0.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 15:17:08.000000 piel-0.0.29/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:17:08.000000 piel-0.0.29/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/gdsfactory/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/parse_results_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/parse_results_v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/piel/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-21 15:17:08.000000 piel-0.0.29/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 15:17:08.000000 piel-0.0.29/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/simple_design/tb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/examples/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-21 15:17:08.000000 piel-0.0.29/docs/examples/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 15:17:08.000000 piel-0.0.29/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:17:08.000000 piel-0.0.29/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 15:17:08.000000 piel-0.0.29/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 15:17:08.000000 piel-0.0.29/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 15:17:08.000000 piel-0.0.29/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.382924 piel-0.0.29/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 15:17:08.000000 piel-0.0.29/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 15:17:08.000000 piel-0.0.29/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 15:17:08.000000 piel-0.0.29/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 15:17:08.000000 piel-0.0.29/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-21 15:17:08.000000 piel-0.0.29/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-21 15:17:08.000000 piel-0.0.29/piel/cocotb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 15:17:08.000000 piel-0.0.29/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-06-21 15:17:08.000000 piel-0.0.29/piel/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 15:17:08.000000 piel-0.0.29/piel/gdsfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/parse_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-21 15:17:08.000000 piel-0.0.29/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 15:17:08.000000 piel-0.0.29/piel/piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-21 15:17:29.394924 piel-0.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-21 15:17:08.000000 piel-0.0.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 15:17:08.000000 piel-0.0.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 15:17:08.000000 piel-0.0.29/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.170741 piel-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-25 21:43:32.000000 piel-0.0.30/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-25 21:43:32.000000 piel-0.0.30/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-25 21:43:32.000000 piel-0.0.30/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 21:43:32.000000 piel-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-25 21:43:32.000000 piel-0.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 21:43:52.170741 piel-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-25 21:43:32.000000 piel-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-25 21:43:32.000000 piel-0.0.30/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 21:43:32.000000 piel-0.0.30/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/cocotb/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/integration/openlane_gdsfactory_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/integration/sax_cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/integration/sax_cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.154741 piel-0.0.30/docs/autoapi/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/parse/run_output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/parse/run_output/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 21:43:32.000000 piel-0.0.30/docs/autoapi/piel/piel/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-25 21:43:32.000000 piel-0.0.30/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 21:43:32.000000 piel-0.0.30/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.146741 piel-0.0.30/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.146741 piel-0.0.30/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/examples/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-25 21:43:32.000000 piel-0.0.30/docs/examples/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.158741 piel-0.0.30/docs/examples/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-25 21:43:32.000000 piel-0.0.30/docs/examples/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-25 21:43:32.000000 piel-0.0.30/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 21:43:32.000000 piel-0.0.30/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 21:43:32.000000 piel-0.0.30/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 21:43:32.000000 piel-0.0.30/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 21:43:32.000000 piel-0.0.30/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.146741 piel-0.0.30/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.162741 piel-0.0.30/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-25 21:43:32.000000 piel-0.0.30/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.162741 piel-0.0.30/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-25 21:43:32.000000 piel-0.0.30/docs/sections/environment/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.162741 piel-0.0.30/docs/sections/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-25 21:43:32.000000 piel-0.0.30/docs/sections/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.162741 piel-0.0.30/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-25 21:43:32.000000 piel-0.0.30/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-25 21:43:32.000000 piel-0.0.30/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.166741 piel-0.0.30/piel/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 21:43:32.000000 piel-0.0.30/piel/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-25 21:43:32.000000 piel-0.0.30/piel/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 21:43:32.000000 piel-0.0.30/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-25 21:43:32.000000 piel-0.0.30/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.166741 piel-0.0.30/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 21:43:32.000000 piel-0.0.30/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-25 21:43:32.000000 piel-0.0.30/piel/integration/openlane_gdsfactory_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:32.000000 piel-0.0.30/piel/integration/sax_cocotb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.166741 piel-0.0.30/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.170741 piel-0.0.30/piel/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/parse/run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-25 21:43:32.000000 piel-0.0.30/piel/openlane/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-25 21:43:32.000000 piel-0.0.30/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 21:43:32.000000 piel-0.0.30/piel/piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.166741 piel-0.0.30/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:43:51.000000 piel-0.0.30/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 21:43:52.000000 piel-0.0.30/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-25 21:43:52.170741 piel-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-25 21:43:32.000000 piel-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:43:52.170741 piel-0.0.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 21:43:32.000000 piel-0.0.30/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 21:43:32.000000 piel-0.0.30/tests/test_piel.py
```

### Comparing `piel-0.0.29/CONTRIBUTING.rst` & `piel-0.0.30/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/LICENSE` & `piel-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/PKG-INFO` & `piel-0.0.30/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.29
+Version: 0.0.30
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# `piel` - Photonic and Integrated ELectronic system design
+# `piel` - Photonic and Integrated ELectronic tools
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -39,31 +39,22 @@
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
-* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
-  electronic logic and outputs performance parameters of the implemented circuitry.
+* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
 Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
 - Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
 - `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-
-
-=======
-History
-=======
-
-0.0.1 (2023-06-10)
-------------------
-
-* First release on PyPI.
```

### Comparing `piel-0.0.29/README.md` & `piel-0.0.30/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `piel` - Photonic and Integrated ELectronic system design
+# `piel` - Photonic and Integrated ELectronic tools
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -16,17 +16,18 @@
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
-* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
-  electronic logic and outputs performance parameters of the implemented circuitry.
+* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
 Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
```

### Comparing `piel-0.0.29/docs/Makefile` & `piel-0.0.30/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/docs/autoapi/piel/cocotb/index.rst` & `piel-0.0.30/docs/autoapi/piel/cocotb/core/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-:py:mod:`piel.cocotb`
-=====================
+:py:mod:`piel.cocotb.core`
+==========================
 
-.. py:module:: piel.cocotb
+.. py:module:: piel.cocotb.core
 
 .. autoapi-nested-parse::
 
    The objective of this file is to provide the simulation ports and interconnection to consider modelling digital and mixed signal logic.
 
    The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital simulations.
    The cocotb verification software can also be used to perform mixed signal simulation, and digital data can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do this) writes an equivalent python-based or C++ based python time-domain simulation solver.
@@ -19,27 +19,27 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.cocotb.check_cocotb_testbench_exists
-   piel.cocotb.configure_cocotb_simulation
-   piel.cocotb.run_cocotb_simulation
+   piel.cocotb.core.check_cocotb_testbench_exists
+   piel.cocotb.core.configure_cocotb_simulation
+   piel.cocotb.core.run_cocotb_simulation
 
 
 
 Attributes
 ~~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.cocotb.write_cocotb_makefile
-   piel.cocotb.make_cocotb
+   piel.cocotb.core.write_cocotb_makefile
+   piel.cocotb.core.make_cocotb
 
 
 .. py:function:: check_cocotb_testbench_exists(design_directory: str | pathlib.Path) -> bool
 
    Checks if a cocotb testbench exists in the design directory.
 
    :param design_directory: Design directory.
```

### Comparing `piel-0.0.29/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.30/docs/autoapi/piel/file_system/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,36 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
+   piel.file_system.check_path_exists
    piel.file_system.check_example_design
    piel.file_system.copy_source_folder
    piel.file_system.permit_script_execution
    piel.file_system.return_path
    piel.file_system.run_script
    piel.file_system.setup_example_design
    piel.file_system.write_script
 
 
 
+.. py:function:: check_path_exists(path: str | pathlib.Path, raise_errors: bool = False) -> bool
+
+   Checks if a directory exists.
+
+   :param path: Input path.
+   :type path: str | pathlib.Path
+
+   :returns: True if directory exists.
+   :rtype: directory_exists(bool)
+
+
 .. py:function:: check_example_design(design_name: str | pathlib.Path = 'simple_design') -> bool
 
    We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
    :param design_name: Name of the design to check.
    :type design_name: str
```

### Comparing `piel-0.0.29/docs/autoapi/piel/gdsfactory/index.rst` & `piel-0.0.30/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-:py:mod:`piel.gdsfactory`
-=========================
+:py:mod:`piel.integration.openlane_gdsfactory_core`
+===================================================
 
-.. py:module:: piel.gdsfactory
+.. py:module:: piel.integration.openlane_gdsfactory_core
 
 .. autoapi-nested-parse::
 
    There are a number of ways to generate gdsfactory integration.
 
    It is worth noting that GDSFactory has already the following PDKs installed:
    * SKY130nm https://gdsfactory.github.io/skywater130/
@@ -18,24 +18,28 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.gdsfactory.create_gdsfactory_component_from_openlane
+   piel.integration.openlane_gdsfactory_core.create_gdsfactory_component_from_openlane
 
 
 
-.. py:function:: create_gdsfactory_component_from_openlane(design_directory: str | pathlib.Path, run_name: str | None = None) -> gdsfactory.Component
+.. py:function:: create_gdsfactory_component_from_openlane(design_name_v1: str | None = None, design_directory: str | pathlib.Path | None = None, run_name: str | None = None, v1: bool = True) -> gdsfactory.Component
 
    This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
 
    It will look into the latest design run and extract the final OpenLane-generated GDS. You do not have to have run this with OpenLane2 as it just looks at the latest run.
 
+   :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
+   :type design_name_v1: str
    :param design_directory: Design directory PATH.
    :type design_directory: str
    :param run_name: Name of the run to extract the GDS from. If None, it will look at the latest run.
    :type run_name: str
+   :param v1: If True, it will import the design from the OpenLane v1 configuration.
+   :type v1: bool
 
    :returns: GDSFactory component.
    :rtype: component(gf.Component)
```

### Comparing `piel-0.0.29/docs/autoapi/piel/openlane/index.rst` & `piel-0.0.30/docs/autoapi/piel/openlane/v1/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,40 @@
-:py:mod:`piel.openlane`
-=======================
+:py:mod:`piel.openlane.v1`
+==========================
 
-.. py:module:: piel.openlane
+.. py:module:: piel.openlane.v1
 
+.. autoapi-nested-parse::
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
+   These set of functions aim to provide functionality to automate interacting with OpenLanes v1 design into Python environment, whilst `OpenLanes2` is under development.
 
-   parse_results_v1/index.rst
-   utils/index.rst
-   v1/index.rst
-   v2/index.rst
 
 
-Package Contents
-----------------
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.openlane.configure_parametric_designs
-   piel.openlane.create_parametric_designs
-   piel.openlane.find_design_run
-   piel.openlane.check_config_json_exists_openlane_v1
-   piel.openlane.check_design_exists_openlane_v1
-   piel.openlane.configure_and_run_design_openlane_v1
-   piel.openlane.configure_flow_script_openlane_v1
-   piel.openlane.get_latest_version_root_openlane_v1
-   piel.openlane.write_configuration_openlane_v1
-   piel.openlane.run_openlane_flow
+   piel.openlane.v1.check_config_json_exists_openlane_v1
+   piel.openlane.v1.check_design_exists_openlane_v1
+   piel.openlane.v1.configure_and_run_design_openlane_v1
+   piel.openlane.v1.configure_flow_script_openlane_v1
+   piel.openlane.v1.configure_parametric_designs_openlane_v1
+   piel.openlane.v1.create_parametric_designs_openlane_v1
+   piel.openlane.v1.get_latest_version_root_openlane_v1
+   piel.openlane.v1.get_design_directory_from_root_openlane_v1
+   piel.openlane.v1.read_configuration_openlane_v1
+   piel.openlane.v1.write_configuration_openlane_v1
 
 
 
-.. py:function:: configure_parametric_designs(parameter_sweep_dictionary: dict, source_design_directory: str | pathlib.Path) -> list
-
-   For a given `source_design_directory`, this function reads in the config.json file and returns a set of parametric sweeps that gets used when creating a set of parametric designs.
-
-   :param parameter_sweep_dictionary: Dictionary of parameters to sweep.
-   :type parameter_sweep_dictionary: dict
-   :param source_design_directory: Source design directory.
-   :type source_design_directory: str | pathlib.Path
-
-   :returns: List of configurations to sweep.
-   :rtype: configuration_sweep(list)
-
-
-.. py:function:: create_parametric_designs(parameter_sweep_dictionary: dict, source_design_directory: str | pathlib.Path, target_directory: str | pathlib.Path) -> None
-
-   Takes a OpenLane v1 source directory and creates a parametric combination of these designs.
-
-   :param parameter_sweep_dictionary: Dictionary of parameters to sweep.
-   :type parameter_sweep_dictionary: dict
-   :param source_design_directory: Source design directory.
-   :type source_design_directory: str
-   :param target_directory: Target directory.
-   :type target_directory: str
-
-   :returns: None
-
-
-.. py:function:: find_design_run(design_directory: str | pathlib.Path, run_name: str | None = None) -> str
-
-   For a given `design_directory`, the `openlane` output can be found in the `runs` subdirectory.
-
-   They get sorted based on a reverse `list.sort()` method.
-
-
 .. py:function:: check_config_json_exists_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> bool
 
    Checks if a design has a `config.json` file.
 
    :param design_name: Name of the design.
    :type design_name: str
 
@@ -122,34 +81,77 @@
 
    :param design_directory: Design directory. Defaults to latest OpenLane root.
    :type design_directory: str | pathlib.Path | None
 
    :returns: None
 
 
+.. py:function:: configure_parametric_designs_openlane_v1(design_name: str, parameter_sweep_dictionary: dict, add_id: bool = True) -> list
+
+   For a given `source_design_directory`, this function reads in the config.json file and returns a set of parametric sweeps that gets used when creating a set of parametric designs.
+
+   :param add_id: Add an ID to the design name. Defaults to True.
+   :type add_id: bool
+   :param parameter_sweep_dictionary: Dictionary of parameters to sweep.
+   :type parameter_sweep_dictionary: dict
+   :param source_design_directory: Source design directory.
+   :type source_design_directory: str | pathlib.Path
+
+   :returns: List of configurations to sweep.
+   :rtype: configuration_sweep(list)
+
+
+.. py:function:: create_parametric_designs_openlane_v1(design_name: str, parameter_sweep_dictionary: dict, target_directory: str | pathlib.Path | None = None) -> None
+
+   Takes a OpenLane v1 source directory and creates a parametric combination of these designs.
+
+   :param design_name: Name of the design.
+   :type design_name: str
+   :param parameter_sweep_dictionary: Dictionary of parameters to sweep.
+   :type parameter_sweep_dictionary: dict
+   :param target_directory: Optional target directory.
+   :type target_directory: str | pathlib.Path | None
+
+   :returns: None
+
+
 .. py:function:: get_latest_version_root_openlane_v1() -> pathlib.Path
 
    Gets the latest version root of OpenLane v1.
 
 
-.. py:function:: write_configuration_openlane_v1(configuration: dict, design_directory: str | pathlib.Path) -> None
+.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
 
-   Writes a `config.json` onto a `design_directory`
+   Gets the design directory from the root directory.
 
-   :param configuration: OpenLane configuration dictionary.
-   :type configuration: dict
-   :param design_directory: Design directory PATH.
-   :type design_directory: str
+   :param design_name: Name of the design.
+   :type design_name: str
+   :param root_directory: Design directory.
+   :type root_directory: str | pathlib.Path
 
-   :returns: None
+   :returns: Design directory.
+   :rtype: design_directory(pathlib.Path)
 
 
-.. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: str = '/foss/designs/spm') -> None
+.. py:function:: read_configuration_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> dict
 
-   Runs the OpenLane flow.
+   Reads a `config.json` from a design directory.
 
-   :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
+   :param design_name: Design name.
+   :type design_name: str
+   :param root_directory: Design directory.
+   :type root_directory: str | pathlib.Path
+
+   :returns: Configuration dictionary.
+   :rtype: configuration(dict)
+
+
+.. py:function:: write_configuration_openlane_v1(configuration: dict, design_directory: str | pathlib.Path) -> None
+
+   Writes a `config.json` onto a `design_directory`
+
+   :param configuration: OpenLane configuration dictionary.
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
```

### Comparing `piel-0.0.29/docs/autoapi/piel/openlane/v2/index.rst` & `piel-0.0.30/docs/autoapi/piel/openlane/v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.30/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/docs/conf.py` & `piel-0.0.30/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/docs/examples/simple_design/tb/default/Makefile` & `piel-0.0.30/docs/examples/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/docs/make.bat` & `piel-0.0.30/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/piel/cocotb.py` & `piel-0.0.30/piel/cocotb/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The cocotb verification software can also be used to perform mixed signal simulation, and digital data can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do this) writes an equivalent python-based or C++ based python time-domain simulation solver.
 
 The nice thing about cocotb is that as long as the photonic simulations can be written asyncrhonously, time-domain simulations can be closely integrated or simulated through this verification software.
 """
 import pathlib
 import subprocess
 from typing import Literal
-from .file_system import return_path, write_script
+from piel.file_system import return_path, write_script
 
 
 def check_cocotb_testbench_exists(
     design_directory: str | pathlib.Path,
 ) -> bool:
     """
     Checks if a cocotb testbench exists in the design directory.
```

### Comparing `piel-0.0.29/piel/defaults.py` & `piel-0.0.30/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/piel/file_system.py` & `piel-0.0.30/piel/file_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-import subprocess
-
+import glob
 import openlane
 import os
 import pathlib
 import shutil
 import stat
+import subprocess
 from typing import Literal
 
 
-def check_directory_exists(directory_path: str | pathlib.Path) -> bool:
+def check_path_exists(
+    path: str | pathlib.Path,
+    raise_errors: bool = False,
+) -> bool:
     """
     Checks if a directory exists.
 
     Args:
-        directory_path(str | pathlib.Path): Input path.
+        path(str | pathlib.Path): Input path.
 
     Returns:
         directory_exists(bool): True if directory exists.
     """
     directory_exists = False
-    directory_path = return_path(directory_path)
-    if directory_path.exists():
+    path = return_path(path)
+    if path.exists():
         directory_exists = True
     else:
-        pass
+        if raise_errors:
+            raise ValueError("Path: " + str(path) + " does not exist.")
     return directory_exists
 
 
 def check_example_design(design_name: str | pathlib.Path = "simple_design") -> bool:
     """
     We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
@@ -105,14 +109,36 @@
     if parent_directory_permissions != "0o777":
         permit_directory_all(parent_directory)
 
     # Create the directory
     directory_path.mkdir(parents=True)
 
 
+def get_files_recursively_in_directory(
+    path: str | pathlib.Path,
+    extension: str = "*",
+):
+    """
+    Returns a list of files in a directory.
+
+    Args:
+        path(str | pathlib.Path): Input path.
+        extension(str): File extension.
+
+    Returns:
+        file_list(list): List of files.
+    """
+    path = return_path(path)
+    file_list = []
+    for x in os.walk(str(path.resolve())):
+        for file_path in glob.glob(os.path.join(x[0], f"*.{extension}")):
+            file_list.append(file_path)
+    return file_list
+
+
 def permit_script_execution(script_path: str | pathlib.Path) -> None:
     """
     Permits the execution of a script.
 
     Args:
         script_path(str): Script path.
 
@@ -225,15 +251,15 @@
         script_name(str): Name of the script.
 
     Returns:
         None
     """
     directory_path = return_path(directory_path)
 
-    directory_exists = check_directory_exists(directory_path)
+    directory_exists = check_path_exists(directory_path)
 
     if directory_exists:
         pass
     else:
         try:
             create_new_directory(directory_path)
         except PermissionError:
@@ -247,14 +273,15 @@
 
     file = open(str(directory_path / script_name), "w")
     file.write(script)
     file.close()
 
 
 __all__ = [
+    "check_path_exists",
     "check_example_design",
     "copy_source_folder",
     "permit_script_execution",
     "setup_example_design",
     "return_path",
     "run_script",
     "write_script",
```

### Comparing `piel-0.0.29/piel/gdsfactory.py` & `piel-0.0.30/piel/integration/openlane_gdsfactory_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 """
 There are a number of ways to generate gdsfactory integration.
 
 It is worth noting that GDSFactory has already the following PDKs installed:
 * SKY130nm https://gdsfactory.github.io/skywater130/
 * GF180nm https://gdsfactory.github.io/gf180/
-
 """
 import gdsfactory as gf
 import pathlib
-from .openlane.utils import find_design_run
-from .file_system import return_path
+from ..file_system import check_path_exists
+from ..openlane.migrate import get_design_from_openlane_migration
+from ..openlane.utils import find_design_run
 
 
 def create_gdsfactory_component_from_openlane(
-    design_directory: str | pathlib.Path, run_name: str | None = None
+    design_name_v1: str | None = None,
+    design_directory: str | pathlib.Path | None = None,
+    run_name: str | None = None,
+    v1: bool = True,
 ) -> gf.Component:
     """
     This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
 
     It will look into the latest design run and extract the final OpenLane-generated GDS. You do not have to have run this with OpenLane2 as it just looks at the latest run.
 
     Args:
+        design_name_v1(str): Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
         design_directory(str): Design directory PATH.
         run_name(str): Name of the run to extract the GDS from. If None, it will look at the latest run.
+        v1(bool): If True, it will import the design from the OpenLane v1 configuration.
 
     Returns:
         component(gf.Component): GDSFactory component.
     """
-    design_directory = return_path(design_directory)
-    design_name = design_directory.parent.name
+    design_name, design_directory = get_design_from_openlane_migration(
+        v1=v1, design_name_v1=design_name_v1, design_directory=design_directory
+    )
     latest_design_run_directory = find_design_run(design_directory, run_name=run_name)
     final_gds_run = (
-        latest_design_run_directory / "results" / "final" / "gds" / design_name + ".gds"
+        latest_design_run_directory
+        / "results"
+        / "final"
+        / "gds"
+        / (design_name + ".gds")
     )
+    check_path_exists(final_gds_run, raise_errors=True)
     component = gf.import_gds(final_gds_run, name=design_name)
     return component
 
 
 __all__ = ["create_gdsfactory_component_from_openlane"]
```

### Comparing `piel-0.0.29/piel/openlane/v1.py` & `piel-0.0.30/piel/openlane/v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,41 @@
+"""
+These set of functions aim to provide functionality to automate interacting with OpenLanes v1 design into Python environment, whilst `OpenLanes2` is under development.
+"""
+
 import os
 import pathlib
 import json
+from ..parametric import multi_parameter_sweep
 from ..file_system import (
+    copy_source_folder,
+    permit_script_execution,
     return_path,
-    write_script,
     run_script,
-    permit_script_execution,
+    write_script,
 )
 
 
-def configure_flow_script_openlane_v1(
-    design_name: str,
-    root_directory: str | pathlib.Path | None = None,
-) -> None:
-    """
-    Configures the OpenLane v1 flow script after checking that the design directory exists.
-
-    Args:
-        design_directory(str | pathlib.Path | None): Design directory. Defaults to latest OpenLane root.
-
-    Returns:
-        None
-    """
-    if root_directory is None:
-        root_directory = get_latest_version_root_openlane_v1()
-
-    design_directory = root_directory / "designs" / design_name
-    if check_design_exists_openlane_v1(design_name):
-        commands_list = [
-            "#!/bin/sh",
-            "cd " + str(root_directory),
-            "./flow.tcl -design " + design_name,
-        ]
-        script = " \n".join(commands_list)
-        write_script(
-            directory_path=design_directory / "scripts",
-            script=script,
-            script_name="openlane_flow.sh",
-        )
-    else:
-        raise ValueError(
-            "Design: "
-            + str(design_name)
-            + " not found in "
-            + os.environ["OPENLANE_ROOT"]
-        )
-
-
 def check_config_json_exists_openlane_v1(
     design_name: str,
     root_directory: str | pathlib.Path | None = None,
 ) -> bool:
     """
     Checks if a design has a `config.json` file.
 
     Args:
         design_name(str): Name of the design.
 
     Returns:
         config_json_exists(bool): True if `config.json` exists.
     """
-    if root_directory is None:
-        root_directory = get_latest_version_root_openlane_v1()
-
     config_json_exists = False
-    openlane_v1_design_directory = root_directory / "designs"
-    design_directory = openlane_v1_design_directory / design_name
+    design_directory = get_design_directory_from_root_openlane_v1(
+        design_name=design_name, root_directory=root_directory
+    )
     if (design_directory / "config.json").exists():
         config_json_exists = True
     return config_json_exists
 
 
 def check_design_exists_openlane_v1(
     design_name: str,
@@ -115,31 +81,18 @@
         design_name(str): Name of the design.
         configuration(dict | None): Configuration dictionary.
         root_directory(str | pathlib.Path): Design directory.
 
     Returns:
         None
     """
-    if root_directory is None:
-        root_directory = get_latest_version_root_openlane_v1()
 
-    root_directory = return_path(root_directory)
-    design_exists = check_design_exists_openlane_v1(design_name)
-    design_directory = root_directory / "designs" / design_name
-
-    # Check design existence
-    if design_exists:
-        pass
-    else:
-        raise ValueError(
-            "Design: "
-            + design_name
-            + " is not found in "
-            + str(root_directory / "designs")
-        )
+    design_directory = get_design_directory_from_root_openlane_v1(
+        design_name=design_name, root_directory=root_directory
+    )
 
     # Check configuration
     config_json_exists = check_config_json_exists_openlane_v1(design_name)
 
     if config_json_exists:
         pass
     else:
@@ -157,24 +110,198 @@
 
     # Execute script
     openlane_flow_script_path = design_directory / "scripts" / "openlane_flow.sh"
     permit_script_execution(openlane_flow_script_path)
     run_script(openlane_flow_script_path)
 
 
+def configure_flow_script_openlane_v1(
+    design_name: str,
+    root_directory: str | pathlib.Path | None = None,
+) -> None:
+    """
+    Configures the OpenLane v1 flow script after checking that the design directory exists.
+
+    Args:
+        design_directory(str | pathlib.Path | None): Design directory. Defaults to latest OpenLane root.
+
+    Returns:
+        None
+    """
+    design_directory = get_design_directory_from_root_openlane_v1(
+        design_name=design_name, root_directory=root_directory
+    )
+    if check_design_exists_openlane_v1(design_name):
+        commands_list = [
+            "#!/bin/sh",
+            "cd " + str(root_directory),
+            "./flow.tcl -design " + design_name,
+        ]
+        script = " \n".join(commands_list)
+        write_script(
+            directory_path=design_directory / "scripts",
+            script=script,
+            script_name="openlane_flow.sh",
+        )
+    else:
+        raise ValueError(
+            "Design: "
+            + str(design_name)
+            + " not found in "
+            + os.environ["OPENLANE_ROOT"]
+        )
+
+
+def configure_parametric_designs_openlane_v1(
+    design_name: str,
+    parameter_sweep_dictionary: dict,
+    add_id: bool = True,
+) -> list:
+    """
+    For a given `source_design_directory`, this function reads in the config.json file and returns a set of parametric sweeps that gets used when creating a set of parametric designs.
+
+    Args:
+        add_id(bool): Add an ID to the design name. Defaults to True.
+        parameter_sweep_dictionary(dict): Dictionary of parameters to sweep.
+        source_design_directory(str | pathlib.Path): Source design directory.
+
+    Returns:
+        configuration_sweep(list): List of configurations to sweep.
+    """
+    source_configuration = read_configuration_openlane_v1(design_name=design_name)
+    configuration_sweep = multi_parameter_sweep(
+        base_design_configuration=source_configuration,
+        parameter_sweep_dictionary=parameter_sweep_dictionary,
+    )
+    if add_id:
+        i = 0
+        for configuration_i in configuration_sweep:
+            # Checks the unique ID of the configuration
+            configuration_id = id(configuration_i)
+            # Adds the ID to the configuration list
+            configuration_sweep[i]["id"] = configuration_id
+            i += 1
+    return configuration_sweep
+
+
+def create_parametric_designs_openlane_v1(
+    design_name: str,
+    parameter_sweep_dictionary: dict,
+    target_directory: str | pathlib.Path | None = None,
+) -> None:
+    """
+    Takes a OpenLane v1 source directory and creates a parametric combination of these designs.
+
+    Args:
+        design_name(str): Name of the design.
+        parameter_sweep_dictionary(dict): Dictionary of parameters to sweep.
+        target_directory(str | pathlib.Path | None): Optional target directory.
+
+    Returns:
+        None
+    """
+    source_design_directory = get_design_directory_from_root_openlane_v1(
+        design_name=design_name
+    )
+    source_design_name = design_name
+
+    if target_directory is None:
+        target_directory = get_latest_version_root_openlane_v1() / "designs"
+
+    parameter_sweep_configuration_list = configure_parametric_designs_openlane_v1(
+        add_id=True,
+        design_name=design_name,
+        parameter_sweep_dictionary=parameter_sweep_dictionary,
+    )
+
+    for configuration_i in parameter_sweep_configuration_list:
+        # Create a target directory with the name of the design and the configuration ID
+        target_directory_i = (
+            target_directory / source_design_name + "_" + str(configuration_i["id"])
+        )
+        # Copy the source design directory to the target directory
+        copy_source_folder(
+            source_directory=source_design_directory,
+            target_directory=target_directory_i,
+        )
+
+
 def get_latest_version_root_openlane_v1() -> pathlib.Path:
     """
     Gets the latest version root of OpenLane v1.
     """
     openlane_tool_directory = pathlib.Path(os.environ["OPENLANE_ROOT"])
     latest_openlane_version = list(openlane_tool_directory.iterdir())
     openlane_v1_design_directory = openlane_tool_directory / latest_openlane_version[-1]
     return openlane_v1_design_directory
 
 
+def get_design_directory_from_root_openlane_v1(
+    design_name: str,
+    root_directory: str | pathlib.Path | None = None,
+) -> pathlib.Path:
+    """
+    Gets the design directory from the root directory.
+
+    Args:
+        design_name(str): Name of the design.
+        root_directory(str | pathlib.Path): Design directory.
+
+    Returns:
+        design_directory(pathlib.Path): Design directory.
+    """
+    if root_directory is None:
+        root_directory = get_latest_version_root_openlane_v1()
+
+    root_directory = return_path(root_directory)
+    design_exists = check_design_exists_openlane_v1(design_name)
+    if design_exists:
+        pass
+    else:
+        raise ValueError(
+            "Design: "
+            + design_name
+            + " is not found in "
+            + str(root_directory / "designs")
+        )
+    design_directory = root_directory / "designs" / design_name
+    return design_directory
+
+
+def read_configuration_openlane_v1(
+    design_name: str,
+    root_directory: str | pathlib.Path | None = None,
+) -> dict:
+    """
+    Reads a `config.json` from a design directory.
+
+    Args:
+        design_name(str): Design name.
+        root_directory(str | pathlib.Path): Design directory.
+
+    Returns:
+        configuration(dict): Configuration dictionary.
+    """
+    config_json_exists = check_config_json_exists_openlane_v1(design_name)
+    if config_json_exists:
+        design_directory = get_design_directory_from_root_openlane_v1(
+            design_name=design_name, root_directory=root_directory
+        )
+        with open(str((design_directory / "config.json").resolve()), "r") as read_file:
+            configuration = json.load(read_file)
+        return configuration
+    else:
+        raise ValueError(
+            "Configuration file for design: "
+            + design_name
+            + " is not found in "
+            + str(root_directory / "designs" / design_name)
+        )
+
+
 def write_configuration_openlane_v1(
     configuration: dict,
     design_directory: str | pathlib.Path,
 ) -> None:
     """
     Writes a `config.json` onto a `design_directory`
 
@@ -189,11 +316,15 @@
         json.dump(configuration, write_file, indent=4)
 
 
 __all__ = [
     "check_config_json_exists_openlane_v1",
     "check_design_exists_openlane_v1",
     "configure_and_run_design_openlane_v1",
+    "configure_parametric_designs_openlane_v1",
     "configure_flow_script_openlane_v1",
+    "create_parametric_designs_openlane_v1",
+    "get_design_directory_from_root_openlane_v1",
     "get_latest_version_root_openlane_v1",
+    "read_configuration_openlane_v1",
     "write_configuration_openlane_v1",
 ]
```

### Comparing `piel-0.0.29/piel/openlane/v2.py` & `piel-0.0.30/piel/openlane/v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/piel/parametric.py` & `piel-0.0.30/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.29/piel.egg-info/PKG-INFO` & `piel-0.0.30/piel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.29
+Version: 0.0.30
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# `piel` - Photonic and Integrated ELectronic system design
+# `piel` - Photonic and Integrated ELectronic tools
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -39,31 +39,22 @@
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
 ## Dependency Toolset
 This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some individual tools already integrated are:
-* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
-  electronic logic and outputs performance parameters of the implemented circuitry.
+* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 
 Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
 - Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
 - `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-
-
-=======
-History
-=======
-
-0.0.1 (2023-06-10)
-------------------
-
-* First release on PyPI.
```

### Comparing `piel-0.0.29/setup.py` & `piel-0.0.30/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     history = history_file.read()
 
 requirements = [
     "Click>=7.0",
     "openlane",
     "cocotb",
     "gdsfactory",
+    "pandas",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
@@ -55,18 +56,18 @@
             "pandoc",
             "flake8",
         ]
     },
     install_requires=requirements,
     license="MIT license",
     long_description_content_type="text/markdown",
-    long_description=readme + "\n\n" + history,
+    long_description=readme,
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.29",
+    version="0.0.30",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.29/tests/test_piel.py` & `piel-0.0.30/tests/test_piel.py`

 * *Files identical despite different names*

