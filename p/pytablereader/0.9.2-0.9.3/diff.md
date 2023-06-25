# Comparing `tmp/pytablereader-0.9.2.tar.gz` & `tmp/pytablereader-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytablereader-0.9.2.tar", last modified: Fri May  5 11:06:32 2017, max compression
+gzip compressed data, was "dist/pytablereader-0.9.3.tar", last modified: Sun May 14 08:26:45 2017, max compression
```

## Comparing `pytablereader-0.9.2.tar` & `pytablereader-0.9.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/docs/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/docs/pages/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/docs/pages/introduction/
--rw-r--r--   0 travis    (1000) travis    (1000)      148 2017-05-05 11:05:19.000000 pytablereader-0.9.2/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/csv/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/csv/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6863 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/csv/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1246 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/csv/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/factory/
--rw-r--r--   0 travis    (1000) travis    (1000)      206 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/factory/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3004 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/factory/_base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5377 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/factory/_file.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8263 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/factory/_url.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/html/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/html/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4875 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/html/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3029 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/html/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/json/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/json/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7030 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/json/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4380 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/json/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/loadermanager/
--rw-r--r--   0 travis    (1000) travis    (1000)      192 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/loadermanager/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      727 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/loadermanager/_base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2320 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/loadermanager/_file.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2506 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/loadermanager/_url.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/ltsv/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/ltsv/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6093 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/ltsv/core.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/markdown/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/markdown/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4198 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/markdown/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)      581 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/markdown/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/mediawiki/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/mediawiki/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4724 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/mediawiki/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)      459 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/mediawiki/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/spreadsheet/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/spreadsheet/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1597 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/spreadsheet/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4656 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/spreadsheet/excelloader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5467 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/spreadsheet/gsloader.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/sqlite/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/sqlite/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2073 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/sqlite/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1393 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/sqlite/formatter.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader/tsv/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/tsv/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1312 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/tsv/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1383 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      597 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_acceptor.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1282 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_common.py
--rw-r--r--   0 travis    (1000) travis    (1000)      634 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_constant.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1994 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_logger.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7011 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_tabledata_sanitizer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2289 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/_validator.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1668 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/error.py
--rw-r--r--   0 travis    (1000) travis    (1000)      856 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/formatter.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4028 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/interface.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6498 2017-05-05 11:05:19.000000 pytablereader-0.9.2/pytablereader/tabledata.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     7813 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     2314 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      221 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-05-05 11:06:32.000000 pytablereader-0.9.2/pytablereader.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/requirements/
--rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-05-05 11:05:19.000000 pytablereader-0.9.2/requirements/docs_requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      221 2017-05-05 11:05:19.000000 pytablereader-0.9.2/requirements/requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       65 2017-05-05 11:05:19.000000 pytablereader-0.9.2/requirements/test_requirements.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/test/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-05 11:06:32.000000 pytablereader-0.9.2/test/data/
--rw-r--r--   0 travis    (1000) travis    (1000)    71819 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/data/python - Wiktionary.html
--rw-r--r--   0 travis    (1000) travis    (1000)     6863 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/data/validdata.xlsx
--rw-r--r--   0 travis    (1000) travis    (1000)     1727 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_common.py
--rw-r--r--   0 travis    (1000) travis    (1000)    13673 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_csv_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8015 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_excel_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7062 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_fileloader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1551 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_gsloader.py
--rw-r--r--   0 travis    (1000) travis    (1000)    21423 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_html_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)      794 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_html_reader_from_file.py
--rw-r--r--   0 travis    (1000) travis    (1000)    11265 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_json_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4193 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_loader_factory.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7643 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_ltsv_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)    12288 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_markdown_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)    13530 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_mediawiki_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6021 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_sqlite_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8375 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_tabledata.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4433 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_tabledata_sanitizer.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10537 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_tsv_reader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8532 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_urlloader.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2551 2017-05-05 11:05:19.000000 pytablereader-0.9.2/test/test_validator.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1074 2017-05-05 11:05:19.000000 pytablereader-0.9.2/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-05-05 11:05:19.000000 pytablereader-0.9.2/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     5136 2017-05-05 11:05:19.000000 pytablereader-0.9.2/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2151 2017-05-05 11:05:19.000000 pytablereader-0.9.2/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      118 2017-05-05 11:05:19.000000 pytablereader-0.9.2/tox.ini
--rw-r--r--   0 travis    (1000) travis    (1000)     7813 2017-05-05 11:06:32.000000 pytablereader-0.9.2/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-05-05 11:06:32.000000 pytablereader-0.9.2/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/docs/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/docs/pages/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/docs/pages/introduction/
+-rw-r--r--   0 travis    (1000) travis    (1000)      148 2017-05-14 08:24:15.000000 pytablereader-0.9.3/docs/pages/introduction/summary.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/csv/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/csv/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6864 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/csv/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1246 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/csv/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/factory/
+-rw-r--r--   0 travis    (1000) travis    (1000)      206 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/factory/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3005 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/factory/_base.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5377 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/factory/_file.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8263 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/factory/_url.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/html/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/html/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4876 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/html/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3030 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/html/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/json/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/json/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7031 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/json/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4381 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/json/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/loadermanager/
+-rw-r--r--   0 travis    (1000) travis    (1000)      192 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/loadermanager/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      727 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/loadermanager/_base.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2320 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/loadermanager/_file.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2506 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/loadermanager/_url.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/ltsv/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/ltsv/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6095 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/ltsv/core.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/markdown/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/markdown/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4198 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/markdown/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      581 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/markdown/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/mediawiki/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/mediawiki/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4724 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/mediawiki/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      459 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/mediawiki/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/spreadsheet/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/spreadsheet/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1598 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/spreadsheet/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4656 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/spreadsheet/excelloader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5467 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/spreadsheet/gsloader.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/sqlite/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/sqlite/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2073 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/sqlite/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1393 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/sqlite/formatter.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader/tsv/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/tsv/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1312 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/tsv/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1383 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      598 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_acceptor.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1282 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      634 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_constant.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1994 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_logger.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7011 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_tabledata_sanitizer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2289 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/_validator.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1668 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/error.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      857 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/formatter.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4028 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/interface.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6499 2017-05-14 08:24:15.000000 pytablereader-0.9.3/pytablereader/tabledata.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     7813 2017-05-14 08:26:44.000000 pytablereader-0.9.3/pytablereader.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     2314 2017-05-14 08:26:45.000000 pytablereader-0.9.3/pytablereader.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-14 08:26:44.000000 pytablereader-0.9.3/pytablereader.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      221 2017-05-14 08:26:44.000000 pytablereader-0.9.3/pytablereader.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-05-14 08:26:44.000000 pytablereader-0.9.3/pytablereader.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/requirements/
+-rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-05-14 08:24:15.000000 pytablereader-0.9.3/requirements/docs_requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      221 2017-05-14 08:24:15.000000 pytablereader-0.9.3/requirements/requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       65 2017-05-14 08:24:15.000000 pytablereader-0.9.3/requirements/test_requirements.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/test/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-14 08:26:45.000000 pytablereader-0.9.3/test/data/
+-rw-r--r--   0 travis    (1000) travis    (1000)    71819 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/data/python - Wiktionary.html
+-rw-r--r--   0 travis    (1000) travis    (1000)     6863 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/data/validdata.xlsx
+-rw-r--r--   0 travis    (1000) travis    (1000)     1727 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    13673 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_csv_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8015 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_excel_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7062 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_fileloader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1551 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_gsloader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    21423 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_html_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      794 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_html_reader_from_file.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    11265 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_json_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4193 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_loader_factory.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7643 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_ltsv_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    12288 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_markdown_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    13530 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_mediawiki_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5963 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_sqlite_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8375 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_tabledata.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4433 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_tabledata_sanitizer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10537 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_tsv_reader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8532 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_urlloader.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2551 2017-05-14 08:24:15.000000 pytablereader-0.9.3/test/test_validator.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1074 2017-05-14 08:24:15.000000 pytablereader-0.9.3/LICENSE
+-rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-05-14 08:24:15.000000 pytablereader-0.9.3/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     5136 2017-05-14 08:24:15.000000 pytablereader-0.9.3/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)     2151 2017-05-14 08:24:15.000000 pytablereader-0.9.3/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      118 2017-05-14 08:24:15.000000 pytablereader-0.9.3/tox.ini
+-rw-r--r--   0 travis    (1000) travis    (1000)     7813 2017-05-14 08:26:45.000000 pytablereader-0.9.3/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-05-14 08:26:45.000000 pytablereader-0.9.3/setup.cfg
```

### Comparing `pytablereader-0.9.2/pytablereader/csv/core.py` & `pytablereader-0.9.3/pytablereader/csv/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import csv
 import io
 import platform
 
 from mbstrdecoder import MultiByteStrDecoder
 import six
 import typepy
```

### Comparing `pytablereader-0.9.2/pytablereader/csv/formatter.py` & `pytablereader-0.9.3/pytablereader/csv/formatter.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/factory/_base.py` & `pytablereader-0.9.3/pytablereader/factory/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import abc
 
 import six
 
 from ..error import LoaderNotFoundError
```

### Comparing `pytablereader-0.9.2/pytablereader/factory/_file.py` & `pytablereader-0.9.3/pytablereader/factory/_file.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/factory/_url.py` & `pytablereader-0.9.3/pytablereader/factory/_url.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/html/core.py` & `pytablereader-0.9.3/pytablereader/html/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import io
 
 from .._constant import TableNameTemplate as tnt
 from .._logger import (
     FileSourceLogger,
     TextSourceLogger,
 )
```

### Comparing `pytablereader-0.9.2/pytablereader/html/formatter.py` & `pytablereader-0.9.3/pytablereader/html/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import re
 
 import bs4
 import typepy
 
 from .._constant import TableNameTemplate as tnt
 from ..error import InvalidDataError
```

### Comparing `pytablereader-0.9.2/pytablereader/json/core.py` & `pytablereader-0.9.3/pytablereader/json/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import json
 
 from .._constant import (
     SourceType,
     TableNameTemplate as tnt
 )
 from .._logger import (
```

### Comparing `pytablereader-0.9.2/pytablereader/json/formatter.py` & `pytablereader-0.9.3/pytablereader/json/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import abc
 
 import jsonschema
 import six
 
 from .._constant import TableNameTemplate as tnt
 from ..error import ValidationError
```

### Comparing `pytablereader-0.9.2/pytablereader/loadermanager/_base.py` & `pytablereader-0.9.3/pytablereader/loadermanager/_base.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/loadermanager/_file.py` & `pytablereader-0.9.3/pytablereader/loadermanager/_file.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/loadermanager/_url.py` & `pytablereader-0.9.3/pytablereader/loadermanager/_url.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/ltsv/core.py` & `pytablereader-0.9.3/pytablereader/ltsv/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import io
 
 import typepy
+
 import pathvalidate as pv
 
 from .._constant import TableNameTemplate as tnt
 from .._logger import (
     FileSourceLogger,
     TextSourceLogger,
 )
```

### Comparing `pytablereader-0.9.2/pytablereader/markdown/core.py` & `pytablereader-0.9.3/pytablereader/markdown/core.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/markdown/formatter.py` & `pytablereader-0.9.3/pytablereader/markdown/formatter.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/mediawiki/core.py` & `pytablereader-0.9.3/pytablereader/mediawiki/core.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/spreadsheet/core.py` & `pytablereader-0.9.3/pytablereader/spreadsheet/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
+
 import abc
 
 from .._constant import TableNameTemplate as tnt
 from ..interface import TableLoader
 
 
 class SpreadSheetLoader(TableLoader):
```

### Comparing `pytablereader-0.9.2/pytablereader/spreadsheet/excelloader.py` & `pytablereader-0.9.3/pytablereader/spreadsheet/excelloader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/spreadsheet/gsloader.py` & `pytablereader-0.9.3/pytablereader/spreadsheet/gsloader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/sqlite/core.py` & `pytablereader-0.9.3/pytablereader/sqlite/core.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/sqlite/formatter.py` & `pytablereader-0.9.3/pytablereader/sqlite/formatter.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/tsv/core.py` & `pytablereader-0.9.3/pytablereader/tsv/core.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/__init__.py` & `pytablereader-0.9.3/pytablereader/__init__.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/_acceptor.py` & `pytablereader-0.9.3/pytablereader/_acceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # encoding: utf-8
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
+
 import abc
 
 import six
 
 
 @six.add_metaclass(abc.ABCMeta)
 class LoaderAcceptorInterface(object):
```

### Comparing `pytablereader-0.9.2/pytablereader/_common.py` & `pytablereader-0.9.3/pytablereader/_common.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/_constant.py` & `pytablereader-0.9.3/pytablereader/_constant.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/_logger.py` & `pytablereader-0.9.3/pytablereader/_logger.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/_tabledata_sanitizer.py` & `pytablereader-0.9.3/pytablereader/_tabledata_sanitizer.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/_validator.py` & `pytablereader-0.9.3/pytablereader/_validator.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/error.py` & `pytablereader-0.9.3/pytablereader/error.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/formatter.py` & `pytablereader-0.9.3/pytablereader/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # encoding: utf-8
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
+
 import abc
 
 import six
 
 from ._acceptor import LoaderAcceptor
 from .error import InvalidDataError
```

### Comparing `pytablereader-0.9.2/pytablereader/interface.py` & `pytablereader-0.9.3/pytablereader/interface.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/pytablereader/tabledata.py` & `pytablereader-0.9.3/pytablereader/tabledata.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             |True| if the data :py:attr:`.header_list` or
             :py:attr:`.value_matrix` is empty.
         :rtype: bool
         """
 
         return any([self.is_empty_header(), self.is_empty_record()])
 
-    def asdict(self):
+    def as_dict(self):
         """
         :return: Table data as a |dict| instance.
         :rtype: dict
         """
 
         self.__dp_extractor.float_type = float
 
@@ -161,14 +161,20 @@
             if typepy.is_empty_sequence(dict_record):
                 continue
 
             dict_body.append(dict(dict_record))
 
         return {self.table_name: dict_body}
 
+    def asdict(self):
+        return self.asdict()
+
+        # alias to as_dict method.
+        # this method will be deleted in the future.
+
     def as_dataframe(self):
         """
         :return: Table data as a ``pandas.DataFrame`` instance.
         :rtype: pandas.DataFrame
 
         .. note::
             ``Pandas`` package required to execute this method.
@@ -237,13 +243,7 @@
         if typepy.is_empty_sequence(self.header_list):
             return record_list
 
         return [
             self.__to_record(record)
             for record in record_list
         ]
-
-    def as_dict(self):
-        return self.asdict()
-
-        # alias to asdict method.
-        # this method will be deleted in the future.
```

### Comparing `pytablereader-0.9.2/pytablereader.egg-info/PKG-INFO` & `pytablereader-0.9.3/pytablereader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pytablereader
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library to load structured table data from files/URL with various data format: CSV/Excel/Google-Sheets/HTML/JSON/LTSV/Markdown/SQLite/TSV.
 
 Home-page: https://github.com/thombashi/pytablereader
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: pytablereader
```

### Comparing `pytablereader-0.9.2/pytablereader.egg-info/SOURCES.txt` & `pytablereader-0.9.3/pytablereader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/data/python - Wiktionary.html` & `pytablereader-0.9.3/test/data/python - Wiktionary.html`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/data/validdata.xlsx` & `pytablereader-0.9.3/test/data/validdata.xlsx`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_common.py` & `pytablereader-0.9.3/test/test_common.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_csv_reader.py` & `pytablereader-0.9.3/test/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_excel_reader.py` & `pytablereader-0.9.3/test/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_fileloader.py` & `pytablereader-0.9.3/test/test_fileloader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_gsloader.py` & `pytablereader-0.9.3/test/test_gsloader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_html_reader.py` & `pytablereader-0.9.3/test/test_html_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_html_reader_from_file.py` & `pytablereader-0.9.3/test/test_html_reader_from_file.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_json_reader.py` & `pytablereader-0.9.3/test/test_json_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_loader_factory.py` & `pytablereader-0.9.3/test/test_loader_factory.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_ltsv_reader.py` & `pytablereader-0.9.3/test/test_ltsv_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_markdown_reader.py` & `pytablereader-0.9.3/test/test_markdown_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_mediawiki_reader.py` & `pytablereader-0.9.3/test/test_mediawiki_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_sqlite_reader.py` & `pytablereader-0.9.3/test/test_sqlite_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 """
 
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import collections
 from decimal import Decimal
-import io
 
 from path import Path
-from pytablereader import InvalidTableNameError
 from pytablereader import TableData
 from pytablereader.interface import TableLoader
 import pytest
 from simplesqlite import SimpleSQLite
 
 import pytablereader as ptr
 import pytablewriter as ptw
```

### Comparing `pytablereader-0.9.2/test/test_tabledata.py` & `pytablereader-0.9.3/test/test_tabledata.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_tabledata_sanitizer.py` & `pytablereader-0.9.3/test/test_tabledata_sanitizer.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_tsv_reader.py` & `pytablereader-0.9.3/test/test_tsv_reader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_urlloader.py` & `pytablereader-0.9.3/test/test_urlloader.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/test/test_validator.py` & `pytablereader-0.9.3/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/LICENSE` & `pytablereader-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/README.rst` & `pytablereader-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytablereader-0.9.2/setup.py` & `pytablereader-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     install_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     tests_require = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name="pytablereader",
-    version="0.9.2",
+    version="0.9.3",
     url="https://github.com/thombashi/pytablereader",
 
     author="Tsuyoshi Hombashi",
     author_email="gogogo.vm@gmail.com",
     description=summary,
     include_package_data=True,
     install_requires=install_requires,
```

### Comparing `pytablereader-0.9.2/PKG-INFO` & `pytablereader-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pytablereader
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library to load structured table data from files/URL with various data format: CSV/Excel/Google-Sheets/HTML/JSON/LTSV/Markdown/SQLite/TSV.
 
 Home-page: https://github.com/thombashi/pytablereader
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: pytablereader
```

