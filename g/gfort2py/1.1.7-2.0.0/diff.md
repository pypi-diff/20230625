# Comparing `tmp/gfort2py-1.1.7.tar.gz` & `tmp/gfort2py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfort2py-1.1.7.tar", last modified: Sun Mar 20 15:46:24 2022, max compression
+gzip compressed data, was "gfort2py-2.0.0.tar", last modified: Sun Jun 25 11:02:05 2023, max compression
```

## Comparing `gfort2py-1.1.7.tar` & `gfort2py-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,88 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.978414 gfort2py-1.1.7/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1107 2022-03-20 14:30:57.000000 gfort2py-1.1.7/.gitignore
--rw-rw-r--   0 rob       (1000) rob       (1000)     2940 2022-03-20 14:30:57.000000 gfort2py-1.1.7/.travis.yml
--rw-rw-r--   0 rob       (1000) rob       (1000)     5229 2022-03-20 15:42:09.000000 gfort2py-1.1.7/CODE_OF_CONDUCT.md
--rw-rw-r--   0 rob       (1000) rob       (1000)    15219 2019-07-20 14:21:29.000000 gfort2py-1.1.7/COPYING.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      191 2022-03-20 14:30:57.000000 gfort2py-1.1.7/MANIFEST.in
--rw-rw-r--   0 rob       (1000) rob       (1000)      958 2022-03-20 15:46:24.978414 gfort2py-1.1.7/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     7382 2022-03-20 15:46:21.000000 gfort2py-1.1.7/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.973414 gfort2py-1.1.7/extras/
--rw-rw-r--   0 rob       (1000) rob       (1000)     6816 2019-07-20 14:21:29.000000 gfort2py-1.1.7/extras/py.supp
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.975414 gfort2py-1.1.7/gfort2py/
--rw-rw-r--   0 rob       (1000) rob       (1000)       97 2022-01-08 20:42:32.000000 gfort2py-1.1.7/gfort2py/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    23976 2022-03-20 15:42:09.000000 gfort2py-1.1.7/gfort2py/arrays.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1981 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/cmplx.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       73 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/errors.py
--rw-rw-r--   0 rob       (1000) rob       (1000)   192810 2022-03-20 15:34:26.000000 gfort2py-1.1.7/gfort2py/fnumpy.c
--rw-rw-r--   0 rob       (1000) rob       (1000)      370 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/fnumpy.pyx
--rw-rw-r--   0 rob       (1000) rob       (1000)    11797 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/functions.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6784 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/gfort2py.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.977414 gfort2py-1.1.7/gfort2py/parseMod/
--rw-rw-r--   0 rob       (1000) rob       (1000)       82 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       80 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/makefile
--rw-rw-r--   0 rob       (1000) rob       (1000)     1803 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/parseMod.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      262 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/parseMod14.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1833 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/parseMod15.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    17727 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/parseModCommon.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1298 2022-03-20 15:42:09.000000 gfort2py-1.1.7/gfort2py/parseMod/utils.py
--rw-rw-r--   0 rob       (1000) rob       (1000)   150002 2022-03-20 15:34:26.000000 gfort2py-1.1.7/gfort2py/parseMod/utils_cpython.c
--rw-rw-r--   0 rob       (1000) rob       (1000)     1130 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/parseMod/utils_cpython.pyx
--rw-rw-r--   0 rob       (1000) rob       (1000)     3101 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/strings.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     9117 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/types.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      236 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/utils.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    11726 2022-03-20 14:30:57.000000 gfort2py-1.1.7/gfort2py/var.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       22 2022-03-20 15:46:21.000000 gfort2py-1.1.7/gfort2py/version.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.975414 gfort2py-1.1.7/gfort2py.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      958 2022-03-20 15:46:24.000000 gfort2py-1.1.7/gfort2py.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      976 2022-03-20 15:46:24.000000 gfort2py-1.1.7/gfort2py.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-03-20 15:46:24.000000 gfort2py-1.1.7/gfort2py.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       24 2022-03-20 15:46:24.000000 gfort2py-1.1.7/gfort2py.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       15 2022-03-20 15:46:24.000000 gfort2py-1.1.7/gfort2py.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)      634 2022-03-20 15:42:56.000000 gfort2py-1.1.7/new_release.sh
--rw-rw-r--   0 rob       (1000) rob       (1000)       17 2022-03-20 14:30:57.000000 gfort2py-1.1.7/requirements.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2022-03-20 15:46:24.978414 gfort2py-1.1.7/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1791 2022-03-20 15:42:09.000000 gfort2py-1.1.7/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-03-20 15:46:24.977414 gfort2py-1.1.7/tests/
--rw-rw-r--   0 rob       (1000) rob       (1000)      317 2022-03-20 15:42:09.000000 gfort2py-1.1.7/tests/Makefile
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2021-11-01 10:24:39.000000 gfort2py-1.1.7/tests/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      685 2022-03-20 15:42:09.000000 gfort2py-1.1.7/tests/conftest.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    28253 2022-03-20 15:42:09.000000 gfort2py-1.1.7/tests/gfort2py_test.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      662 2020-12-21 16:35:19.000000 gfort2py-1.1.7/tests/memory_leak.f90
--rw-rw-r--   0 rob       (1000) rob       (1000)     1796 2021-12-07 09:13:47.000000 gfort2py-1.1.7/tests/memory_leak.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      481 2022-03-20 14:30:57.000000 gfort2py-1.1.7/tests/test2.f90
--rw-rw-r--   0 rob       (1000) rob       (1000)    28381 2022-03-20 14:30:57.000000 gfort2py-1.1.7/tests/test_mod.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.370244 gfort2py-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.358244 gfort2py-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci_old.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/coveralls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-25 11:01:49.000000 gfort2py-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-25 11:01:49.000000 gfort2py-2.0.0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 11:01:49.000000 gfort2py-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-25 11:02:05.370244 gfort2py-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-25 11:01:49.000000 gfort2py-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-25 11:01:49.000000 gfort2py-2.0.0/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/fortranabi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/mod_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/testsuite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.366244 gfort2py-2.0.0/gfort2py/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fArrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fProc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fProcPtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fScalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fStrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fUnary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fVar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fVar_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/gfort2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21658 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/module_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.366244 gfort2py-2.0.0/gfort2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-25 11:01:49.000000 gfort2py-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 11:01:49.000000 gfort2py-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 11:01:49.000000 gfort2py-2.0.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 11:02:05.370244 gfort2py-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:01:49.000000 gfort2py-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.370244 gfort2py-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/basic.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/complex.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/complex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dummy_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dummy_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/elemental.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/explicit_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/explicit_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/interface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/namelist.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/oo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/oo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pdt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pdt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pointers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/proc_ptrs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/proc_ptrs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/strings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/strings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/template._f90
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tox.ini
```

### Comparing `gfort2py-1.1.7/.gitignore` & `gfort2py-2.0.0/.gitignore`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 # C extensions
 *.so
 *.c
 *.s
 tests/tester
 tests/*.f90.*
+tests/*.gz.*
+tests/*.gz
+*.smod
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
@@ -93,7 +96,11 @@
 .ropeproject
 
 
 *.mod
 *.o
 *.fpy
 *.pickle
+.vscode/*
+
+docs/build
+docs/source/_build
```

### Comparing `gfort2py-1.1.7/CODE_OF_CONDUCT.md` & `gfort2py-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gfort2py-1.1.7/COPYING.txt` & `gfort2py-2.0.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `gfort2py-1.1.7/README.md` & `gfort2py-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,176 @@
-![Build status](https://travis-ci.org/rjfarmer/gfort2py.svg?branch=master)
-[![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=master)](https://coveralls.io/github/rjfarmer/gfort2py?branch=master)
+[![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
 
 
 
 # gfort2py
-Library to allow calling fortran code from python. Requires gfortran>=5.3.1, Works with both python 2.7 and python 3.*
+Library to allow calling Fortran code from Python. Requires gfortran>=8.0, Works with python >= 3.7
 
-Current stable version is 1.1.7
+The current stable version is 1.1.7
 
 ## Build
 ````bash
-ipython3 setup.py install --user
+pip3 install -r requirements.txt
+python3 setup.py install --user
 ````
 
 or install via pip
 ````bash
-pip install --user gfort2py
+python -m pip install --upgrade --user gfort2py
 ````
 
-## Why use this over other fortran to python translators?
+## Why use this over other Fortran to Python translators?
 
-gfort2py use gfortran .mod files to translate your fortran code's ABI to python 
-compatible types using python's ctype library. The advantage here is that it can
-(in principle) handle anything the compiler can compile. gfort2py is almost entirely
-python and there are no changes needed to your fortran source code (some changes in the build
-process may be needed, as gfort2py needs your code compiled as a shared library). Disadvantage
-means we are tied to gfortran and can't support other compilers and may break when
-gfortran updates its .mod file format, though this happens rarely.
+gfort2py has three main aims:
 
+1. Make it trivially easy to call Fortran code from Python
+2. Minimise the number of changes needed in the Fortran code to make this work.
+3. Support as many Fortran features as possible.
+
+We achieve this by tightly coupling the code to the gfortran compiler, by doing so we can easily embed assumptions about how advanced Fortran features work which makes development easier and minimises the number of changes needed on the Fortran side. 
+
+gfort2py use the gfortran ``mod`` files to translate your Fortran code's ABI to Python-compatible types using Python's ctype library.
+By using the ``mod`` file we can determine the call signature of all procedures, components of derived types, and the size and shapes of all module-level variables. As long as your code is inside a Fortran module, no other changes are needed to your Fortran code.
+
+The downside to this approach is that we are tightly tied to gfortran's ABI, which means we can not support other non-gfortran compilers and we do not support all versions of gfortran. When gfortran next breaks its ABI (which happens rarely, the last break was gfortran 8) we will re-evaluate our supported gfortran versions.
 
 ## Using
 ### Fortran side
-Compile code with -fPIC and -shared as options, then link togethter as a shared lib at the end
+Your Fortran code must be inside a module and then compiled as a shared library.
 
+On linux: 
 ````bash
 gfortran -fPIC -shared -c file.f90
 gfortran -fPIC -shared -o libfile file.f90
 ````
-If your code comes as  program that does everything, then just turn the program into a function call inside a module,
+
+On MacOS: 
+````bash
+gfortran -dynamiclib -c file.f90
+gfortran -dynamiclib -o libfile file.f90
+````
+
+If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
-shared libraries you will need to set LD_LIBRARY_PATH environment variable, and its also recommended is to run chrpath on the 
+shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
 shared libraries so you can access them from anywhere.
 
 ### Python side
 ````python
 
 import gfort2py as gf
 
-SHARED_LIB_NAME='./test_mod.so'
+SHARED_LIB_NAME=f'./test_mod.{gf.lib_ext()}' # Handle whether on Linux or Mac
 MOD_FILE_NAME='tester.mod'
 
 x=gf.fFort(SHARED_LIB_NAME,MOD_FILE_NAME)
 
 ````
 
-x now contains all variables, parameters and functions from the module (tab completable). 
+``x`` now contains all variables, parameters and procedures from the module (tab completable). 
 
 ### Functions
 ````python
 y = x.func_name(a,b,c)
 ````
 
-Will call the fortran function with variables a,b,c and will return the result in y,
-subroutines will return a dict (possibly empty) with any intent out, inout or undefined intent variables.
+Will call the Fortran function with variables ``a,b,c`` and returns the result in ``y``.
 
-Optional arguments are handled by not passing anything for that item (python side), but
-they must be at the end of the argument list (on the fortran side)
+``y`` will be  named tuple which contains (result, args). Where result is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
 
-Array arguments must pass a numpy array, either pre filled (if the array is intent(in)) or made with zeros
-if the array is intent out or allocatable.
 
 ### Variables
 
 ````python
 x.some_var = 1
 ````
 
-Sets a module variable to 1, will attempt to coerce it to the fortran type
+Sets a module variable to 1, will attempt to coerce it to the Fortran type
 
 ````python
 x.some_var
-x.some_var.get()
 ````
 
-First will print the value in some_var while get() will return the value
+Will return a Python object 
+
+
+Optional arguments that are not present should be passed as a Python ``None``.
+
 
 ### Arrays
 
-Remember that fortran by default has 1-based array numbering while numpy
+Arrays should be passed as a NumPy array of the correct size and shape.
+
+
+Remember that Fortran by default has 1-based array numbering while Numpy
 is 0-based.
 
 
+If a procedure expects an unallocated array, then pass None as the argument, otherwise pass an array of the correct shape.
+
 ### Derived types
 
 Derived types can be set with a dict 
 ````python
 x.my_dt={'x':1,'y':'abc'}
 ````
-And return a dict when the .get() method is called, unless you pass
-copy=False to the get call in which case a ctype is returned (and fields
-access via the dot interface)
 
 ````python
-y=x.my_dt.get(copy=False)
-y.x
-y.y
+y=x.my_dt
+y['x']
+y['y']
 ````
 If the derived type contains another derived type then you can set a dict in a dict
 
 ````python
 x.my_dt={'x':1,'y':{'a':1}}
 ````
 
-This can then be accessed either via:
+When setting the components of a derived type you do not need to specify
+all of them at the same time.
 
-````python
-x.my_dt.y
+
+If you have an array of derived types
+
+````fortran
+type(my_type), dimension(5) :: my_dt
+type(my_type), dimension(5,5) :: my_dt2
 ````
 
-To get a dict back, or:
+Elements can be accessed via an index:
 
 ````python
-x.my_dt.y.a
-x.my_dt['a']
+x.my_dt[0]['x']
+x.my_dt2[0,0]['x']
 ````
 
-To get a single value.
+You can only access one component at a time (i.e no striding [:]). Allocatable derived types are not yet supported.
 
-When setting the components of a derived type you do not need to specify
-all of them at the same time.
+Derived types that are dummy arguments to a procedure are returned as a ``fDT`` type. This is a dict-like object where the components
+can only be accessed via the item interface ``['x']`` and not as attributes ``.x``.  This was done so that we do not have a name collision
+between Python functions (``keys``, ``items`` etc) and any Fortran-derived type components.
+
+You can pass a ``fDT`` as an argument to a procedure.
 
 
 ## Testing
 
 ````bash
-ipython3 setup.py test
+pytest
+````
+
+or 
+
+````bash
+tox
 ````
 
 To run unit tests
 
 ## Things that work
 
 ### Module variables
@@ -153,121 +181,157 @@
 - [x] Explicit size arrays
 - [X] Complex numbers (Scalar and parameters)
 - [x] Getting a pointer
 - [x] Getting the value of a pointer
 - [x] Allocatable arrays
 - [x] Derived types
 - [x] Nested derived types
-- [ ] Arrays of derived types
-- [ ] Functions inside derived types
-- [ ] Arrays with dimension (:) (pointer, allocatable) inside derived types (it doesn't break if their there, but you cant access them easily)
+- [X] Explicit Arrays of derived types
+- [ ] Allocatable Arrays of derived types
+- [ ] Procedure pointers inside derived types
+- [x] Derived types with dimension(:) array components (pointer, allocatable, target)
+- [x] Allocatable strings (partial)
+- [x] Explicit Arrays of strings
+- [x] Allocatable arrays of strings
 - [ ] Classes
 - [ ] Abstract interfaces
-- [x] Common blocks (parital)
-- [x] Equivalences 
+- [x] Common blocks (partial)
+- [ ] Equivalences 
 - [ ] Namelists
 - [ ] Quad precision variables
+- [ ] function overloading 
 
-### Functions/subroutines
+### Procedures
 
 - [X] Basic calling (no arguments)
 - [x] Argument passing (scalars)
 - [x] Argument passing (strings)
 - [X] Argument passing (explicit arrays)
 - [x] Argument passing (assumed size arrays)
 - [x] Argument passing (assumed shape arrays)
 - [x] Argument passing (allocatable arrays)
 - [x] Argument passing (derived types)
 - [x] Argument intents (in, out, inout and none)
-- [x] Passing characters
-- [x] Pointer Arguments 
+- [x] Passing characters of fixed size (len=10 or len=* etc)
+- [x] Functions that return a character as their result
+- [x] Allocatable strings (Only for things that do not get altered inside the procedure)
+- [x] Explicit arrays of strings
+- [x] Allocatable arrays of strings
+- [x] Pointer arguments 
 - [x] Optional arguments
-- [ ] Keyword arguments
+- [x] Value arguments
+- [x] Keyword arguments
 - [ ] Generic/Elemental functions
-- [x] Functions as an argument
+- [ ] Functions as an argument
+- [ ] Unary operations (arguments that involve an expression to evaluate like dimension(n+1))
 
 ### Accessing common block elements
 
-Theres no direct way to access the common block elements, but if you declare the the common block as a module variable you may acccess the elements by their name:
+There's no direct way to access the common block elements, but if you declare the common block as a module variable you may access the elements by their name:
 
 
 ````fortran
 module my_mod
-	implicit none
-	
-	integer :: a,b,c
-	common /comm1/ a,b,c
-	
+    implicit none
+    
+    integer :: a,b,c
+    common /comm1/ a,b,c
+    
 ````
 
 Elements in the common block can thus be accessed as:
 
 ````python
 x.a
 x.b
 x.c
 ````
 
-### Functions pointers:
+<!-- ### Procedure pointers:
 
-#### Functions as arguments
+#### Procedures as arguments
 
 Consider:
 
 ````fortran
 integer function my_func(func_arg)
-	integer func_arg
-	
-	my_func = func_arg(5)
+    integer func_arg
+    
+    my_func = func_arg(5)
 end function my_func
-	
+    
 ````
 
 Assuming that func_arg is another fortran function then we can call my_func as:
 
 
 ````python
-
-x.my_func('func_arg') # With a string of the name of the argument of the function
-#or
-x.my_func(x.func_arg) # With the functin itself
+x.my_func(x.func_arg) # With the function itself
 ````
 
-Its left the the user to make sure that the function func_arg takes the correct inputs and returns the correct output
+It is left the the user to make sure that the function func_arg takes the correct inputs and returns the correct output -->
 
 
-If instead you want func_arg to be a python function then things are a little different:
+<!-- Needs readding once fixed
+#### Procedure pointers
 
-````python
-def my_py_func(x): # Python function that will be func_arg
-	xv=x.contents.value # Values are passed by reference, this works for ints, floats. Characters, arrays and derived types are more complicated.
-	return 10*xv
+Consider a procedure like:
+
+````fortran
+procedure(my_func), pointer:: func_ptr => NULL()
+````
+
+This can be set similar to how we handle functions as arguments:
 
-# We must "pair" the python function with an existing fortran function that has the same inputs/oupts and return type.
-x.func_func_run.load() # This function call forces func_func_run to be initliazed without callling the function
-y = x.func_func_arg([my_py_func,'func_func_run']) # This "pairs" the python function with a fortran function that has been loaded
 
+````python
+x.func_ptr = x.func_arg # With the function itself
 ````
 
-#### Procedure pointers
+Its left the the user to make sure that the function func_arg takes the correct inputs and returns the correct output. If you have a function
+that accepts a function pointer then its the same as if the it just accepted a function argument
 
-Consider a prcoedure like:
+If func_ptr already points a a function at compile time:
 
 ````fortran
-procedure(my_func), pointer:: func_ptr => NULL()
+procedure(my_func), pointer:: func_ptr => my_func
+````
+
+You must still first set it to something
+
+````python
+x.func_ptr = x.func_arg # With the function itself
+```` -->
+
+## Accessing module file data
 
+For those wanting to explore the module file format, there is a routine ``mod_info`` available from the top-level ``gfort2py`` module:
+
+````
+module = gf.mod_info('file.mod')
 ````
 
-We can not at this time set func_ptr from python, instead it must be set by fortran. The func_ptr can however be called from python if set, if it has not been set
-then we raise ValueError.
+That will parse the mod file and convert it into an intermediate format inside ``module``.
 
-Its left to the user to enforce that the function has the correct interface
+Variables or procedures can be looked up via the item interface (I also recommend using pprint for easier viewing):
 
+````
+from pprint import pprint
+
+pprint(module['a_variable'])
+````
+
+Accessing the list of all available components can be had via ``module.keys()``.
 
 ## Contributing
 
-Pull requests should target the maint branch for fixing issues, please check the test suite
-passes before sending a pull request.
-Maint will be periodically merged with master for new releases, master should never have 
-a broken test suite.
+Bug reports are of course welcome and PR's should target the main branch.
+
+For those wanting to get more involved, adding Fortran examples to the test suite of currently untested or unsupported features would be helpful. Bonus points if you also provide a Python test case (that can be marked ``@pytest.mark.skip`` if it does not work) that demonstrates the proposed interface to the new Fortran feature. Features with test cases will move higher in the order of things I add to the code.
+
+See [how to write a test case](tests/README.md) for details on how to write test cases.
+
+For those wanting to go further and add the new feature themselves open a bug report and we can chat about what needs doing.
+
+
```

### Comparing `gfort2py-1.1.7/gfort2py/parseMod/parseModCommon.py` & `gfort2py-2.0.0/gfort2py/module_parse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,579 +1,835 @@
 # SPDX-License-Identifier: GPL-2.0+
 
-from __future__ import print_function
-try:
-    import __builtin__ 
-except ImportError:
-    import builtins as __builtin__
+from pyparsing import OneOrMore, nestedExpr
+from dataclasses import dataclass
+import numpy as np
 import gzip
-import ctypes
-import os
-import pickle
 import sys
-import re
-import subprocess
-import numpy as np
-import multiprocessing as mp
 
-from .utils import *
-from .utils_cpython import *
+import pprint
 
-PARALLEL = False
+import typing as t
 
-class parseModBase(object):
-    def __init__(self,data,filename,res,PYFILE_VERSION):
-        self.data = data
-        self.filename = filename
-        self.mod_data = res
-        self.PYFILE_VERSION = PYFILE_VERSION
-        
-        self.funcs={}
-        self.func_ptrs={}
-        self.mod_vars={}
-        self.param={}
-        self.dt_defs={}
-        self.dt_defines=[]
-        self._unpacked=False
-    
-    def processData(self):
-        self.data = split_brackets(self.data)
-        
-        #Store the split data once:
-        _t=[]
-        for i in self.data:
-            _t.append(split_brackets(i.strip(),remove_b=True))
-        self.data = _t
-        
-    
-        self.parseAllIntrinsic()
-        self.parseAllOperator()
-        self.parseAllDTDefines()
-        self.parseAllCommon()
-        self.parseAllEqv()
-        self.parseAllNameSymbols()
-        self.parseAllSymbols()
-        
-        self.matchFuncArgs()
-        # Must match func ptrs after function args so we get all the inputs/outputs correct
-        self.matchFuncPtrs()
-        
-        self.data=None
-        
-        self.unpackData()
-    
-    def save(self,output):
-        if not self._unpacked:
-            self.unpackData()
-        
-        self.pickler(output, self.PYFILE_VERSION, 
-                    self.mod_data, self.mod_vars, self.param, 
-                    self.funcs, self.dt_defs, self.func_ptrs)
-    
-    
-    def pickler(self,filename, *args):   
-        with open(filename, 'wb') as f:
-            for i in args:
-                pickle.dump(i, f, protocol=2)
-            
-    def unpackData(self):
-        self._unpacked = True
-        
-        for key in self.all_symbols:
-            i = self.all_symbols[key]
-            if len(i):
-                try:
-                    name = i['name']
-                except KeyError:
-                    print(i)
-                    name = i['mangled_name']
-                if 'proc' in i and 'var' in i:
-                    self.func_ptrs[name] = i
-                elif 'proc' in i:
-                    self.funcs[name] = i
-                elif 'var' in i and 'func_arg' not in i:
-                    self.mod_vars[name] = i
-                elif 'param' in i:
-                    self.param[name] = i
-                elif 'dt_def' in i:
-                    self.dt_defs[name] = i
-                
-    def getUnpackedData(self):
-        if not self._unpacked:
-            self.unpackData()
-            
-        return  self.mod_data, self.mod_vars, self.param, self.funcs, self.dt_defs, self.func_ptrs
-    
-    def mangleName(self,item):
-        return '__' + item['module'] + '_MOD_' + item['name'].lower()
-        
-    def parseAllIntrinsic(self):
-        x = self.data[0]
-        #Remove the module header
-        #x = x[x.index("("):]
-        
-    def parseAllOperator(self):
-        x = self.data[1]
-        
-    def parseAllDTDefines(self):
-        # This isnt just dt names, its also the name and number(s) for 
-        # generic interfaces
-        x = self.data[2]
-        #x = split_brackets(x.strip(),remove_b=True) 
-        
-        for i in x:
-            i=i.replace("(","").replace(")",'').strip()
-            r={}
-            z = i.split()
-            r['name'] = z[0].lower().replace("'","")
-            r['module'] = z[1].replace("'","")
-            r['num'] = int(z[2])
-            if(len(z))> 3:
-                r['num_alts']=z[2:]
-            self.dt_defines.append(r)
-            
-            
-        # Find the dt's used by the module but not defined by the module,
-        # but its defintion is still copied in here
-        for symbol in self.data[6]:
-            try:
-                splitPoint = symbol.index("(")
-            except ValueError:
-                continue
-            info = symbol[splitPoint:].strip()
-            info = split_brackets(info)
-            type_line = info[0]
-            
-            if 'DERIVED ' in type_line:
-                num,name,module  =  symbol.split()[0:3]
-                if len(self.dt_defines)>0:
-                    found=False
-                    for i in self.dt_defines:
-                        if int(i['num']) == int(num):
-                            found=True
-                else:
-                    found = False
-                
-                if not found:
-                    self.dt_defines.append({'name':name,
-                                        'module':module.replace("'",""),
-                                        'num':num})
-    
-    def parseAllCommon(self):
-        x = self.data[3]
-        
-    def parseAllEqv(self):
-        x = self.data[4]
-    
-    def parseAllNameSymbols(self):
-        x = self.data[7]
-        x = x[0].split()
-        self.symbol_names = []
-        for i in range(len(x)//3):
-            self.symbol_names.append({'name':x[i*3],'num':x[i*3+2],'ambiguous_flag':bool(x[i*3+1])})
-        
-    
-    def parseAllSymbols(self):
-        split_data = self.data[6]
-        
-        # if PARALLEL:
-            # with mp.Pool() as pool:
-                # all_symbols = pool.map(self.parseSymbol,split_data)
-        # else:
-            # all_symbols = [self.parseSymbol(i) for i in split_data]
-        all_symbols = {}
-        for i in split_data:
-            x = self.parseSymbol(i)
-            if 'num' in x:
-                all_symbols[x['num']] = self.parseSymbol(i)
-            
-        self.all_symbols = all_symbols
-        
-    def parseSymbol(self,symbol):
-        symbol = symbol.strip()
-        #things to skip
-    
-        if ('__' in symbol or '(intrinsic)' in symbol or 
-            'INTRINSIC' in symbol or len(symbol)==0 or
-            ' RESULT' in symbol):
-            return {}
-    
-        r = {}
-        r['num'], r['name'],r['module'], _, r['parent_id']  =  symbol.split()[0:5]
-        
-        for i in ['num','name','module','parent_id']:
-            r[i]=r[i].lower().replace("'","")
-        
-        if len(r['name'])==0:
-            return {}
-        
-        ## things to left of '(' are basic info right of '(' contains detailed info
-        ## about the symbol  
-        splitPoint = symbol.index("(")
-        
-        info = symbol[splitPoint:].strip()
-        
-        
-        info = split_brackets(info)
-        r['info'] = info
-        type_line = info[0]
-        
-        
-        # need spaces on end of names as sometimes we have name-something etc
-        if 'VARIABLE ' in type_line or 'DUMMY ' in type_line:
-            if len(r['module'])>0:
-                r['var'] = self.parseVar(info)
-            else:
-                r['var'] = self.parseFuncArg(info)
-                r['func_arg']=True
-        elif 'PROCEDURE ' in type_line:
-            if 'GENERIC' in type_line:
-                pass #Uneeded
-                #r['dt_type'] = self.parseDTType(info)
-            elif 'PROC_POINTER' in type_line:
-                # prcoedure pointers treat as vars and funcs
-                r['var'] = self.parseVar(info)
-                r['proc'] = self.parseProc(info)
-                r['arg'] = []
-            else:
-                r['proc'] = self.parseProc(info)
-                r['arg']=[]
-        elif 'MODULE ' in type_line:
-            r['module_info'] = self.parseModule(info)
-        elif 'PARAMETER ' in type_line:
-            r['param'] = self.parseParam(info)
-        elif 'DERIVED ' in type_line:
-            #This definition of a dt 
-            r['dt_def'] = self.parseDT(info)
-        elif 'NAMELIST ' in type_line:
-            print("Skipping namelist "+r['name'])
+
+def string_clean(string):
+    if string is None:
+        return
+    if string.startswith("'") or string.startswith('"'):
+        string = string[1:]
+    if string.endswith("'") or string.endswith('"'):
+        string = string[:-1]
+
+    return string
+
+
+class VersionError(Exception):
+    pass
+
+
+class NotAnArrayError(Exception):
+    pass
+
+
+#################################
+
+
+@dataclass
+class s_item:
+    name: str
+    ambiguous: bool
+    id: int
+
+    def __post_init__(self):
+        self.name = string_clean(self.name)
+        self.ambiguous = self.ambiguous != "0"
+        self.id = int(self.id)
+
+
+class Summary:
+    def __init__(self, summ):
+        self._item_id = {}
+        self._item_name = {}
+
+        for i in range(0, len(summ), 3):
+            d = s_item(*summ[i : i + 3])
+            self._item_id[d.id] = d
+            self._item_name[d.name] = d
+
+    def __getitem__(self, key):
+        if isinstance(key, int):
+            return self._item_id[key]
+        if isinstance(key, str):
+            return self._item_name[key]
         else:
-            raise ValueError("Unknown object "+symbol)
-            
-        r['mangled_name'] = self.mangleName(r)
-            
-        r.pop('info')
-    
-        return r 
-        
-       
-    def parseVar(self,info):
-        res={}
-    
-        type_info = info[2]
-        symbol_info = info[0]
-        p, c, s=self.getVarType(type_info)
-        
-        res['pytype'] = p
-        res['ctype'] = c
-        res['bytes'] = s
-        
-        if res['pytype'] == 'str':
-            res['length'] = self.getStrLen(info)
-        
-        if 'DIMENSION' in symbol_info:
-            #Array
-            res['array'] = self.processArray(info)
-        if 'DERIVED' in type_info:
-            #Both dts but sometimes the definition moves
-            res['dt'] = self.processDTVar(info)
-            
-        res['optional']=False
-        if 'POINTER' in symbol_info:
-            res['pointer']=True
-        if 'TARGET' in symbol_info:
-            res['target']=True
-        if 'OPTIONAL' in symbol_info:
-            res['optional']=True
-        if 'DUMMY' in symbol_info:
-            res['intent'] = self.parseIntent(symbol_info)
-        if 'DUMMY-PROC' in symbol_info:
-            res['is_func'] = True
-            
-        if 'PROC_POINTER' in symbol_info:
-            res['proc_ptr_id'] = type_info.split()[2]
-    
-        return res
-        
-    def parseProc(self,info):
-        res={}
-        type_info = info[2]
-        
-        if 'FUNCTION ' in info[0]:        
-            p, c, s=self.getVarType(type_info)
+            raise TypeError(f"Dont understand type of {key}")
+
+    def keys(self):
+        return list(self._item_id.keys()) + list(self._item_name.keys())
+
+    def __contains__(self, key):
+        if isinstance(key, int):
+            return key in self._item_id
+        if isinstance(key, str):
+            return key in self._item_name
         else:
-            p = None
-            c = None
-            s = None
-            
-        res['pytype'] = p
-        res['ctype'] = c
-        res['bytes'] = s
-        
-        x=info[3][info[3].index("("):]
-        res['arg_nums']=x.replace("(","").replace(")","").split()
-        
-        if 'SUBROUTINE' in info[0]:
-            res['sub']=True
+            raise TypeError(f"Dont understand type of {key}")
+
+    def names(self):
+        return self._item_name.keys()
+
+
+#################################
+
+
+@dataclass
+class c_item:
+    name: str
+    id: int
+    saved_flag: bool
+    _unknown: int
+    _unknown2: str
+
+    def __post_init__(self):
+        self.name = string_clean(self.name)
+        self.id = int(self.id)
+        self.saved_flag = int(self.saved_flag)
+        self._unknown = int(self._unknown)
+        self._unknown2 = string_clean(self._unknown2)
+
+
+#################################
+
+
+@dataclass(init=False)
+class generics:
+    name: str = ""
+    module: str = ""
+    id: t.List[int] = -1
+
+    def __init__(self, *args):
+        self.name = string_clean(args[0])
+        self.module = string_clean(args[1])
+        self.id = []
+        for i in args[2:]:
+            self.id.append(int(i))
+
+
+#################################
+
+
+def hextofloat(s):
+    # Given hex like parameter '0.12decde@9' returns 5065465344.0
+    man, exp = s.split("@")
+    exp = int(exp)
+    decimal = man.index(".")
+    negative = man[0] == "-"
+    man = man[decimal + 1 :]
+    man = man.ljust(exp, "0")
+    man = man[:exp] + "." + man[exp:]
+    man = man + "P0"
+    if negative:
+        man = "-" + man
+    return float.fromhex(man)
+
+
+#####################################
+
+
+def print_args(x):
+    print()
+    for i in x:
+        print(i)
+    print()
+
+
+class utils:
+    def shape(self):
+        if self.is_array():
+            return self.sym.array_spec.pyshape
         else:
-            res['sub']=False
-        
-        #Return value
-        res['ret'] = self.parseVar(info)
-        
-        func_args = info[3].split()
-        res['func_arg_id'] = int(func_args[0])
-        
-        if 'ABSTRACT 'in type_info:
-            res={}
-        
-        
-        return res
-        
-    def parseModule(self,info):
-        res={}
-        type_info = info[2]
-        return res
-        
-    def parseDT(self,info):
-        res={}
-        res['arg']=[]
-        
-        e = split_brackets(info[1].strip())
-        
-        for i in e:
-            #Remove whitespace and the first and last bracket
-            i=i.strip()[1:-1]
-            dtEl={}
-            dtEl['num'], dtEl['name'] = i.split()[0:2]
-            dtEl['name'] = dtEl['name'].lower().replace("'","")
-            info_el = split_brackets(i[i.index("(")-1:],remove_b=False)
-            #Re-order to be the same as everything else
-            newL = [info_el[2],'()',info_el[0],'()',info_el[1]]
-            dtEl['var'] = self.parseVar(newL)
-            #Fix size 
-            if 'dt' in dtEl['var']:
-                dtEl['var']['bytes'] = ctypes.sizeof(ctypes.c_void_p)
-            res['arg'].append(dtEl)
-            
-        
-        return res
-        
-    def parseFuncArg(self,info):
-        r=self.parseVar(info)
-        return r
-        
-    def parseParam(self,info):
-        res={}
-        
-        type_info = info[2]
-        value = info[4]
-        
-        p, c, s=self.getVarType(type_info)
-        
-        res['pytype'] = p
-        res['ctype'] = c
-        res['bytes'] = s
-        
-        res['value']=self.getParamValue(value,res['pytype'])
-        
-        res['array']=False
-        if 'ARRAY' in value:
-            res['array']=True
-        
-        return res
-    
-    
-    def getVarType(self,x):
-        x=x.strip()
-        if x.startswith('('):
-            x=x[1:].strip()
-       
-        x = x.split()
-        size = x[1]
-        pytype, ctype = self.getTypes(x[0],size)
-        
-        return pytype, ctype, size
-        
-    def getParamValue(self,x,typ):
-        if 'ARRAY' in x:
-            x = split_brackets(x.strip())
-            arrLen = int(''.join(c for c in x[-1] if c not in "'()"))
-            x2 = split_brackets(x[1][x[1].index("("):])
-            listParam = [y.split("'")[-2] for y in x2]
-            p = [self.parseSingleParam(y,typ) for y in listParam]
+            raise NotAnArrayError("Not an array")
+
+    def dtype(self):
+        t = self.type()
+        k = int(self.kind())
+
+        if t == "INTEGER" or t == "LOGICAL":
+            if k == 4:
+                return "i4"
+            elif k == 8:
+                return "i8"
+        elif t == "REAL":
+            if k == 4:
+                return "f4"
+            elif k == 8:
+                return "f8"
+        elif t == "COMPLEX":
+            if k == 4:
+                return "c4"
+            elif k == 8:
+                return "c8"
+        elif t == "CHARACTER":
+            return f"S{self.strlen.value}"
+
+        raise NotImplementedError(f"Object of type {t} and kind {k} not supported yet")
+
+    def type(self):
+        return self.sym.ts.type
+
+    def ref(self):
+        return self.head.id
+
+    def flavor(self):
+        return self.sym.attr.flavor
+
+    def kind(self):
+        return self.sym.ts.kind
+
+    def is_pointer(self):
+        return "POINTER" in self.sym.attr.attributes
+
+    def is_parameter(self):
+        return self.flavor() == "PARAMETER"
+
+    def is_value(self):
+        return "VALUE" in self.sym.attr.attributes
+
+    def is_optional(self):
+        return "OPTIONAL" in self.sym.attr.attributes
+
+    def is_optional_value(self):
+        return self.is_optional() and self.is_value()
+
+    def is_char(self):
+        return self.type() == "CHARACTER"
+
+    def is_variable(self):
+        return self.flavor() == "VARIABLE"
+
+    def is_procedure(self):
+        return self.flavor() == "PROCEDURE"
+
+    def is_proc_pointer(self):
+        return "PROC_POINTER" in self.sym.attr.attributes
+
+    def is_logical(self):
+        return self.sym.ts.type == "LOGICAL"
+
+    def is_complex(self):
+        return self.sym.ts.type == "COMPLEX"
+
+    def is_subroutine(self):
+        return self.sym.sym_ref.ref == 0
+
+    def is_function(self):
+        return self.sym.sym_ref.ref != 0
+
+    def is_array(self):
+        return "DIMENSION" in self.sym.attr.attributes
+
+    def is_always_explicit(self):
+        return "ALWAYS_EXPLICIT" in self.sym.attr.attributes
+
+    def is_dummy(self):
+        return "DUMMY" in self.sym.attr.attributes
+
+    def is_allocatable(self):
+        return "ALLOCATABLE" in self.sym.attr.attributes
+
+    def needs_array_desc(self):
+        return self.is_dummy() or self.is_allocatable() or self.is_always_explicit()
+
+    def not_a_pointer(self):
+        return (
+            self.needs_array_desc()
+            and self.is_array()
+            and not self.is_assumed_shape()
+            and not self.is_assumed_size()
+        )
+
+    def is_explicit(self):
+        return (
+            self.sym.array_spec.array_type == "EXPLICIT"
+            and not self.is_always_explicit()
+        )
+
+    def is_assumed_size(self):
+        return self.sym.array_spec.array_type == "ASSUMED_SIZE"
+
+    def is_assumed_shape(self):
+        return self.sym.array_spec.array_type == "ASSUMED_SHAPE"
+
+    def is_deferred_len(self):
+        # Only needed for things that need an extra function argument for their length
+        if self.is_char():
+            try:
+                self.sym.ts.charlen.value
+                return False
+            except AttributeError:
+                return True
+        elif self.is_array():
+            return self.is_assumed_size()
+
+        return False
+
+    def is_derived(self):
+        return self.sym.ts.type == "DERIVED"
+
+    def is_pdt_def(self):
+        return "PDT_TEMPLATE" in self.sym.attr.attributes
+
+    @property
+    def strlen(self):
+        if self.is_char() and not self.is_deferred_len():
+            return self.sym.ts.charlen
+        raise AttributeError("Not a deferred length type")
+
+    @property
+    def ndim(self):
+        if self.is_array():
+            return self.sym.array_spec.rank
         else:
-            if 'COMPLEX' in x:
-                yy = x.split("'")
-                p = complex(self.parseSingleParam(yy[-4],'float'),
-                     self.parseSingleParam(yy[-2],'float'))
+            raise NotAnArrayError("Not an array")
+
+    @property
+    def size(self):
+        if self.is_array():
+            return np.prod(self.shape())
+        else:
+            raise NotAnArrayError("Not an array")
+
+    def value(self):
+        if self.is_parameter():
+            v = self.sym.parameter.value
+            if not self.is_array():
+                return v
             else:
-                y = x.split()[-1][:-1]
-                y = y.replace("'","")
-                p = self.parseSingleParam(y,typ) 
-            
-        return p
-    
-    def parseSingleParam(self,x,typ):
-        if '@' in x:
-            return hextofloat(x)
+                return np.array(v, dtype=self.dtype()).reshape(self.shape(), order="F")
         else:
-            return getattr(__builtin__, typ)(x)
-            
-    def processArray(self,info):
-        r = {}
-        if 'ALLOCATABLE' in info[0]:
-            r['atype'] = 'alloc'
-        elif 'POINTER' in info[0]:
-            r['atype'] = 'pointer'
-        elif 'ASSUMED_SHAPE' in info[4]:
-            r['atype'] = 'assumed_shape'
-        elif 'ASSUMED_SIZE' in info[4]:
-            r['atype'] = 'assumed_size'
-        elif 'CONSTANT' in info[4]:
-            r['shape'] = self.getBounds(info)
-            r['atype'] = 'explicit'
-        r['ndim'] = self.getNdims(info)
-        
-        p, c, s=self.getVarType(info[2])
-        
-        r['pytype'] = p
-        r['ctype'] = c
-        r['bytes'] = s
-        
-        return r
-        
-    def parseDTType(self, info):
-        #Nothing of any use in the info list
-        return None
-        
-    def getNdims(self, info):
-        return info[4].replace("(", "").strip().split()[0]
-    
-    def getBounds(self, info):
-        try:
-            # Horrible but easier than splitting the nested brackets
-            return [int(x) for x in info[4].split("'")[1:-1:2]]
-        except ValueError:
-            # Sometimes we cant know the size till run time
-            return -1
-    
-    def getStrLen(self, info):
-        # Horrible but easier than splitting the nested brackets
-        y=info[2].split("'")[1:-1:2]
-        if len(y)==0:
-            y=-1
+            raise AttributeError("Not a parameter")
+
+    def type_kind(self):
+        return self.type(), self.kind()
+
+    def return_arg(self):
+        if self.is_procedure():
+            return self.sym.sym_ref.ref
+        raise AttributeError("Not a procedure")
+
+    def args(self):
+        if self.is_procedure():
+            return self.sym.formal_arg
+        raise AttributeError("Not a procedure")
+
+    def dt_type(self):
+        return self.sym.ts.class_ref.ref
+
+    def dt_components(self):
+        return self.sym.comp
+
+
+@dataclass(init=False)
+class attribute:
+    flavor: str = ""
+    intent: str = ""
+    proc: str = ""
+    if_source: str = ""
+    save: str = ""
+    ext_attr: int = -1
+    extension: int = -1
+    attributes: t.Set[str] = None
+
+    def __init__(self, *args):
+        self.flavor = string_clean(args[0])
+        self.intent = string_clean(args[1])
+        self.proc = string_clean(args[2])
+        self.if_source = string_clean(args[3])
+        self.save = string_clean(args[4])
+        self.ext_attr = int(args[5])
+        self.extension = int(args[6])
+        self.attributes = set([string_clean(i) for i in args[7:]])
+
+
+@dataclass
+class namespace:
+    ref: int = -1
+
+    def __post_init__(self):
+        self.ref = symbol_ref(self.ref)
+
+
+@dataclass
+class header:
+    id: int
+    name: str  # If first letter is capitalized then its a dt
+    module: str
+    bindc: str
+    parent_id: int
+
+    def __post_init__(self):
+        self.id = int(self.id)
+        self.parent_id = int(self.parent_id)
+        self.name = string_clean(self.name)
+        self.module = string_clean(self.module)
+        self.bindc = len(string_clean(self.bindc)) > 0
+
+    @property
+    def mn_name(self):
+        if self.module:
+            return f"__{self.module}_MOD_{self.name}"
+
+
+@dataclass
+class symbol_ref:
+    ref: int = -1
+
+    def __post_init__(self):
+        self.ref = int(self.ref)
+
+
+@dataclass(init=False)
+class formal_arglist:
+    symbol: t.List[symbol_ref] = None
+
+    def __init__(self, *args):
+        self.symbol = []
+        for i in args:
+            self.symbol.append(symbol_ref(i))
+
+    def __len__(self):
+        return len(self.symbol)
+
+    def __iter__(self):
+        return iter(self.symbol)
+
+
+@dataclass(init=False)
+class typebound_proc:
+    name: str = ""
+    access: str = ""
+    overridable: str = ""
+    nopass: str = ""
+    is_generic: str = ""
+    ppc: str = ""
+    pass_arg: str = ""
+    pass_arg_num: symbol_ref = None
+    proc_ref: symbol_ref = None
+
+    def __init__(self, *args, **kwargs):
+        self.name = string_clean(args[0][0])
+        self.access = args[0][1][0]
+        self.overridable = args[0][1][1]
+        self.nopass = args[0][1][2]
+        self.is_generic = args[0][1][3]
+        self.ppc = args[0][1][4]
+        self.pass_arg = string_clean(args[0][1][5])
+        self.pass_arg_num = symbol_ref(args[0][1][6])
+
+        # TODO: Handle is_generic
+        self.proc_ref = symbol_ref(args[0][1][7][0])
+
+
+@dataclass(init=False)
+class derived_ns:
+    unknown1: str = None
+    proc: t.List[typebound_proc] = None
+
+    def __init__(self, *args, **kwargs):
+        if not len(args):
+            return
+        self.unknown1 = args[0]
+        self.proc = []
+        for i in args[1]:
+            self.proc.append(typebound_proc(i))
+
+
+@dataclass(init=False)
+class actual_arglist:
+    args: None
+    kwargs: None
+
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
+
+
+@dataclass(init=False)
+class typespec:
+    type: str = ""
+    kind: int = -1  # If class symbol_ref else kind
+    class_ref: symbol_ref = None  # If class/derived type symbol_ref else kind
+    interface: symbol_ref = None
+    is_c_interop: int = -1
+    is_iso_c: int = -1
+    type2: str = ""  # Repeat of type
+    charlen: int = -1  # If character
+    deferred_cl: bool = False  # if character and deferred length
+
+    def __init__(self, *args):
+        self.type = args[0]
+        if self.type == "CLASS" or self.type == "DERIVED":
+            self.class_ref = symbol_ref(args[1])
         else:
-            y=y[0]
-            if len(y) == 0:
-                y = -1
-        return int(y)
-    
-    def processDTVar(self,info):
-        # size is actually the dt definition number
-        p, c, s=self.getVarType(info[2])
-        return self.matchDtDef(int(s))
-    
-    
-    def getTypes(self,x,size):
-        if 'CHARACTER' in x:
-            pytype='str'
-            ctype='c_char_p'
-        elif 'INTEGER' in x:
-            pytype='int'
-            ctype=self.getCtypeIntSize(size)
-        elif 'REAL' in x:
-            pytype,ctype=self.getCtypeFloatSize(size)
-        elif 'COMPLEX' in x:
-            pytype,ctype=self.getCtypeFloatSize(size)
-            pytype='complex'
-        elif 'LOGICAL' in x:
-            pytype='bool'
-            ctype='c_int'
-        elif 'UNKNOWN' in x:
-            pytype='None'
-            ctype='c_void_p'
-        elif "DERIVED" in x:
-            pytype='dict'
-            ctype='c_void_p'
+            self.kind = int(args[1])
+
+        if len(args[2]):
+            self.interface = symbol_ref(args[2])
+
+        self.is_c_interop = bool(int(args[3]))
+        self.is_iso_c = bool(int(args[4]))
+        self.type2 = args[5]
+        try:
+            self.charlen = expression(
+                *args[6][0]
+            )  # TODO: might this need to be iterated for mulit-d strings?
+        except IndexError:
+            self.charlen = -1
+        try:
+            self.deferred_cl = args[7] == "DEFERRED_CL"
+        except (TypeError, IndexError):
+            self.deferred_cl = False
+
+
+@dataclass(init=False)
+class expression:
+    exp_type: str = ""
+    ts: typespec = None
+    rank: int = -1
+    _value: t.Any = None
+    _resolved_value: t.Any = None  # value may by a symbol_ref, so this is the value after resolving the reference
+    arglist: actual_arglist = None  # PDT's?
+    charlen: int = -1
+    unary_op: str = ""
+
+    def __init__(self, *args):
+        self.exp_type = args[0]
+        self.ts = typespec(*args[1])
+        self.rank = int(args[2])
+        self._resolved_value = None
+
+        if self.exp_type == "OP":
+            self._value = None
+            self.unary_op = args[3]
+            self.unary_args = [expression(*args[4]), expression(*args[5])]
+            self._unknown = args[6]  # What is this for?
+        elif self.exp_type == "FUNCTION":
+            self._value = symbol_ref(args[3])
+        elif self.exp_type == "CONSTANT":
+            if self.ts.type == "REAL":
+                self._value = hextofloat(string_clean(args[3]))
+            elif self.ts.type == "INTEGER":
+                self._value = int(string_clean(args[3]))
+            elif self.ts.type == "CHARACTER":
+                self.charlen = int(args[3])
+                self._value = string_clean(args[4])
+            elif self.ts.type == "COMPLEX":
+                self._value = complex(
+                    hextofloat(string_clean(args[3])), hextofloat(string_clean(args[4]))
+                )
+            else:
+                raise NotImplementedError(args)
+        elif self.exp_type == "VARIABLE":
+            self._value = symbol_ref(args[3])
+        elif self.exp_type == "SUBSTRING":
+            raise NotImplementedError(args)
+        elif self.exp_type == "ARRAY":
+            self._value = []
+            for i in args[3]:
+                self._value.append(
+                    expression(*i[0]).value
+                )  # Wheres the extra component comming from?
+        elif self.exp_type == "NULL":
+            self._value = args[3]
+        elif self.exp_type == "COMPCALL":
+            raise NotImplementedError(args)
+        elif self.exp_type == "PPC":
+            raise NotImplementedError(args)
         else:
-            pytype='None'
-            ctype='c_void_p'
-            #raise ValueError("Cant parse " + x)
-            
-        if 'PASS ' in x:
-            pytype='None'
-            ctype='c_void_p'
-            
-        return pytype,ctype
-        
-    def getCtypeIntSize(self,size):
-        size = int(size)
-        if size == ctypes.sizeof(ctypes.c_int):
-            res = 'c_int'
-        elif size == ctypes.sizeof(ctypes.c_int16):
-            res = 'c_int16'
-        elif size == ctypes.sizeof(ctypes.c_int32):
-            res = 'c_int32'
-        elif size == ctypes.sizeof(ctypes.c_int64):
-            res = 'c_int64'
-        elif size == ctypes.sizeof(ctypes.c_byte):
-            res = 'c_byte'
-        elif size == ctypes.sizeof(ctypes.c_short):
-            res = 'c_short'
+            raise AttributeError(f"Can't match {self.exp_type}")
+
+    @property
+    def value(self):
+        if self._resolved_value is not None:
+            return self._resolved_value
         else:
-            raise ValueError("Cant find suitable int for size " + str(size))
+            return self._value
+
+    @value.setter
+    def value(self, value):
+        self._resolved_value = value
+
+
+@dataclass(init=False)
+class arrayspec:
+    rank: int = -1
+    corank: int = -1
+    array_type: str = ""
+    lower: t.List[expression] = None
+    upper: t.List[expression] = None
+
+    def __init__(self, *args):
+        if not len(args):
+            return
+
+        self.rank = int(args[0])
+        self.corank = int(args[1])
+        self.array_type = args[2]
+        self.lower = []
+        self.upper = []
+        for i in range(self.rank + self.corank):
+            if len(args[3 + i * 2]):
+                self.lower.append(expression(*args[3 + i * 2]))
+            if len(args[4 + i * 2]):
+                self.upper.append(expression(*args[4 + i * 2]))
+
+    @property
+    def fshape(self):
+        res = []
+        for l, u in zip(self.lower, self.upper):
+            res.append([l.value, u.value])
+
+        return res
+
+    @property
+    def pyshape(self):
+        res = []
+        if self.lower is None:
+            return []
+
+        for l, u in zip(self.lower, self.upper):
+            res.append(u.value - l.value + 1)
+
         return res
-    
-    def getCtypeFloatSize(self,size):
-        size = int(size)
-        pytype='float'
-        if size == ctypes.sizeof(ctypes.c_float):
-            res = 'c_float'
-        elif size == ctypes.sizeof(ctypes.c_double):
-            res = 'c_double'
-        elif size == ctypes.sizeof(ctypes.c_long):
-            res = 'c_long'
-        elif size == ctypes.sizeof(ctypes.c_longdouble):
-            res = 'c_longdouble'
-            pytype='quad'
-        elif size == ctypes.sizeof(ctypes.c_longlong):
-            res = 'c_longdouble'
-            pytype='quad'
+
+    @property
+    def size(self):
+        return np.prod(self.pyshape)
+
+
+@dataclass(init=False)
+class component(utils):
+    id: int = -1
+    name: str = ""
+    ts: typespec = None
+    array_spec: arrayspec = None
+    expr: expression = None
+    actual_arg: actual_arglist = None
+    attr: attribute = None
+    access: str = ""
+    initializer: expression = None
+    proc_ptr: typebound_proc = None
+
+    def __init__(self, *args):
+        args = list(args)
+
+        self.id = int(args[0])
+        self.name = string_clean(args[1])
+        self.ts = typespec(*args[2])
+        self.array_spec = arrayspec(*args[3])
+        if len(args[4]):
+            self.expr = expression(*args[4])
+        if len(args[5]):
+            self.actual_arg = actual_arglist(*args[5])
+        self.attr = attribute(*args[6])
+        self.access = string_clean(args[7])
+
+        if self.name == "_final" or self.name == "_hash":
+            self.initializer = expression(*args[8])
+            _ = args.pop(8)
+
+        if not self.attr.proc == "UNKNOWN-PROC":
+            self.proc_ptr = typebound_proc(args[8])
+
+        # This lets us reuse the code for accessing symbols
+        # inside the parent utils class
+        self.sym = self
+
+
+@dataclass(init=False)
+class components:
+    comp: t.List[component] = None
+
+    def __init__(self, *args):
+        self.comp = []
+        for i in args:
+            self.comp.append(component(*i))
+
+    def __len__(self):
+        return len(self.comp)
+
+    def __iter__(self):
+        return iter(self.comp)
+
+
+@dataclass(init=False)
+class namelist:
+    sym_ref: t.List[symbol_ref] = None
+
+    def __init__(self, *args):
+        self.sym_ref = []
+        if len(args):
+            for i in args:
+                self.sym_ref.append(symbol_ref(i))
+
+
+@dataclass(init=False)
+class simd_dec:
+    args: None
+    kwargs: None
+
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
+
+
+@dataclass(init=False)
+class data:
+    attr: attribute
+    comp: components = None
+    comp_access: str = ""  # Only for DT's
+    ts: typespec = None
+    ns: namespace = None
+    common_link: symbol_ref = None
+    formal_arg: formal_arglist = None
+    parameter: expression = None  # If parameter
+    array_spec: arrayspec = None
+    sym_ref: symbol_ref = None
+    sym_ref_cray: symbol_ref = None  # If cray_pointer
+    derived: derived_ns = None
+    actual_arg: actual_arglist = None
+    nml: namelist = None
+    intrinsic: int = -1
+    intrinsic_symbol: int = -1
+    hash: int = -1
+    simd: simd_dec = None
+
+    def __init__(self, *args):
+        args = list(
+            args
+        )  # Do it this was as there are optional terms we may need to pop
+        self.attr = attribute(*args[0])
+        self.comp = components(*args[1])
+
+        if isinstance(args[2], str):
+            self.comp_access = args[2]
+            _ = args.pop(2)
+
+        self.ts = typespec(*args[2])
+        self.ns = namespace(args[3])
+        self.common_link = symbol_ref(args[4])
+        self.formal_arg = formal_arglist(*args[5])
+        if self.attr.flavor == "PARAMETER":
+            self.parameter = expression(*args[6])
+            _ = args.pop(6)
+        self.array_spec = arrayspec(*args[6])
+        if True:
+            self.sym_ref = symbol_ref(args[7])
         else:
-            raise ValueError("Cant find suitable float for size " + str(size))
-        return pytype,res
-    
-    def parseIntent(self,info):
-        value = False
-        if ' INOUT ' in info:
-            value = 'inout'
-        elif ' OUT ' in info:
-            value = 'out'
-        elif ' IN ' in info:
-            value = 'in'
-        elif ' UNKNOWN-INTENT ' in info:
-            value = 'na'
-        return value
-    
-    def matchDtDef(self,num):
-        for i in self.dt_defines:
-            if int(num) == int(i['num']):
-                return i
-        
-        print("Cant match dt definition "+str(num))
-    
-    def matchFuncArgs(self):
-        for key in self.all_symbols:
-            value = self.all_symbols[key]
-            if 'proc' in value:
-                self.all_symbols[key]['arg'] = []
-                for i in value['proc']['arg_nums']:
-                    self.all_symbols[key]['arg'].append(self.all_symbols[i])
-        
-    def matchFuncPtrs(self):
-        for key in self.all_symbols:
-            value = self.all_symbols[key]
-            if 'proc' in value and 'var' in value:
-                self.all_symbols[key]['arg'] = self.all_symbols[value['var']['proc_ptr_id']]['arg']
-                self.all_symbols[key]['proc']['arg_nums'] = [-1] * len(self.all_symbols[key]['arg'])
-            
+            pass  # Ignore cray pointers
+        self.derived = derived_ns(*args[8])
+        self.actual_arg = actual_arglist(*args[9])
+        self.nml = namelist(*args[10])
+        self.intrinsic = int(args[11])
+        if len(args) > 12:
+            self.intrinsic_symbol = int(args[12])
+        if len(args) > 13:
+            self.hash = int(args[13])
+        if len(args) > 14:
+            if args[15] is not None:
+                self.simd = simd_dec(*args[14])
+
+
+@dataclass(init=False)
+class symbol(utils):
+    head: header = None
+    sym: data = None
+    raw: str = ""
+
+    def __init__(self, *args):
+        self.head = header(*args[0:5])
+        self.sym = data(*args[5])
+        self.raw = args
+
+    @property
+    def name(self):
+        return self.head.name
+
+    @property
+    def mangled_name(self):
+        return self.head.mn_name
+
+
+class module(object):
+    version = 15
+
+    def __init__(self, filename, load_only=False):
+        self.filename = filename
+
+        with gzip.open(self.filename) as f:
+            x = f.read().decode()
+
+        self.mod_info = x[: x.index("\n")]
+
+        v = int(self.mod_info.split("'")[1])
+
+        if v != self.version:
+            raise VersionError("Unsupported module version")
+
+        data = x[x.index("\n") + 1 :].replace("\n", " ")
+
+        self.parsed_data = OneOrMore(nestedExpr()).parseString(data)
+
+        if not load_only:
+            self.interface = self.parsed_data[0]
+
+            self.operators = self.parsed_data[1]
+            self.generics = self.proc_generics(self.parsed_data[2])
+
+            self.common = self.proc_common(self.parsed_data[3])
+            self.equivalence = self.parsed_data[4]
+
+            self.omp = self.parsed_data[5]
+
+            self.symbols = self.parse_symbols(self.parsed_data[6])
+            self.summary = Summary(self.parsed_data[7])
+
+    def parse_symbols(self, data):
+        result = {}
+        for i in range(0, len(data), 6):
+            s = symbol(*data[i : i + 6])
+            result[s.head.id] = s
+
+        return result
+
+    def proc_common(self, data):
+        result = {}
+        for i in data:
+            d = c_item(*i)
+            result[d.id] = d
+        return result
+
+    def proc_generics(self, data):
+        result = {}
+        for i in data:
+            d = generics(*i)
+            result[d.name] = d
+        return result
+
+    def keys(self):
+        return self.summary.names()
+
+    def __contains__(self, key):
+        return key in self.keys()
+
+    def __getitem__(self, key):
+        try:
+            return self.symbols[self.summary[key].id]
+        except KeyError:
+            # Not a global variable maybe a function argument?
+            return self.symbols[key]
+
+
+if __name__ == "__main__":
+    m = module(filename=sys.argv[1])
+    for i in m.keys():
+        pprint.pprint(m[i])
```

