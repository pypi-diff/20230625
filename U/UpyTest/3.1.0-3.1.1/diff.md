# Comparing `tmp/UpyTest-3.1.0.tar.gz` & `tmp/UpyTest-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.1.0.tar", last modified: Sat Jun 24 22:59:11 2023, max compression
+gzip compressed data, was "UpyTest-3.1.1.tar", last modified: Sat Jun 24 23:05:20 2023, max compression
```

## Comparing `UpyTest-3.1.0.tar` & `UpyTest-3.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.374677 UpyTest-3.1.0/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 22:59:11.374677 UpyTest-3.1.0/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.362676 UpyTest-3.1.0/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 22:59:11.000000 UpyTest-3.1.0/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2311 2023-06-24 22:59:11.000000 UpyTest-3.1.0/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-24 22:59:11.000000 UpyTest-3.1.0/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 22:59:11.000000 UpyTest-3.1.0/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 22:59:11.000000 UpyTest-3.1.0/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-24 22:59:11.374677 UpyTest-3.1.0/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-24 22:59:04.000000 UpyTest-3.1.0/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.366677 UpyTest-3.1.0/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.0/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.0/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.366677 UpyTest-3.1.0/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.0/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35341 2023-06-24 19:19:49.000000 UpyTest-3.1.0/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.0/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4560 2023-06-24 00:10:31.000000 UpyTest-3.1.0/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.0/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.366677 UpyTest-3.1.0/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/SetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.0/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.366677 UpyTest-3.1.0/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.370677 UpyTest-3.1.0/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.0/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.0/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.0/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.0/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.370677 UpyTest-3.1.0/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.0/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1469 2023-06-23 23:48:13.000000 UpyTest-3.1.0/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.0/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.370677 UpyTest-3.1.0/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.0/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.370677 UpyTest-3.1.0/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2768 2023-06-24 15:25:01.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17790 2023-06-24 18:09:36.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36633 2023-06-24 19:59:14.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3544 2023-06-24 22:57:49.000000 UpyTest-3.1.0/thonnycontrib/l1test_frontend/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9423 2023-06-24 22:56:36.000000 UpyTest-3.1.0/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2401 2023-06-24 04:10:46.000000 UpyTest-3.1.0/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:59:11.374677 UpyTest-3.1.0/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.0/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.0/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.0/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.0/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21712 2023-06-24 03:26:11.000000 UpyTest-3.1.0/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.409857 UpyTest-3.1.1/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 23:05:20.409857 UpyTest-3.1.1/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2311 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-24 23:05:20.409857 UpyTest-3.1.1/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-24 23:04:31.000000 UpyTest-3.1.1/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.1/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.1/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.1/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35341 2023-06-24 19:19:49.000000 UpyTest-3.1.1/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.1/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4560 2023-06-24 00:10:31.000000 UpyTest-3.1.1/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.1/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/SetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.1/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.1/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.1/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.1/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1469 2023-06-23 23:48:13.000000 UpyTest-3.1.1/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.1/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.1/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2768 2023-06-24 15:25:01.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17790 2023-06-24 18:09:36.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36633 2023-06-24 19:59:14.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3544 2023-06-24 22:57:49.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9423 2023-06-24 22:56:36.000000 UpyTest-3.1.1/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2401 2023-06-24 04:10:46.000000 UpyTest-3.1.1/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.409857 UpyTest-3.1.1/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21712 2023-06-24 03:26:11.000000 UpyTest-3.1.1/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.1.0/PKG-INFO` & `UpyTest-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.0
+Version: 3.1.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.0/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.1.1/UpyTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.0
+Version: 3.1.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.0/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.1.1/UpyTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/setup.py` & `UpyTest-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.1.0",
+    version="3.1.1",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.1.0/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.1.1/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.1.1/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.1.1/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/evaluator.py` & `UpyTest-3.1.1/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.1.1/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/test_finder.py` & `UpyTest-3.1.1/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/verdicts/FailedVerdict.py` & `UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/error_icon.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/failed.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/outline_class.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/outline_method.gif` & `UpyTest-3.1.1/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/passed.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/restart_icon.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docs/res/warning.png` & `UpyTest-3.1.1/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/environement_vars.py` & `UpyTest-3.1.1/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/exceptions.py` & `UpyTest-3.1.1/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.1.1/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/__init__.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/l1test_frontend/outlines.py` & `UpyTest-3.1.1/thonnycontrib/l1test_frontend/outlines.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/plugin_loader.py` & `UpyTest-3.1.1/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/properties.py` & `UpyTest-3.1.1/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.1.1/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/tests/tests_view.py` & `UpyTest-3.1.1/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.0/thonnycontrib/utils.py` & `UpyTest-3.1.1/thonnycontrib/utils.py`

 * *Files identical despite different names*

