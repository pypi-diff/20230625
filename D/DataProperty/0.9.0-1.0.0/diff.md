# Comparing `tmp/DataProperty-0.9.0.tar.gz` & `tmp/DataProperty-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DataProperty-0.9.0.tar", last modified: Sat Sep 10 14:03:07 2016, max compression
+gzip compressed data, was "DataProperty-1.0.0.tar", last modified: Sun Jun 25 01:23:32 2023, max compression
```

## Comparing `DataProperty-0.9.0.tar` & `DataProperty-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/DataProperty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10540 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1195 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/converter/
--rwxrwxrwx   0 root         (0) root         (0)      391 2016-07-09 04:33:51.000000 DataProperty-0.9.0/dataproperty/converter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4388 2016-09-10 13:05:44.000000 DataProperty-0.9.0/dataproperty/converter/_core.py
--rwxrwxrwx   0 root         (0) root         (0)     1307 2016-09-10 13:05:50.000000 DataProperty-0.9.0/dataproperty/converter/_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/type/
--rwxrwxrwx   0 root         (0) root         (0)      896 2016-07-09 12:32:18.000000 DataProperty-0.9.0/dataproperty/type/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5379 2016-09-10 13:45:18.000000 DataProperty-0.9.0/dataproperty/type/_checker.py
--rwxrwxrwx   0 root         (0) root         (0)     1866 2016-09-10 13:06:00.000000 DataProperty-0.9.0/dataproperty/type/_checker_creator.py
--rwxrwxrwx   0 root         (0) root         (0)      765 2016-09-10 13:13:51.000000 DataProperty-0.9.0/dataproperty/type/_typecode.py
--rwxrwxrwx   0 root         (0) root         (0)     1065 2016-07-23 08:17:19.000000 DataProperty-0.9.0/dataproperty/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      656 2016-05-06 13:38:10.000000 DataProperty-0.9.0/dataproperty/_align.py
--rwxrwxrwx   0 root         (0) root         (0)      797 2016-07-09 12:31:49.000000 DataProperty-0.9.0/dataproperty/_align_getter.py
--rwxrwxrwx   0 root         (0) root         (0)     1687 2016-05-06 13:38:24.000000 DataProperty-0.9.0/dataproperty/_container.py
--rwxrwxrwx   0 root         (0) root         (0)    12825 2016-07-17 01:39:03.000000 DataProperty-0.9.0/dataproperty/_data_property.py
--rwxrwxrwx   0 root         (0) root         (0)      172 2016-06-04 05:30:16.000000 DataProperty-0.9.0/dataproperty/_error.py
--rwxrwxrwx   0 root         (0) root         (0)     3030 2016-09-10 13:06:17.000000 DataProperty-0.9.0/dataproperty/_factory.py
--rwxrwxrwx   0 root         (0) root         (0)     5009 2016-07-23 09:30:49.000000 DataProperty-0.9.0/dataproperty/_function.py
--rwxrwxrwx   0 root         (0) root         (0)      492 2016-09-10 13:06:27.000000 DataProperty-0.9.0/dataproperty/_interface.py
--rwxrwxrwx   0 root         (0) root         (0)     2691 2016-07-27 13:09:16.000000 DataProperty-0.9.0/dataproperty/_property_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/misc/
--rwxrwxrwx   0 root         (0) root         (0)      667 2016-03-20 12:35:01.000000 DataProperty-0.9.0/misc/README_HEADER.rst
--rwxrwxrwx   0 root         (0) root         (0)     1092 2016-02-26 06:26:06.000000 DataProperty-0.9.0/misc/readme_converter.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2016-02-26 04:13:48.000000 DataProperty-0.9.0/misc/summary.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       36 2016-09-10 13:03:18.000000 DataProperty-0.9.0/requirements/docs_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2016-06-04 06:03:03.000000 DataProperty-0.9.0/requirements/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2016-07-03 00:53:22.000000 DataProperty-0.9.0/requirements/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/test/
--rwxrwxrwx   0 root         (0) root         (0)     1558 2016-05-15 12:24:42.000000 DataProperty-0.9.0/test/test_align_getter.py
--rwxrwxrwx   0 root         (0) root         (0)     8709 2016-07-03 08:36:32.000000 DataProperty-0.9.0/test/test_column_property.py
--rwxrwxrwx   0 root         (0) root         (0)     2875 2016-07-03 06:58:08.000000 DataProperty-0.9.0/test/test_container.py
--rwxrwxrwx   0 root         (0) root         (0)     5489 2016-07-09 04:04:01.000000 DataProperty-0.9.0/test/test_converter.py
--rwxrwxrwx   0 root         (0) root         (0)      839 2016-07-09 04:34:38.000000 DataProperty-0.9.0/test/test_converter_creator.py
--rwxrwxrwx   0 root         (0) root         (0)    11014 2016-07-23 09:57:33.000000 DataProperty-0.9.0/test/test_function.py
--rwxrwxrwx   0 root         (0) root         (0)    12901 2016-07-09 16:33:01.000000 DataProperty-0.9.0/test/test_property.py
--rwxrwxrwx   0 root         (0) root         (0)    10202 2016-07-17 02:33:51.000000 DataProperty-0.9.0/test/test_property_extractor.py
--rwxrwxrwx   0 root         (0) root         (0)    10717 2016-09-10 13:51:31.000000 DataProperty-0.9.0/test/test_type_checker.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2016-07-09 12:29:15.000000 DataProperty-0.9.0/test/test_type_checker_creator.py
--rwxrwxrwx   0 root         (0) root         (0)      685 2016-09-10 13:14:40.000000 DataProperty-0.9.0/test/test_typecode.py
--rwxrwxrwx   0 root         (0) root         (0)     1105 2016-02-19 14:57:59.000000 DataProperty-0.9.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      203 2016-02-26 12:26:02.000000 DataProperty-0.9.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     7613 2016-07-25 13:52:01.000000 DataProperty-0.9.0/README.rst
--rwxrwxrwx   0 root         (0) root         (0)      107 2016-09-10 14:03:07.000000 DataProperty-0.9.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2071 2016-09-10 13:39:24.000000 DataProperty-0.9.0/setup.py
--rwxrwxrwx   0 root         (0) root         (0)      109 2016-07-09 11:47:50.000000 DataProperty-0.9.0/tox.ini
--rw-r--r--   0 root         (0) root         (0)    10540 2016-09-10 14:03:07.000000 DataProperty-0.9.0/PKG-INFO
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.687040 DataProperty-1.0.0/DataProperty.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11239 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1262 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 01:23:00.000000 DataProperty-1.0.0/DataProperty.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      138 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-25 01:23:32.000000 DataProperty-1.0.0/DataProperty.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-25 01:22:45.000000 DataProperty-1.0.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      223 2023-06-25 01:22:45.000000 DataProperty-1.0.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11239 2023-06-25 01:23:32.697040 DataProperty-1.0.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     9792 2023-06-25 01:22:45.000000 DataProperty-1.0.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/dataproperty/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1262 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      535 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_align.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      833 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_align_getter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2478 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11654 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_column.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1915 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3767 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_container.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3269 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_converter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11174 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    25832 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_extractor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2936 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_formatter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3115 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      626 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      114 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_line_break.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5433 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/_preprocessor.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/dataproperty/logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      442 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/py.typed
+-rw-r--r--   0 toor      (1000) toor      (1000)     1403 2023-06-25 01:22:45.000000 DataProperty-1.0.0/dataproperty/typing.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/misc/
+-rw-r--r--   0 toor      (1000) toor      (1000)       47 2023-06-25 01:22:45.000000 DataProperty-1.0.0/misc/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1186 2023-06-25 01:22:45.000000 DataProperty-1.0.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       52 2023-06-25 01:22:45.000000 DataProperty-1.0.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 01:23:32.697040 DataProperty-1.0.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2881 2023-06-25 01:22:45.000000 DataProperty-1.0.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 01:23:32.697040 DataProperty-1.0.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1748 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_align_getter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    23178 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_column_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4175 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_container.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    26293 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_dataproperty.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    31362 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_extractor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2727 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_formatter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4806 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      559 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2573 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_preprocessor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1162 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_str_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1312 2023-06-25 01:22:45.000000 DataProperty-1.0.0/test/test_typing.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      982 2023-06-25 01:22:45.000000 DataProperty-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DataProperty-0.9.0/DataProperty.egg-info/PKG-INFO` & `DataProperty-1.0.0/DataProperty.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,267 +1,270 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: DataProperty
-Version: 0.9.0
+Version: 1.0.0
 Summary: Python library for extract property from data.
-
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
-Author-email: gogogo.vm@gmail.com
+Author-email: tsuyoshi.hombashi@gmail.com
+Maintainer: Tsuyoshi Hombashi
+Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Description: **DataProperty**
-        
-        .. image:: https://img.shields.io/pypi/pyversions/DataProperty.svg
-           :target: https://pypi.python.org/pypi/DataProperty
-        .. image:: https://travis-ci.org/thombashi/DataProperty.svg?branch=master
-            :target: https://travis-ci.org/thombashi/DataProperty
-        .. image:: https://ci.appveyor.com/api/projects/status/6ybxtfnle9lhykr9?svg=true
-            :target: https://ci.appveyor.com/project/thombashi/dataproperty
-        .. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
-        
-        .. contents:: Table of contents
-           :backlinks: top
-           :local:
-        
-        Summary
-        =======
-        Python library for extract property from data.
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install DataProperty
-        
-        Usage
-        =====
-        
-        Extract property of data
-        ------------------------
-        
-        e.g. Extract property of a `float` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty(-1.0)
-        
-        ::
-        
-            data=-1.0, typename=FLOAT, align=right, str_len=4, integer_digits=1, decimal_places=1, additional_format_len=1
-        
-        e.g. Extract property of a `int` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty(123456789)
-        
-        ::
-        
-            data=123456789, typename=INT, align=right, str_len=9, integer_digits=9, decimal_places=0, additional_format_len=0
-        
-        e.g. Extract property of a `str` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty("abcdefgh")
-        
-        ::
-        
-            data=abcdefgh, typename=STRING, align=left, str_len=8, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        e.g. Extract property of a time value (from `datetime`)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import DataProperty
-            DataProperty(datetime.datetime(2017, 1, 1, 0, 0, 0))
-        
-        ::
-        
-            data=2017-01-01 00:00:00, typename=DATETIME, align=left, str_len=19, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        e.g. Extract property of a time value (from `str`)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            DataProperty("2017-01-01T01:23:45+0900")
-        
-        ::
-        
-            data=2017-01-01 01:23:45+09:00, typename=DATETIME, align=left, str_len=25, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        
-        e.g. Extract property of a `bool` value.
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            DataProperty(True)
-        
-        ::
-        
-            data=True, typename=BOOL, align=left, str_len=4, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        
-        Extract property of data for each data from a matrix
-        ----------------------------------------------------
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import PropertyExtractor, Typecode
-            import six
-        
-            def display(prop_matrix, name):
-                six.print_()
-                six.print_("---------- %s ----------" % (name))
-                for prop_list in prop_matrix:
-                    six.print_([getattr(prop, name) for prop in prop_list])
-        
-            dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
-            inf = float("inf")
-            nan = float("nan")
-            data_matrix = [
-                [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
-                [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
-                [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
-            ]
-            prop_extractor = PropertyExtractor()
-        
-            prop_extractor.data_matrix = data_matrix
-            prop_matrix = prop_extractor.extract_data_property_matrix()
-        
-            six.print_("---------- typename ----------")
-            for prop_list in prop_matrix:
-                six.print_([Typecode.get_typename(prop.typecode) for prop in prop_list])
-        
-            display(prop_matrix, "data")
-            display(prop_matrix, "align")
-            display(prop_matrix, "str_len")
-            display(prop_matrix, "integer_digits")
-            display(prop_matrix, "decimal_places")
-        
-        ::
-        
-            ---------- typename ----------
-            ['INT', 'FLOAT', 'STRING', 'INT', 'INT', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-            ['INT', 'FLOAT', 'STRING', 'FLOAT', 'FLOAT', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-            ['INT', 'FLOAT', 'STRING', 'INT', 'STRING', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-        
-            ---------- data ----------
-            [1, 1.1, 'aa', 1, 1, True, inf, nan, datetime.datetime(2017, 1, 1, 0, 0)]
-            [2, 2.2, 'bbb', 2.2, 2.2, False, inf, nan, datetime.datetime(2017, 1, 1, 0, 0)]
-            [3, 3.33, 'cccc', -3, 'ccc', True, inf, nan, datetime.datetime(2017, 1, 1, 1, 23, 45, tzinfo=tzoffset(None, 32400))]
-        
-            ---------- align ----------
-            [right, right, left, right, right, left, left, left, left]
-            [right, right, left, right, right, left, left, left, left]
-            [right, right, left, right, left, left, left, left, left]
-        
-            ---------- str_len ----------
-            [1, 3, 2, 1, 1, 4, 3, 3, 19]
-            [1, 3, 3, 3, 3, 5, 3, 3, 19]
-            [1, 4, 4, 2, 3, 4, 3, 3, 24]
-        
-            ---------- integer_digits ----------
-            [1, 1, nan, 1, 1, nan, nan, nan, nan]
-            [1, 1, nan, 1, 1, nan, nan, nan, nan]
-            [1, 1, nan, 1, nan, nan, nan, nan, nan]
-        
-            ---------- decimal_places ----------
-            [0, 1, nan, 0, 0, nan, nan, nan, nan]
-            [0, 1, nan, 1, 1, nan, nan, nan, nan]
-            [0, 2, nan, 0, nan, nan, nan, nan, nan]
-        
-        Extract property of data for each column from a matrix
-        ------------------------------------------------------
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import PropertyExtractor, Typecode
-            import six
-        
-            def display(prop_list, name):
-                six.print_()
-                six.print_("---------- %s ----------" % (name))
-                six.print_([getattr(prop, name) for prop in prop_list])
-        
-            dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
-            inf = float("inf")
-            nan = float("nan")
-            data_matrix = [
-                [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
-                [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
-                [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
-            ]
-            prop_extractor = PropertyExtractor()
-        
-            prop_extractor.header_list = [
-                "int", "float", "str", "num", "mix", "bool", "inf", "nan", "time"]
-            prop_extractor.data_matrix = data_matrix
-            col_prop_list = prop_extractor.extract_column_property_list()
-        
-            six.print_("---------- typename ----------")
-            six.print_([Typecode.get_typename(prop.typecode) for prop in col_prop_list])
-        
-            display(col_prop_list, "align")
-            display(col_prop_list, "padding_len")
-            display(col_prop_list, "decimal_places")
-        
-        ::
-        
-            ---------- typename ----------
-            ['INT', 'FLOAT', 'STRING', 'FLOAT', 'STRING', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-        
-            ---------- align ----------
-            [right, right, left, right, left, left, left, left, left]
-        
-            ---------- padding_len ----------
-            [3, 5, 4, 4, 3, 5, 3, 3, 24]
-        
-            ---------- decimal_places ----------
-            [0, 2, nan, 1, 1, nan, nan, nan, nan]
-        
-        
-        Dependencies
-        ============
-        
-        Python 2.7 or 3.3+
-        
-        - `python-dateutil <https://dateutil.readthedocs.io/en/stable/>`__
-        - `pytz <https://pypi.python.org/pypi/pytz/>`__
-        - `six <https://pypi.python.org/pypi/six/>`__
-        
-        Test dependencies
-        -----------------
-        
-        -  `pytest <https://pypi.python.org/pypi/pytest>`__
-        -  `pytest-runner <https://pypi.python.org/pypi/pytest-runner>`__
-        -  `tox <https://pypi.python.org/pypi/tox>`__
-        
-Keywords: property
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://github.com/thombashi/DataProperty
+Project-URL: Tracker, https://github.com/thombashi/DataProperty/issues
+Keywords: data,library,property
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: logging
+Provides-Extra: test
+License-File: LICENSE
+
+.. contents:: **DataProperty**
+   :backlinks: top
+   :local:
+
+
+Summary
+=======
+A Python library for extract property from data.
+
+
+.. image:: https://badge.fury.io/py/DataProperty.svg
+    :target: https://badge.fury.io/py/DataProperty
+    :alt: PyPI package version
+
+.. image:: https://anaconda.org/conda-forge/DataProperty/badges/version.svg
+    :target: https://anaconda.org/conda-forge/DataProperty
+    :alt: conda-forge package version
+
+.. image:: https://img.shields.io/pypi/pyversions/DataProperty.svg
+   :target: https://pypi.org/project/DataProperty
+    :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/implementation/DataProperty.svg
+    :target: https://pypi.org/project/DataProperty
+    :alt: Supported Python implementations
+
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
+    :alt: Test coverage
+
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
+
+Installation
+============
+
+Installation: pip
+------------------------------
+::
+
+    pip install DataProperty
+
+Installation: conda
+------------------------------
+::
+
+    conda install -c conda-forge dataproperty
+
+Installation: apt
+------------------------------
+::
+
+    sudo add-apt-repository ppa:thombashi/ppa
+    sudo apt update
+    sudo apt install python3-dataproperty
+
+
+Usage
+=====
+
+Extract property of data
+------------------------
+
+e.g. Extract a ``float`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(-1.1)
+    data=-1.1, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=1, extra_len=1
+
+e.g. Extract a ``int`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(123456789)
+    data=123456789, type=INTEGER, align=right, ascii_width=9, int_digits=9, decimal_places=0, extra_len=0
+
+e.g. Extract a ``str`` (ascii) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty("sample string")
+    data=sample string, type=STRING, align=left, length=13, ascii_width=13, extra_len=0
+
+e.g. Extract a ``str`` (multi-byte) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> str(DataProperty("吾輩は猫である"))
+    data=吾輩は猫である, type=STRING, align=left, length=7, ascii_width=14, extra_len=0
+
+e.g. Extract a time (``datetime``) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> import datetime
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(datetime.datetime(2017, 1, 1, 0, 0, 0))
+    data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+
+e.g. Extract a ``bool`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(True)
+    data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+
+
+Extract data property for each element from a matrix
+----------------------------------------------------
+``DataPropertyExtractor.to_dp_matrix`` method returns a matrix of ``DataProperty`` instances from a data matrix.
+An example data set and the result are as follows:
+
+:Sample Code:
+    .. code:: python
+
+        import datetime
+        from dataproperty import DataPropertyExtractor
+
+        dp_extractor = DataPropertyExtractor()
+        dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
+        inf = float("inf")
+        nan = float("nan")
+
+        dp_matrix = dp_extractor.to_dp_matrix([
+            [1, 1.1, "aa", 1, 1, True, inf, nan, dt],
+            [2, 2.2, "bbb", 2.2, 2.2, False, "inf", "nan", dt],
+            [3, 3.33, "cccc", -3, "ccc", "true", inf, "NAN", "2017-01-01T01:23:45+0900"],
+        ])
+
+        for row, dp_list in enumerate(dp_matrix):
+            for col, dp in enumerate(dp_list):
+                print("row={:d}, col={:d}, {}".format(row, col, str(dp)))
+
+:Output:
+    ::
+
+        row=0, col=0, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=1, data=1.1, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=0, col=2, data=aa, type=STRING, align=left, ascii_width=2, length=2, extra_len=0
+        row=0, col=3, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=4, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=5, data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+        row=0, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=0, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=0, col=8, data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+        row=1, col=0, data=2, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=1, col=1, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=2, data=bbb, type=STRING, align=left, ascii_width=3, length=3, extra_len=0
+        row=1, col=3, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=4, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=5, data=False, type=BOOL, align=left, ascii_width=5, extra_len=0
+        row=1, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=1, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=1, col=8, data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+        row=2, col=0, data=3, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=2, col=1, data=3.33, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=2, extra_len=0
+        row=2, col=2, data=cccc, type=STRING, align=left, ascii_width=4, length=4, extra_len=0
+        row=2, col=3, data=-3, type=INTEGER, align=right, ascii_width=2, int_digits=1, decimal_places=0, extra_len=1
+        row=2, col=4, data=ccc, type=STRING, align=left, ascii_width=3, length=3, extra_len=0
+        row=2, col=5, data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+        row=2, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=2, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=2, col=8, data=2017-01-01T01:23:45+0900, type=STRING, align=left, ascii_width=24, length=24, extra_len=0
+
+
+Full example source code can be found at *examples/py/to_dp_matrix.py*
+
+
+Extract properties for each column from a matrix
+------------------------------------------------------
+``DataPropertyExtractor.to_column_dp_list`` method returns a list of ``DataProperty`` instances from a data matrix. The list represents the properties for each column.
+An example data set and the result are as follows:
+
+Example data set and result are as follows:
+
+:Sample Code:
+    .. code:: python
+
+        import datetime
+        from dataproperty import DataPropertyExtractor
+
+        dp_extractor = DataPropertyExtractor()
+        dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
+        inf = float("inf")
+        nan = float("nan")
+
+        data_matrix = [
+            [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
+            [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
+            [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
+        ]
+
+        dp_extractor.headers = ["int", "float", "str", "num", "mix", "bool", "inf", "nan", "time"]
+        col_dp_list = dp_extractor.to_column_dp_list(dp_extractor.to_dp_matrix(dp_matrix))
+
+        for col_idx, col_dp in enumerate(col_dp_list):
+            print(str(col_dp))
+
+:Output:
+    ::
+
+        column=0, type=INTEGER, align=right, ascii_width=3, bit_len=2, int_digits=1, decimal_places=0
+        column=1, type=REAL_NUMBER, align=right, ascii_width=5, int_digits=1, decimal_places=(min=1, max=2)
+        column=2, type=STRING, align=left, ascii_width=4
+        column=3, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=(min=0, max=1), extra_len=(min=0, max=1)
+        column=4, type=STRING, align=left, ascii_width=3, int_digits=1, decimal_places=(min=0, max=1)
+        column=5, type=BOOL, align=left, ascii_width=5
+        column=6, type=INFINITY, align=left, ascii_width=8
+        column=7, type=NAN, align=left, ascii_width=3
+        column=8, type=STRING, align=left, ascii_width=24
+
+
+Full example source code can be found at *examples/py/to_column_dp_list.py*
+
+
+Dependencies
+============
+- Python 3.7+
+- `Python package dependencies (automatically installed) <https://github.com/thombashi/DataProperty/network/dependencies>`__
+
+Optional dependencies
+---------------------
+- `loguru <https://github.com/Delgan/loguru>`__
+    - Used for logging if the package installed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DataProperty-0.9.0/DataProperty.egg-info/SOURCES.txt` & `DataProperty-1.0.0/DataProperty.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
 setup.py
 tox.ini
 DataProperty.egg-info/PKG-INFO
 DataProperty.egg-info/SOURCES.txt
 DataProperty.egg-info/dependency_links.txt
+DataProperty.egg-info/not-zip-safe
 DataProperty.egg-info/requires.txt
 DataProperty.egg-info/top_level.txt
 dataproperty/__init__.py
+dataproperty/__version__.py
 dataproperty/_align.py
 dataproperty/_align_getter.py
+dataproperty/_base.py
+dataproperty/_column.py
+dataproperty/_common.py
 dataproperty/_container.py
-dataproperty/_data_property.py
-dataproperty/_error.py
-dataproperty/_factory.py
+dataproperty/_converter.py
+dataproperty/_dataproperty.py
+dataproperty/_extractor.py
+dataproperty/_formatter.py
 dataproperty/_function.py
 dataproperty/_interface.py
-dataproperty/_property_extractor.py
-dataproperty/converter/__init__.py
-dataproperty/converter/_core.py
-dataproperty/converter/_creator.py
-dataproperty/type/__init__.py
-dataproperty/type/_checker.py
-dataproperty/type/_checker_creator.py
-dataproperty/type/_typecode.py
-misc/README_HEADER.rst
-misc/readme_converter.py
+dataproperty/_line_break.py
+dataproperty/_preprocessor.py
+dataproperty/py.typed
+dataproperty/typing.py
+dataproperty/logger/__init__.py
+dataproperty/logger/_logger.py
+dataproperty/logger/_null_logger.py
 misc/summary.txt
 requirements/docs_requirements.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
+test/__init__.py
+test/common.py
 test/test_align_getter.py
-test/test_column_property.py
+test/test_column_dataproperty.py
 test/test_container.py
-test/test_converter.py
-test/test_converter_creator.py
+test/test_dataproperty.py
+test/test_extractor.py
+test/test_formatter.py
 test/test_function.py
-test/test_property.py
-test/test_property_extractor.py
-test/test_type_checker.py
-test/test_type_checker_creator.py
-test/test_typecode.py
+test/test_logger.py
+test/test_preprocessor.py
+test/test_str_function.py
+test/test_typing.py
```

### Comparing `DataProperty-0.9.0/dataproperty/_align.py` & `DataProperty-1.0.0/dataproperty/_align.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
+import enum
 
-class Align:
-
-    class __AlignData(object):
-
-        @property
-        def align_code(self):
-            return self.__align_code
-
-        @property
-        def align_string(self):
-            return self.__align_string
-
-        def __init__(self, code, string):
-            self.__align_code = code
-            self.__align_string = string
-
-        def __repr__(self):
-            return self.align_string
 
-    AUTO = __AlignData(1 << 0, "auto")
-    LEFT = __AlignData(1 << 1, "left")
-    RIGHT = __AlignData(1 << 2, "right")
-    CENTER = __AlignData(1 << 3, "center")
+@enum.unique
+class Align(enum.Enum):
+    AUTO = (1 << 0, "auto")
+    LEFT = (1 << 1, "left")
+    RIGHT = (1 << 2, "right")
+    CENTER = (1 << 3, "center")
+
+    @property
+    def align_code(self) -> int:
+        return self.__align_code
+
+    @property
+    def align_string(self) -> str:
+        return self.__align_string
+
+    def __init__(self, code: int, string: str) -> None:
+        self.__align_code = code
+        self.__align_string = string
```

### Comparing `DataProperty-0.9.0/dataproperty/_align_getter.py` & `DataProperty-1.0.0/dataproperty/_align_getter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
+from typing import Dict
 
-from ._align import Align
-from .type import Typecode
+from typepy import Typecode
 
+from ._align import Align
 
-class AlignGetter(object):
 
+class AlignGetter:
     @property
     def typecode_align_table(self):
         raise NotImplementedError()
 
     @typecode_align_table.setter
-    def typecode_align_table(self, x):
+    def typecode_align_table(self, x: Dict[Typecode, Align]) -> None:
         self.__typecode_align_table = x
 
-    def get_align_from_typecode(self, typecode):
+    def get_align_from_typecode(self, typecode: Typecode) -> Align:
         return self.__typecode_align_table.get(typecode, self.default_align)
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.typecode_align_table = {
             Typecode.STRING: Align.LEFT,
-            Typecode.INT: Align.RIGHT,
-            Typecode.FLOAT: Align.RIGHT,
+            Typecode.INTEGER: Align.RIGHT,
+            Typecode.REAL_NUMBER: Align.RIGHT,
         }
         self.default_align = Align.LEFT
 
+
 align_getter = AlignGetter()
```

### Comparing `DataProperty-0.9.0/dataproperty/_data_property.py` & `DataProperty-1.0.0/dataproperty/_column.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,439 +1,352 @@
-# encoding: utf-8
+from typing import Any, Dict, List, Optional
 
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
-
-from __future__ import absolute_import
-import math
+from mbstrdecoder import MultiByteStrDecoder
+from typepy import Integer, StrictLevel, Typecode, TypeConversionError
 
+from ._align import Align
 from ._align_getter import align_getter
-from ._container import MinMaxContainer
-from ._error import TypeConversionError
-from ._interface import DataPeropertyInterface
-from .type import Typecode
-from .type import FloatTypeChecker
-
-from ._function import is_nan
-from ._function import get_number_of_digit
-from ._function import get_text_len
-
-from ._factory import NoneTypeFactory
-from ._factory import StringTypeFactory
-from ._factory import IntegerTypeFactory
-from ._factory import FloatTypeFactory
-from ._factory import BoolTypeFactory
-from ._factory import DateTimeTypeFactory
-from ._factory import InfinityTypeFactory
-from ._factory import NanTypeFactory
-
-
-def default_bool_converter(value):
-    return value
-
-
-def default_datetime_converter(value):
-    return value
-
-
-class DataPeropertyBase(DataPeropertyInterface):
-    __slots__ = ("__datetime_format_str")
-
-    @property
-    def format_str(self):
-        format_str = {
-            Typecode.NONE: "",
-            Typecode.INT: "d",
-            Typecode.BOOL: "",
-            Typecode.DATETIME: self.__datetime_format_str,
-        }.get(self.typecode)
-
-        if format_str is not None:
-            return format_str
+from ._base import DataPeropertyBase
+from ._common import DefaultValue
+from ._container import ListContainer, MinMaxContainer
+from ._dataproperty import DataProperty
+from ._function import calc_ascii_char_width
+from .typing import FloatType
 
-        if self.typecode in (Typecode.FLOAT, Typecode.INFINITY, Typecode.NAN):
-            if is_nan(self.decimal_places):
-                return "f"
 
-            return ".{:d}f".format(self.decimal_places)
-
-        return "s"
-
-    def __init__(self, datetime_format_str):
-        self.__datetime_format_str = datetime_format_str
-
-
-class DataProperty(DataPeropertyBase):
+class ColumnDataProperty(DataPeropertyBase):
     __slots__ = (
-        "__data",
-        "__typecode",
-        "__align",
-        "__integer_digits",
-        "__decimal_places",
-        "__additional_format_len",
-        "__str_len",
+        "__header_ascii_char_width",
+        "__body_ascii_char_width",
+        "__column_index",
+        "__dp_list",
+        "__float_type",
+        "__format_map",
+        "__is_calculate",
+        "__max_precision",
+        "__minmax_integer_digits",
+        "__minmax_decimal_places",
+        "__minmax_additional_format_len",
+        "__typecode_bitmap",
     )
 
-    __type_factory_list = [
-        NoneTypeFactory(),
-        IntegerTypeFactory(),
-        InfinityTypeFactory(),
-        NanTypeFactory(),
-        FloatTypeFactory(),
-        BoolTypeFactory(),
-        DateTimeTypeFactory(),
-        StringTypeFactory(),
-    ]
-
     @property
-    def align(self):
-        return self.__align
+    def align(self) -> Align:
+        return align_getter.get_align_from_typecode(self.typecode)
 
     @property
-    def decimal_places(self):
-        """
-        :return:
-            Decimal places if the ``data`` is ``float``.
-            Returns ``0`` if the ``data`` is ``int``.
-            Otherwise, returns ``float("nan")``.
-        :rtype: int
-        """
-
-        return self.__decimal_places
+    def bit_length(self) -> Optional[int]:
+        if self.typecode != Typecode.INTEGER:
+            return None
 
-    @property
-    def typecode(self):
-        """
-        Return the type code that corresponds to the type of the ``data``.
-
-        :return:
-            One of the constants that are defined in the ``Typecode`` class.
-        :rtype: int
-        """
+        bit_length = 0
+        for value_dp in self.__dp_list:
+            try:
+                bit_length = max(bit_length, int.bit_length(value_dp.data))
+            except TypeError:
+                pass
 
-        return self.__typecode
+        return bit_length
 
     @property
-    def data(self):
-        """
-        :return: Original data.
-        :rtype: Original data type.
-        """
-
-        return self.__data
+    def column_index(self) -> int:
+        return self.__column_index
 
     @property
-    def str_len(self):
-        """
-        :return: Length of the ``data`` as a string.
-        :rtype: int
-        """
+    def decimal_places(self) -> Optional[int]:
+        return self._decimal_places
 
-        return self.__str_len
+    @property
+    def ascii_char_width(self) -> int:
+        return max(self.__header_ascii_char_width, self.__body_ascii_char_width)
 
     @property
-    def integer_digits(self):
-        """
-        :return:
-            Integer digits if the ``data`` is ``int``/``float``.
-            Otherwise, returns ``float("nan")``.
-        :rtype: int
-        """
+    def minmax_integer_digits(self) -> MinMaxContainer:
+        return self.__minmax_integer_digits
 
-        return self.__integer_digits
+    @property
+    def minmax_decimal_places(self) -> ListContainer:
+        return self.__minmax_decimal_places
 
     @property
-    def additional_format_len(self):
-        return self.__additional_format_len
+    def minmax_additional_format_len(self) -> MinMaxContainer:
+        return self.__minmax_additional_format_len
 
     def __init__(
-            self, data,
-            none_value=None, inf_value=float("inf"), nan_value=float("nan"),
-            bool_converter=default_bool_converter,
-            datetime_converter=default_datetime_converter,
-            datetime_format_str="%Y-%m-%dT%H:%M:%S%z",
-            is_convert=True,
-            replace_tabs_with_spaces=True, tab_length=2):
-        super(DataProperty, self).__init__(datetime_format_str)
-
-        self.__set_data(data, none_value, inf_value, nan_value, is_convert)
-        self.__convert_data(bool_converter, datetime_converter)
-        self.__replace_tabs(replace_tabs_with_spaces, tab_length)
-        self.__align = align_getter.get_align_from_typecode(self.typecode)
+        self,
+        column_index: int,
+        float_type: Optional[FloatType],
+        min_width: int = 0,
+        format_flags: Optional[int] = None,
+        is_formatting_float: bool = True,
+        datetime_format_str: str = DefaultValue.DATETIME_FORMAT,
+        east_asian_ambiguous_width: int = 1,
+        max_precision: int = DefaultValue.MAX_PRECISION,
+    ) -> None:
+        super().__init__(
+            format_flags=format_flags,
+            is_formatting_float=is_formatting_float,
+            datetime_format_str=datetime_format_str,
+            east_asian_ambiguous_width=east_asian_ambiguous_width,
+        )
+
+        self.__header_ascii_char_width = 0
+        self.__body_ascii_char_width = min_width
+        self.__column_index = column_index
 
-        try:
-            integer_digits, decimal_places = get_number_of_digit(data)
-        except OverflowError:
-            integer_digits = float("nan")
-            decimal_places = float("nan")
-        self.__integer_digits = integer_digits
-        self.__decimal_places = decimal_places
-        self.__additional_format_len = self.__get_additional_format_len()
-        self.__str_len = self.__get_str_len()
+        self.__float_type = float_type
 
-    def __repr__(self):
-        element_list = []
+        self.__is_calculate = True
+        self.__dp_list: List[DataProperty] = []
+        self.__minmax_integer_digits = MinMaxContainer()
+        self.__minmax_decimal_places = ListContainer()
+        self.__minmax_additional_format_len = MinMaxContainer()
+        self.__max_precision = max_precision
 
-        if self.typecode == Typecode.DATETIME:
-            element_list.append(
-                "data={:s}".format(str(self.data)))
-        else:
-            element_list.append(
-                ("data={:" + self.format_str + "}").format(self.data))
-
-        element_list.extend([
-            "typename=" + Typecode.get_typename(self.typecode),
-            "align=" + str(self.align),
-            "str_len=" + str(self.str_len),
-            "integer_digits=" + str(self.integer_digits),
-            "decimal_places=" + str(self.decimal_places),
-            "additional_format_len=" + str(self.additional_format_len),
-        ])
+        self.__typecode_bitmap = Typecode.NONE.value
+        self.__calc_typecode_from_bitmap()
 
-        return ", ".join(element_list)
+        self.__format_map: Dict[Typecode, str] = self._formatter.make_format_map(
+            decimal_places=self._decimal_places
+        )
 
-    def __get_additional_format_len(self):
-        if not FloatTypeChecker(self.data).is_type():
-            return 0
+    def __repr__(self) -> str:
+        element_list = []
 
-        format_len = 0
+        if self.column_index is not None:
+            element_list.append(f"column={self.column_index}")
 
-        if float(self.data) < 0:
-            # for minus character
-            format_len += 1
+        element_list.extend(
+            [
+                f"type={self.typename}",
+                f"align={self.align.align_string}",
+                f"ascii_width={self.ascii_char_width}",
+            ]
+        )
+
+        if Integer(self.bit_length).is_type():
+            element_list.append(f"bit_len={self.bit_length}")
+
+        if self.minmax_integer_digits.has_value():
+            if self.minmax_integer_digits.is_same_value():
+                value = f"int_digits={self.minmax_integer_digits.min_value}"
+            else:
+                value = f"int_digits=({self.minmax_integer_digits})"
+
+            element_list.append(value)
+
+        if self.minmax_decimal_places.has_value():
+            if self.minmax_decimal_places.is_same_value():
+                value = f"decimal_places={self.minmax_decimal_places.min_value}"
+            else:
+                value = f"decimal_places=({self.minmax_decimal_places})"
+
+            element_list.append(value)
+
+        if not self.minmax_additional_format_len.is_zero():
+            if self.minmax_additional_format_len.is_same_value():
+                value = f"extra_len={self.minmax_additional_format_len.min_value}"
+            else:
+                value = f"extra_len=({self.minmax_additional_format_len})"
 
-        return format_len
+            element_list.append(value)
 
-    def __get_base_float_len(self):
-        if any([self.integer_digits < 0, self.decimal_places < 0]):
-            raise ValueError()
+        return ", ".join(element_list)
 
-        float_len = self.integer_digits + self.decimal_places
-        if self.decimal_places > 0:
-            # for dot
-            float_len += 1
+    def dp_to_str(self, value_dp: DataProperty) -> str:
+        if value_dp.typecode == Typecode.STRING:
+            return str(value_dp.data)
 
-        return float_len
+        try:
+            value = self.__preprocess_value_before_tostring(value_dp)
+        except TypeConversionError:
+            return self.__format_map.get(value_dp.typecode, "{:s}").format(value_dp.data)
 
-    def __get_str_len(self):
-        if self.typecode == Typecode.INT:
-            return self.integer_digits + self.additional_format_len
+        to_string_format_str = self.__get_tostring_format(value_dp)
 
-        if self.typecode == Typecode.FLOAT:
-            return self.__get_base_float_len() + self.additional_format_len
+        try:
+            return to_string_format_str.format(value)
+        except (ValueError, TypeError):
+            pass
 
-        if self.typecode == Typecode.DATETIME:
-            full_format_str = "{:" + self.format_str + "}"
-            return len(full_format_str.format(self.data))
+        try:
+            return MultiByteStrDecoder(value).unicode_str
+        except ValueError:
+            pass
 
-        return get_text_len(self.data)
+        return str(value)
 
-    def __set_data(
-            self, data, none_value, inf_value, nan_value, is_convert):
-        special_value_table = {
-            Typecode.NONE: none_value,
-            Typecode.INFINITY: inf_value,
-            Typecode.NAN: nan_value,
-        }
+    def extend_width(self, ascii_char_width: int) -> None:
+        self.extend_header_width(ascii_char_width)
+        self.extend_body_width(ascii_char_width)
 
-        for type_factory in self.__type_factory_list:
-            checker = type_factory.type_checker_factory.create(
-                data, is_convert)
-            if not checker.is_type():
-                continue
+    def extend_header_width(self, ascii_char_width: int) -> None:
+        self.__header_ascii_char_width += ascii_char_width
 
-            self.__typecode = checker.typecode
+    def extend_body_width(self, ascii_char_width: int) -> None:
+        self.__body_ascii_char_width += ascii_char_width
 
-            special_value = special_value_table.get(self.__typecode)
-            if special_value is not None:
-                self.__data = special_value
-                return
+    def update_header(self, header_db: DataProperty) -> None:
+        self.__header_ascii_char_width = header_db.ascii_char_width
 
-            self.__data = type_factory.value_converter_factory.create(
-                data).convert()
+    def update_body(self, value_dp: DataProperty) -> None:
+        if value_dp.is_include_ansi_escape:
+            assert value_dp.no_ansi_escape_dp
+            value_dp = value_dp.no_ansi_escape_dp
 
-            return
+        self.__typecode_bitmap |= value_dp.typecode.value
+        self.__calc_typecode_from_bitmap()
 
-        raise TypeConversionError(
-            "failed to convert: " + Typecode.get_typename(self.__typecode))
+        if value_dp.typecode in (Typecode.REAL_NUMBER, Typecode.INTEGER):
+            self.__minmax_integer_digits.update(value_dp.integer_digits)
+            self.__minmax_decimal_places.update(value_dp.decimal_places)
+            self.__update_decimal_places()
 
-    def __convert_data(self, bool_converter, datetime_converter):
-        if self.typecode == Typecode.BOOL:
-            self.__data = bool_converter(self.__data)
-        elif self.typecode == Typecode.DATETIME:
-            self.__data = datetime_converter(self.__data)
+        self.__minmax_additional_format_len.update(value_dp.additional_format_len)
 
-    def __replace_tabs(self, replace_tabs_with_spaces, tab_length):
-        if not replace_tabs_with_spaces:
-            return
+        self.__dp_list.append(value_dp)
+        self.__update_ascii_char_width()
 
-        try:
-            self.__data = self.__data.replace("\t", " " * tab_length)
-        except (TypeError, AttributeError):
-            pass
+    def merge(self, column_dp: "ColumnDataProperty") -> None:
+        self.__typecode_bitmap |= column_dp.typecode.value
+        self.__calc_typecode_from_bitmap()
 
+        self.__minmax_integer_digits.merge(column_dp.minmax_integer_digits)
+        self.__minmax_decimal_places.update(column_dp.minmax_decimal_places)
+        self.__update_decimal_places()
 
-class ColumnDataProperty(DataPeropertyBase):
-    __slots__ = (
-        "__typecode_bitmap",
-        "__str_len",
-        "__minmax_integer_digits",
-        "__minmax_decimal_places",
-        "__minmax_additional_format_len",
-        "__data_prop_list",
-    )
+        self.__minmax_additional_format_len.merge(column_dp.minmax_additional_format_len)
 
-    __FACTORY_TABLE = {
-        Typecode.NONE: NoneTypeFactory(),
-        Typecode.STRING: StringTypeFactory(),
-        Typecode.INT: IntegerTypeFactory(),
-        Typecode.INFINITY: InfinityTypeFactory(),
-        Typecode.NAN: NanTypeFactory(),
-        Typecode.FLOAT: FloatTypeFactory(),
-        Typecode.BOOL: BoolTypeFactory(),
-        Typecode.DATETIME: DateTimeTypeFactory(),
-    }
+        self.__body_ascii_char_width = max(self.__body_ascii_char_width, column_dp.ascii_char_width)
+        self.__update_ascii_char_width()
 
-    @property
-    def align(self):
-        return align_getter.get_align_from_typecode(self.typecode)
+    def begin_update(self) -> None:
+        self.__is_calculate = False
 
-    @property
-    def decimal_places(self):
-        try:
-            avg = self.minmax_decimal_places.mean()
-        except TypeError:
-            return float("nan")
+    def end_update(self) -> None:
+        self.__is_calculate = True
 
-        if is_nan(avg):
-            return float("nan")
+        self.__calc_typecode_from_bitmap()
+        self.__update_decimal_places()
+        self.__update_ascii_char_width()
 
-        return int(math.ceil(avg))
+    def __is_not_single_typecode(self, typecode_bitmap: int) -> bool:
+        return bool(
+            self.__typecode_bitmap & typecode_bitmap and self.__typecode_bitmap & ~typecode_bitmap
+        )
 
-    @property
-    def typecode(self):
-        return self.__get_typecode_from_bitmap()
+    def __is_float_typecode(self) -> bool:
+        FLOAT_TYPECODE_BMP = (
+            Typecode.REAL_NUMBER.value | Typecode.INFINITY.value | Typecode.NAN.value
+        )
+        NUMBER_TYPECODE_BMP = FLOAT_TYPECODE_BMP | Typecode.INTEGER.value
 
-    @property
-    def padding_len(self):
-        if self.typecode != Typecode.FLOAT:
-            return self.__str_len
-
-        max_len = self.__str_len
-        col_format_str = "{:" + self.format_str + "}"
-
-        for data_prop in self.__data_prop_list:
-            if data_prop.typecode in [Typecode.INFINITY, Typecode.NAN]:
-                continue
+        if self.__is_not_single_typecode(NUMBER_TYPECODE_BMP | Typecode.NULL_STRING.value):
+            return False
 
-            try:
-                formatted_value = col_format_str.format(data_prop.data)
-            except (TypeError, ValueError):
-                continue
+        if (
+            bin(self.__typecode_bitmap & (FLOAT_TYPECODE_BMP | Typecode.NULL_STRING.value)).count(
+                "1"
+            )
+            >= 2
+        ):
+            return True
 
-            max_len = max(max_len, len(formatted_value))
+        if bin(self.__typecode_bitmap & NUMBER_TYPECODE_BMP).count("1") >= 2:
+            return True
 
-        return max_len
+        return False
 
-    @property
-    def minmax_integer_digits(self):
-        return self.__minmax_integer_digits
+    def __calc_body_ascii_char_width(self) -> int:
+        width_list = [self.__body_ascii_char_width]
 
-    @property
-    def minmax_decimal_places(self):
-        return self.__minmax_decimal_places
+        for value_dp in self.__dp_list:
+            if value_dp.is_include_ansi_escape:
+                assert value_dp.no_ansi_escape_dp
+                value_dp = value_dp.no_ansi_escape_dp
 
-    @property
-    def minmax_additional_format_len(self):
-        return self.__minmax_additional_format_len
+            width_list.append(
+                calc_ascii_char_width(self.dp_to_str(value_dp), self._east_asian_ambiguous_width)
+            )
 
-    @property
-    def type_factory(self):
-        return self.__FACTORY_TABLE.get(self.typecode)
-
-    def __init__(
-            self,
-            min_padding_len=0,
-            datetime_format_str="%Y-%m-%dT%H:%M:%S%z"):
-        super(ColumnDataProperty, self).__init__(datetime_format_str)
-
-        self.__typecode_bitmap = Typecode.NONE
-        self.__str_len = min_padding_len
-        self.__minmax_integer_digits = MinMaxContainer()
-        self.__minmax_decimal_places = MinMaxContainer()
-        self.__minmax_additional_format_len = MinMaxContainer()
-        self.__data_prop_list = []
+        return max(width_list)
 
-    def __repr__(self):
-        return ", ".join([
-            "typename=" + Typecode.get_typename(self.typecode),
-            "align=" + str(self.align),
-            "padding_len=" + str(self.padding_len),
-            "integer_digits=({:s})".format(str(self.minmax_integer_digits)),
-            "decimal_places=({:s})".format(str(self.minmax_decimal_places)),
-            "additional_format_len=({:s})".format(
-                str(self.minmax_additional_format_len)),
-        ])
-
-    def update_header(self, dataprop):
-        self.__str_len = max(self.__str_len, dataprop.str_len)
-
-    def update_body(self, dataprop):
-        self.__typecode_bitmap |= dataprop.typecode
-        self.__str_len = max(self.__str_len, dataprop.str_len)
-
-        if dataprop.typecode in (Typecode.FLOAT, Typecode.INT):
-            self.__minmax_integer_digits.update(dataprop.integer_digits)
-            self.__minmax_decimal_places.update(dataprop.decimal_places)
-
-        self.__minmax_additional_format_len.update(
-            dataprop.additional_format_len)
-
-        self.__data_prop_list.append(dataprop)
-
-    def __is_not_single_typecode(self, typecode):
-        return all([
-            self.__typecode_bitmap & typecode,
-            self.__typecode_bitmap & ~typecode,
-        ])
-
-    def __is_float_typecode(self):
-        number_typecode = (
-            Typecode.INT | Typecode.FLOAT | Typecode.INFINITY | Typecode.NAN)
+    def __calc_decimal_places(self) -> Optional[int]:
+        if self.minmax_decimal_places.max_value is None:
+            return None
 
-        if self.__is_not_single_typecode(number_typecode):
-            return False
+        return int(min(self.__max_precision, self.minmax_decimal_places.max_value))
 
-        if bin(self.__typecode_bitmap & number_typecode).count("1") >= 2:
-            return True
+    def __get_tostring_format(self, value_dp: DataProperty) -> str:
+        if self.typecode == Typecode.STRING:
+            return self.__format_map.get(value_dp.typecode, "{:s}")
 
-        return False
+        return self.__format_map.get(self.typecode, "{:s}")
 
-    def __get_typecode_from_bitmap(self):
+    def __get_typecode_from_bitmap(self) -> Typecode:
         if self.__is_float_typecode():
-            return Typecode.FLOAT
+            return Typecode.REAL_NUMBER
 
-        if any([
-            self.__is_not_single_typecode(Typecode.BOOL),
-            self.__is_not_single_typecode(Typecode.DATETIME),
-        ]):
+        if any(
+            [
+                self.__is_not_single_typecode(Typecode.BOOL.value),
+                self.__is_not_single_typecode(Typecode.DATETIME.value),
+            ]
+        ):
             return Typecode.STRING
 
         typecode_list = [
             Typecode.STRING,
-            Typecode.FLOAT,
-            Typecode.INT,
+            Typecode.REAL_NUMBER,
+            Typecode.INTEGER,
             Typecode.DATETIME,
+            Typecode.DICTIONARY,
+            Typecode.IP_ADDRESS,
+            Typecode.LIST,
             Typecode.BOOL,
             Typecode.INFINITY,
             Typecode.NAN,
+            Typecode.NULL_STRING,
         ]
 
         for typecode in typecode_list:
-            if self.__typecode_bitmap & typecode:
+            if self.__typecode_bitmap & typecode.value:
                 return typecode
 
-        if self.__typecode_bitmap == Typecode.NONE:
+        if self.__typecode_bitmap == Typecode.NONE.value:
             return Typecode.NONE
 
         return Typecode.STRING
+
+    def __update_ascii_char_width(self) -> None:
+        if not self.__is_calculate:
+            return
+
+        self.__body_ascii_char_width = self.__calc_body_ascii_char_width()
+
+    def __update_decimal_places(self) -> None:
+        if not self.__is_calculate:
+            return
+
+        self._decimal_places = self.__calc_decimal_places()
+        self.__format_map = self._formatter.make_format_map(decimal_places=self._decimal_places)
+
+    def __calc_typecode_from_bitmap(self) -> None:
+        if not self.__is_calculate:
+            return
+
+        self._typecode = self.__get_typecode_from_bitmap()
+
+    def __preprocess_value_before_tostring(self, value_dp: DataProperty) -> Any:
+        if self.typecode == value_dp.typecode or self.typecode in [
+            Typecode.STRING,
+            Typecode.BOOL,
+            Typecode.DATETIME,
+        ]:
+            return value_dp.data
+
+        return self.type_class(
+            value_dp.data,
+            strict_level=StrictLevel.MIN,
+            float_type=self.__float_type,
+            strip_ansi_escape=False,
+        ).convert()
```

### Comparing `DataProperty-0.9.0/test/test_align_getter.py` & `DataProperty-1.0.0/test/test_align_getter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from dataproperty import *
-from dataproperty._align_getter import AlignGetter
 import pytest
+from typepy import Typecode
+
+from dataproperty import Align
+from dataproperty._align_getter import AlignGetter
 
 
 @pytest.fixture
 def align_getter():
     return AlignGetter()
 
 
 class Test_AlignGetter_get_align_from_typecode:
-
-    @pytest.mark.parametrize(["value", "expected"], [
-        [Typecode.STRING, Align.LEFT],
-        [Typecode.INT, Align.RIGHT],
-        [Typecode.FLOAT, Align.RIGHT],
-        [Typecode.NONE, Align.LEFT],
-    ])
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            [Typecode.STRING, Align.LEFT],
+            [Typecode.INTEGER, Align.RIGHT],
+            [Typecode.REAL_NUMBER, Align.RIGHT],
+            [Typecode.NONE, Align.LEFT],
+        ],
+    )
     def test_normal(self, align_getter, value, expected):
         assert align_getter.get_align_from_typecode(value) == expected
 
-    @pytest.mark.parametrize(["value", "expected"], [
-        [Typecode.STRING, Align.RIGHT],
-        [Typecode.INT, Align.LEFT],
-        [Typecode.FLOAT, Align.CENTER],
-        [Typecode.NONE, Align.LEFT],
-    ])
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            [Typecode.STRING, Align.RIGHT],
+            [Typecode.INTEGER, Align.LEFT],
+            [Typecode.REAL_NUMBER, Align.CENTER],
+            [Typecode.NONE, Align.LEFT],
+        ],
+    )
     def test_setter(self, align_getter, value, expected):
         align_getter.typecode_align_table = {
             Typecode.STRING: Align.RIGHT,
-            Typecode.INT: Align.LEFT,
-            Typecode.FLOAT: Align.CENTER,
+            Typecode.INTEGER: Align.LEFT,
+            Typecode.REAL_NUMBER: Align.CENTER,
         }
 
         assert align_getter.get_align_from_typecode(value) == expected
 
-    @pytest.mark.parametrize(["value", "expected"], [
-        [Typecode.STRING, Align.LEFT],
-        [Typecode.INT, Align.RIGHT],
-        [Typecode.FLOAT, Align.RIGHT],
-        [Typecode.NONE, Align.CENTER],
-    ])
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            [Typecode.STRING, Align.LEFT],
+            [Typecode.INTEGER, Align.RIGHT],
+            [Typecode.REAL_NUMBER, Align.RIGHT],
+            [Typecode.NONE, Align.CENTER],
+        ],
+    )
     def test_default_align(self, align_getter, value, expected):
         align_getter.default_align = Align.CENTER
 
         assert align_getter.get_align_from_typecode(value) == expected
```

### Comparing `DataProperty-0.9.0/test/test_container.py` & `DataProperty-1.0.0/test/test_container.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,152 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from dataproperty import *
+import sys
+
 import pytest
-import six
+from typepy import Nan
+
+from dataproperty import MinMaxContainer
 
 
 @pytest.fixture
 def container():
     return MinMaxContainer()
 
 
 class Test_MinMaxContainer_property:
-
     def test_null(self, container):
         assert container.min_value is None
         assert container.max_value is None
 
 
 class Test_MinMaxContainer_repr:
-
-    def test_normal(self):
-        container = MinMaxContainer([1, 3])
-        assert str(container) == "min=1, max=3"
-
-    def test_null(self, container):
-        assert container.min_value is None
-        assert container.max_value is None
+    @pytest.mark.parametrize(
+        ["values", "expected"],
+        [[[1, 3], "min=1, max=3"], [[1], "min=1, max=1"], [[None, None], "None"]],
+    )
+    def test_normal(self, values, expected):
+        assert str(MinMaxContainer(values)) == expected
 
 
 class Test_MinMaxContainer_eq_ne:
-
-    @pytest.mark.parametrize(["lhs", "rhs", "expected"], [
-        [
-            MinMaxContainer([1, 3]),
-            MinMaxContainer([1, 3]),
-            True,
-        ],
-        [
-            MinMaxContainer([1, 3]),
-            MinMaxContainer([1, 4]),
-            False,
-        ],
-        [
-            MinMaxContainer([1, 3]),
-            MinMaxContainer([0, 3]),
-            False,
-        ],
+    @pytest.mark.parametrize(
+        ["lhs", "rhs", "expected"],
         [
-            MinMaxContainer([1, 3]),
-            MinMaxContainer([0, 4]),
-            False,
+            [MinMaxContainer([1, 3]), MinMaxContainer([1, 3]), True],
+            [MinMaxContainer([1, 3]), MinMaxContainer([1, 4]), False],
+            [MinMaxContainer([1, 3]), MinMaxContainer([0, 3]), False],
+            [MinMaxContainer([1, 3]), MinMaxContainer([0, 4]), False],
         ],
-    ])
+    )
     def test_normal(self, lhs, rhs, expected):
         assert (lhs == rhs) == expected
         assert (lhs != rhs) == (not expected)
 
 
 class Test_MinMaxContainer_contains:
-
-    @pytest.mark.parametrize(["lhs", "rhs", "expected"], [
+    @pytest.mark.parametrize(
+        ["lhs", "rhs", "expected"],
         [
-            1,
-            MinMaxContainer([1, 3]),
-            True,
+            [1, MinMaxContainer([1, 3]), True],
+            [3, MinMaxContainer([1, 3]), True],
+            [0, MinMaxContainer([1, 3]), False],
+            [4, MinMaxContainer([1, 3]), False],
         ],
-        [
-            3,
-            MinMaxContainer([1, 3]),
-            True,
-        ],
-        [
-            0,
-            MinMaxContainer([1, 3]),
-            False,
-        ],
-        [
-            4,
-            MinMaxContainer([1, 3]),
-            False,
-        ],
-    ])
+    )
     def test_normal(self, lhs, rhs, expected):
         assert (lhs in rhs) == expected
 
 
 class Test_MinMaxContainer_mean:
-
     def test_normal(self, container):
         for value in [1, 3]:
             container.update(value)
 
+        assert container.has_value()
+        assert not container.is_zero()
         assert container.mean() == 2
 
     def test_null(self, container):
-        assert is_nan(container.mean())
+        assert Nan(container.mean()).is_type()
 
 
 class Test_MinMaxContainer_diff:
-
     def test_normal(self, container):
         for value in [1, 3]:
             container.update(value)
 
+        assert container.has_value()
+        assert not container.is_zero()
         assert container.diff() == 2
 
     def test_null(self, container):
-        assert is_nan(container.diff())
+        assert Nan(container.diff()).is_type()
 
 
 class Test_MinMaxContainer_update:
-
     def test_normal_0(self, container):
         for value in [1, 2, 3]:
             container.update(value)
 
+        assert container.has_value()
+        assert not container.is_zero()
         assert container.min_value == 1
         assert container.max_value == 3
 
     def test_normal_1(self, container):
-        for value in [None, -six.MAXSIZE, 0, None, six.MAXSIZE, None]:
+        for value in [None, -sys.maxsize, 0, None, sys.maxsize, None]:
             container.update(value)
 
-        assert container.min_value == -six.MAXSIZE
-        assert container.max_value == six.MAXSIZE
+        assert container.has_value()
+        assert not container.is_zero()
+        assert container.min_value == -sys.maxsize
+        assert container.max_value == sys.maxsize
+
+
+class Test_MinMaxContainer_merge:
+    def test_normal(self, container):
+        for value in [1, 2, 3]:
+            container.update(value)
+
+        other = MinMaxContainer([0, 10])
+
+        container.merge(other)
+
+        assert container.has_value()
+        assert not container.is_zero()
+        assert container.min_value == 0
+        assert container.max_value == 10
+
+
+class Test_MinMaxContainer_is_zero:
+    @pytest.mark.parametrize(
+        ["values", "expected"],
+        [
+            [[0, 0], True],
+            [[0, 0, 0], True],
+            [[0, 1], False],
+            [[1, 0], False],
+            [[1, 1, 1], False],
+            [[None, None], False],
+        ],
+    )
+    def test_normal(self, container, values, expected):
+        assert MinMaxContainer(values).is_zero() == expected
+
+
+class Test_MinMaxContainer_is_same_value:
+    @pytest.mark.parametrize(
+        ["values", "expected"],
+        [
+            [[0, 0], True],
+            [[0, 0, 0], True],
+            [[1, 1, 1], True],
+            [[0, 1], False],
+            [[1, 0], False],
+            [[None, None], False],
+        ],
+    )
+    def test_normal(self, container, values, expected):
+        assert MinMaxContainer(values).is_same_value() == expected
```

### Comparing `DataProperty-0.9.0/LICENSE` & `DataProperty-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2016 Tsuyoshi Hombashi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2016 Tsuyoshi Hombashi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `DataProperty-0.9.0/setup.py` & `DataProperty-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,92 @@
-import sys
+"""
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
+"""
+
 import os.path
+from typing import Dict, Type
+
 import setuptools
 
 
+MODULE_NAME = "DataProperty"
+REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 MISC_DIR = "misc"
 REQUIREMENT_DIR = "requirements"
 
-with open("README.rst") as fp:
-    long_description = fp.read()
+pkg_info: Dict[str, str] = {}
+
+
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
+    try:
+        from releasecmd import ReleaseCommand
+    except ImportError:
+        return {}
+
+    return {"release": ReleaseCommand}
+
+
+with open(os.path.join(MODULE_NAME.lower(), "__version__.py")) as f:
+    exec(f.read(), pkg_info)
+
+with open("README.rst", encoding="utf8") as f:
+    long_description = f.read()
 
-with open(os.path.join(MISC_DIR, "summary.txt")) as f:
-    summary = f.read()
+with open(os.path.join(MISC_DIR, "summary.txt"), encoding="utf8") as f:
+    summary = f.read().strip()
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     install_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
-    tests_require = [line.strip() for line in f if line.strip()]
-
-needs_pytest = set(["pytest", "test", "ptr"]).intersection(sys.argv)
-pytest_runner = ["pytest-runner"] if needs_pytest else []
-
-author = "Tsuyoshi Hombashi"
-email = "gogogo.vm@gmail.com"
-project_name = "DataProperty"
+    tests_requires = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
-    name=project_name,
-    version="0.9.0",
-    url="https://github.com/thombashi/" + project_name,
-    bugtrack_url="https://github.com/thombashi/{:s}/issues".format(
-        project_name),
-
-    author=author,
-    author_email=email,
+    name=MODULE_NAME,
+    version=pkg_info["__version__"],
+    url=REPOSITORY_URL,
+    author=pkg_info["__author__"],
+    author_email=pkg_info["__email__"],
     description=summary,
     include_package_data=True,
-    install_requires=install_requires,
-    keywords=["property"],
-    license="MIT License",
+    keywords=[
+        "data",
+        "library",
+        "property",
+    ],
+    license=pkg_info["__license__"],
     long_description=long_description,
-    maintainer=author,
-    maintainer_email=email,
+    long_description_content_type="text/x-rst",
+    maintainer=pkg_info["__author__"],
+    maintainer_email=pkg_info["__email__"],
     packages=setuptools.find_packages(exclude=["test*"]),
-    setup_requires=[] + pytest_runner,
-    tests_require=tests_require,
-
+    package_data={MODULE_NAME: ["py.typed"]},
+    project_urls={
+        "Source": REPOSITORY_URL,
+        "Tracker": f"{REPOSITORY_URL:s}/issues",
+    },
+    python_requires=">=3.7",
+    install_requires=install_requires,
+    extras_require={
+        "logging": ["loguru>=0.4.1,<1"],
+        "test": tests_requires,
+    },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: POSIX",
-        "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
+        "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    cmdclass=get_release_command_class(),
+    zip_safe=False,
 )
```

### Comparing `DataProperty-0.9.0/PKG-INFO` & `DataProperty-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,267 +1,270 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: DataProperty
-Version: 0.9.0
+Version: 1.0.0
 Summary: Python library for extract property from data.
-
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
-Author-email: gogogo.vm@gmail.com
+Author-email: tsuyoshi.hombashi@gmail.com
+Maintainer: Tsuyoshi Hombashi
+Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Description: **DataProperty**
-        
-        .. image:: https://img.shields.io/pypi/pyversions/DataProperty.svg
-           :target: https://pypi.python.org/pypi/DataProperty
-        .. image:: https://travis-ci.org/thombashi/DataProperty.svg?branch=master
-            :target: https://travis-ci.org/thombashi/DataProperty
-        .. image:: https://ci.appveyor.com/api/projects/status/6ybxtfnle9lhykr9?svg=true
-            :target: https://ci.appveyor.com/project/thombashi/dataproperty
-        .. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
-        
-        .. contents:: Table of contents
-           :backlinks: top
-           :local:
-        
-        Summary
-        =======
-        Python library for extract property from data.
-        
-        Installation
-        ============
-        
-        ::
-        
-            pip install DataProperty
-        
-        Usage
-        =====
-        
-        Extract property of data
-        ------------------------
-        
-        e.g. Extract property of a `float` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty(-1.0)
-        
-        ::
-        
-            data=-1.0, typename=FLOAT, align=right, str_len=4, integer_digits=1, decimal_places=1, additional_format_len=1
-        
-        e.g. Extract property of a `int` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty(123456789)
-        
-        ::
-        
-            data=123456789, typename=INT, align=right, str_len=9, integer_digits=9, decimal_places=0, additional_format_len=0
-        
-        e.g. Extract property of a `str` value
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from dataproperty import DataProperty
-            DataProperty("abcdefgh")
-        
-        ::
-        
-            data=abcdefgh, typename=STRING, align=left, str_len=8, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        e.g. Extract property of a time value (from `datetime`)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import DataProperty
-            DataProperty(datetime.datetime(2017, 1, 1, 0, 0, 0))
-        
-        ::
-        
-            data=2017-01-01 00:00:00, typename=DATETIME, align=left, str_len=19, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        e.g. Extract property of a time value (from `str`)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            DataProperty("2017-01-01T01:23:45+0900")
-        
-        ::
-        
-            data=2017-01-01 01:23:45+09:00, typename=DATETIME, align=left, str_len=25, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        
-        e.g. Extract property of a `bool` value.
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            DataProperty(True)
-        
-        ::
-        
-            data=True, typename=BOOL, align=left, str_len=4, integer_digits=nan, decimal_places=nan, additional_format_len=0
-        
-        
-        Extract property of data for each data from a matrix
-        ----------------------------------------------------
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import PropertyExtractor, Typecode
-            import six
-        
-            def display(prop_matrix, name):
-                six.print_()
-                six.print_("---------- %s ----------" % (name))
-                for prop_list in prop_matrix:
-                    six.print_([getattr(prop, name) for prop in prop_list])
-        
-            dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
-            inf = float("inf")
-            nan = float("nan")
-            data_matrix = [
-                [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
-                [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
-                [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
-            ]
-            prop_extractor = PropertyExtractor()
-        
-            prop_extractor.data_matrix = data_matrix
-            prop_matrix = prop_extractor.extract_data_property_matrix()
-        
-            six.print_("---------- typename ----------")
-            for prop_list in prop_matrix:
-                six.print_([Typecode.get_typename(prop.typecode) for prop in prop_list])
-        
-            display(prop_matrix, "data")
-            display(prop_matrix, "align")
-            display(prop_matrix, "str_len")
-            display(prop_matrix, "integer_digits")
-            display(prop_matrix, "decimal_places")
-        
-        ::
-        
-            ---------- typename ----------
-            ['INT', 'FLOAT', 'STRING', 'INT', 'INT', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-            ['INT', 'FLOAT', 'STRING', 'FLOAT', 'FLOAT', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-            ['INT', 'FLOAT', 'STRING', 'INT', 'STRING', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-        
-            ---------- data ----------
-            [1, 1.1, 'aa', 1, 1, True, inf, nan, datetime.datetime(2017, 1, 1, 0, 0)]
-            [2, 2.2, 'bbb', 2.2, 2.2, False, inf, nan, datetime.datetime(2017, 1, 1, 0, 0)]
-            [3, 3.33, 'cccc', -3, 'ccc', True, inf, nan, datetime.datetime(2017, 1, 1, 1, 23, 45, tzinfo=tzoffset(None, 32400))]
-        
-            ---------- align ----------
-            [right, right, left, right, right, left, left, left, left]
-            [right, right, left, right, right, left, left, left, left]
-            [right, right, left, right, left, left, left, left, left]
-        
-            ---------- str_len ----------
-            [1, 3, 2, 1, 1, 4, 3, 3, 19]
-            [1, 3, 3, 3, 3, 5, 3, 3, 19]
-            [1, 4, 4, 2, 3, 4, 3, 3, 24]
-        
-            ---------- integer_digits ----------
-            [1, 1, nan, 1, 1, nan, nan, nan, nan]
-            [1, 1, nan, 1, 1, nan, nan, nan, nan]
-            [1, 1, nan, 1, nan, nan, nan, nan, nan]
-        
-            ---------- decimal_places ----------
-            [0, 1, nan, 0, 0, nan, nan, nan, nan]
-            [0, 1, nan, 1, 1, nan, nan, nan, nan]
-            [0, 2, nan, 0, nan, nan, nan, nan, nan]
-        
-        Extract property of data for each column from a matrix
-        ------------------------------------------------------
-        
-        .. code:: python
-        
-            import datetime
-            from dataproperty import PropertyExtractor, Typecode
-            import six
-        
-            def display(prop_list, name):
-                six.print_()
-                six.print_("---------- %s ----------" % (name))
-                six.print_([getattr(prop, name) for prop in prop_list])
-        
-            dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
-            inf = float("inf")
-            nan = float("nan")
-            data_matrix = [
-                [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
-                [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
-                [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
-            ]
-            prop_extractor = PropertyExtractor()
-        
-            prop_extractor.header_list = [
-                "int", "float", "str", "num", "mix", "bool", "inf", "nan", "time"]
-            prop_extractor.data_matrix = data_matrix
-            col_prop_list = prop_extractor.extract_column_property_list()
-        
-            six.print_("---------- typename ----------")
-            six.print_([Typecode.get_typename(prop.typecode) for prop in col_prop_list])
-        
-            display(col_prop_list, "align")
-            display(col_prop_list, "padding_len")
-            display(col_prop_list, "decimal_places")
-        
-        ::
-        
-            ---------- typename ----------
-            ['INT', 'FLOAT', 'STRING', 'FLOAT', 'STRING', 'BOOL', 'INFINITY', 'NAN', 'DATETIME']
-        
-            ---------- align ----------
-            [right, right, left, right, left, left, left, left, left]
-        
-            ---------- padding_len ----------
-            [3, 5, 4, 4, 3, 5, 3, 3, 24]
-        
-            ---------- decimal_places ----------
-            [0, 2, nan, 1, 1, nan, nan, nan, nan]
-        
-        
-        Dependencies
-        ============
-        
-        Python 2.7 or 3.3+
-        
-        - `python-dateutil <https://dateutil.readthedocs.io/en/stable/>`__
-        - `pytz <https://pypi.python.org/pypi/pytz/>`__
-        - `six <https://pypi.python.org/pypi/six/>`__
-        
-        Test dependencies
-        -----------------
-        
-        -  `pytest <https://pypi.python.org/pypi/pytest>`__
-        -  `pytest-runner <https://pypi.python.org/pypi/pytest-runner>`__
-        -  `tox <https://pypi.python.org/pypi/tox>`__
-        
-Keywords: property
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://github.com/thombashi/DataProperty
+Project-URL: Tracker, https://github.com/thombashi/DataProperty/issues
+Keywords: data,library,property
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: logging
+Provides-Extra: test
+License-File: LICENSE
+
+.. contents:: **DataProperty**
+   :backlinks: top
+   :local:
+
+
+Summary
+=======
+A Python library for extract property from data.
+
+
+.. image:: https://badge.fury.io/py/DataProperty.svg
+    :target: https://badge.fury.io/py/DataProperty
+    :alt: PyPI package version
+
+.. image:: https://anaconda.org/conda-forge/DataProperty/badges/version.svg
+    :target: https://anaconda.org/conda-forge/DataProperty
+    :alt: conda-forge package version
+
+.. image:: https://img.shields.io/pypi/pyversions/DataProperty.svg
+   :target: https://pypi.org/project/DataProperty
+    :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/implementation/DataProperty.svg
+    :target: https://pypi.org/project/DataProperty
+    :alt: Supported Python implementations
+
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/lint_and_test.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. image:: https://coveralls.io/repos/github/thombashi/DataProperty/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/DataProperty?branch=master
+    :alt: Test coverage
+
+.. image:: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/DataProperty/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
+
+Installation
+============
+
+Installation: pip
+------------------------------
+::
+
+    pip install DataProperty
+
+Installation: conda
+------------------------------
+::
+
+    conda install -c conda-forge dataproperty
+
+Installation: apt
+------------------------------
+::
+
+    sudo add-apt-repository ppa:thombashi/ppa
+    sudo apt update
+    sudo apt install python3-dataproperty
+
+
+Usage
+=====
+
+Extract property of data
+------------------------
+
+e.g. Extract a ``float`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(-1.1)
+    data=-1.1, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=1, extra_len=1
+
+e.g. Extract a ``int`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(123456789)
+    data=123456789, type=INTEGER, align=right, ascii_width=9, int_digits=9, decimal_places=0, extra_len=0
+
+e.g. Extract a ``str`` (ascii) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty("sample string")
+    data=sample string, type=STRING, align=left, length=13, ascii_width=13, extra_len=0
+
+e.g. Extract a ``str`` (multi-byte) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> str(DataProperty("吾輩は猫である"))
+    data=吾輩は猫である, type=STRING, align=left, length=7, ascii_width=14, extra_len=0
+
+e.g. Extract a time (``datetime``) value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> import datetime
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(datetime.datetime(2017, 1, 1, 0, 0, 0))
+    data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+
+e.g. Extract a ``bool`` value property
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code:: python
+
+    >>> from dataproperty import DataProperty
+    >>> DataProperty(True)
+    data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+
+
+Extract data property for each element from a matrix
+----------------------------------------------------
+``DataPropertyExtractor.to_dp_matrix`` method returns a matrix of ``DataProperty`` instances from a data matrix.
+An example data set and the result are as follows:
+
+:Sample Code:
+    .. code:: python
+
+        import datetime
+        from dataproperty import DataPropertyExtractor
+
+        dp_extractor = DataPropertyExtractor()
+        dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
+        inf = float("inf")
+        nan = float("nan")
+
+        dp_matrix = dp_extractor.to_dp_matrix([
+            [1, 1.1, "aa", 1, 1, True, inf, nan, dt],
+            [2, 2.2, "bbb", 2.2, 2.2, False, "inf", "nan", dt],
+            [3, 3.33, "cccc", -3, "ccc", "true", inf, "NAN", "2017-01-01T01:23:45+0900"],
+        ])
+
+        for row, dp_list in enumerate(dp_matrix):
+            for col, dp in enumerate(dp_list):
+                print("row={:d}, col={:d}, {}".format(row, col, str(dp)))
+
+:Output:
+    ::
+
+        row=0, col=0, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=1, data=1.1, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=0, col=2, data=aa, type=STRING, align=left, ascii_width=2, length=2, extra_len=0
+        row=0, col=3, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=4, data=1, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=0, col=5, data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+        row=0, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=0, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=0, col=8, data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+        row=1, col=0, data=2, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=1, col=1, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=2, data=bbb, type=STRING, align=left, ascii_width=3, length=3, extra_len=0
+        row=1, col=3, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=4, data=2.2, type=REAL_NUMBER, align=right, ascii_width=3, int_digits=1, decimal_places=1, extra_len=0
+        row=1, col=5, data=False, type=BOOL, align=left, ascii_width=5, extra_len=0
+        row=1, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=1, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=1, col=8, data=2017-01-01 00:00:00, type=DATETIME, align=left, ascii_width=19, extra_len=0
+        row=2, col=0, data=3, type=INTEGER, align=right, ascii_width=1, int_digits=1, decimal_places=0, extra_len=0
+        row=2, col=1, data=3.33, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=2, extra_len=0
+        row=2, col=2, data=cccc, type=STRING, align=left, ascii_width=4, length=4, extra_len=0
+        row=2, col=3, data=-3, type=INTEGER, align=right, ascii_width=2, int_digits=1, decimal_places=0, extra_len=1
+        row=2, col=4, data=ccc, type=STRING, align=left, ascii_width=3, length=3, extra_len=0
+        row=2, col=5, data=True, type=BOOL, align=left, ascii_width=4, extra_len=0
+        row=2, col=6, data=Infinity, type=INFINITY, align=left, ascii_width=8, extra_len=0
+        row=2, col=7, data=NaN, type=NAN, align=left, ascii_width=3, extra_len=0
+        row=2, col=8, data=2017-01-01T01:23:45+0900, type=STRING, align=left, ascii_width=24, length=24, extra_len=0
+
+
+Full example source code can be found at *examples/py/to_dp_matrix.py*
+
+
+Extract properties for each column from a matrix
+------------------------------------------------------
+``DataPropertyExtractor.to_column_dp_list`` method returns a list of ``DataProperty`` instances from a data matrix. The list represents the properties for each column.
+An example data set and the result are as follows:
+
+Example data set and result are as follows:
+
+:Sample Code:
+    .. code:: python
+
+        import datetime
+        from dataproperty import DataPropertyExtractor
+
+        dp_extractor = DataPropertyExtractor()
+        dt = datetime.datetime(2017, 1, 1, 0, 0, 0)
+        inf = float("inf")
+        nan = float("nan")
+
+        data_matrix = [
+            [1, 1.1,  "aa",   1,   1,     True,   inf,   nan,   dt],
+            [2, 2.2,  "bbb",  2.2, 2.2,   False,  "inf", "nan", dt],
+            [3, 3.33, "cccc", -3,  "ccc", "true", inf,   "NAN", "2017-01-01T01:23:45+0900"],
+        ]
+
+        dp_extractor.headers = ["int", "float", "str", "num", "mix", "bool", "inf", "nan", "time"]
+        col_dp_list = dp_extractor.to_column_dp_list(dp_extractor.to_dp_matrix(dp_matrix))
+
+        for col_idx, col_dp in enumerate(col_dp_list):
+            print(str(col_dp))
+
+:Output:
+    ::
+
+        column=0, type=INTEGER, align=right, ascii_width=3, bit_len=2, int_digits=1, decimal_places=0
+        column=1, type=REAL_NUMBER, align=right, ascii_width=5, int_digits=1, decimal_places=(min=1, max=2)
+        column=2, type=STRING, align=left, ascii_width=4
+        column=3, type=REAL_NUMBER, align=right, ascii_width=4, int_digits=1, decimal_places=(min=0, max=1), extra_len=(min=0, max=1)
+        column=4, type=STRING, align=left, ascii_width=3, int_digits=1, decimal_places=(min=0, max=1)
+        column=5, type=BOOL, align=left, ascii_width=5
+        column=6, type=INFINITY, align=left, ascii_width=8
+        column=7, type=NAN, align=left, ascii_width=3
+        column=8, type=STRING, align=left, ascii_width=24
+
+
+Full example source code can be found at *examples/py/to_column_dp_list.py*
+
+
+Dependencies
+============
+- Python 3.7+
+- `Python package dependencies (automatically installed) <https://github.com/thombashi/DataProperty/network/dependencies>`__
+
+Optional dependencies
+---------------------
+- `loguru <https://github.com/Delgan/loguru>`__
+    - Used for logging if the package installed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

