# Comparing `tmp/pytablewriter-0.9.0.tar.gz` & `tmp/pytablewriter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytablewriter-0.9.0.tar", last modified: Sun Jul 31 02:16:41 2016, max compression
+gzip compressed data, was "pytablewriter-1.0.0.tar", last modified: Sun Jun 25 09:55:55 2023, max compression
```

## Comparing `pytablewriter-0.9.0.tar` & `pytablewriter-1.0.0.tar`

### file list

```diff
@@ -1,63 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/docs/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/docs/pages/introduction/
--rwxrwxrwx   0 root         (0) root         (0)      152 2016-07-23 14:09:39.000000 pytablewriter-0.9.0/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/pytablewriter/
--rwxrwxrwx   0 root         (0) root         (0)      965 2016-07-31 01:38:45.000000 pytablewriter-0.9.0/pytablewriter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      448 2016-07-27 12:58:38.000000 pytablewriter-0.9.0/pytablewriter/_converter.py
--rwxrwxrwx   0 root         (0) root         (0)     1004 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_csv_writer.py
--rwxrwxrwx   0 root         (0) root         (0)      878 2016-07-31 01:31:48.000000 pytablewriter-0.9.0/pytablewriter/_error.py
--rwxrwxrwx   0 root         (0) root         (0)     3244 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_excel_workbook.py
--rwxrwxrwx   0 root         (0) root         (0)    12264 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_excel_writer.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_function.py
--rwxrwxrwx   0 root         (0) root         (0)     2435 2016-07-27 13:19:29.000000 pytablewriter-0.9.0/pytablewriter/_html_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     1271 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_interface.py
--rwxrwxrwx   0 root         (0) root         (0)     2761 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_javascript_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     3475 2016-07-27 13:19:57.000000 pytablewriter-0.9.0/pytablewriter/_json_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     2258 2016-07-27 12:59:27.000000 pytablewriter-0.9.0/pytablewriter/_md_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     2214 2016-07-27 13:20:09.000000 pytablewriter-0.9.0/pytablewriter/_mediawiki_writer.py
--rwxrwxrwx   0 root         (0) root         (0)      767 2016-07-31 01:39:59.000000 pytablewriter-0.9.0/pytablewriter/_null_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     3129 2016-07-27 13:20:15.000000 pytablewriter-0.9.0/pytablewriter/_pandas_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     1333 2016-07-27 12:58:52.000000 pytablewriter-0.9.0/pytablewriter/_python_code_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     4895 2016-07-27 13:12:20.000000 pytablewriter-0.9.0/pytablewriter/_rst_writer.py
--rwxrwxrwx   0 root         (0) root         (0)    12080 2016-07-31 02:06:29.000000 pytablewriter-0.9.0/pytablewriter/_table_writer.py
--rwxrwxrwx   0 root         (0) root         (0)    10021 2016-07-27 13:20:39.000000 pytablewriter-0.9.0/pytablewriter/_text_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/pytablewriter.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10765 2016-07-31 02:16:40.000000 pytablewriter-0.9.0/pytablewriter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1409 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/pytablewriter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2016-07-31 02:16:40.000000 pytablewriter-0.9.0/pytablewriter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2016-07-31 02:16:40.000000 pytablewriter-0.9.0/pytablewriter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2016-07-31 02:16:40.000000 pytablewriter-0.9.0/pytablewriter.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       17 2016-02-14 06:04:47.000000 pytablewriter-0.9.0/requirements/docs_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       69 2016-07-27 13:26:31.000000 pytablewriter-0.9.0/requirements/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       35 2016-07-03 00:52:17.000000 pytablewriter-0.9.0/requirements/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/ss/
--rwxrwxrwx   0 root         (0) root         (0)     6798 2016-07-10 03:23:47.000000 pytablewriter-0.9.0/ss/excel_multi.png
--rwxrwxrwx   0 root         (0) root         (0)     6497 2016-07-10 03:23:00.000000 pytablewriter-0.9.0/ss/excel_single.png
--rwxrwxrwx   0 root         (0) root         (0)    14571 2016-07-10 03:08:00.000000 pytablewriter-0.9.0/ss/markdown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/test/
--rwxrwxrwx   0 root         (0) root         (0)        0 2016-05-17 13:07:13.000000 pytablewriter-0.9.0/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      212 2016-07-04 13:44:25.000000 pytablewriter-0.9.0/test/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     1766 2016-07-27 12:59:36.000000 pytablewriter-0.9.0/test/data.py
--rwxrwxrwx   0 root         (0) root         (0)     4411 2016-07-27 12:59:36.000000 pytablewriter-0.9.0/test/test_csv_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7366 2016-07-24 01:52:37.000000 pytablewriter-0.9.0/test/test_excel_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7228 2016-07-31 01:38:58.000000 pytablewriter-0.9.0/test/test_html_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7277 2016-07-23 15:12:11.000000 pytablewriter-0.9.0/test/test_javascript_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7729 2016-07-23 13:03:47.000000 pytablewriter-0.9.0/test/test_json_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7095 2016-07-23 13:03:47.000000 pytablewriter-0.9.0/test/test_md_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     7068 2016-07-23 13:34:02.000000 pytablewriter-0.9.0/test/test_mediawiki_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     1308 2016-07-23 12:54:47.000000 pytablewriter-0.9.0/test/test_null_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     4790 2016-07-31 01:40:57.000000 pytablewriter-0.9.0/test/test_pandas_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     5161 2016-07-23 13:31:00.000000 pytablewriter-0.9.0/test/test_python_code_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     5261 2016-07-23 13:29:55.000000 pytablewriter-0.9.0/test/test_rst_csv_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     6969 2016-07-31 01:43:11.000000 pytablewriter-0.9.0/test/test_rst_grid_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     4550 2016-07-31 01:43:37.000000 pytablewriter-0.9.0/test/test_rst_simple_writer.py
--rwxrwxrwx   0 root         (0) root         (0)     1105 2016-05-23 13:29:06.000000 pytablewriter-0.9.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      246 2016-06-19 09:35:29.000000 pytablewriter-0.9.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     7677 2016-07-24 05:11:32.000000 pytablewriter-0.9.0/README.rst
--rwxrwxrwx   0 root         (0) root         (0)     1986 2016-07-31 02:08:20.000000 pytablewriter-0.9.0/setup.py
--rwxrwxrwx   0 root         (0) root         (0)      105 2016-05-23 13:40:42.000000 pytablewriter-0.9.0/tox.ini
--rw-r--r--   0 root         (0) root         (0)    10765 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      107 2016-07-31 02:16:41.000000 pytablewriter-0.9.0/setup.cfg
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      265 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    30383 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    27869 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.840155 pytablewriter-1.0.0/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.840155 pytablewriter-1.0.0/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.850155 pytablewriter-1.0.0/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/docs/pages/introduction/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1527 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.850155 pytablewriter-1.0.0/pytablewriter/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2942 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      238 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_converter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10869 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_factory.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2370 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_function.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.850155 pytablewriter-1.0.0/pytablewriter/_logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3119 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9569 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_table_format.py
+-rw-r--r--   0 toor      (1000) toor      (1000)   109604 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/_typing.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      787 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.860155 pytablewriter-1.0.0/pytablewriter/sanitizer/
+-rw-r--r--   0 toor      (1000) toor      (1000)      703 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2898 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      733 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_elasticsearch.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2458 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_excel.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      936 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3570 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_javascript.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3072 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/sanitizer/_python.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.860155 pytablewriter-1.0.0/pytablewriter/style/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1006 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      549 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_cell.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      311 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_font.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11695 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_style.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6971 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_styler.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      828 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_styler_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2026 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/style/_theme.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.860155 pytablewriter-1.0.0/pytablewriter/typehint/
+-rw-r--r--   0 toor      (1000) toor      (1000)      545 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/typehint/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.860155 pytablewriter-1.0.0/pytablewriter/writer/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1766 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      221 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6252 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_elasticsearch.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2564 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1671 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_msgfy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1520 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_null.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    38810 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/_table_writer.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.860155 pytablewriter-1.0.0/pytablewriter/writer/binary/
+-rw-r--r--   0 toor      (1000) toor      (1000)      281 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    15368 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/_excel.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3753 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/_excel_workbook.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1447 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2452 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/_pandas.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2772 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/binary/_sqlite.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/pytablewriter/writer/text/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1298 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4212 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_asciidoc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      982 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_borderless.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      554 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5503 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_css.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1480 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_csv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5986 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_html.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      634 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5067 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_json.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1253 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_jsonlines.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6302 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_latex.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1483 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_ltsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5281 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_markdown.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3102 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_mediawiki.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6872 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_rst.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      869 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_spacealigned.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    20810 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_text_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2192 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_toml.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      438 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_tsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3499 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_unicode.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1970 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/_yaml.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/
+-rw-r--r--   0 toor      (1000) toor      (1000)      297 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4695 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_javascript.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1970 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_numpy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2546 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_pandas.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2526 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_python.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2285 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_sourcecode.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.850155 pytablewriter-1.0.0/pytablewriter.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    30383 2023-06-25 09:55:55.000000 pytablewriter-1.0.0/pytablewriter.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4717 2023-06-25 09:55:55.000000 pytablewriter-1.0.0/pytablewriter.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 09:55:55.000000 pytablewriter-1.0.0/pytablewriter.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-25 09:55:08.000000 pytablewriter-1.0.0/pytablewriter.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)     1409 2023-06-25 09:55:55.000000 pytablewriter-1.0.0/pytablewriter.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-06-25 09:55:55.000000 pytablewriter-1.0.0/pytablewriter.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      136 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      134 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     5012 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/ss/
+-rw-r--r--   0 toor      (1000) toor      (1000)    21221 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/ss/color_filter.png
+-rw-r--r--   0 toor      (1000) toor      (1000)     6497 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/ss/excel_single.png
+-rw-r--r--   0 toor      (1000) toor      (1000)    17833 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/ss/jupyter_notebook.png
+-rw-r--r--   0 toor      (1000) toor      (1000)    14571 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/ss/markdown.png
+-rw-r--r--   0 toor      (1000) toor      (1000)    16769 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/ss/multi_byte_char.png
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      321 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3159 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/data.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/test/sanitizer/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1161 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2382 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/test_elasticsearch.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3141 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/test_excel.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5318 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/test_js_var_name.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4988 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/sanitizer/test_python_var_name.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2647 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/test_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      564 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8951 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/test_style.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3833 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/test_table_format.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10126 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/test_writer_factory.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/test/writer/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.870155 pytablewriter-1.0.0/test/writer/binary/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/binary/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9662 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/binary/test_excel_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4634 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/binary/test_pandas_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8425 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/binary/test_sqlite_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6354 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/test_elasticsearch_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1397 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/test_null_writer.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/test/writer/text/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      203 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/_common.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/test/writer/text/rst/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/rst/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6875 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/rst/test_rst_csv_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11959 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/rst/test_rst_grid_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6337 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/rst/test_rst_simple_writer.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-25 09:55:55.880155 pytablewriter-1.0.0/test/writer/text/sourcecode/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/sourcecode/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16054 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/sourcecode/test_javascript_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6388 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/sourcecode/test_numpy_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9685 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/sourcecode/test_pandas_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7278 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/sourcecode/test_python_code_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10261 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_asciidoc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1320 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_borderless_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9131 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_css.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7845 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_csv_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14391 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_html_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10602 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_json_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4266 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_jsonlines_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4792 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_latex_matrix_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3776 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_latex_table_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3285 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_ltsv_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    51368 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_markdown_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11594 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_mediawiki_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1414 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_multibyte.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2913 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_space_aligned_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4340 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_toml_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2695 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_tsv_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6809 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_unicode_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3668 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/test/writer/text/test_yaml_writer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1384 2023-06-25 09:54:51.000000 pytablewriter-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_error.py` & `pytablewriter-1.0.0/pytablewriter/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
-
 
 class NotSupportedError(Exception):
     pass
 
 
 class EmptyTableNameError(Exception):
     """
-    Raised when a table writer class of the |table_name| attribute is null
-    and the class is not accepted null |table_name|.
+    Exception raised when a table writer class of the |table_name| attribute
+    is null and the class is not accepted null |table_name|.
     """
 
 
-class EmptyHeaderError(Exception):
+class EmptyValueError(Exception):
     """
-    Raised when a table writer class of the |header_list| attribute is null
-    and the class is not accepted null |header_list|.
+    Exception raised when a table writer class of the |value_matrix| attribute
+    is null, and the class is not accepted null |value_matrix|.
     """
 
 
-class EmptyValueError(Exception):
+class EmptyTableDataError(Exception):
     """
-    Raised when a table writer class of the |value_matrix| attribute is null
-    and the class is not accepted null |value_matrix|.
+    Exception raised when a table writer class of the |headers| and
+    |value_matrix| attributes are null.
     """
 
 
-class EmptyTableDataError(Exception):
+class WriterNotFoundError(Exception):
     """
-    Raised when a table writer class of the |header_list| and |value_matrix|
-    attributes are null
+    Exception raised when appropriate loader writer found.
     """
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_excel_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/binary/_excel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,442 +1,505 @@
-# encoding: utf-8
-
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
-
-from __future__ import absolute_import
 import abc
+import copy
+import warnings
+from typing import Any, ClassVar, Dict, Optional, Union, cast
+
+import dataproperty
+import typepy
+from dataproperty import DataProperty
+from tabledata import TableData
+from typepy import Integer
+
+from .._common import import_error_msg_template
+from ._excel_workbook import ExcelWorkbookInterface, ExcelWorkbookXls, ExcelWorkbookXlsx
+from ._interface import AbstractBinaryTableWriter
 
-import dataproperty as dp
-from dataproperty.type import IntegerTypeChecker
-from six.moves import range
-import xlwt
-
-from ._converter import str_datetime_converter
-from ._excel_workbook import ExcelWorkbookXls
-from ._excel_workbook import ExcelWorkbookXlsx
-from ._interface import TextWriterInterface
-from ._table_writer import TableWriter
 
-
-class ExcelTableWriter(TableWriter, TextWriterInterface):
+class ExcelTableWriter(AbstractBinaryTableWriter, metaclass=abc.ABCMeta):
     """
-    Abstract class of a table writer for Excel format.
+    An abstract class of a table writer for Excel file format.
     """
 
+    FORMAT_NAME = "excel"
+
     @property
-    def support_split_write(self):
-        return True
+    def format_name(self) -> str:
+        return self.FORMAT_NAME
 
     @property
-    def workbook(self):
+    def workbook(self) -> Optional[ExcelWorkbookInterface]:
         return self._workbook
 
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+        self._workbook: Optional[ExcelWorkbookInterface] = None
+
+        self._dp_extractor.type_value_map = {
+            typepy.Typecode.INFINITY: "Inf",
+            typepy.Typecode.NAN: "NaN",
+        }
+
+        self._first_header_row = 0
+        self._last_header_row = self.first_header_row
+        self._first_data_row = self.last_header_row + 1
+        self._first_data_col = 0
+        self._last_data_row: Optional[int] = None
+        self._last_data_col: Optional[int] = None
+
+        self._current_data_row = self._first_data_row
+
+        self._quoting_flags = copy.deepcopy(dataproperty.NOT_QUOTING_FLAGS)
+        self._quoting_flags[typepy.Typecode.DATETIME] = True
+
     @property
-    def first_header_row(self):
+    def first_header_row(self) -> int:
         """
         :return: Index of the first row of the header.
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._first_header_row
 
     @property
-    def last_header_row(self):
+    def last_header_row(self) -> int:
         """
         :return: Index of the last row of the header.
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._last_header_row
 
     @property
-    def first_data_row(self):
+    def first_data_row(self) -> int:
         """
         :return: Index of the first row of the data (table body).
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._first_data_row
 
     @property
-    def last_data_row(self):
+    def last_data_row(self) -> Optional[int]:
         """
         :return: Index of the last row of the data (table body).
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._last_data_row
 
     @property
-    def first_data_col(self):
+    def first_data_col(self) -> int:
         """
         :return: Index of the first column of the table.
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._first_data_col
 
     @property
-    def last_data_col(self):
+    def last_data_col(self) -> Optional[int]:
         """
         :return: Index of the last column of the table.
         :rtype: int
 
         .. note:: |excel_attr|
         """
 
         return self._last_data_col
 
-    def __init__(self):
-        super(ExcelTableWriter, self).__init__()
+    def is_opened(self) -> bool:
+        return self.workbook is not None
 
-        self.stream = None
-        self._workbook = None
-
-        self._prop_extractor.inf_value = "Inf"
-        self._prop_extractor.nan_value = "NaN"
-        self._prop_extractor.datetime_converter = str_datetime_converter
-        self._prop_extractor.datetime_format_str = "s"
+    def open(self, file_path: str) -> None:
+        """
+        Open an Excel workbook file.
 
-        self._first_header_row = 0
-        self._last_header_row = self.first_header_row
-        self._first_data_row = self.last_header_row + 1
-        self._first_data_col = 0
-        self._last_data_row = None
-        self._last_data_col = None
+        :param str file_path: Excel workbook file path to open.
+        """
 
-        self._current_data_row = self._first_data_row
+        if self.workbook and self.workbook.file_path == file_path:
+            self._logger.logger.debug(f"workbook already opened: {self.workbook.file_path}")
+            return
 
-    @abc.abstractproperty
-    def open_workbook(self, workbook_path):
-        """
-        Open workbook.
+        self.close()
+        self._open(file_path)
 
-        :param str workbook_path: File path to open.
-        """
+    @abc.abstractmethod
+    def _open(self, workbook_path: str) -> None:  # pragma: no cover
+        pass
 
-    def close(self):
+    def close(self) -> None:
         """
         Close the current workbook.
         """
 
-        if self.workbook is not None:
-            self.workbook.close()
+        if self.is_opened():
+            self.workbook.close()  # type: ignore
             self._workbook = None
 
-    def make_worksheet(self, sheet_name):
+    def from_tabledata(self, value: TableData, is_overwrite_table_name: bool = True) -> None:
+        """
+        Set following attributes from |TableData|
+
+        - :py:attr:`~.table_name`.
+        - :py:attr:`~.headers`.
+        - :py:attr:`~.value_matrix`.
+
+        And create worksheet named from :py:attr:`~.table_name` ABC
+        if not existed yet.
+
+        :param tabledata.TableData value: Input table data.
         """
-        Make a worksheet to the current workbook.
 
-        :param str sheet_name:
-            Name of the worksheet to create. Name of the work sheet will
-            automatically decided (like ``"Sheet1"``)
-            if the ``sheet_name`` is empty.
+        super().from_tabledata(value)
+
+        if self.is_opened():
+            self.make_worksheet(self.table_name)
+
+    def make_worksheet(self, sheet_name: Optional[str] = None) -> None:
+        """Make a worksheet to the current workbook.
+
+        Args:
+            sheet_name (str):
+                Name of the worksheet to create. The name will be automatically generated
+                (like ``"Sheet1"``) if the ``sheet_name`` is empty.
         """
 
         if sheet_name is None:
+            sheet_name = self.table_name
+        if not sheet_name:
             sheet_name = ""
-        self.stream = self.workbook.add_worksheet(sheet_name)
+
+        self._stream = self.workbook.add_worksheet(sheet_name)  # type: ignore
         self._current_data_row = self._first_data_row
 
-    def write_null_line(self):
-        pass
+    def dump(self, output: str, close_after_write: bool = True, **kwargs) -> None:
+        """Write a worksheet to the current workbook.
 
-    def write_table(self):
+        Args:
+            output (str):
+                Path to the workbook file to write.
+            close_after_write (bool, optional):
+                Close the workbook after write.
+                Defaults to |True|.
         """
-        Write a table to the current worksheet.
 
-        :raises IOError: If failed to write data to the worksheet.
-        """
+        self.open(output)
+        try:
+            self.make_worksheet(self.table_name)
+            self.write_table(**kwargs)
+        finally:
+            if close_after_write:
+                self.close()
 
-        self._verify_property()
-        self._preprocess_property()
+    @abc.abstractmethod
+    def _write_header(self) -> None:
+        pass
+
+    @abc.abstractmethod
+    def _write_cell(self, row: int, col: int, value_dp: DataProperty) -> None:
+        pass
 
+    def _write_table(self, **kwargs) -> None:
+        self._preprocess_table_dp()
+        self._preprocess_table_property()
         self._write_header()
         self._write_value_matrix()
-
         self._postprocess()
 
-    def _write_value_row_separator(self):
-        pass
-
-    def _write_value_matrix(self):
-        for value_prop_list in self._value_prop_matrix:
-            for col, prop in enumerate(value_prop_list):
-                self._write_cell(self._current_data_row, col, prop)
+    def _write_value_matrix(self) -> None:
+        for value_dp_list in self._table_value_dp_matrix:
+            for col_idx, value_dp in enumerate(value_dp_list):
+                self._write_cell(self._current_data_row, col_idx, value_dp)
 
             self._current_data_row += 1
 
-    def _get_last_column(self):
-        if dp.is_not_empty_sequence(self.header_list):
-            return len(self.header_list) - 1
+    def _get_last_column(self) -> int:
+        if typepy.is_not_empty_sequence(self.headers):
+            return len(self.headers) - 1
 
-        if dp.is_not_empty_sequence(self.value_matrix):
+        if typepy.is_not_empty_sequence(self.value_matrix):
             return len(self.value_matrix[0]) - 1
 
-        raise ValueError()
+        raise ValueError("data not found")
 
-    def _postprocess(self):
+    def _postprocess(self) -> None:
         self._last_data_row = self._current_data_row
         self._last_data_col = self._get_last_column()
 
 
 class ExcelXlsTableWriter(ExcelTableWriter):
     """
-    Concrete class of a table writer for Excel format
-    (older or equal to Office 2003).
+    A table writer class for Excel file format: ``.xls`` (older or equal to Office 2003).
+
+    ``xlwt`` package required to use this class.
+
+    .. py:method:: write_table()
+
+        Write a table to the current opened worksheet.
+
+        :raises IOError: If failed to write data to the worksheet.
+
+        .. note::
+            Specific values in the tabular data are converted when writing:
+
+            - |None|: written as an empty string
+            - |inf|: written as ``Inf``
+            - |nan|: written as ``NaN``
     """
 
-    def __init__(self):
-        super(ExcelXlsTableWriter, self).__init__()
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
-        self.__col_style_table = {}
+        self.__col_style_table: Dict[int, Any] = {}
 
-    def open_workbook(self, workbook_path):
+    def _open(self, workbook_path: str) -> None:
         self._workbook = ExcelWorkbookXls(workbook_path)
 
-    def _write_header(self):
-        if any([
-            not self.is_write_header,
-            dp.is_empty_sequence(self.header_list),
-        ]):
+    def _write_header(self) -> None:
+        if not self.is_write_header or typepy.is_empty_sequence(self.headers):
             return
 
-        for col, value in enumerate(self.header_list):
+        for col, value in enumerate(self.headers):
             self.stream.write(self.first_header_row, col, value)
 
-    def _write_cell(self, row, col, prop):
-        if prop.typecode in [dp.Typecode.FLOAT]:
+    def _write_cell(self, row: int, col: int, value_dp: DataProperty) -> None:
+        if value_dp.typecode in [typepy.Typecode.REAL_NUMBER]:
             try:
                 cell_style = self.__get_cell_style(col)
             except ValueError:
                 pass
             else:
-                self.stream.write(
-                    row, col, prop.data, cell_style)
+                self.stream.write(row, col, value_dp.data, cell_style)
                 return
 
-        self.stream.write(row, col, prop.data)
+        self.stream.write(row, col, value_dp.data)
 
-    def _postprocess(self):
-        super(ExcelXlsTableWriter, self)._postprocess()
+    def _postprocess(self) -> None:
+        super()._postprocess()
 
         self.__col_style_table = {}
 
-    def __get_cell_style(self, col):
+    def __get_cell_style(self, col: int):
+        try:
+            import xlwt
+        except ImportError:
+            warnings.warn(import_error_msg_template.format("excel"))
+            raise
+
         if col in self.__col_style_table:
             return self.__col_style_table.get(col)
 
         try:
-            col_prop = self._column_prop_list[col]
+            col_dp = self._column_dp_list[col]
         except KeyError:
             return {}
 
-        if col_prop.typecode not in [dp.Typecode.FLOAT]:
+        if col_dp.typecode not in [typepy.Typecode.REAL_NUMBER]:
             raise ValueError()
 
-        if not IntegerTypeChecker(col_prop.minmax_decimal_places.max_value).is_type():
+        if not Integer(col_dp.minmax_decimal_places.max_value).is_type():
             raise ValueError()
 
-        float_digit = col_prop.minmax_decimal_places.max_value
+        float_digit = col_dp.minmax_decimal_places.max_value
         if float_digit <= 0:
             raise ValueError()
 
-        num_format_str = "#,{:s}0.{:s}".format(
-            "#" * float_digit, "0" * float_digit)
+        num_format_str = "#,{:s}0.{:s}".format("#" * int(float_digit), "0" * int(float_digit))
         cell_style = xlwt.easyxf(num_format_str=num_format_str)
         self.__col_style_table[col] = cell_style
 
         return cell_style
 
 
 class ExcelXlsxTableWriter(ExcelTableWriter):
     """
-    Concrete class of a table writer for Excel format
-    (newer or equal to Office 2007).
+    A table writer class for Excel file format: ``.xlsx`` (newer or equal to Office 2007).
 
-    :Examples:
+    .. py:method:: write_table()
 
-        :ref:`example-excel-table-writer`
+        Write a table to the current opened worksheet.
+
+        :raises IOError: If failed to write data to the worksheet.
+        :Examples:
+            :ref:`example-excel-table-writer`
+
+        .. note::
+            Specific values in the tabular data are converted when writing:
+
+            - |None|: written as an empty string
+            - |inf|: written as ``Inf``
+            - |nan|: written as ``NaN``
     """
 
-    MAX_CELL_WIDTH = 60
+    MAX_CELL_WIDTH: ClassVar[int] = 60
 
-    class FormatName(object):
+    class TableFormat:
         HEADER = "header"
         CELL = "cell"
         NAN = "nan"
 
-    class Default(object):
-        FONT_NAME = "MS Gothic"
-        FONT_SIZE = 9
+    class Default:
+        FONT_NAME: ClassVar[str] = "MS Gothic"
+        FONT_SIZE: ClassVar[int] = 9
 
-        CELL_FORMAT = {
+        CELL_FORMAT: Dict[str, Union[int, str, bool]] = {
             "font_name": FONT_NAME,
             "font_size": FONT_SIZE,
             "align": "top",
             "text_wrap": True,
             "top": 1,
             "left": 1,
             "bottom": 1,
             "right": 1,
         }
-        HEADER_FORMAT = {
+        HEADER_FORMAT: Dict[str, Union[int, str, bool]] = {
             "font_name": FONT_NAME,
             "font_size": FONT_SIZE,
             "bg_color": "#DFDFFF",
             "bold": True,
             "left": 1,
             "right": 1,
         }
-        NAN_FORMAT = {
+        NAN_FORMAT: Dict[str, Union[int, str, bool]] = {
             "font_name": FONT_NAME,
             "font_size": FONT_SIZE,
             "font_color": "silver",
             "top": 1,
             "left": 1,
             "bottom": 1,
             "right": 1,
         }
 
     @property
-    def __nan_format_property(self):
-        return self.format_table.get(self.FormatName.NAN, self.default_format)
+    def __nan_format_property(self) -> Dict[str, Union[int, str, bool]]:
+        return self.format_table.get(self.TableFormat.NAN, self.default_format)
 
     @property
-    def __cell_format_property(self):
-        return self.format_table.get(self.FormatName.CELL, self.default_format)
+    def __cell_format_property(self) -> Dict[str, Union[int, str, bool]]:
+        return self.format_table.get(self.TableFormat.CELL, self.default_format)
 
-    def __init__(self):
-        super(ExcelXlsxTableWriter, self).__init__()
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
         self.default_format = self.Default.CELL_FORMAT
         self.format_table = {
-            self.FormatName.CELL: self.Default.CELL_FORMAT,
-            self.FormatName.HEADER: self.Default.HEADER_FORMAT,
-            self.FormatName.NAN: self.Default.NAN_FORMAT,
+            self.TableFormat.CELL: self.Default.CELL_FORMAT,
+            self.TableFormat.HEADER: self.Default.HEADER_FORMAT,
+            self.TableFormat.NAN: self.Default.NAN_FORMAT,
         }
 
-        self.__col_cell_format_cache = {}
-        self.__col_numprops_table = {}
+        self.__col_cell_format_cache: Dict[int, Any] = {}
+        self.__col_numprops_table: Dict[int, Dict[str, str]] = {}
 
-    def open_workbook(self, workbook_path):
+    def _open(self, workbook_path: str) -> None:
         self._workbook = ExcelWorkbookXlsx(workbook_path)
 
-    def _write_header(self):
-        if any([
-            not self.is_write_header,
-            dp.is_empty_sequence(self.header_list),
-        ]):
+    def _write_header(self) -> None:
+        if not self.is_write_header or typepy.is_empty_sequence(self.headers):
             return
 
-        header_format_props = self.format_table.get(
-            self.FormatName.HEADER, self.default_format)
+        header_format_props = self.format_table.get(self.TableFormat.HEADER, self.default_format)
         header_format = self.__add_format(header_format_props)
 
         self.stream.write_row(
-            row=self.first_header_row, col=0,
-            data=self.header_list, cell_format=header_format)
+            row=self.first_header_row, col=0, data=self.headers, cell_format=header_format
+        )
         for row in range(self.first_header_row, self.last_header_row):
             self.stream.write_row(
-                row=row, col=0, data=[""] * len(self.header_list),
-                cell_format=header_format)
+                row=row, col=0, data=[""] * len(self.headers), cell_format=header_format
+            )
 
-    def _write_cell(self, row, col, prop):
+    def _write_cell(self, row: int, col: int, value_dp: DataProperty) -> None:
         base_props = dict(self.__cell_format_property)
-        format_key = "{:d}_{:d}".format(col, prop.typecode)
+        format_key = f"{col:d}_{value_dp.typecode.name:s}"
 
-        if prop.typecode in [dp.Typecode.INT, dp.Typecode.FLOAT]:
+        if value_dp.typecode in [typepy.Typecode.INTEGER, typepy.Typecode.REAL_NUMBER]:
             num_props = self.__get_number_property(col)
             base_props.update(num_props)
             cell_format = self.__get_cell_format(format_key, base_props)
 
             try:
-                self.stream.write_number(
-                    row, col, float(prop.data), cell_format)
+                self.stream.write_number(row, col, float(value_dp.data), cell_format)
                 return
             except TypeError:
                 pass
 
-        if prop.typecode is dp.Typecode.NAN:
+        if value_dp.typecode is typepy.Typecode.NAN:
             base_props = dict(self.__nan_format_property)
 
         cell_format = self.__get_cell_format(format_key, base_props)
-        self.stream.write(
-            row, col, prop.data, cell_format)
+        self.stream.write(row, col, value_dp.data, cell_format)
 
-    def __get_number_property(self, col):
+    def __get_number_property(self, col: int) -> Dict[str, str]:
         if col in self.__col_numprops_table:
-            return self.__col_numprops_table.get(col)
+            return self.__col_numprops_table[col]
 
         try:
-            col_prop = self._column_prop_list[col]
+            col_dp = self._column_dp_list[col]
         except KeyError:
             return {}
 
-        if col_prop.typecode not in [dp.Typecode.INT, dp.Typecode.FLOAT]:
+        if col_dp.typecode not in [typepy.Typecode.INTEGER, typepy.Typecode.REAL_NUMBER]:
             return {}
 
         num_props = {}
-        if IntegerTypeChecker(col_prop.minmax_decimal_places.max_value).is_type():
-            float_digit = col_prop.minmax_decimal_places.max_value
+        if Integer(col_dp.minmax_decimal_places.max_value).is_type():
+            float_digit = col_dp.minmax_decimal_places.max_value
             if float_digit > 0:
-                num_props = {"num_format": "0.{:s}".format("0" * float_digit)}
+                num_props = {"num_format": "0.{:s}".format("0" * int(float_digit))}
 
         self.__col_numprops_table[col] = num_props
 
         return num_props
 
-    def __get_cell_format(self, format_key, cell_props):
+    def __get_cell_format(self, format_key, cell_props) -> Dict:
         cell_format = self.__col_cell_format_cache.get(format_key)
         if cell_format is not None:
             return cell_format
 
         # cache miss
         cell_format = self.__add_format(cell_props)
         self.__col_cell_format_cache[format_key] = cell_format
 
         return cell_format
 
     def __add_format(self, dict_property):
+        assert self.workbook
         return self.workbook.workbook.add_format(dict_property)
 
-    def __set_cell_width(self):
-        font_size = self.__cell_format_property.get("font_size")
+    def __set_cell_width(self) -> None:
+        font_size = cast(int, self.__cell_format_property.get("font_size"))
 
-        if not IntegerTypeChecker(font_size).is_type():
+        if not Integer(font_size).is_type():
             return
 
-        for col_idx, col_prop in enumerate(self._column_prop_list):
-            width = (
-                min(col_prop.padding_len, self.MAX_CELL_WIDTH) *
-                (font_size / 10.0) + 2
-            )
+        for col_idx, col_dp in enumerate(self._column_dp_list):
+            width = min(col_dp.ascii_char_width, self.MAX_CELL_WIDTH) * (font_size / 10.0) + 2
             self.stream.set_column(col_idx, col_idx, width=width)
 
-    def _preprocess_property(self):
-        super(ExcelXlsxTableWriter, self)._preprocess_property()
+    def _preprocess_table_property(self) -> None:
+        super()._preprocess_table_property()
 
         self.__set_cell_width()
 
-    def _postprocess(self):
-        super(ExcelXlsxTableWriter, self)._postprocess()
+    def _postprocess(self) -> None:
+        super()._postprocess()
 
         self.stream.autofilter(
-            self.last_header_row, self.first_data_col,
-            self.last_data_row, self.last_data_col)
+            self.last_header_row, self.first_data_col, self.last_data_row, self.last_data_col
+        )
         self.stream.freeze_panes(self.first_data_row, self.first_data_col)
 
         self.__col_cell_format_cache = {}
         self.__col_numprops_table = {}
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_javascript_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/text/_yaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,71 @@
-# encoding: utf-8
-
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
-
-from __future__ import absolute_import
+import copy
+import warnings
+from typing import Any, Dict, List, Union
 
 import dataproperty
-import six
 
-from ._converter import lower_bool_converter
-from ._error import EmptyTableNameError
-from ._text_writer import SourceCodeTableWriter
+from .._common import import_error_msg_template
+from ._common import serialize_dp
+from ._text_writer import TextTableWriter
 
 
-def js_datetime_converter(value):
-    return 'new Date("{:s}")'.format(value.strftime("%Y-%m-%dT%H:%M:%S%z"))
+class YamlTableWriter(TextTableWriter):
+    """
+    A table writer class for `YAML <https://yaml.org/>`__ format.
 
+        :Example:
+            :ref:`example-yaml-table-writer`
+    """
 
-def str_datetime_converter(value):
-    return '"{:s}"'.format(value.strftime("%Y-%m-%d %H:%M:%S%z"))
+    FORMAT_NAME = "yaml"
 
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
-class JavaScriptTableWriter(SourceCodeTableWriter):
-    """
-    Concrete class of a table writer for JavaScript format.
+        self.is_padding = False
 
-    :Examples:
-
-        :ref:`example-js-table-writer`
-    """
+        self._dp_extractor.float_type = float
+        self._quoting_flags = copy.deepcopy(dataproperty.NOT_QUOTING_FLAGS)
 
     @property
-    def support_split_write(self):
-        return True
-
-    def __init__(self):
-        super(JavaScriptTableWriter, self).__init__()
+    def format_name(self) -> str:
+        return self.FORMAT_NAME
 
-        self._prop_extractor.none_value = "null"
-        self._prop_extractor.inf_value = "Infinity"
-        self._prop_extractor.nan_value = "NaN"
-        self._prop_extractor.bool_converter = lower_bool_converter
-        self._prop_extractor.datetime_format_str = "s"
-        self.is_quote_table[dataproperty.Typecode.DATETIME] = False
+    @property
+    def support_split_write(self) -> bool:
+        return False
 
-    def write_table(self):
+    def write_table(self, **kwargs) -> None:
         """
-        |write_table| with JavaScript nested list variable definition format.
+        |write_table| with
+        YAML format.
 
-        :raises pytablewriter.EmptyTableNameError:
-            If the |table_name| is empty.
-        :raises pytablewriter.EmptyTableDataError:
-            If the |header_list| and the |value_matrix| is empty.
+        :Example:
+            :ref:`example-yaml-table-writer`
         """
 
-        if self.is_datetime_instance_formatting:
-            self._prop_extractor.datetime_converter = js_datetime_converter
-        else:
-            self._prop_extractor.datetime_converter = str_datetime_converter
-
-        self._verify_property()
-        self._preprocess()
-
-        org_stream = self.stream
-        self.stream = six.StringIO()
-
-        self.inc_indent_level()
-        super(JavaScriptTableWriter, self).write_table()
-        self.dec_indent_level()
-        data_frame_text = self.stream.getvalue().rstrip(u"\n")
-        if self.is_write_closing_row:
-            data_frame_line_list = data_frame_text.splitlines()
-            data_frame_line_list[-2] = data_frame_line_list[-2].rstrip(u",")
-            data_frame_text = u"\n".join(data_frame_line_list)
-
-        self.stream.close()
-        self.stream = org_stream
-
-        self.dec_indent_level()
-        self._write_line(data_frame_text)
-        self.inc_indent_level()
-
-    def _verify_table_name(self):
-        if dataproperty.is_empty_string(self.table_name):
-            raise EmptyTableNameError()
-
-    def _get_opening_row_item_list(self):
-        return u"var {:s} = [".format(self.variable_name)
-
-    def _get_closing_row_item_list(self):
-        return u"];"
+        try:
+            import yaml
+        except ImportError:
+            warnings.warn(import_error_msg_template.format("yaml"))
+            raise
+
+        with self._logger:
+            self._verify_property()
+            self._preprocess()
+
+            if self.headers:
+                matrix: List[Union[Dict[str, Any], List[Any]]] = [
+                    dict(zip(self.headers, [serialize_dp(value_dp) for value_dp in value_dp_list]))
+                    for value_dp_list in self._table_value_dp_matrix
+                ]
+            else:
+                matrix = [
+                    [serialize_dp(value_dp) for value_dp in value_dp_list]
+                    for value_dp_list in self._table_value_dp_matrix
+                ]
+
+            if self.table_name:
+                self._write(yaml.safe_dump({self.table_name: matrix}, default_flow_style=False))
+            else:
+                self._write(yaml.safe_dump(matrix, default_flow_style=False))
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_json_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/text/_mediawiki.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,101 @@
-# encoding: utf-8
+import copy
+import re
+from typing import List, Sequence
 
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
+import dataproperty as dp
+import typepy
+from dataproperty import ColumnDataProperty, DataProperty, LineBreakHandling
+from mbstrdecoder import MultiByteStrDecoder
 
-from __future__ import absolute_import
-try:
-    import json
-except ImportError:   # pragma: no cover
-    import simplejson as json
+from ...style import Align, get_align_char
+from ._text_writer import TextTableWriter
 
-import dataproperty
-from six.moves import zip
-
-from ._converter import lower_bool_converter
-from ._converter import strip_quote
-from ._error import EmptyHeaderError
-from ._text_writer import IndentationTextTableWriter
 
+class MediaWikiTableWriter(TextTableWriter):
+    """
+    A table writer class for `MediaWiki <https://www.mediawiki.org/wiki/MediaWiki>`__ format.
 
-class JsonTableWriter(IndentationTextTableWriter):
+        :Example:
+            :ref:`example-mediawiki-table-writer`
     """
-    Concrete class of a table writer for JSON format.
 
-    :Examples:
+    FORMAT_NAME = "mediawiki"
+    __RE_TABLE_SEQUENCE = re.compile(r"^[\s]+[*|#]+")
 
-        :ref:`example-json-table-writer`
-    """
+    @property
+    def format_name(self) -> str:
+        return self.FORMAT_NAME
 
     @property
-    def support_split_write(self):
+    def support_split_write(self) -> bool:
         return True
 
-    def __init__(self):
-        super(JsonTableWriter, self).__init__()
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+        self.column_delimiter = "\n"
 
+        self.is_padding = False
+        self.is_write_header_separator_row = True
+        self.is_write_value_separator_row = True
         self.is_write_opening_row = True
         self.is_write_closing_row = True
-        self.char_right_side_row = u","
 
-        self._prop_extractor.none_value = "null"
-        self._prop_extractor.inf_value = "Infinity"
-        self._prop_extractor.nan_value = "NaN"
-        self._prop_extractor.bool_converter = lower_bool_converter
-
-    def write_null_line(self):
-        self._verify_stream()
-        self.stream.write(u"\n")
-
-    def write_table(self):
-        """
-        |write_table| with JSON format.
-
-        :raises pytablewriter.EmptyHeaderError: If the |header_list| is empty.
-        """
-
-        self._verify_property()
-        self._preprocess_value_matrix()
-
-        self._write_opening_row()
-        self.inc_indent_level()
-
-        json_text_list = []
-        for json_data in self._value_matrix:
-            json_text = json.dumps(
-                json_data, sort_keys=True, indent=4 * self._indent_level)
-            json_text = strip_quote(json_text, self._prop_extractor.none_value)
-            json_text = strip_quote(json_text, "true")
-            json_text = strip_quote(json_text, "false")
-            json_text_list.append(json_text)
-
-        joint_text = self.char_right_side_row + u"\n"
-        json_text = joint_text.join(json_text_list)
-        if all([
-            not self.is_write_closing_row,
-            dataproperty.is_not_empty_string(json_text),
-        ]):
-            json_text += joint_text
-
-        self.stream.write(json_text)
-
-        self.dec_indent_level()
-        self._write_closing_row()
-
-    def _verify_header(self):
-        if dataproperty.is_empty_sequence(self.header_list):
-            raise EmptyHeaderError()
+        self.update_preprocessor(line_break_handling=LineBreakHandling.NOP)
 
-    def _preprocess_value_matrix(self):
-        from ._function import _get_data_helper
+        self._quoting_flags = copy.deepcopy(dp.NOT_QUOTING_FLAGS)
 
-        if self._preprocessed_value_matrix:
-            return
-
-        self._prop_extractor.data_matrix = self.value_matrix
-
-        try:
-            data_prop_matrix = self._prop_extractor.extract_data_property_matrix()
-        except TypeError:
-            data_prop_matrix = []
+        # experimental: This attribute may change in the future release
+        self.table_style = kwargs.get("table_style", "")
 
-        value_matrix = [
-            [_get_data_helper(data_prop) for data_prop in prop_list]
-            for prop_list in data_prop_matrix
-        ]
-
-        self._value_matrix = [
-            dict(zip(self.header_list, value_list))
-            for value_list in value_matrix
-        ]
+    def _write_header(self) -> None:
+        if not self.is_write_header:
+            return
 
-        self._preprocessed_value_matrix = True
+        if typepy.is_not_null_string(self.table_name):
+            self._write_line("|+" + MultiByteStrDecoder(self.table_name).unicode_str)
 
-    def _get_opening_row_item_list(self):
-        if dataproperty.is_not_empty_string(self.table_name):
-            return u'{{ "{:s}" : ['.format(self.table_name)
+        super()._write_header()
 
-        return u"["
+    def _write_value_row(
+        self, row: int, values: Sequence[str], value_dp_list: Sequence[DataProperty]
+    ) -> None:
+        self._write_row(
+            row,
+            [
+                self.__modify_table_element(value, value_dp)
+                for value, value_dp, in zip(values, value_dp_list)
+            ],
+        )
+
+    def _get_opening_row_items(self) -> List[str]:
+        item = '{| class="wikitable"'
+        if self.table_style:
+            item += f' style="{self.table_style}"'
+
+        return [item]
+
+    def _get_header_row_separator_items(self) -> List[str]:
+        return ["|-"]
+
+    def _get_value_row_separator_items(self) -> List[str]:
+        return self._get_header_row_separator_items()
+
+    def _get_closing_row_items(self) -> List[str]:
+        return ["|}"]
+
+    def _get_header_format_string(self, col_dp: ColumnDataProperty, value_dp: DataProperty) -> str:
+        return "! {{:{:s}{:s}}}".format(
+            get_align_char(Align.CENTER), str(self._get_padding_len(col_dp, value_dp))
+        )
+
+    def __modify_table_element(self, value: str, value_dp: DataProperty) -> str:
+        if value_dp.align is Align.LEFT:
+            forma_stirng = "| {1:s}"
+        else:
+            forma_stirng = '| style="text-align:{0:s}"| {1:s}'
 
-    def _get_closing_row_item_list(self):
-        if dataproperty.is_not_empty_string(self.table_name):
-            return u"]}"
+        if self.__RE_TABLE_SEQUENCE.search(value) is not None:
+            value = "\n" + value.lstrip()
 
-        return u"]"
+        return forma_stirng.format(value_dp.align.align_string, value)
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_md_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/text/sourcecode/_sourcecode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-# encoding: utf-8
+import abc
+from typing import List
 
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
+import typepy
 
-from __future__ import absolute_import
+from .._text_writer import IndentationTextTableWriter
 
-import dataproperty
 
-from ._error import EmptyHeaderError
-from ._text_writer import IndentationTextTableWriter
-
-
-class MarkdownTableWriter(IndentationTextTableWriter):
+class SourceCodeTableWriter(IndentationTextTableWriter):
     """
-    Concrete class of a table writer for Markdown format.
+    Base class of table writer with a source code (variable definition) format.
 
-    :Examples:
+    .. py:attribute:: is_datetime_instance_formatting
+        :type: bool
 
-        :ref:`example-markdown-table-writer`
+        Write |datetime| values in the table as definition of |datetime| class
+        instances coincide with specific language if this value is |True|.
+        Write as |str| if this value is |False|.
     """
 
-    @property
-    def support_split_write(self):
-        return True
-
-    def __init__(self):
-        super(MarkdownTableWriter, self).__init__()
-
-        self.indent_string = u""
-        self.column_delimiter = u"|"
-        self.char_cross_point = u"|"
-        self.is_write_opening_row = True
-        self.is_quote_header = False
-        self.is_quote_table[dataproperty.Typecode.STRING] = False
-        self.is_quote_table[dataproperty.Typecode.DATETIME] = False
-
-        self._prop_extractor.min_padding_len = 3
+    @abc.abstractmethod
+    def get_variable_name(self, value: str) -> str:  # pragma: no cover
+        pass
 
-    def write_table(self):
+    @property
+    def variable_name(self) -> str:
         """
-        |write_table| with Markdown table format.
+        Return a valid variable name that converted from the |table_name|.
 
-        :raises pytablewriter.EmptyHeaderError: If the |header_list| is empty.
+        :return: A variable name.
+        :rtype: str
         """
 
-        super(MarkdownTableWriter, self).write_table()
-
-    def _verify_header(self):
-        if dataproperty.is_empty_sequence(self.header_list):
-            raise EmptyHeaderError()
+        return self.get_variable_name(self.table_name)
 
-    def _get_opening_row_item_list(self):
-        if dataproperty.is_empty_string(self.table_name):
-            return []
+    @property
+    def margin(self) -> int:
+        return self._margin
 
-        return [u"#" * (self._indent_level + 1) + u" " + self.table_name]
+    @margin.setter
+    def margin(self, value: int) -> None:
+        # margin setting must be ignored
+        return
+
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+        self.indent_string = kwargs.get("indent_string", "    ")
+        self.column_delimiter = ", "
+        self._margin = 0
+
+        self.char_left_side_row = "["
+        self.char_right_side_row = "],"
+        self.char_cross_point = ""
+        self.char_opening_row_cross_point = ""
+        self.char_closing_row_cross_point = ""
 
-    def _get_header_row_separator_item_list(self):
-        header_separator_list = []
-        for col_prop in self._column_prop_list:
-            padding_len = self._get_padding_len(col_prop)
+        self.is_padding = False
+        self.is_write_header_separator_row = False
+        self.is_write_opening_row = True
+        self.is_write_closing_row = True
 
-            if col_prop.align == dataproperty.Align.RIGHT:
-                separator_item = u"-" * (padding_len - 1) + u":"
-            elif col_prop.align == dataproperty.Align.CENTER:
-                separator_item = u":" + u"-" * (padding_len - 2) + u":"
-            else:
-                separator_item = u"-" * padding_len
+        self.is_formatting_float = False
+        self.is_datetime_instance_formatting = True
 
-            header_separator_list.append(separator_item)
+        self._quoting_flags[typepy.Typecode.DATETIME] = False
+        self._is_require_table_name = True
 
-        return header_separator_list
+        self._init_cross_point_maps()
 
-    def _get_value_row_separator_item_list(self):
+    def _get_value_row_separator_items(self) -> List[str]:
         return []
 
-    def _get_closing_row_item_list(self):
-        return []
+    def _write_opening_row(self) -> None:
+        self.dec_indent_level()
+        super()._write_opening_row()
+        self.inc_indent_level()
+
+    def _write_closing_row(self) -> None:
+        self.dec_indent_level()
+        super()._write_closing_row()
+        self.inc_indent_level()
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_mediawiki_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/text/_csv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,63 @@
-# encoding: utf-8
+from typing import List
 
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
-
-from __future__ import absolute_import
-
-import dataproperty
-from six.moves import zip
+import typepy
 
 from ._text_writer import TextTableWriter
 
 
-class MediaWikiTableWriter(TextTableWriter):
+class CsvTableWriter(TextTableWriter):
     """
-    Concrete class of a table writer for MediaWiki format.
+    A table writer class for character separated values format.
+    The default separated character is a comma (``","``).
 
-    :Examples:
-
-        :ref:`example-mediawiki-table-writer`
+        :Example:
+            :ref:`example-csv-table-writer`
     """
 
+    FORMAT_NAME = "csv"
+
     @property
-    def support_split_write(self):
+    def format_name(self) -> str:
+        return self.FORMAT_NAME
+
+    @property
+    def support_split_write(self) -> bool:
         return True
 
-    def __init__(self):
-        super(MediaWikiTableWriter, self).__init__()
+    @property
+    def margin(self) -> int:
+        return self._margin
 
-        self.column_delimiter = u"\n"
+    @margin.setter
+    def margin(self, value: int) -> None:
+        # margin setting must be ignored
+        return
+
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+        self._set_chars("")
+        self.indent_string = ""
+        self.column_delimiter = kwargs.get("column_delimiter", ",")
+        self._margin = 0
 
         self.is_padding = False
-        self.is_write_header_separator_row = True
-        self.is_write_value_separator_row = True
-        self.is_write_opening_row = True
-        self.is_write_closing_row = True
-        self.is_quote_header = False
-        self.is_quote_table = {}
+        self.is_formatting_float = False
+        self.is_write_header_separator_row = False
+
+        self._quoting_flags[typepy.Typecode.NULL_STRING] = False
 
-    def _write_header(self):
-        if not self.is_write_header:
+    def _write_header(self) -> None:
+        if typepy.is_empty_sequence(self.headers):
             return
 
-        if dataproperty.is_not_empty_string(self.table_name):
-            self._write_line(u"|+" + self.table_name)
+        super()._write_header()
 
-        super(MediaWikiTableWriter, self)._write_header()
+    def _get_opening_row_items(self) -> List[str]:
+        return []
 
-    def _write_value_row(self, value_list, value_prop_list):
-        self._write_row([
-            self.__modify_table_element(value, value_prop)
-            for value, value_prop, in zip(value_list, value_prop_list)
-        ])
-
-    def _get_opening_row_item_list(self):
-        return u'{| class="wikitable"'
-
-    def _get_header_row_separator_item_list(self):
-        return [u"|-"]
-
-    def _get_value_row_separator_item_list(self):
-        return self._get_header_row_separator_item_list()
-
-    def _get_closing_row_item_list(self):
-        return u"|}"
-
-    def _get_header_format_string(self, col_prop):
-        return u"! {{:{:s}{:s}}}".format(
-            self._get_center_align_formatformat(),
-            str(self._get_padding_len(col_prop)))
-
-    @staticmethod
-    def __modify_table_element(value, value_prop):
-        if value_prop.align is dataproperty.Align.LEFT:
-            forma_stirng = u'| {1:s}'
-        else:
-            forma_stirng = u'| style="text-align:{0:s}"| {1:s}'
+    def _get_value_row_separator_items(self) -> List[str]:
+        return []
 
-        return forma_stirng.format(
-            value_prop.align.align_string, value)
+    def _get_closing_row_items(self) -> List[str]:
+        return []
```

### Comparing `pytablewriter-0.9.0/pytablewriter/_python_code_writer.py` & `pytablewriter-1.0.0/pytablewriter/writer/text/_ltsv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-# encoding: utf-8
+import pathvalidate
+import typepy
 
-"""
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
-"""
+from ._csv import CsvTableWriter
 
-from __future__ import absolute_import
-
-import dataproperty
-
-from ._text_writer import SourceCodeTableWriter
 
+class LtsvTableWriter(CsvTableWriter):
+    """
+    A table writer class for
+    `Labeled Tab-separated Values (LTSV) <http://ltsv.org/>`__ format.
 
-class PythonCodeTableWriter(SourceCodeTableWriter):
+        :Example:
+            :ref:`example-ltsv-table-writer`
     """
-    Concrete class of a table writer for Python code (nested list) format.
 
-    :Examples:
+    FORMAT_NAME = "ltsv"
 
-        :ref:`example-python-code-table-writer`
-    """
+    @property
+    def format_name(self) -> str:
+        return self.FORMAT_NAME
 
     @property
-    def support_split_write(self):
+    def support_split_write(self) -> bool:
         return True
 
-    def __init__(self):
-        super(PythonCodeTableWriter, self).__init__()
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
-        self.table_name = u""
-        self._prop_extractor.inf_value = 'float("inf")'
-        self._prop_extractor.nan_value = 'float("nan")'
+        self.is_write_header = False
 
-    def write_table(self):
-        """
-        |write_table| with Python nested list variable definition format.
+        self._is_require_header = True
 
-        :raises pytablewriter.EmptyTableDataError:
-            If the |header_list| and the |value_matrix| is empty.
+    def write_table(self, **kwargs) -> None:
         """
+        |write_table| with
+        `Labeled Tab-separated Values (LTSV) <http://ltsv.org/>`__ format.
+        Invalid characters in labels/data are removed.
 
-        self._verify_property()
-
-        self.inc_indent_level()
-        super(PythonCodeTableWriter, self).write_table()
-        self.dec_indent_level()
+        :Example:
+            :ref:`example-ltsv-table-writer`
+        """
 
-    def _get_opening_row_item_list(self):
-        if dataproperty.is_not_empty_string(self.table_name):
-            return [self.variable_name + u" = ["]
+        with self._logger:
+            self._verify_property()
+            self._preprocess()
+
+            for values in self._table_value_matrix:
+                ltsv_item_list = [
+                    f"{pathvalidate.sanitize_ltsv_label(header_name):s}:{value}"
+                    for header_name, value in zip(self.headers, values)
+                    if typepy.is_not_null_string(value)
+                ]
 
-        return u"["
+                if typepy.is_empty_sequence(ltsv_item_list):
+                    continue
 
-    def _get_closing_row_item_list(self):
-        return u"]"
+                self._write_line("\t".join(ltsv_item_list))
```

### Comparing `pytablewriter-0.9.0/ss/excel_single.png` & `pytablewriter-1.0.0/ss/excel_single.png`

 * *Files identical despite different names*

### Comparing `pytablewriter-0.9.0/ss/markdown.png` & `pytablewriter-1.0.0/ss/markdown.png`

 * *Files identical despite different names*

### Comparing `pytablewriter-0.9.0/test/test_csv_writer.py` & `pytablewriter-1.0.0/test/writer/text/test_toml_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,197 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
 import collections
 import itertools
+from decimal import Decimal
 
-import pytablewriter
 import pytest
+import toml
+from dateutil.parser import parse
+
+import pytablewriter as ptw
 
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
-from .data import value_matrix_iter
+from ..._common import print_test_result
+from ...data import float_header_list, float_value_matrix, headers, value_matrix
 
 
-Data = collections.namedtuple("Data", "col_delim header value expected")
+Data = collections.namedtuple("Data", "table_name header value expected")
 
 normal_test_data_list = [
     Data(
-        col_delim=",",
-        header=header_list,
+        table_name="normal",
+        header=headers,
         value=value_matrix,
-        expected=""""a","b","c","dd","e"
-1,123.1,"a",1.0,"1"
-2,2.2,"bb",2.2,"2.2"
-3,3.3,"ccc",3.0,"cccc"
-"""
-    ),
-    Data(
-        col_delim=",",
-        header=header_list,
-        value=[],
-        expected=""""a","b","c","dd","e"
-"""
+        expected="""[[normal]]
+a = 1
+c = "a"
+b = 123.1
+e = 1
+dd = 1
+[[normal]]
+a = 2
+c = "bb"
+b = 2.2
+e = 2.2
+dd = 2.2
+[[normal]]
+a = 3
+c = "ccc"
+b = 3.3
+e = "cccc"
+dd = 3
+""",
     ),
     Data(
-        col_delim=",",
-        header=[],
-        value=value_matrix,
-        expected="""1,123.1,"a",1.0,"1"
-2,2.2,"bb",2.2,"2.2"
-3,3.3,"ccc",3.0,"cccc"
-"""
+        table_name="sparse",
+        header=headers,
+        value=[
+            ["1", "", "a", "1", None],
+            [None, 2.2, None, "2.2", 2.2],
+            [None, None, None, None, None],
+            [3, 3.3, "ccc", None, "cccc"],
+            [None, None, None, None, None],
+        ],
+        expected="""[[sparse]]
+a = 1
+b = ""
+c = "a"
+dd = 1
+
+[[sparse]]
+b = 2.2
+dd = 2.2
+e = 2.2
+
+[[sparse]]
+
+[[sparse]]
+a = 3
+b = 3.3
+c = "ccc"
+e = "cccc"
+
+[[sparse]]
+""",
     ),
     Data(
-        col_delim="\t",
-        header=None,
-        value=value_matrix,
-        expected="""1\t123.1\t"a"\t1.0\t"1"
-2\t2.2\t"bb"\t2.2\t"2.2"
-3\t3.3\t"ccc"\t3.0\t"cccc"
-"""
+        table_name="symbols",
+        header=["a!0", "a#1", "a.2$", "a_%3", "a-&4"],
+        value=[["a?b", "c   d", "e+f", "g=h", "i*j"], [1, 2.0, 3.3, Decimal("4.4"), ""]],
+        expected="""[[symbols]]
+"a-&4" = "i*j"
+"a#1" = "c   d"
+"a_%3" = "g=h"
+"a!0" = "a?b"
+"a.2$" = "e+f"
+[[symbols]]
+"a-&4" = ""
+"a#1" = 2
+"a_%3" = 4.4
+"a!0" = 1
+"a.2$" = 3.3
+""",
     ),
     Data(
-        col_delim=",",
-        header=header_list,
-        value=value_matrix_with_none,
-        expected=""""a","b","c","dd","e"
-1,,"a",1.0,
-,2.2,,2.2,"2.2"
-3,3.3,"ccc",,"cccc"
-,,,,
-"""
+        table_name="mixtype",
+        header=["int", "float", "bool", "datetime"],
+        value=[
+            [0, 2.2, True, parse("2017-01-02T03:04:05")],
+            [-1, Decimal("4.4"), False, parse("2022-01-01T00:00:00")],
+        ],
+        expected="""[[mixtype]]
+int = 0
+float = 2.2
+bool = true
+datetime = "2017-01-02T03:04:05"
+
+[[mixtype]]
+int = -1
+float = 4.4
+bool = false
+datetime = "2022-01-01T00:00:00"
+""",
     ),
     Data(
-        col_delim=",",
-        header=mix_header_list,
-        value=mix_value_matrix,
-        expected=""""i","f","c","if","ifc","bool","inf","nan","mix_num","time"
-1,1.10,"aa",1.0,"1",True,inf,nan,1.0,"2017-01-01 00:00:00"
-2,2.20,"bbb",2.2,"2.2",False,inf,nan,inf,"2017-01-02 03:04:05+0900"
-3,3.33,"cccc",-3.0,"ccc",True,inf,nan,nan,"2017-01-01 00:00:00"
-"""
+        table_name="float",
+        header=float_header_list,
+        value=float_value_matrix,
+        expected="""[[float]]
+a = 0.01
+b = 0.00125
+c = 0
+
+[[float]]
+a = 1
+b = 99.90000000000001
+c = 0.01
+
+[[float]]
+a = 1.2
+b = 999999.123
+c = 0.001
+""",
     ),
 ]
 
 exception_test_data_list = [
-    Data(
-        col_delim=",",
-        header=header,
-        value=value,
-        expected=pytablewriter.EmptyTableDataError
-    )
+    Data(table_name="dummy", header=header, value=value, expected=ptw.EmptyTableDataError)
     for header, value in itertools.product([None, [], ""], [None, [], ""])
+] + [
+    Data(table_name="empty_header", header=None, value=value_matrix, expected=ValueError),
+    Data(table_name=None, header=headers, value=value_matrix, expected=ptw.EmptyTableNameError),
 ]
 
-table_writer_class = pytablewriter.CsvTableWriter
-
+table_writer_class = ptw.TomlTableWriter
 
-class Test_CsvTableWriter_write_new_line:
 
+class Test_TomlTableWriter_write_new_line:
     def test_normal(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
         assert out == "\n"
 
 
-class Test_CsvTableWriter_write_table:
-
-    @pytest.mark.parametrize(["col_delim", "header", "value", "expected"], [
-        [data.col_delim, data.header, data.value, data.expected]
-        for data in normal_test_data_list
-    ])
-    def test_normal(self, capsys, col_delim, header, value, expected):
-        writer = table_writer_class()
-        writer.column_delimiter = col_delim
-        writer.header_list = header
-        writer.value_matrix = value
-        writer.write_table()
-
-        out, _err = capsys.readouterr()
-        assert out == expected
-
-    @pytest.mark.parametrize(["header", "value", "expected"], [
-        [data.header, data.value, data.expected]
-        for data in exception_test_data_list
-    ])
-    def test_exception(self, capsys, header, value, expected):
-        writer = table_writer_class()
-        writer.header_list = header
-        writer.value_matrix = value
-
-        with pytest.raises(expected):
-            writer.write_table()
-
-
-class Test_CsvTableWriter_write_table_iter:
-
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
+class Test_TomlTableWriter_write_table:
+    @pytest.mark.parametrize(
+        ["table_name", "header", "value", "expected"],
         [
-            "tablename",
-            ["ha", "hb", "hc"],
-            value_matrix_iter,
-            """"ha","hb","hc"
-1,2,3
-11,12,13
-1,2,3
-11,12,13
-101,102,103
-1001,1002,1003
-""",
+            [data.table_name, data.header, data.value, data.expected]
+            for data in normal_test_data_list
         ],
-    ])
-    def test_normal(self, capsys, table, header, value, expected):
+    )
+    def test_normal(self, capsys, table_name, header, value, expected):
         writer = table_writer_class()
-        writer.table_name = table
-        writer.header_list = header
+        writer.table_name = table_name
+        writer.headers = header
         writer.value_matrix = value
-        writer.iteration_length = len(value)
-        writer.write_table_iter()
+        writer.write_table()
 
-        out, _err = capsys.readouterr()
-        assert out == expected
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+        assert toml.loads(out) == toml.loads(expected)
+
+        # margin setting must be ignored
+        writer.margin = 1
+        dumps_out = writer.dumps()
+        print_test_result(expected=out, actual=dumps_out)
+        assert dumps_out == out
 
     @pytest.mark.parametrize(
-        ["header", "value", "expected"],
+        ["table_name", "header", "value", "expected"],
         [
-            [data.header, data.value, data.expected]
+            [data.table_name, data.header, data.value, data.expected]
             for data in exception_test_data_list
-        ]
+        ],
     )
-    def test_exception(self, capsys, header, value, expected):
+    def test_exception(self, capsys, table_name, header, value, expected):
         writer = table_writer_class()
-        writer.header_list = header
+        writer.table_name = table_name
+        writer.headers = header
         writer.value_matrix = value
 
         with pytest.raises(expected):
-            writer.write_table_iter()
+            writer.write_table()
```

### Comparing `pytablewriter-0.9.0/test/test_javascript_writer.py` & `pytablewriter-1.0.0/test/writer/text/sourcecode/test_numpy_writer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,266 +1,232 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
-import collections
-import itertools
-
-import pytablewriter
 import pytest
 
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
-from .data import value_matrix_iter
+import pytablewriter as ptw
 
+from ...._common import print_test_result
+from ....data import (
+    Data,
+    headers,
+    mix_header_list,
+    mix_value_matrix,
+    null_test_data_list,
+    value_matrix,
+    value_matrix_iter,
+    value_matrix_with_none,
+)
+
+
+try:
+    import numpy as np  # noqa: W0611
+
+    SKIP_DATAFRAME_TEST = False
+except ImportError:
+    SKIP_DATAFRAME_TEST = True
 
-Data = collections.namedtuple(
-    "Data",
-    "table indent header value is_write_header is_dti_fmt expected")
 
 normal_test_data_list = [
     Data(
         table="table-name ho'ge",
         indent=0,
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""var table_name_ho_ge = [
+        expected="""table_name_ho_ge = np.array([
     ["a", "b", "c", "dd", "e"],
-    [1, 123.1, "a", 1.0, "1"],
-    [2, 2.2, "bb", 2.2, "2.2"],
-    [3, 3.3, "ccc", 3.0, "cccc"]
-];
-"""
+    [1, 123.1, "a", 1, 1],
+    [2, 2.2, "bb", 2.2, 2.2],
+    [3, 3.3, "ccc", 3, "cccc"],
+])
+""",
     ),
     Data(
-        table="tablename",
+        table="empty value",
         indent=0,
-        header=header_list,
+        header=headers,
         value=None,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""var tablename = [
-    ["a", "b", "c", "dd", "e"]
-];
-"""
-    ),
-    Data(
-        table="table name",
-        indent=0,
-        header=None,
-        value=value_matrix,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""var table_name = [
-    [1, 123.1, "a", 1.0, "1"],
-    [2, 2.2, "bb", 2.2, "2.2"],
-    [3, 3.3, "ccc", 3.0, "cccc"]
-];
-"""
-    ),
-    Data(
-        table="tablename",
-        indent=1,
-        header=header_list,
-        value=value_matrix,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""    var tablename = [
-        ["a", "b", "c", "dd", "e"],
-        [1, 123.1, "a", 1.0, "1"],
-        [2, 2.2, "bb", 2.2, "2.2"],
-        [3, 3.3, "ccc", 3.0, "cccc"]
-    ];
-"""
+        expected="""empty_value = np.array([
+    ["a", "b", "c", "dd", "e"],
+])
+""",
     ),
     Data(
-        table="tablename",
+        table="table with%null-value",
         indent=0,
-        header=header_list,
+        header=headers,
         value=value_matrix_with_none,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""var tablename = [
+        expected="""table_with_null_value = np.array([
     ["a", "b", "c", "dd", "e"],
-    [1, null, "a", 1.0, null],
-    [null, 2.2, null, 2.2, "2.2"],
-    [3, 3.3, "ccc", null, "cccc"],
-    [null, null, null, null, null]
-];
-"""
+    [1, None, "a", 1, None],
+    [None, 2.2, None, 2.2, 2.2],
+    [3, 3.3, "ccc", None, "cccc"],
+    [None, None, None, None, None],
+])
+""",
     ),
     Data(
-        table="tablename",
+        table="mix data types",
         indent=0,
         header=mix_header_list,
         value=mix_value_matrix,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected="""var tablename = [
+        expected="""mix_data_types = np.array([
     ["i", "f", "c", "if", "ifc", "bool", "inf", "nan", "mix_num", "time"],
-    [1, 1.10, "aa", 1.0, "1", true, Infinity, NaN, 1.0, new Date("2017-01-01T00:00:00")],
-    [2, 2.20, "bbb", 2.2, "2.2", false, Infinity, NaN, Infinity, new Date("2017-01-02T03:04:05+0900")],
-    [3, 3.33, "cccc", -3.0, "ccc", true, Infinity, NaN, NaN, new Date("2017-01-01T00:00:00")]
-];
-"""
+    [1, 1.1, "aa", 1, 1, True, np.inf, np.nan, 1, dateutil.parser.parse("2017-01-01T00:00:00")],
+    [2, 2.2, "bbb", 2.2, 2.2, False, np.inf, np.nan, np.inf, "2017-01-02 03:04:05+09:00"],
+    [3, 3.33, "cccc", -3, "ccc", True, np.inf, np.nan, np.nan, dateutil.parser.parse("2017-01-01T00:00:00")],
+])
+""",
     ),
     Data(
-        table="tablename",
+        table="mix data types wo header",
         indent=0,
-        header=mix_header_list,
+        header=None,
         value=mix_value_matrix,
-        is_write_header=True,
-        is_dti_fmt=False,
-        expected="""var tablename = [
-    ["i", "f", "c", "if", "ifc", "bool", "inf", "nan", "mix_num", "time"],
-    [1, 1.10, "aa", 1.0, "1", true, Infinity, NaN, 1.0, "2017-01-01 00:00:00"],
-    [2, 2.20, "bbb", 2.2, "2.2", false, Infinity, NaN, Infinity, "2017-01-02 03:04:05+0900"],
-    [3, 3.33, "cccc", -3.0, "ccc", true, Infinity, NaN, NaN, "2017-01-01 00:00:00"]
-];
-"""
+        expected="""mix_data_types_wo_header = np.array([
+    [1, 1.1, "aa", 1, 1, True, np.inf, np.nan, 1, dateutil.parser.parse("2017-01-01T00:00:00")],
+    [2, 2.2, "bbb", 2.2, 2.2, False, np.inf, np.nan, np.inf, "2017-01-02 03:04:05+09:00"],
+    [3, 3.33, "cccc", -3, "ccc", True, np.inf, np.nan, np.nan, dateutil.parser.parse("2017-01-01T00:00:00")],
+])
+""",
     ),
-]
-
-exception_test_data_list = [
-    Data(
-        table="",
-        indent=normal_test_data_list[0].indent,
-        header=normal_test_data_list[0].header,
-        value=normal_test_data_list[0].value,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected=pytablewriter.EmptyTableNameError
-    )
-] + [
     Data(
-        table="dummy",
+        table="float-with-null",
         indent=0,
-        header=header,
-        value=value,
-        is_write_header=True,
-        is_dti_fmt=True,
-        expected=pytablewriter.EmptyTableDataError
-    )
-    for header, value in itertools.product([None, [], ""], [None, [], ""])
+        header=["a", "b"],
+        value=[
+            ["0.03785679191278808", "826.21158713263"],
+            [None, "826.21158713263"],
+            [0.1, "1.0499675627886724"],
+        ],
+        expected="""float_with_null = np.array([
+    ["a", "b"],
+    [0.03785679191278808, 826.21158713263],
+    [None, 826.21158713263],
+    [0.1, 1.0499675627886724],
+])
+""",
+    ),
 ]
 
-table_writer_class = pytablewriter.JavaScriptTableWriter
 
+table_writer_class = ptw.NumpyTableWriter
 
-class Test_JavaScriptTableWriter_write_new_line:
 
+class Test_NumpyTableWriter_write_new_line:
     def test_normal(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
-        assert out == "\n"
 
+        assert out == "\n"
 
-class Test_JavaScriptTableWriter_write_table:
 
+class Test_NumpyTableWriter_write_table:
     @pytest.mark.parametrize(
+        ["table", "indent", "header", "value", "expected"],
         [
-            "table", "indent", "header", "value",
-            "is_write_header", "is_dti_fmt", "expected"
-        ],
-        [
-            [
-                data.table, data.indent, data.header, data.value,
-                data.is_write_header, data.is_dti_fmt, data.expected
-            ]
+            [data.table, data.indent, data.header, data.value, data.expected]
             for data in normal_test_data_list
-        ]
+        ],
     )
-    def test_normal_single(
-            self, capsys, table, indent, header, value,
-            is_write_header, is_dti_fmt, expected):
+    def test_normal(self, capsys, table, indent, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
         writer.set_indent_level(indent)
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
-        writer.is_write_header = is_write_header
-        writer.is_datetime_instance_formatting = is_dti_fmt
-
         writer.write_table()
 
-        out, _err = capsys.readouterr()
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
         assert out == expected
 
     @pytest.mark.parametrize(
-        ["table", "indent", "header", "value", "is_write_header", "expected"],
+        ["table", "indent", "header", "value", "expected"],
         [
-            [
-                data.table, data.indent, data.header, data.value,
-                data.is_write_header, data.expected
+            [data.table, data.indent, data.header, data.value, data.expected]
+            for data in null_test_data_list
+        ],
+    )
+    def test_exception_null(self, table, indent, header, value, expected):
+        writer = table_writer_class()
+        writer.table_name = table
+        writer.set_indent_level(indent)
+        writer.headers = header
+        writer.value_matrix = value
+
+        assert writer.dumps() == ""
+
+    @pytest.mark.parametrize(
+        ["table", "indent", "header", "value", "expected"],
+        [
+            [data.table, data.indent, data.header, data.value, data.expected]
+            for data in [
+                Data(
+                    table=None,
+                    indent=0,
+                    header=headers,
+                    value=value_matrix,
+                    expected="",
+                )
             ]
-            for data in exception_test_data_list
-        ]
+        ],
     )
-    def test_exception(
-            self, capsys, table, indent, header, value,
-            is_write_header, expected):
+    def test_exception(self, table, indent, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
         writer.set_indent_level(indent)
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
-        writer.is_write_header = is_write_header
 
-        with pytest.raises(expected):
+        with pytest.raises(ptw.EmptyTableNameError):
             writer.write_table()
 
 
-class Test_JavaScriptTableWriter_write_table_iter:
-
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
+class Test_NumpyTableWriter_write_table_iter:
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
         [
-            "tablename",
-            ["ha", "hb", "hc"],
-            value_matrix_iter,
-            """var tablename = [
+            [
+                "tablename",
+                ["ha", "hb", "hc"],
+                value_matrix_iter,
+                """tablename = np.array([
     ["ha", "hb", "hc"],
     [1, 2, 3],
     [11, 12, 13],
     [1, 2, 3],
     [11, 12, 13],
     [101, 102, 103],
-    [1001, 1002, 1003]
-];
+    [1001, 1002, 1003],
+])
 """,
+            ]
         ],
-    ])
+    )
     def test_normal(self, capsys, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.iteration_length = len(value)
         writer.write_table_iter()
 
         out, _err = capsys.readouterr()
+
         assert out == expected
 
     @pytest.mark.parametrize(
         ["table", "header", "value", "expected"],
-        [
-            [data.table, data.header, data.value, data.expected]
-            for data in exception_test_data_list
-        ]
+        [[data.table, data.header, data.value, data.expected] for data in null_test_data_list],
     )
-    def test_exception(self, capsys, table, header, value, expected):
+    def test_normal_empty(self, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
-        with pytest.raises(expected):
-            writer.write_table_iter()
+        writer.write_table_iter()
```

### Comparing `pytablewriter-0.9.0/test/test_json_writer.py` & `pytablewriter-1.0.0/test/writer/text/test_json_writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
 import collections
-try:
-    import json
-except ImportError:
-    import simplejson as json
+import json
+import platform as m_platform
+import sys
+from textwrap import dedent
 
-import pytablewriter
 import pytest
 
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
-from .data import value_matrix_iter
+import pytablewriter
+
+from ..._common import print_test_result
+from ...data import (
+    float_header_list,
+    float_value_matrix,
+    headers,
+    mix_header_list,
+    mix_value_matrix,
+    value_matrix,
+    value_matrix_iter,
+    value_matrix_with_none,
+)
 
 
 Data = collections.namedtuple("Data", "table header value expected")
 
 normal_test_data_list = [
     Data(
         table="",
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        expected=json.loads("""[
+        expected=json.loads(
+            """[
             {
                 "a": 1,
                 "b": 123.1,
                 "c": "a",
                 "dd": 1,
                 "e": 1
             },
@@ -48,27 +52,24 @@
                 "a": 3,
                 "b": 3.3,
                 "c": "ccc",
                 "dd": 3,
                 "e": "cccc"
             }
         ]
-        """)
-    ),
-    Data(
-        table="",
-        header=header_list,
-        value=None,
-        expected=json.loads("[]")
+        """
+        ),
     ),
+    Data(table="", header=headers, value=None, expected="[\n\n]\n"),
     Data(
         table="tablename",
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        expected=json.loads("""{
+        expected=json.loads(
+            """{
             "tablename": [
                 {
                     "a": 1,
                     "b": 123.1,
                     "c": "a",
                     "dd": 1,
                     "e": 1
@@ -85,22 +86,24 @@
                     "b": 3.3,
                     "c": "ccc",
                     "dd": 3,
                     "e": "cccc"
                 }
             ]
         }
-        """)
+        """
+        ),
     ),
     Data(
-        table="table name",
-        header=header_list,
+        table="with none values",
+        header=headers,
         value=value_matrix_with_none,
-        expected=json.loads("""{
-            "table name": [
+        expected=json.loads(
+            """{
+            "with none values": [
                 {
                     "a": 1,
                     "b": null,
                     "c": "a",
                     "dd": 1,
                     "e": null
                 },
@@ -123,127 +126,229 @@
                     "b": null,
                     "c": null,
                     "dd": null,
                     "e": null
                 }
             ]
         }
-        """)
+        """
+        ),
     ),
     Data(
-        table="table name",
+        table="mixed values",
         header=mix_header_list,
         value=mix_value_matrix,
-        expected=json.loads("""{ "table name" : [
+        expected=json.loads(
+            """{ "mixed values" : [
             {
                 "bool": true,
                 "c": "aa",
                 "f": 1.1,
                 "i": 1,
                 "if": 1,
                 "ifc": 1,
                 "inf": "Infinity",
                 "mix_num": 1.0,
                 "nan": "NaN",
-                "time": "2017-01-01 00:00:00"
+                "time": "2017-01-01T00:00:00"
             },
             {
                 "bool": false,
                 "c": "bbb",
                 "f": 2.2,
                 "i": 2,
                 "if": 2.2,
                 "ifc": 2.2,
                 "inf": "Infinity",
                 "mix_num": "Infinity",
                 "nan": "NaN",
-                "time": "2017-01-02 03:04:05+0900"
+                "time": "2017-01-02 03:04:05+09:00"
             },
             {
                 "bool": true,
                 "c": "cccc",
                 "f": 3.33,
                 "i": 3,
                 "if": -3,
                 "ifc": "ccc",
                 "inf": "Infinity",
                 "mix_num": "NaN",
                 "nan": "NaN",
-                "time": "2017-01-01 00:00:00"
+                "time": "2017-01-01T00:00:00"
             }]}
-        """)
+        """
+        ),
     ),
+    Data(
+        table="float",
+        header=float_header_list,
+        value=float_value_matrix,
+        expected=json.loads(
+            """{ "float" : [
+{
+    "a": 0.01,
+    "b": 0.00125,
+    "c": 0
+},
+{
+    "a": 1,
+    "b": 99.9,
+    "c": 0.01
+},
+{
+    "a": 1.2,
+    "b": 999999.123,
+    "c": 0.001
+}]}
+
+"""
+        ),
+    ),
+    Data(table="", header=[], value=[], expected=""),
 ]
 
 exception_test_data_list = [
     Data(
         table="",
         header=[],
-        value=[],
-        expected=pytablewriter.EmptyHeaderError
-    ),
-    Data(
-        table="",
-        header=[],
         value=normal_test_data_list[0].value,
-        expected=pytablewriter.EmptyHeaderError
+        expected=ValueError,
     ),
 ]
 
 table_writer_class = pytablewriter.JsonTableWriter
 
 
 class Test_JsonTableWriter_write_new_line:
-
     def test_normal(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
         assert out == "\n"
 
 
 class Test_JsonTableWriter_write_table:
-
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
-        [data.table, data.header, data.value, data.expected]
-        for data in normal_test_data_list
-    ])
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
+        [[data.table, data.header, data.value, data.expected] for data in normal_test_data_list],
+    )
     def test_normal(self, capsys, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.write_table()
 
-        out, _err = capsys.readouterr()
-        assert json.loads(out) == expected
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
+        if not value:
+            assert out == expected
+        else:
+            assert json.loads(out) == expected
+
+        # margin setting must be ignored
+        writer.margin = 1
+        dumps_out = writer.dumps()
+        print_test_result(expected=out, actual=dumps_out)
+        assert dumps_out == out
+
+    @pytest.mark.skipif(
+        m_platform.system() == "Windows" and sys.version_info < (3, 6), reason="env dependent tests"
+    )
+    def test_normal_sort_keys(self):
+        writer = table_writer_class()
+        writer.headers = ["z", "i"]
+        writer.value_matrix = [
+            {"z": "abc", "i": 1},
+            {"z": "efg", "i": 2},
+        ]
+
+        assert writer.dumps(sort_keys=True) != writer.dumps(sort_keys=False)
 
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
-        [data.table, data.header, data.value, data.expected]
-        for data in exception_test_data_list
-    ])
-    def test_exception(self, capsys, table, header, value, expected):
+    def test_normal_json_rows(self):
+        writer = table_writer_class()
+        writer.headers = ["a", "i", "f", "b", "n"]
+        writer.value_matrix = [
+            {"a": "abc", "b": True, "f": "NaN", "i": 0, "n": 0.1},
+            {"a": "abcdef", "b": False, "f": "Infinity", "i": -1, "n": None},
+            {"n": None, "f": "Infinity", "a": "", "i": 1, "b": False},
+        ]
+        out = writer.dumps(sort_keys=True)
+
+        expected = dedent(
+            """\
+            [
+                {
+                    "a": "abc",
+                    "b": true,
+                    "f": "NaN",
+                    "i": 0,
+                    "n": 0.1
+                },
+                {
+                    "a": "abcdef",
+                    "b": false,
+                    "f": "Infinity",
+                    "i": -1,
+                    "n": null
+                },
+                {
+                    "a": "",
+                    "b": false,
+                    "f": "Infinity",
+                    "i": 1,
+                    "n": null
+                }
+            ]
+            """
+        )
+
+        print_test_result(expected=expected, actual=out)
+        assert out == expected
+
+    def test_normal_indent_wo_table_name(self):
+        writer = table_writer_class()
+        writer.headers = ["a", "i"]
+        writer.value_matrix = [
+            ["abc", 1],
+            ["efg", 2],
+        ]
+
+        assert writer.dumps(sort_keys=True) == writer.dumps(sort_keys=True, indent=4)
+        assert writer.dumps(sort_keys=True, indent=2) != writer.dumps(sort_keys=True, indent=4)
+
+        writer.table_name = "example"
+        assert writer.dumps(sort_keys=True, indent=2) != writer.dumps(sort_keys=True, indent=4)
+
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
+        [[data.table, data.header, data.value, data.expected] for data in exception_test_data_list],
+    )
+    def test_exception(self, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
         with pytest.raises(expected):
             writer.write_table()
 
 
 class Test_JsonTableWriter_write_table_iter:
-
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
         [
-            "tablename",
-            ["ha", "hb", "hc"],
-            value_matrix_iter,
-            json.loads("""{ "tablename" : [
+            [
+                "tablename",
+                ["ha", "hb", "hc"],
+                value_matrix_iter,
+                json.loads(
+                    """{ "tablename" : [
                 {
                     "ha": 1,
                     "hb": 2,
                     "hc": 3
                 },
                 {
                     "ha": 11,
@@ -265,36 +370,36 @@
                     "hb": 102,
                     "hc": 103
                 },
                 {
                     "ha": 1001,
                     "hb": 1002,
                     "hc": 1003
-                }]}"""),
+                }]}"""
+                ),
+            ]
         ],
-    ])
+    )
     def test_normal(self, capsys, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.iteration_length = len(value)
         writer.write_table_iter()
 
-        out, _err = capsys.readouterr()
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
         assert json.loads(out) == expected
 
     @pytest.mark.parametrize(
         ["table", "header", "value", "expected"],
-        [
-            [data.table, data.header, data.value, data.expected]
-            for data in exception_test_data_list
-        ]
+        [[data.table, data.header, data.value, data.expected] for data in exception_test_data_list],
     )
-    def test_exception(self, capsys, table, header, value, expected):
+    def test_exception(self, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
         with pytest.raises(expected):
             writer.write_table_iter()
```

### Comparing `pytablewriter-0.9.0/test/test_mediawiki_writer.py` & `pytablewriter-1.0.0/test/writer/text/test_mediawiki_writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,342 +1,425 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
 import collections
+from textwrap import dedent
 
-import pytablewriter
 import pytest
 
-from .data import null_test_data_list
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
-from .data import value_matrix_iter
+import pytablewriter
+
+from ..._common import print_test_result
+from ...data import (
+    headers,
+    mix_header_list,
+    mix_value_matrix,
+    null_test_data_list,
+    value_matrix,
+    value_matrix_iter,
+    value_matrix_with_none,
+)
 
 
 Data = collections.namedtuple("Data", "table header value expected")
 
 normal_test_data_list = [
     Data(
         table="test table",
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        expected="""{| class="wikitable"
-|+test table
-! a
-! b
-! c
-! dd
-! e
-|-
-| style="text-align:right"| 1
-| style="text-align:right"| 123.1
-| a
-| style="text-align:right"| 1.0
-| style="text-align:right"| 1
-|-
-| style="text-align:right"| 2
-| style="text-align:right"| 2.2
-| bb
-| style="text-align:right"| 2.2
-| style="text-align:right"| 2.2
-|-
-| style="text-align:right"| 3
-| style="text-align:right"| 3.3
-| ccc
-| style="text-align:right"| 3.0
-| cccc
-|}
-"""
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            |+test table
+            ! a
+            ! b
+            ! c
+            ! dd
+            ! e
+            |-
+            | style="text-align:right"| 1
+            | style="text-align:right"| 123.1
+            | a
+            | style="text-align:right"| 1.0
+            | style="text-align:right"| 1
+            |-
+            | style="text-align:right"| 2
+            | style="text-align:right"| 2.2
+            | bb
+            | style="text-align:right"| 2.2
+            | style="text-align:right"| 2.2
+            |-
+            | style="text-align:right"| 3
+            | style="text-align:right"| 3.3
+            | ccc
+            | style="text-align:right"| 3.0
+            | cccc
+            |}
+            """
+        ),
     ),
     Data(
         table=None,
-        header=header_list,
+        header=headers,
         value=None,
-        expected="""{| class="wikitable"
-! a
-! b
-! c
-! dd
-! e
-|-
-|}
-"""
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            ! a
+            ! b
+            ! c
+            ! dd
+            ! e
+            |-
+            |}
+            """
+        ),
+    ),
+    Data(
+        table=None,
+        header=["ho ge", "foo - bar"],
+        value=[
+            [1, "\n".join([" # a b c", "# h o g e"])],
+            [2, "\n".join([" *hoge", "* abc"])],
+            [3, "\n".join([" a * b", "a # b ## c ###"])],
+            [3, "\n".join([" a # b", "a * b ** c ***"])],
+        ],
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            ! ho ge
+            ! foo - bar
+            |-
+            | style="text-align:right"| 1
+            | 
+            # a b c
+            # h o g e
+            |-
+            | style="text-align:right"| 2
+            | 
+            *hoge
+            * abc
+            |-
+            | style="text-align:right"| 3
+            |  a * b
+            a # b ## c ###
+            |-
+            | style="text-align:right"| 3
+            |  a # b
+            a * b ** c ***
+            |}
+            """
+        ),
     ),
     Data(
         table=None,
         header=None,
         value=value_matrix,
-        expected="""{| class="wikitable"
-| style="text-align:right"| 1
-| style="text-align:right"| 123.1
-| a
-| style="text-align:right"| 1.0
-| style="text-align:right"| 1
-|-
-| style="text-align:right"| 2
-| style="text-align:right"| 2.2
-| bb
-| style="text-align:right"| 2.2
-| style="text-align:right"| 2.2
-|-
-| style="text-align:right"| 3
-| style="text-align:right"| 3.3
-| ccc
-| style="text-align:right"| 3.0
-| cccc
-|}
-"""
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            | style="text-align:right"| 1
+            | style="text-align:right"| 123.1
+            | a
+            | style="text-align:right"| 1.0
+            | style="text-align:right"| 1
+            |-
+            | style="text-align:right"| 2
+            | style="text-align:right"| 2.2
+            | bb
+            | style="text-align:right"| 2.2
+            | style="text-align:right"| 2.2
+            |-
+            | style="text-align:right"| 3
+            | style="text-align:right"| 3.3
+            | ccc
+            | style="text-align:right"| 3.0
+            | cccc
+            |}
+            """
+        ),
     ),
     Data(
         table="test table",
-        header=header_list,
+        header=headers,
         value=value_matrix_with_none,
-        expected="""{| class="wikitable"
-|+test table
-! a
-! b
-! c
-! dd
-! e
-|-
-| style="text-align:right"| 1
-| 
-| a
-| style="text-align:right"| 1.0
-| 
-|-
-| 
-| style="text-align:right"| 2.2
-| 
-| style="text-align:right"| 2.2
-| style="text-align:right"| 2.2
-|-
-| style="text-align:right"| 3
-| style="text-align:right"| 3.3
-| ccc
-| 
-| cccc
-|-
-| 
-| 
-| 
-| 
-| 
-|}
-"""
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            |+test table
+            ! a
+            ! b
+            ! c
+            ! dd
+            ! e
+            |-
+            | style="text-align:right"| 1
+            | 
+            | a
+            | style="text-align:right"| 1.0
+            | 
+            |-
+            | 
+            | style="text-align:right"| 2.2
+            | 
+            | style="text-align:right"| 2.2
+            | style="text-align:right"| 2.2
+            |-
+            | style="text-align:right"| 3
+            | style="text-align:right"| 3.3
+            | ccc
+            | 
+            | cccc
+            |-
+            | 
+            | 
+            | 
+            | 
+            | 
+            |}
+            """
+        ),
     ),
     Data(
         table="test table",
         header=mix_header_list,
         value=mix_value_matrix,
-        expected="""{| class="wikitable"
-|+test table
-! i
-! f
-! c
-! if
-! ifc
-! bool
-! inf
-! nan
-! mix_num
-! time
-|-
-| style="text-align:right"| 1
-| style="text-align:right"| 1.10
-| aa
-| style="text-align:right"| 1.0
-| style="text-align:right"| 1
-| True
-| inf
-| nan
-| style="text-align:right"| 1.0
-| 2017-01-01 00:00:00
-|-
-| style="text-align:right"| 2
-| style="text-align:right"| 2.20
-| bbb
-| style="text-align:right"| 2.2
-| style="text-align:right"| 2.2
-| False
-| inf
-| nan
-| inf
-| 2017-01-02 03:04:05+0900
-|-
-| style="text-align:right"| 3
-| style="text-align:right"| 3.33
-| cccc
-| style="text-align:right"| -3.0
-| ccc
-| True
-| inf
-| nan
-| nan
-| 2017-01-01 00:00:00
-|}
-"""
+        expected=dedent(
+            """\
+            {| class="wikitable"
+            |+test table
+            ! i
+            ! f
+            ! c
+            ! if
+            ! ifc
+            ! bool
+            ! inf
+            ! nan
+            ! mix_num
+            ! time
+            |-
+            | style="text-align:right"| 1
+            | style="text-align:right"| 1.10
+            | aa
+            | style="text-align:right"| 1.0
+            | style="text-align:right"| 1
+            | True
+            | Infinity
+            | NaN
+            | style="text-align:right"| 1
+            | 2017-01-01T00:00:00
+            |-
+            | style="text-align:right"| 2
+            | style="text-align:right"| 2.20
+            | bbb
+            | style="text-align:right"| 2.2
+            | style="text-align:right"| 2.2
+            | False
+            | Infinity
+            | NaN
+            | Infinity
+            | 2017-01-02 03:04:05+09:00
+            |-
+            | style="text-align:right"| 3
+            | style="text-align:right"| 3.33
+            | cccc
+            | style="text-align:right"| -3.0
+            | ccc
+            | True
+            | Infinity
+            | NaN
+            | NaN
+            | 2017-01-01T00:00:00
+            |}
+            """
+        ),
     ),
 ]
 
 table_writer_class = pytablewriter.MediaWikiTableWriter
 
 
 class Test_MediaWikiTableWriter_write_new_line:
-
     def test_normal(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
         assert out == "\n"
 
 
 class Test_MediaWikiTableWriter_write_table:
-
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
-        [data.table, data.header, data.value, data.expected]
-        for data in normal_test_data_list
-    ])
+    @pytest.mark.xfail(run=False)
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
+        [[data.table, data.header, data.value, data.expected] for data in normal_test_data_list],
+    )
     def test_normal(self, capsys, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.write_table()
 
-        out, _err = capsys.readouterr()
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
         assert out == expected
+        assert writer.dumps() == expected
+        assert str(writer) == expected
+
+    def test_normal_(self):
+        writer = table_writer_class(
+            headers=["hoge", "foo"],
+            value_matrix=[
+                [1, "abc"],
+                [2, "xyz"],
+            ],
+            table_style="display: inline-table;",
+        )
+        expected = dedent(
+            """\
+            {| class="wikitable" style="display: inline-table;"
+            ! hoge
+            ! foo
+            |-
+            | style="text-align:right"| 1
+            | abc
+            |-
+            | style="text-align:right"| 2
+            | xyz
+            |}
+            """
+        )
+        output = writer.dumps()
+
+        print_test_result(expected=expected, actual=output)
+
+        assert output == expected
 
     @pytest.mark.parametrize(
         ["table", "header", "value", "expected"],
-        [
-            [data.table, data.header, data.value, data.expected]
-            for data in null_test_data_list
-        ]
+        [[data.table, data.header, data.value, data.expected] for data in null_test_data_list],
     )
-    def test_exception(self, capsys, table, header, value, expected):
+    def test_normal_empty(self, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
-        with pytest.raises(expected):
-            writer.write_table()
+        assert writer.dumps() == ""
 
 
 def simple_write_callback(iter_count, iteration_length):
-    import six
-
-    six.print_("{:d}/{:d}".format(iter_count, iteration_length))
+    print(f"{iter_count:d}/{iteration_length:d}")
 
 
 class Test_MediaWikiTableWriter_write_table_iter:
-
-    @pytest.mark.parametrize(["table", "header", "value", "callback", "expected"], [
-        [
-            "tablename",
-            ["ha", "hb", "hc"],
-            value_matrix_iter,
-            None,
-            """{| class="wikitable"
-|+tablename
-! ha
-! hb
-! hc
-|-
-| style="text-align:right"| 1
-| style="text-align:right"| 2
-| style="text-align:right"| 3
-|-
-| style="text-align:right"| 11
-| style="text-align:right"| 12
-| style="text-align:right"| 13
-|-
-| style="text-align:right"| 1
-| style="text-align:right"| 2
-| style="text-align:right"| 3
-|-
-| style="text-align:right"| 11
-| style="text-align:right"| 12
-| style="text-align:right"| 13
-|-
-| style="text-align:right"| 101
-| style="text-align:right"| 102
-| style="text-align:right"| 103
-|-
-| style="text-align:right"| 1001
-| style="text-align:right"| 1002
-| style="text-align:right"| 1003
-|}
-""",
-        ],
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "callback", "expected"],
         [
-            None,
-            None,
-            value_matrix_iter,
-            simple_write_callback,
-            """{| class="wikitable"
-| style="text-align:right"| 1
-| style="text-align:right"| 2
-| style="text-align:right"| 3
-|-
-| style="text-align:right"| 11
-| style="text-align:right"| 12
-| style="text-align:right"| 13
-|-
-1/3
-| style="text-align:right"| 1
-| style="text-align:right"| 2
-| style="text-align:right"| 3
-|-
-| style="text-align:right"| 11
-| style="text-align:right"| 12
-| style="text-align:right"| 13
-|-
-2/3
-| style="text-align:right"| 101
-| style="text-align:right"| 102
-| style="text-align:right"| 103
-|-
-| style="text-align:right"| 1001
-| style="text-align:right"| 1002
-| style="text-align:right"| 1003
-|}
-3/3
-""",
+            [
+                "tablename",
+                ["ha", "hb", "hc"],
+                value_matrix_iter,
+                lambda a, b: None,
+                dedent(
+                    """\
+                {| class="wikitable"
+                |+tablename
+                ! ha
+                ! hb
+                ! hc
+                |-
+                | style="text-align:right"| 1
+                | style="text-align:right"| 2
+                | style="text-align:right"| 3
+                |-
+                | style="text-align:right"| 11
+                | style="text-align:right"| 12
+                | style="text-align:right"| 13
+                |-
+                | style="text-align:right"| 1
+                | style="text-align:right"| 2
+                | style="text-align:right"| 3
+                |-
+                | style="text-align:right"| 11
+                | style="text-align:right"| 12
+                | style="text-align:right"| 13
+                |-
+                | style="text-align:right"| 101
+                | style="text-align:right"| 102
+                | style="text-align:right"| 103
+                |-
+                | style="text-align:right"| 1001
+                | style="text-align:right"| 1002
+                | style="text-align:right"| 1003
+                |}
+                """
+                ),
+            ],
+            [
+                None,
+                None,
+                value_matrix_iter,
+                simple_write_callback,
+                dedent(
+                    """\
+                {| class="wikitable"
+                | style="text-align:right"| 1
+                | style="text-align:right"| 2
+                | style="text-align:right"| 3
+                |-
+                | style="text-align:right"| 11
+                | style="text-align:right"| 12
+                | style="text-align:right"| 13
+                |-
+                1/3
+                | style="text-align:right"| 1
+                | style="text-align:right"| 2
+                | style="text-align:right"| 3
+                |-
+                | style="text-align:right"| 11
+                | style="text-align:right"| 12
+                | style="text-align:right"| 13
+                |-
+                2/3
+                | style="text-align:right"| 101
+                | style="text-align:right"| 102
+                | style="text-align:right"| 103
+                |-
+                | style="text-align:right"| 1001
+                | style="text-align:right"| 1002
+                | style="text-align:right"| 1003
+                |}
+                3/3
+                """
+                ),
+            ],
         ],
-    ])
+    )
     def test_normal(self, capsys, table, header, value, callback, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.iteration_length = len(value)
         writer.write_callback = callback
         writer.write_table_iter()
 
         out, _err = capsys.readouterr()
         assert out == expected
 
     @pytest.mark.parametrize(
         ["table", "header", "value", "expected"],
-        [
-            [data.table, data.header, data.value, data.expected]
-            for data in null_test_data_list
-        ]
+        [[data.table, data.header, data.value, data.expected] for data in null_test_data_list],
     )
-    def test_exception(self, capsys, table, header, value, expected):
+    def test_smoke_empty(self, table, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
-        with pytest.raises(expected):
-            writer.write_table_iter()
+        writer.write_table_iter()
```

### Comparing `pytablewriter-0.9.0/test/test_null_writer.py` & `pytablewriter-1.0.0/test/writer/test_null_writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
-
 import pytablewriter
 
 
 table_writer_class = pytablewriter.NullTableWriter
 
 
 class Test_NullTableWriter_set_indent_level:
-
-    def test_smoke(self, capsys):
+    def test_smoke(self):
         writer = table_writer_class()
         writer.set_indent_level(0)
 
 
 class Test_NullTableWriter_inc_indent_level:
-
-    def test_smoke(self, capsys):
+    def test_smoke(self):
         writer = table_writer_class()
         writer.inc_indent_level()
 
 
 class Test_NullTableWriter_dec_indent_level:
-
-    def test_smoke(self, capsys):
+    def test_smoke(self):
         writer = table_writer_class()
         writer.dec_indent_level()
 
 
 class Test_NullTableWriter_write_new_line:
-
     def test_smoke(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
         assert out == ""
 
 
 class Test_NullTableWriter_write_table:
-
     def test_smoke(self, capsys):
         writer = table_writer_class()
         writer.write_table()
 
         out, _err = capsys.readouterr()
         assert out == ""
 
 
-class Test_NullTableWriter_write_table_iter:
+class Test_NullTableWriter_dumps:
+    def test_smoke(self):
+        writer = table_writer_class()
 
+        assert writer.dumps() == ""
+        assert str(writer) == ""
+
+
+class Test_NullTableWriter_write_table_iter:
     def test_smoke(self, capsys):
         writer = table_writer_class()
         writer.write_table_iter()
 
         out, _err = capsys.readouterr()
         assert out == ""
```

### Comparing `pytablewriter-0.9.0/test/test_python_code_writer.py` & `pytablewriter-1.0.0/test/writer/binary/test_pandas_writer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,195 +1,151 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
+import collections
+import os
+import sys
+from decimal import Decimal
 
-import pytablewriter
 import pytest
+from tabledata import TableData
+
+import pytablewriter as ptw
+
+from ..._common import print_test_result
+from ...data import headers, value_matrix
+
+
+try:
+    import pandas as pd
+
+    SKIP_DATAFRAME_TEST = False
+except ImportError:
+    SKIP_DATAFRAME_TEST = True
 
-from .data import Data
-from .data import null_test_data_list
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
-from .data import value_matrix_iter
 
+inf = Decimal("Infinity")
+nan = None
+
+Data = collections.namedtuple("Data", "table header value expected")
 
 normal_test_data_list = [
     Data(
-        table="table-name ho'ge",
-        indent=0,
-        header=header_list,
-        value=value_matrix,
-        expected="""table_name_ho_ge = [
-    ["a", "b", "c", "dd", "e"],
-    [1, 123.1, "a", 1.0, "1"],
-    [2, 2.2, "bb", 2.2, "2.2"],
-    [3, 3.3, "ccc", 3.0, "cccc"],
-]
-"""
-    ),
-    Data(
         table="tablename",
-        indent=0,
-        header=header_list,
-        value=None,
-        expected="""tablename = [
-    ["a", "b", "c", "dd", "e"],
-]
-"""
-    ),
-    Data(
-        table=None,
-        indent=0,
-        header=None,
+        header=headers,
         value=value_matrix,
-        expected="""[
-    [1, 123.1, "a", 1.0, "1"],
-    [2, 2.2, "bb", 2.2, "2.2"],
-    [3, 3.3, "ccc", 3.0, "cccc"],
-]
-"""
+        expected=TableData(
+            "tablename",
+            ["a", "b", "c", "dd", "e"],
+            [[1, 123.1, "a", 1, 1], [2, 2.2, "bb", 2.2, 2.2], [3, 3.3, "ccc", 3, "cccc"]],
+        ),
     ),
     Data(
-        table="tablename",
-        indent=1,
-        header=header_list,
+        table="empty header",
+        header=[],
         value=value_matrix,
-        expected="""    tablename = [
-        ["a", "b", "c", "dd", "e"],
-        [1, 123.1, "a", 1.0, "1"],
-        [2, 2.2, "bb", 2.2, "2.2"],
-        [3, 3.3, "ccc", 3.0, "cccc"],
-    ]
-"""
-    ),
-    Data(
-        table="table name",
-        indent=0,
-        header=header_list,
-        value=value_matrix_with_none,
-        expected="""table_name = [
-    ["a", "b", "c", "dd", "e"],
-    [1, None, "a", 1.0, None],
-    [None, 2.2, None, 2.2, "2.2"],
-    [3, 3.3, "ccc", None, "cccc"],
-    [None, None, None, None, None],
-]
-"""
+        expected=TableData(
+            "empty_header",
+            ["A", "B", "C", "D", "E"],
+            [[1, 123.1, "a", 1, 1], [2, 2.2, "bb", 2.2, 2.2], [3, 3.3, "ccc", 3, "cccc"]],
+        ),
     ),
-    Data(
-        table="tablename",
-        indent=0,
-        header=mix_header_list,
-        value=mix_value_matrix,
-        expected="""tablename = [
-    ["i", "f", "c", "if", "ifc", "bool", "inf", "nan", "mix_num", "time"],
-    [1, 1.10, "aa", 1.0, "1", True, float("inf"), float("nan"), 1.0, "2017-01-01 00:00:00"],
-    [2, 2.20, "bbb", 2.2, "2.2", False, float("inf"), float("nan"), float("inf"), "2017-01-02 03:04:05+0900"],
-    [3, 3.33, "cccc", -3.0, "ccc", True, float("inf"), float("nan"), float("nan"), "2017-01-01 00:00:00"],
 ]
-"""
-    ),
+
+empty_test_data_list = [
+    Data(table="dummy", header=[], value=[], expected=None),
+    Data(table="dummy", header=headers, value=[], expected=None),
 ]
 
-table_writer_class = pytablewriter.PythonCodeTableWriter
 
+@pytest.mark.skipif(SKIP_DATAFRAME_TEST, reason="required package not found")
+class Test_PandasDataFramePickleWriter_write_table:
+    @pytest.mark.parametrize(
+        ["table", "header", "value", "expected"],
+        [[data.table, data.header, data.value, data.expected] for data in normal_test_data_list],
+    )
+    def test_normal(self, tmpdir, table, header, value, expected):
+        test_filepath = tmpdir.join("test1.pkl")
 
-class Test_PythonCodeTableWriter_write_new_line:
+        writer = ptw.PandasDataFramePickleWriter(
+            table_name=table,
+            headers=header,
+            value_matrix=value,
+        )
+        writer.open(str(test_filepath))
+        writer.write_table()
 
-    def test_normal(self, capsys):
-        writer = table_writer_class()
-        writer.write_null_line()
+        print(expected, file=sys.stderr)
 
-        out, _err = capsys.readouterr()
-        assert out == "\n"
+        actual = ptw.PandasDataFramePickleWriter()
+        actual.from_dataframe(pd.read_pickle(test_filepath))
+        actual.table_name = expected.table_name
 
+        print_test_result(
+            expected=ptw.dumps_tabledata(expected), actual=ptw.dumps_tabledata(actual.tabledata)
+        )
 
-class Test_PythonCodeTableWriter_write_table:
+        assert ptw.dumps_tabledata(actual.tabledata) == ptw.dumps_tabledata(expected)
 
     @pytest.mark.parametrize(
-        ["table", "indent", "header", "value", "expected"],
-        [
-            [data.table, data.indent, data.header, data.value, data.expected]
-            for data in normal_test_data_list
-        ]
+        ["table", "header", "value", "expected"],
+        [[data.table, data.header, data.value, data.expected] for data in empty_test_data_list],
     )
-    def test_normal(self, capsys, table, indent, header, value, expected):
-        writer = table_writer_class()
-        writer.table_name = table
-        writer.set_indent_level(indent)
-        writer.header_list = header
-        writer.value_matrix = value
+    def test_smoke_empty(self, tmpdir, table, header, value, expected):
+        test_filepath = str(tmpdir.join("empty.pkl"))
+        writer = ptw.PandasDataFramePickleWriter(
+            table_name=table, headers=header, value_matrix=value
+        )
+        writer.open(test_filepath)
         writer.write_table()
+        assert not os.path.isfile(test_filepath)
 
-        out, _err = capsys.readouterr()
-        assert out == expected
+    def test_exception(self):
+        writer = ptw.PandasDataFramePickleWriter(
+            table_name="tablename",
+            headers=["ha", "hb", "hc"],
+            value_matrix=[[1.0, 2.0, 3.0], [11.0, 12.0, 13.0], [1.0, 2.0, 3.0]],
+        )
 
-    @pytest.mark.parametrize(
-        ["table", "indent", "header", "value", "expected"],
-        [
-            [data.table, data.indent, data.header, data.value, data.expected]
-            for data in null_test_data_list
-        ]
-    )
-    def test_exception(self, capsys, table, indent, header, value, expected):
-        writer = table_writer_class()
-        writer.table_name = table
-        writer.set_indent_level(indent)
-        writer.header_list = header
-        writer.value_matrix = value
+        writer.write_table()
 
-        with pytest.raises(expected):
-            writer.write_table()
 
+@pytest.mark.skipif(SKIP_DATAFRAME_TEST, reason="required package not found")
+class Test_PandasDataFramePickleWriter_dump:
+    def test_normal_single_table(self, tmpdir):
+        test_filepath = str(tmpdir.join("test.pkl"))
+        data = TableData(
+            "tablename", ["ha", "hb", "hc"], [[1.0, 2.0, 3.0], [11.0, 12.0, 13.0], [1.0, 2.0, 3.0]]
+        )
 
-class Test_PythonCodeTableWriter_write_table_iter:
+        writer = ptw.PandasDataFramePickleWriter()
+        writer.from_tabledata(data)
+        writer.dump(test_filepath)
 
-    @pytest.mark.parametrize(["table", "header", "value", "expected"], [
-        [
-            "tablename",
-            ["ha", "hb", "hc"],
-            value_matrix_iter,
-            """tablename = [
-    ["ha", "hb", "hc"],
-    [1, 2, 3],
-    [11, 12, 13],
-    [1, 2, 3],
-    [11, 12, 13],
-    [101, 102, 103],
-    [1001, 1002, 1003],
-]
-""",
-        ],
-    ])
-    def test_normal(self, capsys, table, header, value, expected):
-        writer = table_writer_class()
-        writer.table_name = table
-        writer.header_list = header
-        writer.value_matrix = value
-        writer.iteration_length = len(value)
-        writer.write_table_iter()
+        actual = ptw.PandasDataFramePickleWriter()
+        actual.from_dataframe(pd.read_pickle(test_filepath))
+        actual.table_name = data.table_name
 
-        out, _err = capsys.readouterr()
-        assert out == expected
+        assert actual.tabledata == data
 
-    @pytest.mark.parametrize(
-        ["table", "header", "value", "expected"],
-        [
-            [data.table, data.header, data.value, data.expected]
-            for data in null_test_data_list
-        ]
-    )
-    def test_exception(self, capsys, table, header, value, expected):
-        writer = table_writer_class()
-        writer.table_name = table
-        writer.header_list = header
-        writer.value_matrix = value
+    def test_normal_multi_table(self, tmpdir):
+        test_filepath = str(tmpdir.join("test.pkl"))
+        data = TableData("first", ["ha1", "hb1", "hc1"], [[1.0, 2.0, 3.0], [11.0, 12.0, 13.0]])
+        writer = ptw.PandasDataFramePickleWriter()
+
+        writer.from_tabledata(data)
+        writer.dump(test_filepath, close_after_write=False)
+
+        actual = ptw.PandasDataFramePickleWriter()
+        actual.from_dataframe(pd.read_pickle(test_filepath))
+        actual.table_name = data.table_name
+
+        assert actual.tabledata == data
+
+
+class Test_PandasDataFramePickleWriter_dumps:
+    def test_exception(self, tmpdir):
+        writer = ptw.PandasDataFramePickleWriter()
 
-        with pytest.raises(expected):
-            writer.write_table_iter()
+        with pytest.raises(NotImplementedError):
+            writer.dumps()
```

### Comparing `pytablewriter-0.9.0/test/test_rst_grid_writer.py` & `pytablewriter-1.0.0/test/writer/text/rst/test_rst_grid_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,241 +1,360 @@
-# encoding: utf-8
-
 """
-.. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
+.. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from __future__ import absolute_import
+from textwrap import dedent
 
-import pytablewriter
 import pytest
+from tabledata import TableData
+
+import pytablewriter
 
-from .data import Data
-from .data import null_test_data_list
-from .data import header_list
-from .data import value_matrix
-from .data import value_matrix_with_none
-from .data import mix_header_list
-from .data import mix_value_matrix
+from ...._common import print_test_result
+from ....data import (
+    Data,
+    headers,
+    mix_header_list,
+    mix_value_matrix,
+    null_test_data_list,
+    value_matrix,
+    value_matrix_with_none,
+    vut_style_tabledata,
+    vut_styles,
+)
+from .._common import regexp_ansi_escape, strip_ansi_escape
 
 
 normal_test_data_list = [
     Data(
         table="table name",
         indent=0,
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        expected=""".. table:: table name
-
-    +-+-----+---+---+----+
-    |a|  b  | c |dd | e  |
-    +=+=====+===+===+====+
-    |1|123.1|a  |1.0|1   |
-    +-+-----+---+---+----+
-    |2|  2.2|bb |2.2|2.2 |
-    +-+-----+---+---+----+
-    |3|  3.3|ccc|3.0|cccc|
-    +-+-----+---+---+----+
-"""
+        expected=dedent(
+            """\
+            .. table:: table name
+
+                +-+-----+---+---+----+
+                |a|  b  | c |dd | e  |
+                +=+=====+===+===+====+
+                |1|123.1|a  |1.0|   1|
+                +-+-----+---+---+----+
+                |2|  2.2|bb |2.2| 2.2|
+                +-+-----+---+---+----+
+                |3|  3.3|ccc|3.0|cccc|
+                +-+-----+---+---+----+
+            """
+        ),
     ),
     Data(
         table="",
         indent=0,
-        header=header_list,
+        header=headers,
         value=None,
-        expected=""".. table:: 
-
-    +-+-+-+--+-+
-    |a|b|c|dd|e|
-    +=+=+=+==+=+
-    +-+-+-+--+-+
-"""
+        expected=dedent(
+            """\
+            .. table::
+
+                +-+-+-+--+-+
+                |a|b|c|dd|e|
+                +=+=+=+==+=+
+                +-+-+-+--+-+
+            """
+        ),
     ),
     Data(
         table=None,
         indent=0,
         header=None,
         value=value_matrix,
-        expected=""".. table:: 
-
-    +-+-----+---+---+----+
-    |1|123.1|a  |1.0|1   |
-    +-+-----+---+---+----+
-    |2|  2.2|bb |2.2|2.2 |
-    +-+-----+---+---+----+
-    |3|  3.3|ccc|3.0|cccc|
-    +-+-----+---+---+----+
-"""
+        expected=dedent(
+            """\
+            .. table::
+
+                +-+-----+---+---+----+
+                |1|123.1|a  |1.0|   1|
+                +-+-----+---+---+----+
+                |2|  2.2|bb |2.2| 2.2|
+                +-+-----+---+---+----+
+                |3|  3.3|ccc|3.0|cccc|
+                +-+-----+---+---+----+
+            """
+        ),
     ),
     Data(
-        table=None,
+        table="INDENTATION",
         indent=1,
-        header=header_list,
+        header=headers,
         value=value_matrix,
-        expected="""    .. table:: 
-    
+        expected="""    .. table:: INDENTATION
+
         +-+-----+---+---+----+
         |a|  b  | c |dd | e  |
         +=+=====+===+===+====+
-        |1|123.1|a  |1.0|1   |
+        |1|123.1|a  |1.0|   1|
         +-+-----+---+---+----+
-        |2|  2.2|bb |2.2|2.2 |
+        |2|  2.2|bb |2.2| 2.2|
         +-+-----+---+---+----+
         |3|  3.3|ccc|3.0|cccc|
         +-+-----+---+---+----+
-"""
+""",
     ),
     Data(
         table="zone",
         indent=0,
         header=["zone_id", "country_code", "zone_name"],
         value=[
             ["1", "AD", "Europe/Andorra"],
             ["2", "AE", "Asia/Dubai"],
             ["3", "AF", "Asia/Kabul"],
             ["4", "AG", "America/Antigua"],
-            ["5", "AI", "America/Anguilla"],
+            ["5", "AI", "America\nAnguilla"],
         ],
-        expected=""".. table:: zone
-
-    +-------+------------+----------------+
-    |zone_id|country_code|   zone_name    |
-    +=======+============+================+
-    |      1|AD          |Europe/Andorra  |
-    +-------+------------+----------------+
-    |      2|AE          |Asia/Dubai      |
-    +-------+------------+----------------+
-    |      3|AF          |Asia/Kabul      |
-    +-------+------------+----------------+
-    |      4|AG          |America/Antigua |
-    +-------+------------+----------------+
-    |      5|AI          |America/Anguilla|
-    +-------+------------+----------------+
-"""
+        expected=dedent(
+            """\
+            .. table:: zone
+
+                +-------+------------+----------------+
+                |zone_id|country_code|   zone_name    |
+                +=======+============+================+
+                |      1|AD          |Europe/Andorra  |
+                +-------+------------+----------------+
+                |      2|AE          |Asia/Dubai      |
+                +-------+------------+----------------+
+                |      3|AF          |Asia/Kabul      |
+                +-------+------------+----------------+
+                |      4|AG          |America/Antigua |
+                +-------+------------+----------------+
+                |      5|AI          |America Anguilla|
+                +-------+------------+----------------+
+            """
+        ),
     ),
     Data(
-        table="table name",
+        table="table with None values.",
         indent=0,
-        header=header_list,
+        header=headers,
         value=value_matrix_with_none,
-        expected=""".. table:: table name
-
-    +-+---+---+---+----+
-    |a| b | c |dd | e  |
-    +=+===+===+===+====+
-    |1|   |a  |1.0|    |
-    +-+---+---+---+----+
-    | |2.2|   |2.2|2.2 |
-    +-+---+---+---+----+
-    |3|3.3|ccc|   |cccc|
-    +-+---+---+---+----+
-    | |   |   |   |    |
-    +-+---+---+---+----+
-"""
+        expected=dedent(
+            """\
+            .. table:: table with None values.
+
+                +-+---+---+---+----+
+                |a| b | c |dd | e  |
+                +=+===+===+===+====+
+                |1|   |a  |1.0|    |
+                +-+---+---+---+----+
+                | |2.2|   |2.2| 2.2|
+                +-+---+---+---+----+
+                |3|3.3|ccc|   |cccc|
+                +-+---+---+---+----+
+                | |   |   |   |    |
+                +-+---+---+---+----+
+            """
+        ),
     ),
     Data(
-        table="table name",
+        table="Mixed-Type-Columns",
         indent=0,
         header=mix_header_list,
         value=mix_value_matrix,
-        expected=""".. table:: table name
-
-    +-+----+----+----+---+-----+---+---+-------+------------------------+
-    |i| f  | c  | if |ifc|bool |inf|nan|mix_num|          time          |
-    +=+====+====+====+===+=====+===+===+=======+========================+
-    |1|1.10|aa  | 1.0|1  |True |inf|nan|    1.0|2017-01-01 00:00:00     |
-    +-+----+----+----+---+-----+---+---+-------+------------------------+
-    |2|2.20|bbb | 2.2|2.2|False|inf|nan|    inf|2017-01-02 03:04:05+0900|
-    +-+----+----+----+---+-----+---+---+-------+------------------------+
-    |3|3.33|cccc|-3.0|ccc|True |inf|nan|    nan|2017-01-01 00:00:00     |
-    +-+----+----+----+---+-----+---+---+-------+------------------------+
-"""
+        expected=dedent(
+            """\
+            .. table:: Mixed-Type-Columns
+
+                +-+----+----+----+---+-----+--------+---+--------+-------------------------+
+                |i| f  | c  | if |ifc|bool |  inf   |nan|mix_num |          time           |
+                +=+====+====+====+===+=====+========+===+========+=========================+
+                |1|1.10|aa  | 1.0|  1|True |Infinity|NaN|       1|2017-01-01T00:00:00      |
+                +-+----+----+----+---+-----+--------+---+--------+-------------------------+
+                |2|2.20|bbb | 2.2|2.2|False|Infinity|NaN|Infinity|2017-01-02 03:04:05+09:00|
+                +-+----+----+----+---+-----+--------+---+--------+-------------------------+
+                |3|3.33|cccc|-3.0|ccc|True |Infinity|NaN|     NaN|2017-01-01T00:00:00      |
+                +-+----+----+----+---+-----+--------+---+--------+-------------------------+
+            """
+        ),
     ),
     Data(
         table="table name",
         indent=0,
         header=["int", "float", "str", "bool", "mix", "time"],
         value=[
-            [0,   0.1,      "hoge", True,   0,
-                "2017-01-01 03:04:05+0900"],
-            [2,   "-2.23",  "foo",  False,  None,
-                "2017-12-23 12:01:23+0900"],
-            [3,   0,        "bar",  "true",
-                "inf", "2017-03-03 22:44:55+0900"],
-            [-10, -9.9,     "",     "FALSE",
-                "nan", "2017-01-01 00:00:00+0900"],
+            [0, 0.1, "hoge", True, 0, "2017-01-01 03:04:05+0900"],
+            [2, "-2.23", "foo", False, None, "2017-12-23 12:01:23+0900"],
+            [3, 0, "bar", "true", "inf", "2017-03-03 22:44:55+0900"],
+            [-10, -9.9, "", "FALSE", "nan", "2017-01-01 00:00:00+0900"],
         ],
-        expected=""".. table:: table name
-
-    +---+-----+----+-----+---+------------------------+
-    |int|float|str |bool |mix|          time          |
-    +===+=====+====+=====+===+========================+
-    |  0|  0.1|hoge|True |  0|2017-01-01 03:04:05+0900|
-    +---+-----+----+-----+---+------------------------+
-    |  2| -2.2|foo |False|   |2017-12-23 12:01:23+0900|
-    +---+-----+----+-----+---+------------------------+
-    |  3|  0.0|bar |True |inf|2017-03-03 22:44:55+0900|
-    +---+-----+----+-----+---+------------------------+
-    |-10| -9.9|    |False|nan|2017-01-01 00:00:00+0900|
-    +---+-----+----+-----+---+------------------------+
-"""
+        expected=dedent(
+            """\
+            .. table:: table name
+
+                +---+-----+----+-----+--------+------------------------+
+                |int|float|str |bool |  mix   |          time          |
+                +===+=====+====+=====+========+========================+
+                |  0| 0.10|hoge|True |       0|2017-01-01 03:04:05+0900|
+                +---+-----+----+-----+--------+------------------------+
+                |  2|-2.23|foo |False|        |2017-12-23 12:01:23+0900|
+                +---+-----+----+-----+--------+------------------------+
+                |  3| 0.00|bar |True |Infinity|2017-03-03 22:44:55+0900|
+                +---+-----+----+-----+--------+------------------------+
+                |-10|-9.90|    |False|     NaN|2017-01-01 00:00:00+0900|
+                +---+-----+----+-----+--------+------------------------+
+            """
+        ),
+    ),
+    Data(
+        table="line breaks will be converted to a white space",
+        indent=0,
+        header=["a\nb", "\nc\n\nd\n", "e\r\nf"],
+        value=[["v1\nv1", "v2\n\nv2", "v3\r\nv3"]],
+        expected=dedent(
+            """\
+            .. table:: line breaks will be converted to a white space
+
+                +-----+------+-----+
+                | a b | c  d | e f |
+                +=====+======+=====+
+                |v1 v1|v2  v2|v3 v3|
+                +-----+------+-----+
+            """
+        ),
     ),
 ]
 
 table_writer_class = pytablewriter.RstGridTableWriter
 
 
 class Test_RstGridTableWriter_write_new_line:
-
     def test_normal(self, capsys):
         writer = table_writer_class()
         writer.write_null_line()
 
         out, _err = capsys.readouterr()
+
         assert out == "\n"
 
 
 class Test_RstGridTableWriter_write_table:
-
     @pytest.mark.parametrize(
         ["table", "indent", "header", "value", "expected"],
         [
             [data.table, data.indent, data.header, data.value, data.expected]
             for data in normal_test_data_list
-        ]
+        ],
     )
     def test_normal(self, capsys, table, indent, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
         writer.set_indent_level(indent)
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
         writer.write_table()
 
-        out, _err = capsys.readouterr()
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
+        assert out == expected
+        assert writer.dumps() == expected
+        assert str(writer) == expected
+
+    def test_normal_margin_1(self, capsys):
+        writer = table_writer_class()
+        writer.from_tabledata(TableData("margin 1", headers, value_matrix))
+        writer.margin = 1
+        writer.write_table()
+
+        expected = dedent(
+            """\
+            .. table:: margin 1
+
+                +---+-------+-----+-----+------+
+                | a |   b   |  c  | dd  |  e   |
+                +===+=======+=====+=====+======+
+                | 1 | 123.1 | a   | 1.0 |    1 |
+                +---+-------+-----+-----+------+
+                | 2 |   2.2 | bb  | 2.2 |  2.2 |
+                +---+-------+-----+-----+------+
+                | 3 |   3.3 | ccc | 3.0 | cccc |
+                +---+-------+-----+-----+------+
+            """
+        )
+
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
         assert out == expected
 
+    def test_normal_margin_2(self, capsys):
+        writer = table_writer_class()
+        writer.from_tabledata(TableData("margin 2", headers, value_matrix))
+        writer.margin = 2
+        writer.write_table()
+
+        expected = dedent(
+            """\
+            .. table:: margin 2
+
+                +-----+---------+-------+-------+--------+
+                |  a  |    b    |   c   |  dd   |   e    |
+                +=====+=========+=======+=======+========+
+                |  1  |  123.1  |  a    |  1.0  |     1  |
+                +-----+---------+-------+-------+--------+
+                |  2  |    2.2  |  bb   |  2.2  |   2.2  |
+                +-----+---------+-------+-------+--------+
+                |  3  |    3.3  |  ccc  |  3.0  |  cccc  |
+                +-----+---------+-------+-------+--------+
+            """
+        )
+
+        out, err = capsys.readouterr()
+        print_test_result(expected=expected, actual=out, error=err)
+
+        assert out == expected
+
+    def test_normal_styles(self):
+        writer = table_writer_class()
+        writer.from_tabledata(vut_style_tabledata)
+        writer.column_styles = vut_styles
+
+        expected = dedent(
+            """\
+            .. table:: style test
+
+                +----+-----+----+-----+------+-----+------------+--------+--------+-------------+
+                |none|empty|tiny|small|medium|large|null w/ bold| L bold |S italic|L bold italic|
+                +====+=====+====+=====+======+=====+============+========+========+=============+
+                | 111|  111| 111|  111|   111|  111|            | **111**|   *111*|      **111**|
+                +----+-----+----+-----+------+-----+------------+--------+--------+-------------+
+                |1234| 1234|1234| 1234| 1,234|1 234|            |**1234**|  *1234*|     **1234**|
+                +----+-----+----+-----+------+-----+------------+--------+--------+-------------+
+            """
+        )
+        out = writer.dumps()
+        print_test_result(expected=expected, actual=out)
+
+        assert regexp_ansi_escape.search(out)
+        assert strip_ansi_escape(out) == expected
+
     @pytest.mark.parametrize(
         ["table", "indent", "header", "value", "expected"],
         [
             [data.table, data.indent, data.header, data.value, data.expected]
             for data in null_test_data_list
-        ]
+        ],
     )
-    def test_exception(self, capsys, table, indent, header, value, expected):
+    def test_normal_empty(self, table, indent, header, value, expected):
         writer = table_writer_class()
         writer.table_name = table
         writer.set_indent_level(indent)
-        writer.header_list = header
+        writer.headers = header
         writer.value_matrix = value
 
-        with pytest.raises(expected):
-            writer.write_table()
+        assert writer.dumps() == ".. table:: dummy\n\n"
 
 
 class Test_RstGridTableWriter_write_table_iter:
-
     def test_exception(self):
         writer = table_writer_class()
 
         with pytest.raises(pytablewriter.NotSupportedError):
             writer.write_table_iter()
```

### Comparing `pytablewriter-0.9.0/LICENSE` & `pytablewriter-1.0.0/LICENSE`

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

