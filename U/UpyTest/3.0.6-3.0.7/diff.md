# Comparing `tmp/UpyTest-3.0.6.tar.gz` & `tmp/UpyTest-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.0.6.tar", last modified: Mon May  1 00:19:53 2023, max compression
+gzip compressed data, was "UpyTest-3.0.7.tar", last modified: Sat Jun 24 22:35:59 2023, max compression
```

## Comparing `UpyTest-3.0.6.tar` & `UpyTest-3.0.7.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.449178 UpyTest-3.0.6/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-05-01 00:19:53.449178 UpyTest-3.0.6/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.441178 UpyTest-3.0.6/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-05-01 00:19:53.000000 UpyTest-3.0.6/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2192 2023-05-01 00:19:53.000000 UpyTest-3.0.6/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-05-01 00:19:53.000000 UpyTest-3.0.6/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-05-01 00:19:53.000000 UpyTest-3.0.6/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-05-01 00:19:53.000000 UpyTest-3.0.6/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-05-01 00:19:53.449178 UpyTest-3.0.6/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-05-01 00:19:48.000000 UpyTest-3.0.6/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.441178 UpyTest-3.0.6/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.6/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.445178 UpyTest-3.0.6/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 22:45:13.000000 UpyTest-3.0.6/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:44:56.000000 UpyTest-3.0.6/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.6/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.6/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.6/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.445178 UpyTest-3.0.6/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/EmptyTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/ExceptionTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/FailedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/PassedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/Test.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.445178 UpyTest-3.0.6/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.445178 UpyTest-3.0.6/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.0.6/thonnycontrib/docs/res/outline-class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.0.6/thonnycontrib/docs/res/outline-method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.449178 UpyTest-3.0.6/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.6/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.6/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.449178 UpyTest-3.0.6/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.6/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.449178 UpyTest-3.0.6/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17883 2023-05-01 00:19:18.000000 UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36644 2023-04-20 23:21:08.000000 UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3328 2023-04-23 13:33:11.000000 UpyTest-3.0.6/thonnycontrib/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9776 2023-04-30 23:34:26.000000 UpyTest-3.0.6/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.6/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:19:53.449178 UpyTest-3.0.6/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.6/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.6/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.6/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.6/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.6/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.625978 UpyTest-3.0.7/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 22:35:59.625978 UpyTest-3.0.7/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.613978 UpyTest-3.0.7/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 22:35:59.000000 UpyTest-3.0.7/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2295 2023-06-24 22:35:59.000000 UpyTest-3.0.7/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-24 22:35:59.000000 UpyTest-3.0.7/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 22:35:59.000000 UpyTest-3.0.7/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 22:35:59.000000 UpyTest-3.0.7/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-24 22:35:59.625978 UpyTest-3.0.7/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-24 22:35:54.000000 UpyTest-3.0.7/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.613978 UpyTest-3.0.7/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      946 2023-06-24 15:21:28.000000 UpyTest-3.0.7/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      297 2023-06-21 20:49:58.000000 UpyTest-3.0.7/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.617978 UpyTest-3.0.7/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.0.7/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35341 2023-06-24 19:19:49.000000 UpyTest-3.0.7/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.0.7/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4560 2023-06-24 00:10:31.000000 UpyTest-3.0.7/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.0.7/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.617978 UpyTest-3.0.7/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/SetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.0.7/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.617978 UpyTest-3.0.7/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.621978 UpyTest-3.0.7/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.0.7/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.0.7/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.0.7/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.0.7/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.621978 UpyTest-3.0.7/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.0.7/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1469 2023-06-23 23:48:13.000000 UpyTest-3.0.7/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.0.7/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.621978 UpyTest-3.0.7/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.7/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.621978 UpyTest-3.0.7/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2768 2023-06-24 15:25:01.000000 UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17790 2023-06-24 18:09:36.000000 UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36633 2023-06-24 19:59:14.000000 UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3517 2023-06-24 19:53:43.000000 UpyTest-3.0.7/thonnycontrib/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9404 2023-06-24 00:13:45.000000 UpyTest-3.0.7/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2401 2023-06-24 04:10:46.000000 UpyTest-3.0.7/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:35:59.625978 UpyTest-3.0.7/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.7/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.7/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.7/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.0.7/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21712 2023-06-24 03:26:11.000000 UpyTest-3.0.7/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.0.6/PKG-INFO` & `UpyTest-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.6
+Version: 3.0.7
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.0.6/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.0.7/UpyTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.6
+Version: 3.0.7
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.0.6/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.0.7/UpyTest.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,31 @@
 thonnycontrib/utils.py
 thonnycontrib/backend/__init__.py
 thonnycontrib/backend/ast_parser.py
 thonnycontrib/backend/doctest_parser.py
 thonnycontrib/backend/evaluator.py
 thonnycontrib/backend/l1test_backend.py
 thonnycontrib/backend/test_finder.py
-thonnycontrib/backend/verdicts/EmptyTest.py
-thonnycontrib/backend/verdicts/ExceptionTest.py
-thonnycontrib/backend/verdicts/FailedTest.py
-thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
-thonnycontrib/backend/verdicts/PassedTest.py
-thonnycontrib/backend/verdicts/Test.py
+thonnycontrib/backend/verdicts/ExampleVerdict.py
+thonnycontrib/backend/verdicts/ExceptionVerdict.py
+thonnycontrib/backend/verdicts/FailedVerdict.py
+thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+thonnycontrib/backend/verdicts/PassedVerdict.py
+thonnycontrib/backend/verdicts/SetupVerdict.py
 thonnycontrib/backend/verdicts/__init__.py
 thonnycontrib/docs/__init__.py
+thonnycontrib/docs/res/error_icon.png
 thonnycontrib/docs/res/failed.png
 thonnycontrib/docs/res/l1test_icon.png
 thonnycontrib/docs/res/l1test_icon_old.png
-thonnycontrib/docs/res/outline-class.png
-thonnycontrib/docs/res/outline-method.gif
+thonnycontrib/docs/res/outline_class.png
+thonnycontrib/docs/res/outline_method.gif
 thonnycontrib/docs/res/passed.png
 thonnycontrib/docs/res/pending_icon.png
+thonnycontrib/docs/res/restart_icon.png
 thonnycontrib/docs/res/test_only_btn.png
 thonnycontrib/docs/res/warning.png
 thonnycontrib/docstring_generator/__init__.py
 thonnycontrib/docstring_generator/doc_generator.py
 thonnycontrib/docstring_generator/doc_template.py
 thonnycontrib/l1test_configuration/__init__.py
 thonnycontrib/l1test_configuration/l1test_options.py
```

### Comparing `UpyTest-3.0.6/setup.py` & `UpyTest-3.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.0.6",
+    version="3.0.7",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.0.6/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.0.7/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 '''
 Permet de générer pour le plugin de log une synthèse des tests exécutés.
 Corentin.
 '''
 
+from typing import List
 from thonny import get_workbench
+from .backend.ast_parser import L1DocTest
 
 #Attention si le nom change ici, il faut aussi le changer dans Thonny-LoggingPlugin
 NOM_EVENT_TEST = "l1Tests"
 NOM_EVENT_DOC = "l1Tests.DocGenerator"
 wb = get_workbench()
 
-def log_in_thonny(test_results, selected):
-    for i in test_results :
-        for j in test_results[i] :
-            wb.event_generate(NOM_EVENT_TEST, None, selected=selected, name=j.get_ast_node().name, **vars(j))
+def log_in_thonny(l1doctests: List[L1DocTest], selected):
+    for l1doctest in l1doctests:
+        for example in l1doctest.get_examples():
+            wb.event_generate(NOM_EVENT_TEST, None, selected=selected, name=l1doctest.get_name(), **vars(example))
 
 def log_doc_in_thonny(node):
     if wb:
-        wb.event_generate(NOM_EVENT_DOC, None, name=node.name)
-    
+        wb.event_generate(NOM_EVENT_DOC,None, name = node.name)
 #La fonction anonyme car il faut une fonction pour bind, avec un argument parce qu'elle reçoit l'événement. 
 if wb:   
     wb.bind(NOM_EVENT_TEST, lambda x : 0, True)
-    wb.bind(NOM_EVENT_DOC, lambda x : 0, True)
+    wb.bind(NOM_EVENT_DOC, lambda x : 0, True)
```

### Comparing `UpyTest-3.0.6/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.0.7/thonnycontrib/backend/doctest_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,24 +38,24 @@
     # 3. Doctest Parser
     'DocTestParser',
 ]
 from abc import *
 import __future__
 import re
 from collections import namedtuple
-import sys
+import sys, ast
 
 # ajout L1test
 from thonnycontrib.properties import L1TEST_EXCEPTION_SYMBOL, L1TEST_SYMBOL1, L1TEST_SYMBOL2, L1TEST_SYMBOL3
 
-from thonnycontrib.backend.verdicts.EmptyTest import *
-from thonnycontrib.backend.verdicts.FailedTest import *
-from thonnycontrib.backend.verdicts.FailedWhenExceptionExpectedTest import *
-from thonnycontrib.backend.verdicts.PassedTest import *
-from thonnycontrib.backend.verdicts.ExceptionTest import *
+from .verdicts.FailedVerdict import *
+from .verdicts.FailedWhenExceptionExpectedVerdict import *
+from .verdicts.PassedVerdict import *
+from .verdicts.ExceptionVerdict import *
+from .verdicts.SetupVerdict import *
 
 from thonnycontrib.exceptions import *
 from thonnycontrib.utils import *
 
 TestResults = namedtuple('TestResults', 'failed attempted')
 
 # There are 2 basic classes:
@@ -173,53 +173,83 @@
         self.want = want
         self.lineno = lineno
         self.indent = indent
         self.invite = invite
         if options is None: options = {}
         self.options = options
         self.exc_msg = exc_msg
+        
+        # the verdict of this example. By default is an empty verdict.
+        self.__verdict:ExampleVerdict = None
 
     @abstractmethod
-    def exec_and_computes_verdict(self, node:ast, globals:dict={}, locals:dict={}):
+    def is_a_test(self) -> bool:
+        """
+        Returns:
+            bool: Return True if the example is considered to have an oracle. 
+            Return False if the example is considered as a setup.
+        """
         pass
     
-    def _execute_statement(self, source:str, globals:dict, locals:dict, lineno:int):
+    @abstractmethod
+    def _exec_and_computes_verdict(self, globals:dict={}):
+        '''Executes the example and returns a verdict, eg FailedTest,
+        PassedTest...
+
+        Args : 
+        - globals : the dict of globals variables
+        '''
+        pass
+    
+    def compute_and_set_verdict(self, globals:dict={}):
+        '''
+        This is the main method to evaluate and compute the verdict 
+        of an example. This method invokes the abstract method `_exec_and_computes_verdict`, 
+        then set the returned verdict to this example.
+        
+        Args : 
+        - globals : the dict of globals variables
+        '''
+        self.__verdict = self._exec_and_computes_verdict(globals)
+        return self.__verdict
+    
+    def _execute_statement(self, source:str, globals:dict, lineno:int):
         """
         Execute a source code using the given globals. 
         
         This function should be invoked after a `compile()`. The compile() function is removed from 
         this function because it's hard to know if an exception is raised by a compilation error
         or by an executed statement(using exec()). 
         
         Args:
             source (str): A string representing a source code. 
             globals (dict): The dictionary of the global variables.
-            locals (dict): The dictionary of the local variables. 
             lineno (int): The line of the test to execute.
         Raises:
             RuntimeException: When the source code raises a runtime error(ex. NameError...)
         """
         try:
-            exec(source, globals, locals)
+            exec(source, globals)
         except BaseException as e:
             error_info = sys.exc_info()
             formatted_error = replace_filename(self.filename, get_last_exception(error_info))
+            
             # For runtime errors the line mentionned in the error raised by `exec()` is always equal to 1.
             # To learn about runtime errors in python: https://www.geeksforgeeks.org/runtime-errors/
             has_error_lineno = re.search(r'line (\d+)', formatted_error)
             if has_error_lineno:
                 error_line = int(has_error_lineno.group(1))
                 # comme cette fonction est toujours appelée pour executer un test ou sa valeur attendu
                 # alors on aura jamais la ligne d'erreur est égal à 1. Donc, on remplace la ligne d'erreur
                 # par le numéro de ligne du test.
                 if error_line == 1: 
                     formatted_error = replace_error_line(formatted_error, lineno)
             raise RuntimeException(formatted_error)
     
-    def _check_source_syntax(self, source:str, lineno:int, mode="single"):
+    def _check_syntax(self, source:str, lineno:int, mode="single"):
         """
         Compile the `source` of a test statement and raise an exception when a 
         compilation error occurs.
 
         Args:
             source (str): The statement to be compiled
             mode (str): Defaults to "single".
@@ -227,31 +257,14 @@
             CompilationError: when a compilation error occurs.
         """
         try:
             compile(source, filename=self.filename, mode=mode)
         except Exception:
             formatted_error = get_last_exception(sys.exc_info())
             raise CompilationError(replace_error_line(formatted_error, lineno))
-
-    def _check_want_syntax(self, got:str, lineno:int, mode="single"):
-        """
-        Compile the `want` statement of a test and raise an exception when 
-        a compilation error occurs.
-
-        Args:
-            source (str): The statement to be compiled
-            mode (str): Defaults to "single".
-        Raises:
-            CompilationError: when a compilation error occurs.
-        """
-        try:
-            compile(got, filename=self.filename, mode=mode)
-        except Exception:
-            formatted_error = get_last_exception(sys.exc_info())
-            raise CompilationError(replace_error_line(formatted_error, lineno))
     
     def _create_affectation_statement(self, statement1, statement2):
         """
         Creates an affectation expression by affecting the statement2 to statement1.
 
         The result will be : "%s = %s" % (statement1, statement2)
         
@@ -259,165 +272,120 @@
             statement1 (str): the left side of the affectation expression
             statement2 (str): the right side of the affectation expression
 
         Returns:
             (str): the affectation expression using `statement1` and `statement1`. 
         """
         return "%s = (%s)" % (statement1, statement2)
+    
+    def get_verdict(self):
+        return self.__verdict
+    
+    def is_evaluated(self):
+        """Returns True if the example has a verdict, False otherwise."""
+        return self.__verdict is not None
         
     def __eq__(self, other):
         if type(self) is not type(other):
             return NotImplemented
 
         return self.filename == other.filename and \
                self.source == other.source and \
                self.want == other.want and \
                self.lineno == other.lineno and \
                self.indent == other.indent and \
                self.options == other.options and \
-               self.exc_msg == other.exc_msg
+               self.exc_msg == other.exc_msg and \
+               self.__verdict == other.get_verdict()
 
     def __hash__(self):
         return hash((self.filename, self.source, self.want, self.lineno, 
                      self.indent, self.exc_msg))
 
-        
-class ExampleWithExpected(Example):
-    """
-    An `ExampleWithExpected` is a test example that expects a value to be returned.
-    """
-    def exec_and_computes_verdict(self, node:ast, globals:dict={}, locals:dict={}):
-        executed, wanted = add_random_suffix("executed"), add_random_suffix("wanted")
-        want = self.want.strip("\n")   
-        try:             
-            # we should check the syntax of the `source` before executing it   
-            self._check_source_syntax(self.source, self.lineno)
-            # we should check the syntax of the `want` before executing it 
-            self._check_want_syntax(self.want, self.lineno)
-            
-            # si on est là alors la syntaxe de la source et du want est valide
-            # et on doit pouvoir les executer sans problème
-            self._execute_statement(self._create_affectation_statement(executed, self.source), 
-                                    globals, locals, self.lineno)
-            self._execute_statement(self._create_affectation_statement(wanted, self.want), 
-                                    globals, locals, self.lineno)
-            
-            self._check_source_syntax(self.str_comparaison(self.source, self.want), self.filename, "single")
-            
-            if locals[executed] == locals[wanted]:
-                verdict = PassedTest(self.filename, node=node, tested_line=self.source.strip(), 
-                                      expected_result=want, lineno=self.lineno)
-            else:
-                verdict = FailedTest(self.filename, node=node, tested_line=self.source.strip(), 
-                                      expected_result=want, obtained_result=locals[executed], 
-                                      lineno=self.lineno)
-        except (CompilationError, RuntimeException) as e:
-            verdict = ExceptionTest(self.filename, node=node, tested_line=self.source.strip(), 
-                                    expected_result=want, lineno=self.lineno, message=str(e))
-        return verdict
-
-    def str_comparaison(self, expected, got):
-        return  "(%s) == (%s)" % (expected, got) 
     
 class ExampleWithoutExpected(Example):
     """
     An `ExampleWithNoExpected` is an example without a `want` and cannot be considered as a test.
     """
-    def exec_and_computes_verdict(self, node:ast, globals:dict={}, locals:dict={}):
+    def _exec_and_computes_verdict(self, globals:dict={}):
         try:  
-            # we check the syntax of the test before its execution
-            self._check_source_syntax(self.source, self.lineno) 
-            self._execute_statement(self.source, globals, locals, self.lineno)
-            return None
+            # we chech the syntax of the test before its execution
+            self._check_syntax(self.source, self.lineno) 
+            self._execute_statement(self.source, globals, self.lineno)
+            return SetupVerdict(self.filename, tested_line=self.source, lineno=self.lineno)
         except (RuntimeException, CompilationError) as error:
-            return ExceptionTest(self.filename, node=node, tested_line=self.source.strip(), 
+            return ExceptionVerdict(self.filename, tested_line=self.source.strip(), 
                                  expected_result=self.want.strip("\n"), lineno=self.lineno, 
-                                 message=str(error))
+                                 error_details=str(error))
+            
+    def is_a_test(self) -> bool:
+        return False
 
 class ExampleExceptionExpected(Example):
     """
     An `ExampleExceptionExpected` is a test example that expects an exception to be raised.
-    """
-    def exec_and_computes_verdict(self, node:ast, globals:dict={}, locals:dict={}):
+    """    
+    def _exec_and_computes_verdict(self, globals:dict={}):
         want = self.want.strip("\n").strip()
         try:
-            self.__check_want_validity(want, globals)
-            return self.__execute_and_get_verdict_(node, globals, locals, want) 
+            self.__check_is_an_exception(self.want.strip("\n"))
+            # On vérifie si l'exception hérite de la BaseException
+            self.__is_exception_inherits_from_BaseException(globals, want)
+            return self.__execute_and_get_verdict(globals, want)  
         except (ValueError, TypeError, NameError) as e:
-            return self.__build_exception_verdict(e, node, want)      
+            error_msg = "%s:\n  %s" % (e.__class__.__name__, str(e))
+            return self.__build_exception_verdict(error_msg, want)         
     
-    def __execute_and_get_verdict_(self, node:ast.AST, globals, locals, want:str):
+    def __execute_and_get_verdict(self, globals, want:str):
         try:
             # il faudrait quand même compiler la source avant de l'executer
-            self._check_source_syntax(self.source, self.lineno)
+            self._check_syntax(self.source, self.lineno)
             
-            exec(self.source, globals, locals)
+            exec(self.source, globals)
             
             # si on est ici alors aucune exc levée -> FailedTest
             # <nom_exc> was not raised by <source>
-            failure_msg = "%s was not raised by %s" % (want, self.source.strip()) 
-            return FailedWhenExceptionExpectedTest(self.filename, node=node, tested_line=self.source.strip(), 
-                                expected_result=want,lineno=self.lineno, failure_message=failure_msg)        
+            return FailedWhenExceptionExpectedVerdict(self.filename, tested_line=self.source.strip(), 
+                                expected_result=want, lineno=self.lineno)
+            
         except BaseException as e: # ici on a forcément une exception levée par le code source
                 # mais a priori rien de syntaxique car on est sur un seul nom
             error_type, _, _ = sys.exc_info()    
             exc_name_effective = str(error_type.__name__)
             if want == exc_name_effective: 
-                return PassedTest(self.filename, node=node, tested_line=self.source.strip(), 
+                return PassedVerdict(self.filename, tested_line=self.source.strip(), 
                                     expected_result=want, lineno=self.lineno)   
             else: # forcément une erreur de compilation ou encore une erreur de runtime
                 # si c'est une erreur `CompilationError` alors on récupère seulement sa représentation      
                 if isinstance(e, CompilationError):   # if CompilationError -> ExceptionTest verdict
-                    return ExceptionTest(self.filename, node=node, tested_line=self.source.strip(), 
-                                            expected_result=want, lineno=self.lineno, message=str(e))
+                    return ExceptionVerdict(self.filename, tested_line=self.source.strip(), 
+                                            expected_result=want, lineno=self.lineno, error_details=str(e))
                 else: # sinon on doit chercher la dernière exception. 
-                    formatted_error = get_last_exception(sys.exc_info())                  
-                    failure_msg = "%s was not raised by %s\nInstead, it raises :\n%s" % (want, self.source.strip(), formatted_error) 
-                    return FailedWhenExceptionExpectedTest(self.filename, node=node, tested_line=self.source.strip(), 
+                    failure_msg = "Instead, it raises :\n%s" % (get_last_exception(sys.exc_info())) 
+                    return FailedWhenExceptionExpectedVerdict(self.filename, tested_line=self.source.strip(), 
                                 expected_result=want,lineno=self.lineno, failure_message=failure_msg) 
     
-    def __build_exception_verdict(self, exception, node, want):
+    def __build_exception_verdict(self, exception_msg, want):
         """
         Returns an exception verdict with the given exception message. 
 
         Args:
             exception_msg (str): The exception message
-            node (ast.AST): The node ast associated to that Example.
             want (str): The want of the Example.
 
         Returns:
             ExceptionTest: an exception verdict with the given exception message. 
         """
-        common_msg = 'File "%s", line %s\n' % (self.filename, self.lineno) 
-        error_msg = common_msg + "%s:\n  %s" % (exception.__class__.__name__, str(exception))
-        return ExceptionTest(self.filename, node=node, tested_line=self.source.strip(), 
-                             expected_result=want, lineno=self.lineno, 
-                             message=error_msg)  
-    
-    def __check_want_validity(self, want:str, globals:dict):
-        """_summary_
-        Checks if the <want> syntax is an exception and if it inherits 
-        from the BaseException class.
-        Args:
-            want (str): The value of the <want> to check.
-            globals (dict): The global is needed to look for the associated 
-            given exception.
+        common_msg = 'File "%s", line %s\n'%(self.filename, self.lineno+1) 
+        error_msg = common_msg + exception_msg
+        return ExceptionVerdict(self.filename, tested_line=self.source.strip(), 
+                                expected_result=want, lineno=self.lineno, 
+                                error_details=error_msg)  
         
-        Raises: 
-            - ValueError: when the want doesn't respect the syntaxe.
-            - TypeError: if the retrieved exception from the given exception name is not an exception that
-                        inherits from `BaseException`. 
-            - NameError: if cannot retrieve the exception from the given exception name.
-        """
-        # On vérifie si la syntaxe du <want> est une exception -> lève exception sinon
-        self.__is_an_exception(want)
-        # On vérifie si l'exception hérite de la BaseException -> lève exception sinon
-        self.__is_exception_inherits_from_BaseException(globals, want)
-        
-    def __is_an_exception(self, want):
+    def __check_is_an_exception(self, want):
         """Check if the want is a valid exception name that contains letters, 
         numbers and/or underscore.
 
         Args:
             want (str): a string.
 
         Raises:
@@ -479,14 +447,56 @@
                     return None
                 else:
                     raise TypeError("The expected exception `%s` is not a class of type exception." % exception_name) 
             except:
                 raise TypeError("The expected exception `%s` is not a class of type exception." % exception_name) 
         raise NameError("The expected exception `%s` cannot be found." % exception_name)
 
+    def is_a_test(self) -> bool:
+        return True
+    
+class ExampleWithExpected(Example):
+    """
+    An `ExampleWithExpected` is a test example that expects a value to be returned.
+    """
+    def is_a_test(self) -> bool:
+        return True
+    
+    def _exec_and_computes_verdict(self, globals:dict={}):
+        executed, wanted = add_random_suffix("executed"), add_random_suffix("wanted")
+        want = self.want.strip("\n")   
+        try:             
+            # we should check the syntax of the `source` before executing it   
+            self._check_syntax(self.source, self.lineno)
+            # we should check the syntax of the `want` before executing it 
+            self._check_syntax(self.want, self.lineno+1)
+            
+            # si on est là alors la syntaxe de la source et du want est valide
+            # et on doit pouvoir les executer sans problème
+            self._execute_statement(self._create_affectation_statement(executed, self.source), 
+                                    globals, self.lineno)
+            self._execute_statement(self._create_affectation_statement(wanted, self.want), 
+                                    globals, self.lineno+1)
+            
+            self._check_syntax(self.str_comparaison(self.source, self.want), self.filename, "single")
+            
+            if globals[executed] == globals[wanted]:
+                verdict = PassedVerdict(self.filename, tested_line=self.source.strip(), 
+                                      expected_result=want, lineno=self.lineno)
+            else:
+                verdict = FailedVerdict(self.filename, tested_line=self.source.strip(), 
+                                      expected_result=want, real_result=globals[executed], 
+                                      lineno=self.lineno)
+        except (CompilationError, RuntimeException) as e:
+            verdict = ExceptionVerdict(self.filename, tested_line=self.source.strip(), 
+                                    expected_result=want, lineno=self.lineno, error_details=str(e))
+        return verdict
+
+    def str_comparaison(self, expected, got):
+        return  "(%s) == (%s)" % (expected, got) 
     
     
 ######################################################################
 ## 3. DocTestParser
 ######################################################################
 
 class DocTestParser:
```

### Comparing `UpyTest-3.0.6/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.0.7/thonnycontrib/backend/l1test_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import os
 from types import ModuleType
 
-from thonnycontrib.backend.test_finder import FindSelectedL1DoctestStrategy
+from .test_finder import FindSelectedL1DoctestStrategy
 from ..exceptions import BackendException
 from ..environement_vars import *
 from .evaluator import Evaluator 
 from thonny.common import ToplevelCommand, ToplevelResponse
 from ..properties import BACKEND_COMMAND, L1TEST_EXCEPTION, VERDICTS
 # Ce n'est pas une API publique
 from thonny.plugins.cpython_backend.cp_back import (
     Executor,
     MainCPythonBackend
 )
 import thonny.plugins.cpython_backend.cp_back
 import pickle
-from ..properties import FINISHED_STATE
-from ..utils import send_current_state
 
 BACKEND: MainCPythonBackend = thonny.plugins.cpython_backend.cp_back.get_backend()
 
 def _cmd_l1test(cmd: ToplevelCommand) -> ToplevelResponse:   
     """
     Cette fonction est invoquée lorsque un événement de type `ToplevelCommand` (associé 
     à la commande L1test) est récupéré.
@@ -39,39 +37,38 @@
         """Cette fonction est invoquée par la méthode `BACKEND._execute_file(cmd, L1TestExecutor)`
         située en haut de ce fichier.
 
         Returns:
             dict: doit retourner, obligatoirement, un dictionnaire dont les données sont séralisées.
         """
         assert mode == "exec"
-        
-        is_selected = eval(os.environ.get(IS_SELECTED_VAR))
-        
         try:
             evaluator = Evaluator(filename, source)
             
+            is_selected = eval(os.environ.get(IS_SELECTED_VAR))
             if is_selected: # si un seul test a été ciblé
-                selected_line = int(os.environ[NODE_LINENO_VAR])
+                selected_line: int = int(os.environ.get(SELECTED_LINE_VAR))
                 evaluator.set_finder_strategy(FindSelectedL1DoctestStrategy(selected_line))
             
             verdicts = evaluator.evaluate()
             
             # on récupère la valeur de l'option qui indique si on doit importer le module dans le shell
-            import_module_option = eval(os.environ.get(IMPORT_MODULE_VAR))
+            import_module_option = eval(os.environ.get(IMPORT_MODULE_VAR)) 
+            # importation du module dans le shell.
             if import_module_option: 
                 # importation du module dans le shell.
                 self._import_module_in_shell(evaluator.get_module())                                                
             
             # Sérialiser les données en binaires. 
             serialized_data = pickle.dumps(verdicts)
             
             # The serialized data should necessary be a dictionary and the returned statement should
             # also be a dictionary
             return {VERDICTS: serialized_data}
-        except (BackendException, InterruptedError) as e:
+        except BaseException as e:
             # pas besoin de sérialiser la valeur du dictionaire car il conteint que des types primitifs.
             return {L1TEST_EXCEPTION: self._build_backend_exception(e, str(e))}
     
     def _import_module_in_shell(self, module:ModuleType):
         """
         Imports the given `module` into Thonny's shell.
```

### Comparing `UpyTest-3.0.6/thonnycontrib/backend/test_finder.py` & `UpyTest-3.0.7/thonnycontrib/backend/test_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             test_finder (TestFinder): The testFinder fo which the docstring 
             will be retrived.
 
         Returns:
             List[L1DocTest]: Returns a list of the L1DocTest. Each of L1DocTest 
             represents an AST node.
         """
-        ast_nodes = self.__parse_editor_content()
+        ast_nodes = self._ast_parser.get_supported_nodes()
         return self._find_docstring(ast_nodes)
     
     @abstractmethod
     def _find_docstring(self, ast_nodes: List[ast.AST]=[]) -> List[L1DocTest]:
         """Gets the docstrings from the source detained by the test_finder.
 
         Args:
@@ -53,26 +53,14 @@
             represents an AST node.
             
         Raises:
             The overriden methods could throw an exception. For each case, the raised 
             exceptions should be specified and explained into the docstrings.
         """
         pass
-    
-    def __parse_editor_content(self) -> List[ast.AST]:
-        """
-        Returns a list of AST nodes that may contains a doctsring.
-        
-        As the AST python module stated in its documentation, the AST nodes that can 
-        contain a dosctring are reported at ~SourceParser.SUPPORTED_TYPES~.
-        
-        Raises: 
-            Error: a compilation error raised by the AST module.
-        """
-        return self._ast_parser._get_supported_nodes()
 
     def get_ast_nodes(self):
         return self._ast_nodes 
     
     def set_ast_nodes(self, ast_nodes):
         self._ast_nodes = ast_nodes
     
@@ -80,17 +68,16 @@
         self._ast_parser.set_filename(filename)
     
     def set_source(self, source):
         self._ast_parser.set_source(source)
     
     
 class FindAllL1DoctestsStrategy(TestFinderStrategy):
-        
     def _find_docstring(self, ast_nodes):
-        return self._ast_parser.get_l1_doctests(ast_nodes)
+        return self._ast_parser.get_l1doctests(ast_nodes)
 
 
 class FindSelectedL1DoctestStrategy(TestFinderStrategy):
     def __init__(self, selected_line) -> None:
         super().__init__()
         self._selected_line = selected_line
     
@@ -104,24 +91,24 @@
             function or a class declaration.
         """
         selected_node = find_node(self._selected_line, ast_nodes)
         if not selected_node:
             msg = "%s\n\n%s" %  ("No function is selected to test !", 
                                  "The selected line must have a function or a class declaration.")
             raise NoFunctionSelectedToTestException(msg)
-        return self._ast_parser.get_l1_doctest(selected_node)
+        return self._ast_parser.get_l1doctest(selected_node)
     
     def get_selected_line(self):
         return self._selected_line    
     
     def set_selected_line(self, selected_line):
         self._selected_line = selected_line   
         
 
-class TestFinder:
+class L1TestFinder:
     """
         The `TestFinder` relies on the `AST` module to parse the script and extracts 
         the nodes with their docstrings. 
         
         For each node, it invokes the `DoctestParser` to parse its docstring. Then, 
         for each dectected test, it associates an `Example` type that will contains 
         the `source`, `want` and the `line` of the test.
```

### Comparing `UpyTest-3.0.6/thonnycontrib/backend/verdicts/FailedTest.py` & `UpyTest-3.0.7/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # Auteur : Esteban COLLARD, Nordine EL AMMARI
 
-from .Test import Test
+from .ExampleVerdict import ExampleVerdict
 
-class FailedTest(Test):
-    def __init__(self, filename:str, node, tested_line, expected_result, lineno, obtained_result):
-        super().__init__(filename, node, tested_line, expected_result, lineno)
-        self.obtained_result = obtained_result
-
-    def get_obtained_result(self):
-        return self.obtained_result
-    
-    def get_status(self):
-        return super()._FAILED_STATUS
-    
-    def get_tag(self):
+class FailedVerdict(ExampleVerdict):
+    def __init__(self, filename:str, lineno, tested_line, expected_result, real_result):
+        super().__init__(filename, lineno, tested_line, expected_result, real_result)
+ 
+    def get_color(self):
         return "red"
-    
-    def __str__(self):
-        report = "Test failed for: %s" % (self.tested_line)
-        return report
 
-    def get_detail_failure(self):
-        want, got = self.expected_result, self.obtained_result
+    def isSuccess(self):
+        return False
+    
+    def get_details(self):
+        want, got = self.expected_result, self.details
         
         if isinstance(got, str): # "''"
             got = "\'\'" if got == str() else "\'%s\'" % got
-        return 'Expected: %s, Got: %s' % (want, got)
+        return 'Expected: %s, Got: %s' % (want, got)
+    
+    def __str__(self):
+        return "Test failed for: %s" % (self.tested_line)
```

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/failed.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/outline-class.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/outline-method.gif` & `UpyTest-3.0.7/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/passed.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docs/res/warning.png` & `UpyTest-3.0.7/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.0.7/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             the raised exception. If `None`, so the error line mentioned in the error will 
             be kept. 
         
         Raises:
             DocGeneratorParserException: if the ast parser is failed.
         """
         try :
-            return self._ast_parser._get_supported_nodes()
+            return self._ast_parser.get_supported_nodes()
         except Exception as e: # if a compilation error occurs during the parsing
             error_info = sys.exc_info()
             last_exception = get_last_exception(error_info)
             if error_line:
                 last_exception = replace_error_line(last_exception, error_line)
             raise DocGeneratorParserException(last_exception)
```

### Comparing `UpyTest-3.0.6/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.0.7/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/environement_vars.py` & `UpyTest-3.0.7/thonnycontrib/environement_vars.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 
 # `IS_SELECTED_VAR` est une variable d'environnment qui stocke si oui(`True`) ou non(`False`)
 # on a ciblé un seul test
 IS_SELECTED_VAR = "is_selected"
 
 # `SELECTED_LINE_VAR` est une variable d'environnment qui stocke le numéro de ligne de 
 # la fonction séléctionnée si `IS_SELECTED_VAR` est à True, sinon elle stocke `None`.
-NODE_LINENO_VAR = "node_lineno"
+SELECTED_LINE_VAR = "selected_line"
 
 # `TEST_ONLY_VAR` est une variable d'environnment qui stocke si oui(`True`) ou non(`False`)
 # on a cliqué sur le button qui lancent les fonction qui possède le `@test_only`
 TEST_ONLY_VAR = "test_only"
 
-IS_FORCIBLY_INTERRUPTED = 'is_forcibly_interrupted'
+IS_FORCIBLY_INTERRUPTED = 'is_forcibly_interrupted'
```

### Comparing `UpyTest-3.0.6/thonnycontrib/exceptions.py` & `UpyTest-3.0.7/thonnycontrib/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,14 @@
     
 class NoFunctionSelectedToTestException(BackendException):
     """
     Exception raised when the selected line doesn't contain a function/class signature.
     """
     pass 
 
-class TestOnlyDecoratorException(BackendException):
-    """
-    Exception raised when no `@test_only` decorator is detected in the source code.
-    """
-    pass
-
 class CannotImportModuleException(BackendException):
     """
     Exception raised when a module cannot be imported by the importlib library.
     """
     pass
 
 class RuntimeException(BackendException):
@@ -120,8 +114,8 @@
 
 class CannotSelectSeveralLines(FrontendException):
     """
     Exception raised when several lines are selected. For example, This exception 
     is raised when the user tries to select several lines to run the tests of the selected
     lines. Or, when a user tries to select several lines to generate the docstring.
     """
-    pass
+    pass
```

### Comparing `UpyTest-3.0.6/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.0.7/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import List
 from .l1test_error_view import L1TestErrorView
 from .l1test_treeview import L1TestTreeView
 from ..properties import *
 from ..l1test_configuration.l1test_options import *
+from ..backend.ast_parser import L1DocTest
 from thonny.codeview import *
 from ..utils import format_filename_to_hyperlink, remove_url_part
 import thonny
 
 class L1TestReporter():    
     def __init__(self, main_view_class=L1TestTreeView, error_view_class=L1TestErrorView):
         self.__treeview_class = main_view_class
@@ -36,19 +38,19 @@
         if hyperlink_error: 
             self.__error_view.append_rst(hyperlink_error) # hyperlink doit être ajouté en mode RST
             error_msg = remove_url_part(error_msg) 
             self.__error_view.append_text(error_msg, tags=color) # le reste du message est ajouté en mode texte
         else:
             self.__error_view.append_text(error_msg, tags=color)
                        
-    def display_tests_results(self, verdicts):
+    def display_tests_results(self, verdicts: List[L1DocTest]):
         """Display the verdicts into the `L1TestTreeView`.
 
         Args:
-            verdicts (Dict[AST: list[Test]]): the dictionary of verdicts.
+            verdicts (List[L1DocTest]): the dictionary of verdicts.
         """
         self.__treeview.set_verdicts(verdicts)
         self.__treeview.update_tree_contents(verdicts)
     
     def set_treeview_class(self, treeview_class):
         self.__treeview_class = treeview_class
```

### Comparing `UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import namedtuple
+from typing import List
+from ..backend.ast_parser import L1DocTest
 from thonny.workbench import WorkbenchEvent
 from ..utils import send_to_backend
-from ..backend.verdicts.Test import Test
+from ..backend.verdicts.ExampleVerdict import ExampleVerdict
 from ..environement_vars import IS_SELECTED_VAR
 from ..exceptions import *
 from .l1test_reporter import *
 from ..properties import *
 from thonny.common import ToplevelResponse, InlineResponse
 from thonnycontrib import l1test_frontend 
 from ..ThonnyLogsGenerator import log_in_thonny
@@ -60,37 +62,31 @@
         received response and then it will show the state of the execution.
         """
         if msg.get("command_name") == BACKEND_COMMAND:
             self.clean_error_view()
 
             state:str = msg.get("state")
 
-            l1test_treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
-            l1test_treeview.disable_menu()
+            treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
+            treeview.disable_menu()
              
-            l1test_treeview.insert_in_header(L1TEST_IN_PROGRESS, clear=True, tags="blue", image=l1test_treeview.pending_img)
+            treeview.insert_in_header(L1TEST_IN_PROGRESS, clear=True, tags="blue", image="pending_icon.png")
             
             if state == PENDING_STATE:
                 self.set_pending(True)
                 self.clean_treeview(all=False)
                 source, invite, lineno = msg.get("source"), msg.get("invite"), msg.get("lineno") 
 
                 row_content = "%s for line %s, %s %s" % (state, lineno, invite, source)
-                self.row = l1test_treeview.insert_row(text=row_content, open=True, tags=("clickable",), values=lineno)
-                l1test_treeview.insert_row(parent=self.row, 
+                self.row = treeview.insert_row(text=row_content, open=True, tags=("clickable",), values=lineno)
+                treeview.insert_row(parent=self.row, 
                                            text="Interrompez avec 'ctrl+c', si ce test prend plus de temps.", 
                                            tags=("nonClickable", "orange"))
             elif state == EXECUTED_STATE: 
-                l1test_treeview.insert_row(parent=self.row, text=state, tags=("nonClickable", "green"))  
-            elif state == INTERRUPTED_STATE:
-                # print("here")
-                # breakpoint()
-                self.set_pending(True) 
-                # l1test_treeview.insert_row(parent=self.row, text=state, tags=("nonClickable", "red")) 
-                # l1test_treeview.get_treeview().item(self.row, open=True)
+                treeview.insert_row(parent=self.row, text=state, tags=("nonClickable", "green"))  
             else: # si le state == FINISHED_STATE
                 self.set_pending(False)     
     
     def report_verdicts(self, msg: ToplevelResponse):     
         """
             This method is binded to the `TopLevelResponse` event sent by the backend.
             
@@ -124,24 +120,24 @@
                 l1test_treeview.enable_menu()    
                 
                 if msg.get(VERDICTS): # We check if the response contains the "verdicts" attribute 
                     self.set_has_exception(False)
                     received_verdicts = msg.get(VERDICTS)
 
                     # deserialization of the data
-                    verdicts:dict[str, list[Test]] = pickle.loads(received_verdicts)                    
+                    verdicts: List[L1DocTest] = pickle.loads(received_verdicts)                    
                     log_in_thonny(verdicts, eval(os.environ.get(IS_SELECTED_VAR)))
             self.show_right_view(verdicts=verdicts, error_msg=error_msg.msg, error_title=error_msg.title)
         else:
             # Le TopLevelReponse reçu ne nous intéresse pas.
             return 
         # On indique l'état de l'execution du la commande comme terminée
         self.terminate_running()
     
-    def show_verdicts(self, test_results:dict[ast.AST, list[Test]]):
+    def show_verdicts(self, test_results:List[L1DocTest]):
         """
         Report the verdicts on the view.
 
         Args:
             test_results (dict): The recieved verdicts from the backend.
         """
         self._reporter.display_tests_results(test_results) 
@@ -158,33 +154,36 @@
         the proxy to be initialized.
 
         Args:
             is_selected (bool): Set as True if only one method is selected to run
                             it's tests.
             selected_line (int): The number of the selected line.
         """
-        if not self.is_running(): # si le plugin n'est pas en execution 
-            self.__send_to_backend(is_selected, selected_line)
-        else: # si le plugin est en cours d'execution et pas encore terminé
+        treeview = self._reporter.get_l1test_treeview()
+        if self.is_running(): # si le plugin est en cours d'execution et pas encore terminé
             thonny.get_runner().cmd_stop_restart() # invoke le restart backend
             
             # on affiche sur la treeview comme quoi un restart backend forcé est en cours
-            self.get_reporter() \
-                .get_l1test_treeview() \
-                .insert_in_header("/!\ Force to restart backand ...", clear=True, tags=("red"))
+            treeview.insert_in_header("Force to restart backend ...", 
+                                      clear=True, tags=("red"), image="restart_icon.png")
             
             # on indique que l'état du plugin n'est plus en execution
             self.set_is_running(False)
             
             # On donne un peu du temps au proxy pour se réinitialiser.
             # La valeur choisit n'affecte pas le temps d'execution du plugin.
             time.sleep(1) 
             
-            # On invoque la commande magique L1test
+        # On invoque la commande magique L1test
+        try:
             self.__send_to_backend(is_selected, selected_line)
+        except:
+            self.set_is_running(False)
+            treeview.insert_in_header("Coudn't restart the backend.\nPlease restart with the 'Stop' button !", 
+                                      clear=True, tags=("red"), image="error_icon.png")
     
     def __send_to_backend(self, is_selected, selected_line):
         self.set_is_running()
         send_to_backend(is_selected=is_selected, selected_line=selected_line)
         
     def __handle_raised_exception(self, exception: dict) -> ErrorMsg:
         """
@@ -281,16 +280,17 @@
             if event.get("full"):
                 self.terminate_running()
                 self.clean_treeview()          
             else:       
                 # on vérifie si le l1test a été invoqué
                 if self.is_running(): 
                     self.clean_treeview()
-                    l1test_treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
-                    l1test_treeview.insert_in_header("Starting executing tests ...", clear=True, tags="blue", image=l1test_treeview.pending_img)
+                    treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
+                    treeview.insert_in_header("Starting executing tests ...", clear=True, tags="blue", 
+                                              image="pending_icon.png")
                 else: # probablement une autre commande a déclenché le Restart du backend -> on fait rien
                     pass
         self.show_right_view()
      
     def show_right_view(self, event:WorkbenchEvent=None, verdicts=None, error_msg:str=None, error_title:str=None, both=False):
         """
             Displays either the L1TestTreeView or the L1TestErrorView.
```

### Comparing `UpyTest-3.0.6/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.0.7/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from thonny import  tktextext, ui_utils
 from thonny.ui_utils import scrollbar_style
 from thonnycontrib.utils import get_font_size_option, get_font_family_option
 from .l1test_error_view import L1TestErrorView
 from ..properties import *
-from ..backend.verdicts.EmptyTest import EmptyTest
-from ..backend.verdicts.ExceptionTest import ExceptionTest
-from ..backend.verdicts.FailedTest import FailedTest
-from ..backend.verdicts.Test import Test
-from ..backend.verdicts.FailedWhenExceptionExpectedTest import *
-from ..backend.verdicts.PassedTest import PassedTest
+from ..backend.doctest_parser import Example
+from ..backend.ast_parser import L1DocTest, L1DocTestFlag
+from ..backend.verdicts.ExceptionVerdict import ExceptionVerdict
+from ..backend.verdicts.FailedVerdict import FailedVerdict
+from ..backend.verdicts.FailedWhenExceptionExpectedVerdict import FailedWhenExceptionExpectedVerdict
 from ..utils import *
 from functools import partial
 from ..l1test_configuration.l1test_options import *
-import os, tkinter as tk, tkinter.font as tk_font, thonny
+import tkinter as tk, tkinter.font as tk_font, thonny
 from collections import namedtuple
 from thonny.codeview import *
-from collections import defaultdict
 from typing import Dict, List
+from copy import deepcopy
 
 # La hauteur, par défault, d'une ligne dans une Treeview
 ROW_HEIGHT  = 40
 
 clickable_tag = "clickable"
 
 # L'objet qui représente un summarize
@@ -39,16 +38,16 @@
 class L1TestTreeView(ttk.Frame):    
     def __init__(self, master=None):
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
         
         self._init_treeview()
         
-        self._origin_verdicts: Dict[ast.AST, List[Test]] = dict()
-        self._copy_verdicts = self._origin_verdicts.copy()
+        self._origin_l1doctests: List[L1DocTest] = dict()
+        self._copy_l1doctests = self._origin_l1doctests.copy()
         
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.__observe_font_changing, True)
         self.workbench.bind("<Control-minus>", self.__observe_font_changing, True)
             
     def _init_treeview(self):
         """
@@ -85,23 +84,24 @@
         self.treeview.tag_bind("clickable", "<<TreeviewSelect>>", self._on_select)
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
         
         self.style = ttk.Style()
         self.style_mapping = self.style.map('Treeview')
 
         self.__update_tree_font(get_font_family_option(), get_font_size_option())
-       
-        # le chemin c'est par rapport au dossier /l1test 
-        # donc il faut remonter vers /thonnycontrib/ pour rentrer dans docs/res
-        parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-        
-        self.passed_icon = tk.PhotoImage(file=os.path.join(parent_dir, "docs/res", "passed.png"))
-        self.failed_icon = tk.PhotoImage(file=os.path.join(parent_dir, "docs/res", "failed.png"))
-        self.warning_icon = tk.PhotoImage(file=os.path.join(parent_dir, "docs/res", "warning.png"))
-        self.pending_img = tk.PhotoImage(file=os.path.join(parent_dir, "docs/res", "pending_icon.png"))
+
+        # All the icons used in the treeview should be loaded here to keep thier references.
+        # Otherwise, they will be garbage collected and the treeview will not show them.
+        self.image_references = {}
+        for flag in L1DocTestFlag:
+            self.image_references[flag.name] = get_photoImage(flag.get_image())
+
+        self.image_references["pending_icon.png"] = get_photoImage("pending_icon.png")
+        self.image_references["error_icon.png"] = get_photoImage("error_icon.png")
+        self.image_references["restart_icon.png"] = get_photoImage("restart_icon.png")
         
         # add a menu to the treeview
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)
 
         # Here we handle the motion event of the treeview
         self.treeview.bind("<Configure>", partial(self.__wrap_tree_content, self.treeview))
         self.selected_item = None
@@ -167,24 +167,24 @@
         )
     
     def add_menu_options(self):
         """
             Adds the options inside the menu button.
         """
         self.menu.delete(0, "end") 
-        
+         
         self.menu.add_command(label=PLACE_RED_TEST_ON_TOP_LABEL, command=self.sort_by_red_tests)
         self.menu.add_command(label=RESUME_ORIGINAL_ORDER, command=self.remove_sort_filter)
         self.menu.add_separator() 
         self.menu.add_command(label=SHOW_ONLY_RED_TESTS, command=self.show_only_red_tests)
         self.menu.add_command(label=SHOW_ALL_TESTS, command=self.show_all_tests)
         self.menu.add_separator()
         self.menu.add_command(label=GROUP_BY_VERDICTS, command=self.group_by_verdicts)
         self.menu.add_separator()    
-        self.menu.add_command(label=EXPAND_TEST_RESULTS, command=self.expand_rows)
+        self.menu.add_command(label=EXPAND_TEST_RESULTS, command=self.expand_rows) 
         self.menu.add_command(label=FOLD_TEST_RESULTS, command=self.fold_rows)
         self.menu.add_separator()
         self.menu.add_command(label=UPDATE_FONT_LABEL, command=self.update_font)
         self.menu.add_command(label=REDUCE_SPACE_BETWEEN_ROWS, command=self.reduce_space_between_rows)
         self.menu.add_command(label=REMOVE_ERROR_DETAILS if not get_option(EXCEPTION_DETAIL) else INCLUDE_ERROR_DETAILS, 
                               command=self.remove_error_details)
         self.menu.add_separator()
@@ -217,157 +217,150 @@
             rowheight = self.get_optimal_row_height(self.treeview, all_childs)
                      
         self.resize_header_bar()
         # on applique la nouvelle police pour la treeview
         self.__observe_font_changing(rowheight=rowheight)
     
     def sort_by_red_tests(self):
-        priority = Test._FAILED_STATUS
-        # On filtre que les noeuds qui ont au moins un test rouge.
-        sorted_failed_nodes = {node: results for node, results in self._copy_verdicts.items() \
-                                    if priority in self.__deduce_global_node_verdict(node, results).keys()
-                            } 
-        
-        # On met les tests rouges en haut et cela pour tous les noeuds AST qui ont au moins un test rouge.
-        sorted_failed_tests = {node: sorted(results, key=lambda x: isinstance(x, (FailedTest, ExceptionTest)), reverse=True) \
-                                    for node, results in sorted_failed_nodes.items() \
-                                        if priority in self.__deduce_global_node_verdict(node, results).keys() 
-                            }
         
+        # On filtre que les l1doctest qui ont un flag rouge.
+        sorted_failed_nodes = [l1doctest for l1doctest in self._copy_l1doctests if l1doctest.get_flag() == L1DocTestFlag.FAILED_FLAG ]
+        
+        # On met les tests rouges en haut et cela pour tous les l1doctest qui ont au moins un test rouge.
+        sorted_failed_tests = []
+        for l1doctest in sorted_failed_nodes:
+            new_l1doctest = deepcopy(l1doctest)
+            new_l1doctest.sort_examples_by_verdicts((FailedVerdict, ExceptionVerdict))
+            sorted_failed_tests.append(new_l1doctest)
+           
         # On récupère les autres neouds AST 
-        others = {node: results for node, results in self._copy_verdicts.items() \
-                                    if priority not in self.__deduce_global_node_verdict(node, results).keys()
-                } 
+        others = [l1doctest for l1doctest in self._copy_l1doctests if l1doctest.get_flag() != L1DocTestFlag.FAILED_FLAG]
          # l'addition de tous les noeuds
-        sorted_failed_tests.update(others)
+        sorted_failed_tests.extend(others)
 
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
-            self._copy_verdicts = sorted_failed_tests
+            self._copy_l1doctests = sorted_failed_tests
             self.update_tree_contents(sorted_failed_tests)
     
     def remove_sort_filter(self):
         """
         When invoking this method the treeview will restore 
         the original order of its rows.
         """
         def __is_verdicts_copy_equals_to_original():
-            if len(self._copy_verdicts) != len(self._origin_verdicts):
+            if len(self._copy_l1doctests) != len(self._origin_l1doctests):
                 return False
-            for o_node, o_tests in self._origin_verdicts.items():
-                c_tests = self._copy_verdicts[o_node]
-                if len(o_tests) != len(c_tests): 
+            c_names = [c_l1doctest.get_name() for c_l1doctest in self._copy_l1doctests]
+            for o_l1doctest in self._origin_l1doctests:
+                c_index = c_names.index(o_l1doctest.get_name())
+                c_l1doctest = self._copy_l1doctests[c_index]
+                if len(c_l1doctest.get_examples()) != len(o_l1doctest.get_examples()): 
                     return False 
             return True
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
             if __is_verdicts_copy_equals_to_original():
-                self._copy_verdicts = self._origin_verdicts
-            self.update_tree_contents(self._copy_verdicts)
+                self._copy_l1doctests = self._origin_l1doctests
+            self.update_tree_contents(self._copy_l1doctests)
     
     def show_only_red_tests(self):
-        red_verdicts = (Test._FAILED_STATUS, Test._EXCEPTION_STATUS)
+        from copy import deepcopy
+        red_verdicts = (FailedVerdict, FailedWhenExceptionExpectedVerdict, ExceptionVerdict)
         
-        only_reds = {}
-        for node, tests in self._copy_verdicts.items():
-            red_tests = []
-            for test in tests:
-                if test.get_status() in red_verdicts:
-                    red_tests += [test]
-            if red_tests:
-                only_reds[node] = red_tests
+        only_reds = []
+        for l1doctest in self._copy_l1doctests:
+            if l1doctest.get_flag() == L1DocTestFlag.FAILED_FLAG:
+                red_examples = l1doctest.filter_examples_by_verdicts(red_verdicts)
+                new_l1doctest = deepcopy(l1doctest)
+                new_l1doctest.set_examples(red_examples)
+                only_reds.append(new_l1doctest)
                             
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
-            self._copy_verdicts = only_reds
-            self.update_tree_contents(only_reds)
+            self._copy_l1doctests = only_reds
+            self.update_tree_contents(self._copy_l1doctests)
      
     def show_all_tests(self):
-        self._copy_verdicts = self._origin_verdicts
-        self.update_tree_contents(self._copy_verdicts)
+        self._copy_l1doctests = self._origin_l1doctests
+        self.update_tree_contents(self._copy_l1doctests)
     
-    def __group_by_verdicts(self, verdicts: dict[ast.AST, List[Test]], status_order: List[str]=None) :
+    def __group_by_verdicts(self, l1doctests: List[L1DocTest], status_order: List[L1DocTestFlag]=None) -> Dict[L1DocTestFlag, List[L1DocTest]]: 
         """
-        Group verdicts by status and order the statuses according to the provided 
+        Group l1doctests by status and order the statuses according to the provided 
         status order.
         
-        :param status_order: A list of strings that specifies the order 
-        in which to group the verdicts by status.
+        :param status_order: A list of L1DocTestFlag that specifies the order in which 
+        to group the verdicts by flag.
         :return: A dictionary of verdicts grouped by status.
         """
-        status_groups = {}
-        for ast_node, verdict_list in verdicts.items():
-            for verdict in verdict_list:
-                status = verdict.get_status()
-                if status not in status_groups:
-                    status_groups[status] = {}
-                if ast_node not in status_groups[status]:
-                    status_groups[status][ast_node] = []
-                status_groups[status][ast_node].append(verdict)
+        status_groups:Dict[L1DocTestFlag, List[L1DocTest]] = {}
+        for l1doctest in l1doctests:
+            status = l1doctest.get_flag()
+            if status not in status_groups:
+                status_groups[status] = []
+            status_groups[status].append(l1doctest)
 
         if status_order is None:
-            status_order = Test.get_statutes_by_priority()
+            status_order = L1DocTestFlag.get_priorities()
         
         # mettre en ordre les catégories selon l'ordre défini par le paramètre `status_order`
         ordered_groups = {}
         for status in status_order:
             if status in status_groups:
                 ordered_groups[status] = status_groups[status]
         status_groups = ordered_groups
         
         return status_groups
     
-    def group_by_verdicts(self): 
-        grouped = self.__group_by_verdicts(self._origin_verdicts)
+    def group_by_verdicts(self):  
+        grouped = self.__group_by_verdicts(self._origin_l1doctests)
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
             self.clear_tree(clear_all=False) 
-            for status, verdicts in grouped.items():
-                open = False
-                if status in (Test._EXCEPTION_STATUS, Test._FAILED_STATUS) and verdicts:
-                    open = True
-                row_id = self.insert_row(text=status, open=open, tags=())
-                self.__add_verdicts_to_treeview(verdicts, row_id)
-    
+            for status, l1doctests in grouped.items():
+                row_id = self.insert_row(text=status.short_name(), open=status.should_expand(), 
+                                         tags=(status.get_color()))
+                self.__add_verdicts_to_treeview(l1doctests, row_id)
+     
     def expand_rows(self): 
         """Spreads only the node rows"""
-        self.__apply_row_change(False)
+        self.__apply_row_change(True)
     
     def fold_rows(self):
         """Folds only the node rows"""
-        self.__apply_row_change(True)
+        self.__apply_row_change(False)
     
-    def __apply_row_change(self, to_fold:bool):
+    def __apply_row_change(self, to_expand:bool):
         """Depending on the `to_fold` it folds or spreads the rows that
         correspond to the ast nodes.
          
-        - If `to_fold` is True, the ast nodes are folded.
-        - If `to_fold` is False, the ast nodes are expanded.
+        - If `to_expand` is True, the ast nodes are expanded.
+        - If `to_expand` is False, the ast nodes are folded.
 
         Args:
-            to_fold (bool): set to True to fold the rows that correspond
-            to the ast nodes. Set to False to expand the rows that correspond
-            to the ast nodes.
+            to_expand (bool): set to True to expand the rows that correspond
+            to the ast nodes. Set to False to fold them.
         """
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
             from copy import copy
             # on sauvegarde la valeur initiale de l'option GLOBAL_VIEW
             initial_val = copy(get_option(GLOBAL_VIEW))
             # on applique la nouvelle valeur de l'option `GLOBAL_VIEW`
-            set_option(GLOBAL_VIEW, to_fold)
+            set_option(GLOBAL_VIEW, to_expand)
             # update_tree invoque dynamiquement la valeur de l'option(`GLOBAL_VIEW`) courante
-            self.update_tree_contents(self._copy_verdicts)
+            self.update_tree_contents(self._copy_l1doctests)
             # on restaure la valeur initiale de l'option ??!
             # set_option(GLOBAL_VIEW, initial_val)
     
     def remove_error_details(self):
         if self.treeview.get_children():
             should_report = get_option(EXCEPTION_DETAIL)
             set_option(EXCEPTION_DETAIL, not should_report)
             if not should_report:
                 error_view:L1TestErrorView = self.workbench.get_view(L1TestErrorView.__name__)
                 error_view.clear()
                 error_view.hide_view()
-            self.update_tree_contents(self._copy_verdicts)
+            self.update_tree_contents(self._copy_l1doctests)
             
     def reduce_space_between_rows(self):
         all_childrens = get_all_tree_childrens(self.treeview)
         all_texts = self.__extract_wrapped_texts(self.treeview, all_childrens)
         max_lines = self.__get_longest_wrapped_line(all_texts)
         current_height = self.__compute_optimal_height(max_lines, margin=0.66, padding=1.5)
         self.style.configure("Treeview", rowheight=current_height)
@@ -405,15 +398,15 @@
         
         if (isinstance(widget, ttk.Treeview)): 
             if (self.workbench.get_view(self.__class__.__name__).winfo_ismapped()):  
                 if not self.is_treeview_cleared():
                     width = widget.winfo_width()
                     
                     # Une heuristique a été fait pour décider du nombre de caractères par 100 pixels.
-                    chars_per_100_pixels = width // (get_font_size_option()-2)
+                    chars_per_100_pixels = width // (get_font_size_option())
                     
                     all_childrens = get_all_tree_childrens(self.treeview)
                     for iid in all_childrens:
                         text = widget.item(iid)["text"]
                         wrapped = wrap(text, chars_per_100_pixels)   
                         tree.item(iid, text=wrapped)
                     # il faut changer la hauteur des rows pour afficher tout le texte
@@ -458,54 +451,60 @@
                 (int): The new height.
         """
         default_font = tk_font.nametofont("TkDefaultFont")
         font_size = round(default_font.metrics("linespace") * padding) * margin 
         lines_per_row = max_lines * font_size if max_lines else font_size
         return round(lines_per_row)
     
-    def update_tree_contents(self, results:dict, parent="", full_clear=True):
+    def update_tree_contents(self, l1doctests:List[L1DocTest], parent="", full_clear=True):
         """
             This function contructs and inserts the rows into the treeview.
         """
         def __update_tree_header__():            
             # We build the summarize object 
-            summarize: Summarize = self.build_summarize_object(self._origin_verdicts)
+            summarize: Summarize = self.build_summarize_object(self._origin_l1doctests)
             # We insert the summarize infos into the header bar of the treeview
             self.insert_summarize_in_header_bar(summarize, self.header_bar)
             self.resize_header_bar()
         
         self._show_highlight_selection_effect()   
         self.clear_tree(clear_all=full_clear)
    
         if not self.__check_if_editor_is_open():
             return
 
-        self.__add_verdicts_to_treeview(results, parent)
+        self.__add_verdicts_to_treeview(l1doctests, parent)
         
         if self.treeview.get_children():
             __update_tree_header__()
     
-    def __add_verdicts_to_treeview(self, results:dict, parent=""):
-        for node, verdicts in results.items():
-            _tests = self._origin_verdicts[node]
-            current_node = self._add_node_to_tree(node, _tests, parent)
-            self._add_verdicts_to_node(current_node, verdicts)
-        
+    def __add_verdicts_to_treeview(self, l1doctests:List[L1DocTest], parent=""):
+        o_names = [c_l1doctest.get_name() for c_l1doctest in self._origin_l1doctests]
+        for l1doctest in l1doctests:
+            o_index = o_names.index(l1doctest.get_name())
+            current_node = self._add_node_to_tree(self._origin_l1doctests[o_index], parent)
+            if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
+                self.treeview.insert(current_node, "end", values=l1doctest.get_node_lineno(), 
+                                     text="No tests found", tags=("nonClickable", l1doctest.get_flag().get_color()))
+            else:    
+                self._add_verdicts_to_node(current_node, l1doctest.get_examples())
+         
         self.__wrap_tree_content(self.treeview, None)
         self.enable_menu()
     
-    def _add_node_to_tree(self, node:ast.AST, tests:list[Test], parent=""):      
+    def _add_node_to_tree(self, l1doctest: L1DocTest, parent=""):      
         self.__update_tree_font(get_font_family_option(), get_font_size_option())
                 
-        global_verdict = self.__deduce_global_node_verdict(node, tests)
-        for _, verdict_config in global_verdict.items():
-            return self.treeview.insert(parent, "end", values=node.lineno, 
-                                        tags=(clickable_tag, ), **verdict_config)
+        flag: L1DocTestFlag = l1doctest.get_flag()
+        verdict_config = dict(text=self._get_l1doctest_stats(l1doctest), 
+                              image=self.get_icon(flag.name), 
+                              open=get_option(GLOBAL_VIEW) if flag == L1DocTestFlag.FAILED_FLAG else False)
+        return self.treeview.insert(parent, "end", values=l1doctest.get_node_lineno(), tags=(clickable_tag, ), **verdict_config)
     
-    def _add_verdicts_to_node(self, current_node:str, tests:list[Test]):
+    def _add_verdicts_to_node(self, current_node:str, examples:list[Example]):
         """ 
         This function adds to the treeview all the rows that correspond 
         to the given ast node.
         """
         def __add_as_many_rows_as_text_lines(parent, text:str, lineno:int, tags:str):
             """
             Adds the necessary rows of each text to be inserted in the treeview.
@@ -514,39 +513,40 @@
             """
             splitted = text.split("\n")
             for line in splitted:
                 self.treeview.insert(parent, "end", text=line, values=lineno, tags=tags) 
                 
         # insert the sub-rows that represents the verdicts of the executed tests 
         # of the current AST node.
-        for test in tests:
-            item_text = " " + str(test)
-            verdict_tags = (test.get_tag(), clickable_tag)
-            if isinstance(test, FailedTest):
+        for example in examples:
+            verdict = example.get_verdict()
+            item_text = " " + str(verdict)
+            verdict_tags = (verdict.get_color(), clickable_tag)
+            if isinstance(verdict, FailedVerdict):
                 current_test = self.treeview.insert(current_node, "end",  text=item_text, 
                                                     open=get_option(OPEN_RED_ROWS), 
-                                                  values=test.get_lineno(), tags=verdict_tags)   
-                if (isinstance(test, FailedWhenExceptionExpectedTest)):
+                                                    values=verdict.get_lineno(), tags=verdict_tags)   
+                if (isinstance(verdict, FailedWhenExceptionExpectedVerdict)):
                     # le detail d'une `failure` ne doit pas être cliquable
                     verdict_tags = (verdict_tags[0], "nonClickable")
                 # a failure message can be reported on several line, so we should add as many rows as text lines. 
-                __add_as_many_rows_as_text_lines(current_test, test.get_detail_failure(), test.get_lineno(), tags=verdict_tags)
-            elif isinstance(test, ExceptionTest):
+                __add_as_many_rows_as_text_lines(current_test, verdict.get_details(), verdict.get_lineno(), tags=verdict_tags)
+            elif isinstance(verdict, ExceptionVerdict):
                 extra_tags = ("lightred", ) if get_option(HIGHLIGHT_EXCEPTIONS) else ()
                 current_test = self.treeview.insert(current_node, "end",  text=item_text, 
-                                                    values=[test.get_lineno(), test.__class__.__name__, test.get_detail_failure()], 
+                                                    values=[verdict.get_lineno(), verdict.__class__.__name__, verdict.get_details()], 
                                                     tags=verdict_tags+extra_tags,
                                                     open=get_option(OPEN_RED_ROWS))
                 # le detail d'une `exception` ne doit pas être cliquable
                 error_detail_tags = (verdict_tags[0], "nonClickable")
                 
                 if not get_option(EXCEPTION_DETAIL):
-                    __add_as_many_rows_as_text_lines(current_test, test.get_detail_failure(), test.get_lineno(), tags=error_detail_tags)               
+                    __add_as_many_rows_as_text_lines(current_test, verdict.get_details(), verdict.get_lineno(), tags=error_detail_tags)               
             else :
-                current_test = self.treeview.insert(current_node, "end", text=item_text, values=test.get_lineno(), tags=verdict_tags)
+                current_test = self.treeview.insert(current_node, "end", text=item_text, values=verdict.get_lineno(), tags=verdict_tags)
              
     def insert_row(self, parent="", text="", clear:bool=False, values=(), 
                    open=False, tags:str="", add_empty_line:bool=False):
         """
         Insert a simple row into the treeview. 
 
         Args:
@@ -569,46 +569,24 @@
     def __check_if_editor_is_open(self) -> bool:
         """
             Returns True if an editor is already opened in thonny. 
             Otherwise, returns False 
         """
         return False if not self.workbench.get_editor_notebook().get_current_editor() else True
     
-    def __deduce_global_node_verdict(self, node:ast.AST, tests: list[Test]):
+    def _get_l1doctest_stats(self, l1doctest: L1DocTest):
         """
-        Returns the status of a treeview node(ie. the row that represents the AST node).
-        
-        - If a node contains at least one Failure or one Exception verdict so `FAILED_STATUS`
-        will be returned.
-        
-        - If a node contains only passed verdicts so a `PASSED_STATUS` for the current AST node 
-        will be returned.
-        
-        - If none of the previous conditions is respected so a `WARNING_STATUS` wil be returned.
-
-        Args:
-            tests (list[Test]): The verdicts of an AST node.
-
-        Returns:
-            dict: a status of the ast node associated with some configs.
+        Get a string that represents how many tests are passed of the given l1doctest. 
+        If the l1docstest is empty, returns only the name of the l1doctest.
         """
-        node_repr = " %s" % create_node_representation(node)   
-        def _add_number_passed_tests():
-            """
-                Adds how many tests are executed of the current AST node
-            """
-            # The first space is necessary so that all text will be aligned
-            return "%s ~%s passed~" %(node_repr, len([test for test in tests if test.get_status() == Test._PASSED_STATUS]))
+        # The first space is necessary so that all text will be aligned
+        if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
+            return " %s" % l1doctest.get_name()
+        return " %s ~ %s/%s passed" %(l1doctest.get_name(), l1doctest.count_passed_tests(), l1doctest.count_tests())
         
-        if any([test.get_status() in (Test._FAILED_STATUS, Test._EXCEPTION_STATUS) for test in tests]):
-            return {Test._FAILED_STATUS: dict(text=_add_number_passed_tests(), image=self.failed_icon, open=not get_option(GLOBAL_VIEW))}
-        elif all([test.get_status() == Test._PASSED_STATUS for test in tests]):
-            return {Test._PASSED_STATUS: dict(text=_add_number_passed_tests(), image=self.passed_icon, open=False)}
-        return {Test._EMPTY_STATUS: dict(text=node_repr, image=self.warning_icon, open=False)}
-
     def insert_summarize_in_header_bar(self, summarize:Summarize, view: tktextext.TweakableText):
         """
         Builds the summarize test to be inserted in the header of the treeview.
         
         Args:
             summarize (Summarize): a named tuple that contains the summarize infos.
         """
@@ -626,36 +604,31 @@
         
         insert_label("Errors: ", "darkred")
         insert_how_many(summarize.errors)
         
         insert_label("Empty: ", "orange")
         insert_how_many(summarize.empty, is_last=True)
             
-    def build_summarize_object(self, results:dict[ast.AST: List[Test]]) -> Summarize:
+    def build_summarize_object(self, l1doctests:List[L1DocTest]) -> Summarize:
         """
         Builds the summarize informations. 
         The summarize contains :
             - Total number of executed tests.
-            - How many succesed tests, failed tests, error tests, and empty tests.
+            - How many succeed tests, failed tests, error tests and empty tests.
         
         Args:
-            results (dict): all the verdicts of all the AST nodes.
+            results (List[L1DocTest]): all the l1doctests that have been evaluated.
 
         Returns:
             Summarize: a namedtuple that represents the summarize object.
-        """
-        from collections import Counter
-        # Count the number of tests of each type
-        counts = Counter([t.get_status() for tests in results.values() for t in tests])
-       
-        # Get the counts for each type of test
-        success = counts[Test._PASSED_STATUS]
-        failures = counts[Test._FAILED_STATUS] 
-        errors = counts[Test._EXCEPTION_STATUS]
-        empty = counts[Test._EMPTY_STATUS]
+        """       
+        success = sum([l1doctest.count_passed_tests() for l1doctest in l1doctests])
+        failures = sum([l1doctest.count_failed_tests() for l1doctest in l1doctests])
+        errors = sum([l1doctest.count_error_tests() for l1doctest in l1doctests])
+        empty = sum([1 for l1doctest in l1doctests if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG])
         total = success + failures + errors
         return Summarize(total, success, failures, errors, empty)
                    
     def clear_tree(self, event=None, clear_all=True):
         """Clears the treeview by deleting all items. 
         
         Note: this method is also called when the button `clear` is clicked.
@@ -739,15 +712,15 @@
                     if get_option(EXCEPTION_DETAIL):
                         self.workbench.event_generate(L1TREE_VIEW_EVENT, has_exception=False)
                 
                 self._show_highlight_selection_effect()
                 self.selected_item = focus 
                 
                 if get_option(EXCEPTION_DETAIL): 
-                    if ExceptionTest.__name__ in values:
+                    if ExceptionVerdict.__name__ in values:
                         self.workbench.event_generate(L1TREE_VIEW_EVENT, has_exception=True, both=True,
                                                     error_msg=values[-1], error_title=item["text"])
                            
                 lineno = values[0]
                 self._highlight_line_on_editor(lineno, code_view)
                 self.workbench.event_generate(
                     "OutlineDoubleClick", item_text=self.treeview.item(self.treeview.focus(), option="text")
@@ -757,23 +730,31 @@
         """disable the menu button of the treeview"""
         self.menu_button.state([tk.DISABLED])
         
     def enable_menu(self):
         """enable the menu button of the treeview"""
         self.menu_button.state(["!disabled"])
      
-    def insert_in_header(self, text, image=None, clear=False, tags=tuple()):
-        """
-        Insert in the header of the treeview a text. 
-        If image is not None so the image will be added before the texte.
+    def insert_in_header(self, text, image:str|tk.PhotoImage=None, clear=False, tags=tuple()):
+        """ 
+            Inserts text in the header of the treeview. 
+            Args:
+                text: the text to insert
+                image: the basename with it's extension of an image to insert. 
+                For example: "info.png". The image must be in the folder `docs/res`.
+                clear: if True, the header will be cleared before inserting the text
+                tags: the tags to apply to the text. For example: ("red",)
         """
         if clear:
             self.header_bar.direct_delete("1.0", tk.END)
         if image:
+            if isinstance(image, str):
+                image = self.get_icon(image)
             self.header_bar.image_create(tk.END, image=image)
+            #setattr(self, get_basename(image), photo_image)  # save the image in the treeview
             text = " " + text
         self.header_bar.direct_insert(tk.END, text, tags=tags)
         self.resize_header_bar()
            
     def is_treeview_cleared(self):
         return len(self.treeview.get_children()) == 0
     
@@ -782,13 +763,19 @@
     
     def hide_view(self):
         self.workbench.hide_view(self.__class__.__name__)
     
     def show_view(self):
         self.workbench.show_view(self.__class__.__name__)
         
-    def set_verdicts(self, verdicts: dict):
-        self._origin_verdicts = verdicts
-        self._copy_verdicts = self._origin_verdicts.copy()
+    def set_verdicts(self, verdicts: List[L1DocTest]):
+        self._origin_l1doctests = verdicts
+        self._copy_l1doctests = self._origin_l1doctests.copy()
     
     def get_treeview(self):
-        return self.treeview
+        return self.treeview
+    
+    def get_icon(self, ref_name:str):
+        """
+            Returns the image reference saved in the treeview.
+        """
+        return self.image_references[ref_name]
```

### Comparing `UpyTest-3.0.6/thonnycontrib/outlines.py` & `UpyTest-3.0.7/thonnycontrib/outlines.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from typing import List
 import re
 from thonny import get_workbench
 from functools import partial
 from .properties import PLUGIN_NAME
-import tkinter as tk, os
+import tkinter as tk
+from .utils import get_basename, get_photoImage 
+import thonnycontrib
 
 _OUTLINE_REGEX = r"\s*(?P<type>def|class)[ ]+(?P<name>[\w]+)"
 
-# Ceci est une implémentation de création d'un singleton pour OutlineParser
-_outliner = None
-
 class OutlinedNode():
     def __init__(self, type:str, name:str, lineno:int) -> None:
         self.__type = type
         self.__name = name
         self.__lineno = lineno
+        self.icon = "outline_class.png" if self.__type == "class" else "outline_method.gif"
         
-        icon_filename = "outline-class.png" if self.__type == "class" else "outline-method.gif"
-        icon_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "docs/res", icon_filename)
-        self.__image = tk.PhotoImage(name=icon_path, file=icon_path)
+        self.__image = get_photoImage(self.icon)
     
     def get_type(self):
         return self.__type  
     
     def get_name(self):
         return self.__name  
     
@@ -31,65 +29,69 @@
     
     def get_image(self):
         return self.__image    
 
 class Outliner():   
     def __init__(self, workbench=get_workbench()) -> None:
         super().__init__()
-        global _outliner
-        _outliner = self
+        thonnycontrib._outliner = self
         
         workbench._init_menu()
-        self.menu = tk.Menu(workbench.get_menu(PLUGIN_NAME)) 
-        self.menu.event_add("<<RunOneTest>>", "<Button-1>")
+        self.menu = tk.Menu(workbench.get_menu(PLUGIN_NAME), name="outliner_menu") 
+        get_workbench().bind("<Button-1>", self.update_menu, True)
      
     def __parse(self, source:str) -> List[OutlinedNode]:
         """
         Parses a source and returns a list of the outlined nodes. 
         The outlined nodes are either a class or a function. For 
         each outlined node an object of type `OutlinedNode` is built 
         in which we store the type (class/function), the name and the lineno
         of the outlined node.
         """
         outlines = []
         lineno = 0
         for line in source.split("\n"):
             lineno += 1
-            match = re.match(_OUTLINE_REGEX,line) 
+            match = re.match(_OUTLINE_REGEX, line) 
             if match:
                 outlined = OutlinedNode(match.group("type"), match.group("name"), lineno)
                 outlines.append(outlined)
         return outlines
     
     def from_source_post_menu(self, source):
         self.menu.delete(0, tk.END)
         outlines = self.__parse(source)
         for outline in outlines: 
             label = "%s %s" % (outline.get_type(), outline.get_name())
+            image = outline.get_image()
             self.menu.add_command(label=label, 
-                                  image=outline.get_image(),
+                                  image=image,
                                   command=partial(run_outlined_test, outline.get_lineno()),
                                   activebackground="white",
                                   activeforeground="darkblue",
                                   compound=tk.LEFT)
+            # should save a reference to the image otherwise it will be garbage collected
+            setattr(self, image.name, image)  
+
+    def update_menu(self, event):
+        if isinstance(event.widget, str) and "menu" in event.widget:
+            editor = get_workbench().get_editor_notebook().get_current_editor()
+            if editor is None:
+                return
+            source = editor.get_code_view().get_content()
+            self.from_source_post_menu(source)
     
     def get_menu(self):
         return self.menu
-    
-    
+
 def run_outlined_test(lineno:int):
     """
     Cette fonction est invoquée quand le button `Run test for selected function`
     suite à un clique droit sur une ligne du fichier.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test avec en argument
     is_selected=True.
     
     """
     from .plugin_loader import _send_to_l1test_backend
     _send_to_l1test_backend(is_selected=True, selected_line=lineno)
 
 
-def get_outliner() -> Outliner:
-    """
-    Retourne une instance de `OutlineParser` en tant que singleton.
-    """
-    return Outliner() if not _outliner else _outliner
```

### Comparing `UpyTest-3.0.6/thonnycontrib/plugin_loader.py` & `UpyTest-3.0.7/thonnycontrib/plugin_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 import os, os.path
-from thonny import get_workbench, get_runner
+from thonny import get_workbench
 from thonny.editors import  EditorNotebook
 from thonny import editors
 from thonny.ui_utils import select_sequence
-from thonnycontrib.outlines import get_outliner, run_outlined_test
+from thonnycontrib.outlines import run_outlined_test
 from .docstring_generator.doc_generator import DocGenerator
 from .l1test_frontend.l1test_reporter import L1TestErrorView, L1TestTreeView
 from .exceptions import *
 from .properties import  ERROR_VIEW_LABEL, PLUGIN_NAME, CANNOT_GENERATE_THE_DOCSTRING
 from .utils import (
     get_focused_writable_text,
     get_selected_line, 
-    send_to_backend, 
     assert_one_line_is_selected
 )
 from .l1test_configuration import l1test_options
 from .l1test_frontend import get_l1test_runner
+from . import get_outliner
 from .environement_vars import *
 from thonny.editors import EditorCodeViewText
 
 def run_all_tests():
     """
     Cette fonction est invoquée quand le button `l1test` est cliqué.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test.
     """
     _send_to_l1test_backend()
 
-def update_test_for_one_menu(event):
-    editor = get_workbench().get_editor_notebook().get_current_editor()
-    if editor is None:
-        return
-    source = editor.get_code_view().get_content()
-    
-    outliner = get_outliner()
-    outliner.from_source_post_menu(source)
-
 def run_selected_test():
     """
     Cette fonction est invoquée quand le button `Run test for selected function`
     suite à un clique droit sur une ligne du fichier.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test avec en argument
     is_selected=True.
     
@@ -199,15 +190,14 @@
                                 accelerator="Alt+d"
     )
 
 def __add_event_binding():
     # Quand un saut de ligne est réalisé après la déclaration d'une fonction,
     # alors une docstring sera générée automatiquement.
     get_workbench().bind_class("EditorCodeViewText", "<KeyRelease-Return>", generate_auto_docstring)
-    get_workbench().bind("<<RunOneTest>>", update_test_for_one_menu, True)
 
 def load_plugin():
     """
     load_plugin est un nom de fonction spécifique qui permet à thonny de charger les élements du plugin
     """
     __init_l1test_options()
     __init_l1test_views()
```

### Comparing `UpyTest-3.0.6/thonnycontrib/properties.py` & `UpyTest-3.0.7/thonnycontrib/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 # Le message affiché sur la treeview quand `l1test` est en cours d'execution
 L1TEST_IN_PROGRESS = "Executing tests in progress ..."
 
 # the evaluation states
 PENDING_STATE = "Pending" 
 EXECUTED_STATE = "Executed" 
 FINISHED_STATE = "Finished"
-INTERRUPTED_STATE = "Interrupted"
 
 # The title of the error view when the docstring genertor shows the raised error
 CANNOT_GENERATE_THE_DOCSTRING = "Cannot generate the docstring :"
 # The title of the error view when the l1test shows the raised error
 CANNOT_RUN_TESTS_MSG = "Cannot run %s :" %(PLUGIN_NAME)
 
 # A special event that `L1TestTreeview` sends to ask `L1TestRunner` to shows the right view
```

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.0.7/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest as ut
 from thonnycontrib.tests.backend_mock import *
 from thonnycontrib.backend.doctest_parser import ExampleWithoutExpected
 from unittest.mock import *
 from thonnycontrib.backend.evaluator import Evaluator
 from thonnycontrib.exceptions import *
 from thonnycontrib.backend.verdicts.EmptyTest import EmptyTest
-from thonnycontrib.backend.verdicts.ExceptionTest import ExceptionTest
+from backend.verdicts.ExceptionVerdict import ExceptionVerdict
 from thonnycontrib.backend.doctest_parser import *
 
 # #######################################################
 #    Tous les tests qui suivent utilisent l'invite `$$$`
 #               SANS valeur attendue  
 # #######################################################
 class TestEvaluator(ut.TestCase):
@@ -94,15 +94,15 @@
     
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             self.assertTrue(SyntaxError.__name__ in verdicts[0].get_detail_failure()) 
     
     def _assert_example_type(self, example_type: Example):
         """Assert that the expected `Example` type is of type the given `example_type`"""
         l1doctests = self.evaluator.get_test_finder().extract_examples()
         
         # on assure qu'il existe un seul noeud AST
```

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import ast
 from types import ModuleType
 from thonnycontrib.backend.doctest_parser import ExampleExceptionExpected
 from thonnycontrib.backend.evaluator import Evaluator
 from thonnycontrib.exceptions import *
 from thonnycontrib.backend.verdicts.EmptyTest import EmptyTest
-from thonnycontrib.backend.verdicts.ExceptionTest import ExceptionTest
-from thonnycontrib.backend.verdicts.FailedTest import FailedTest
-from thonnycontrib.backend.verdicts.PassedTest import PassedTest
-from thonnycontrib.backend.verdicts.FailedWhenExceptionExpectedTest import FailedWhenExceptionExpectedTest
+from backend.verdicts.ExceptionVerdict import ExceptionVerdict
+from backend.verdicts.FailedVerdict import FailedVerdict
+from backend.verdicts.PassedVerdict import PassedVerdict
+from backend.verdicts.FailedWhenExceptionExpectedVerdict import FailedWhenExceptionExpectedVerdict
 from thonnycontrib.tests.backend_mock import *
 
 from thonnycontrib.backend.doctest_parser import *
 import unittest as ut
 
 # ########################################################
 #    Tous les tests qui suivent utilisent l'invite `$$e`
@@ -59,15 +59,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `PassedTest`
-            self.assertTrue(isinstance(verdicts[0], PassedTest))
+            self.assertTrue(isinstance(verdicts[0], PassedVerdict))
            
     def test_evaluate_when_exception_expected_but_not_raised(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
         2. Si une exception est attendue et que la fonction executée ne lève pas
@@ -99,15 +99,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `FailedWhenExceptionExpectedTest`
-            self.assertTrue(isinstance(verdicts[0], FailedWhenExceptionExpectedTest))
+            self.assertTrue(isinstance(verdicts[0], FailedWhenExceptionExpectedVerdict))
             self.assertTrue("Exception was not raised by f(-1, -2)" in verdicts[0].get_detail_failure())
             
     def test_evaluate_when_exception_expected_but_dont_inherit_from_base_exception(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
@@ -151,15 +151,15 @@
         # on assure qu'il existe deux noeuds AST 
         self.assertTrue(len(node_verdicts) == 2)
         for node, verdicts in node_verdicts.items():
             if isinstance(node, ast.FunctionDef):
                 # on assure qu'il existe bien un seul verdict
                 self.assertTrue(len(verdicts) == 1) 
                 # on assure que le verdict est bien du type `ExceptionTest`
-                self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+                self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
                 self.assertTrue(TypeError.__name__ in verdicts[0].get_detail_failure())
                 self.assertTrue("is not a class of type exception." in verdicts[0].get_detail_failure())
     
     def test_evaluate_when_exception_expected_but_is_not_declared(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
@@ -193,15 +193,15 @@
         
         # on assure qu'il existe un seul noeud AST 
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             self.assertTrue(NameError.__name__ in verdicts[0].get_detail_failure())
             self.assertTrue("The expected exception `UnknownException` cannot be found." \
                                 in verdicts[0].get_detail_failure())
             
     def test_evaluate_when_exception_expected_but_an_other_exception_is_raised(self):
         """
         Ce test vérifie:
@@ -236,15 +236,15 @@
         
         # on assure qu'il existe un seul noeud AST 
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `FailedWhenExceptionExpectedTest`
-            self.assertTrue(isinstance(verdicts[0], FailedWhenExceptionExpectedTest))
+            self.assertTrue(isinstance(verdicts[0], FailedWhenExceptionExpectedVerdict))
             self.assertTrue("Exception was not raised by f(-1, -2)\nInstead, it raises :" \
                                 in verdicts[0].get_detail_failure())
             self.assertTrue(ValueError.__name__ in verdicts[0].get_detail_failure())
            
     def test_evaluate_when_syntax_error(self):
         """
         Ce test vérifie:
@@ -279,15 +279,15 @@
         
         # on assure qu'il existe un seul noeud AST 
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             self.assertTrue(SyntaxError.__name__ in verdicts[0].get_detail_failure())
              
     def test_evaluate_when_exception_is_blank_or_empty(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
@@ -320,15 +320,15 @@
         
         # on assure qu'il existe un seul noeud AST 
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 2) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             self.assertTrue(ValueError.__name__ in verdicts[0].get_detail_failure())
             self.assertTrue("The expected exception cannot be empty or blank" \
                                 in verdicts[0].get_detail_failure())
     
     
     def _assert_example_types(self, example_type: Example, len_examples=1):
         """
```

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from types import ModuleType
 from thonnycontrib.backend.doctest_parser import ExampleWithExpected
 from thonnycontrib.backend.evaluator import Evaluator
 from thonnycontrib.exceptions import *
 from thonnycontrib.backend.verdicts.EmptyTest import EmptyTest
-from thonnycontrib.backend.verdicts.ExceptionTest import ExceptionTest
-from thonnycontrib.backend.verdicts.FailedTest import FailedTest
-from thonnycontrib.backend.verdicts.PassedTest import PassedTest
+from backend.verdicts.ExceptionVerdict import ExceptionVerdict
+from backend.verdicts.FailedVerdict import FailedVerdict
+from backend.verdicts.PassedVerdict import PassedVerdict
 from thonnycontrib.backend.doctest_parser import *
 import unittest as ut
 from thonnycontrib.tests.backend_mock import *
 
 # ########################################################
 #    Tous les tests qui suivent utilisent l'invite `$$$`
 #               AVEC une valeur attendue  
@@ -99,15 +99,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `PassedTest`
-            self.assertTrue(isinstance(verdicts[0], PassedTest))
+            self.assertTrue(isinstance(verdicts[0], PassedVerdict))
     
     def test_evaluate_when_failed_verdict(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
         2. Le verdict renvoyé est de type `FailedTest`. 
@@ -138,15 +138,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `FailedTest`
-            self.assertTrue(isinstance(verdicts[0], FailedTest))
+            self.assertTrue(isinstance(verdicts[0], FailedVerdict))
             self.assertTrue('Expected: 2, Got: 3' in verdicts[0].get_detail_failure())
     
     def test_evaluate_when_exception_verdict(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
@@ -180,15 +180,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             # on assure que le message d'exception inclu l'erreur `TypeError`
             self.assertTrue("TypeError: '<' not supported between instances of 'str' and 'int'" \
                                 in verdicts[0].get_detail_failure())
     
     def test_evaluate_when_expected_is_none(self):
         """
         Ce test vérifie:
@@ -223,15 +223,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `PassedTest`
-            self.assertTrue(isinstance(verdicts[0], PassedTest))
+            self.assertTrue(isinstance(verdicts[0], PassedVerdict))
     
     def test_evaluate_when_syntax_error(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
         par le doctest parser.
         2. Quand il y a une erreur de syntax au niveau du test alors
@@ -263,15 +263,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             # on assure que le verdict inclu l'erreur de syntaxe dans son message
             self.assertTrue(SyntaxError.__name__ in verdicts[0].get_detail_failure())
     
     def test_evaluate_when_runtime_error(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithExpected` est le type `Example` extrait 
@@ -305,15 +305,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             # on assure que le verdict inclu l'erreur NameError dans son message
             self.assertTrue(NameError.__name__ in verdicts[0].get_detail_failure()) 
             # on assure que le détail de l'erreur est inclue dans le message du verdict 
             self.assertTrue("name 'c' is not defined" in verdicts[0].get_detail_failure())  
             
     def test_evaluate_when_an_exception_is_expected_and_raised(self):
         """
@@ -349,15 +349,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             # on assure que le verdict inclu l'exception Exception dans son message
             self.assertTrue(Exception.__name__ in verdicts[0].get_detail_failure()) 
             # on assure que le message de l'Exception est inclue dans le message du verdict 
             self.assertTrue("a et b doivent être positifs" in verdicts[0].get_detail_failure()) 
             
     def test_evaluate_when_an_exception_is_expected_but_not_raised(self):
         """
@@ -393,15 +393,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `FailedTest`
-            self.assertTrue(isinstance(verdicts[0], FailedTest))
+            self.assertTrue(isinstance(verdicts[0], FailedVerdict))
             self.assertTrue('Expected: Exception, Got: None' in verdicts[0].get_detail_failure())
     
     def test_evaluate_when_setup(self):
         """
         Ce test vérifie:
         1. Le type `ExampleWithoutExpected` est le type `Example` extrait 
         par le doctest parser.
@@ -434,15 +434,15 @@
         
         # on assure qu'il existe un seul noeud AST avec ses verdicts
         self.assertTrue(len(node_verdicts) == 1)
         for node, verdicts in node_verdicts.items():
             # on assure qu'il existe bien un seul verdict
             self.assertTrue(len(verdicts) == 1) 
             # on assure que le verdict est bien du type `ExceptionTest`
-            self.assertTrue(isinstance(verdicts[0], ExceptionTest))
+            self.assertTrue(isinstance(verdicts[0], ExceptionVerdict))
             self.assertTrue(SyntaxError.__name__ in verdicts[0].get_detail_failure()) 
             # on assure que le détail de l'erreur est inclue dans le message du verdict 
             self.assertTrue("invalid syntax. Maybe you meant '==' or ':=' instead of '='?" \
                             in verdicts[0].get_detail_failure()) 
     
     
     def _assert_example_type(self, example_type: Example):
```

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_test_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from ast import AST
 import unittest as ut
 
-from thonnycontrib.backend.evaluator import TestFinder
+from thonnycontrib.backend.evaluator import L1TestFinder
 from thonnycontrib.backend.doctest_parser import (
     ExampleWithoutExpected, 
     ExampleExceptionExpected, 
     ExampleWithExpected
 )
 from thonnycontrib.exceptions import *
 from thonnycontrib.backend.doctest_parser import *
 
 # ########################################################
 #  Tous les tests qui suivent testent le phase du parsing 
 # ########################################################
 class TestTestFinder(ut.TestCase):
     def setUp(self):
-        self.test_finder = TestFinder(filename="<string>")
+        self.test_finder = L1TestFinder(filename="<string>")
     
     def test_doctest_parser_when_no_examples(self):
         """
             Ce test vérifie que s'il n'y a aucun test dans le noeud ast
             alors aucun type `Example` n'est renvoyé mais plutôt une liste vide.
         """
         fake_source = \
```

### Comparing `UpyTest-3.0.6/thonnycontrib/tests/tests_view.py` & `UpyTest-3.0.7/thonnycontrib/tests/tests_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from types import ModuleType
 import unittest as ut
 from thonnycontrib.l1test_frontend.l1test_treeview import L1TestTreeView
 from thonnycontrib.backend.evaluator import Evaluator
 from thonnycontrib.exceptions import *
-from thonnycontrib.backend.verdicts.FailedWhenExceptionExpectedTest import FailedWhenExceptionExpectedTest
+from backend.verdicts.FailedWhenExceptionExpectedVerdict import FailedWhenExceptionExpectedVerdict
 from thonnycontrib.backend.verdicts.EmptyTest import EmptyTest
-from thonnycontrib.backend.verdicts.ExceptionTest import ExceptionTest
-from thonnycontrib.backend.verdicts.FailedTest import FailedTest
-from thonnycontrib.backend.verdicts.PassedTest import PassedTest
+from backend.verdicts.ExceptionVerdict import ExceptionVerdict
+from backend.verdicts.FailedVerdict import FailedVerdict
+from backend.verdicts.PassedVerdict import PassedVerdict
 from thonnycontrib.backend.doctest_parser import *
 from unittest.mock import *
 from thonnycontrib.tests.backend_mock import *
 
 # #######################################################
 #    Tous les tests qui suivent vérifient le rendu ur la treeview
 # #######################################################
@@ -50,17 +50,17 @@
     return a + b
 """
         self.evaluator.set_source(fake_source)
         self.evaluator.set_module(self.__build_module_from_source(fake_source))
         
         # #####################################################
         # ------------- Verification des verdicts -------------
-        expected_verdicts_colors = {PassedTest: "green",
-                                    FailedTest: "red",
-                                    ExceptionTest: "red"}
+        expected_verdicts_colors = {PassedVerdict: "green",
+                                    FailedVerdict: "red",
+                                    ExceptionVerdict: "red"}
         
         node_verdicts = self.evaluator.evaluate()
         
         
         # on s'assure qu'il existe un seul noeud AST 
         self.assertEqual(len(node_verdicts), 1)
         for node, verdicts in node_verdicts.items():
@@ -143,15 +143,15 @@
     return a + b
 """
         self.evaluator.set_source(fake_source)
         self.evaluator.set_module(self.__build_module_from_source(fake_source))
         
         # #####################################################
         # ------------- Verification des verdicts -------------
-        expected_verdicts_colors = {PassedTest: "green"}
+        expected_verdicts_colors = {PassedVerdict: "green"}
         
         node_verdicts = self.evaluator.evaluate()
         
         # on s'assure qu'il existe un seul noeud AST 
         self.assertEqual(len(node_verdicts), 1)
         for node, verdicts in node_verdicts.items():
             # on s'assure que le nombre de verdicts calculés est exactement le nombre de verdicts attendus
@@ -213,15 +213,15 @@
         # on vérifie le verdict de la fonction `minus()`
         minus_verdict = list(node_verdicts.values())[0]
         self.assertTrue(EmptyTest in [v.__class__ for v in minus_verdict])
         self.assertTrue("orange" in [v.get_tag() for v in minus_verdict])
         
         # on vérifie le verdict de la fonction `somme()`
         somme_verdict = list(node_verdicts.values())[1]
-        self.assertTrue(PassedTest in [v.__class__ for v in somme_verdict])
+        self.assertTrue(PassedVerdict in [v.__class__ for v in somme_verdict])
         self.assertTrue("green" in [v.get_tag() for v in somme_verdict])
         
         # ##################################################################
         # ------------------ Verification du SUMMARIZE ---------------------
         summarize = self.l1TestTreeview.build_summarize_object(node_verdicts)
         self.assertTrue(summarize.total == 1) 
         self.assertTrue(summarize.success == 1) 
@@ -269,16 +269,16 @@
         # on s'assure qu'il existe deux noeuds AST : la fonction `somme()` et la classe `NotAnException`
         self.assertEqual(len(node_verdicts), 2)
         
         # on vérifie qu'il existe au total deux verdicts. Un pour la fonction `somme()`
         # et un autre pour la classe `NotAnException`. 
         self.assertEqual(len(node_verdicts.values()), 2)
         
-        expected_verdicts = [FailedWhenExceptionExpectedTest, PassedTest] + \
-                            [ExceptionTest]*3  # there are 3 exceptions verdicts
+        expected_verdicts = [FailedWhenExceptionExpectedVerdict, PassedVerdict] + \
+                            [ExceptionVerdict]*3  # there are 3 exceptions verdicts
         expected_colors = ["red", "green"] + ["red"]*3
         
         # on vérifie le verdict de la fonction `somme()` qui est à la position 1.
         # La position 0 contient le verdict de la classe `NotAnException`
         somme_verdict = list(node_verdicts.values())[1]
         self.assertEqual(expected_verdicts, [v.__class__ for v in somme_verdict])
         self.assertEqual(expected_colors, [v.get_tag() for v in somme_verdict])
```

### Comparing `UpyTest-3.0.6/thonnycontrib/utils.py` & `UpyTest-3.0.7/thonnycontrib/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """ 
     # on stocke dans une variable d'environnment la valeur de l'option `import_module in shell`.
     # le l1test backend retrouvera cette valeur pour décider d'importer ou non le module dans le shell.
     os.environ[IMPORT_MODULE_VAR] = str(l1test_options.get_option(l1test_options.IMPORT_MODULE))
     
     os.environ[IS_SELECTED_VAR] = str(is_selected)
     if (is_selected):
-        os.environ[NODE_LINENO_VAR] = str(selected_line)
+        os.environ[SELECTED_LINE_VAR] = str(selected_line)
     
     # Une fois que execute_current() est executée un restart backend partiel est invoqué
     # pour un nouveau processus pour la commande passé en paramètre.
     get_runner().execute_current(command_name)
     
 def wrap(string:str, length=8, break_long_words=False):   
     """Wrap a text using the `wraptext` module.
@@ -95,21 +95,14 @@
         for iid in tree.get_children(node):
             if tree.get_children(iid) and tree.item(iid)["open"]:
                 _all_childrens(tree, iid, childrens)
             childrens.append(iid)
         return childrens
     return list(dict.fromkeys(_all_childrens(tree, node, childrens=[])))
 
-def send_current_state(state:str, command_name=BACKEND_COMMAND, **options):
-    from thonny.common import InlineResponse
-    import thonnycontrib.backend.l1test_backend
-    backend = thonnycontrib.backend.l1test_backend.BACKEND
-    assert backend != None
-    backend.send_message(InlineResponse(command_name=command_name, state=state, **options))
-
 def create_node_representation(node:ast.AST):
     """
     Returns the node representation. Especially, returns the prototype or the signature of the node.
     This function can only construct a string representation of the supported nodes. 
     The supported nodes are reported in ASTParser.py in the global variable SUPPORTED_TYPES.
     
     Even if unsupported node is given so just it's name is returned.
@@ -282,26 +275,37 @@
 
     Args:
         filename (str): an absolute path
 
     Returns:
         str: the module name of the given filename.
     """
-    return re.sub(r'.py', "", os.path.basename(filename))
+    return  get_basename(filename, "py")
+
+def get_basename(filename:str, extension:str="*"):
+    """
+    Gets the module name from the specified filename.
+    This function simply gets the basename of the filename, then removes 
+    the given extension. 
+
+    Args:
+        filename (str): an absolute path
+        extension (str): the extension to remove from the filename. 
+        Extension can be a regex. Use '*' to remove all extensions.
+
+    Returns:
+        str: the basename of the given filename without the given extension.
+    """
+    return re.sub(r'.'+extension, "", os.path.basename(filename))
    
 def import_module(filename:str) -> ModuleType:
     """
     Import a module from a given filename. 
     The ~filename~ can be also the absolute path of a file.
     
-    Cette méthode ajoute au module importé la fonction de decoration @test.
-    Cela va permettre au module importé de reconnaitre le décorateur 
-    `@test` même si le module ne contient pas d'importation explicite de cette 
-    fonction.
-    
     This function can raise an exception if the imported module 
     contains a compilation error. You should catch it somewhere.
     
     Args:
         filename (str): The filename(or the absolute path) of a file
 
     Returns:
@@ -323,20 +327,17 @@
             msg_error = "The file \"%s\" cannot be imported.\n\n" % filename + \
                         "Please, be sure that the extension of the file is `.py`" 
         else:
             msg_error = "Cannot found the file `%s`" %filename 
         msg_error = "Error when importing the module \"%s\":\n" % module_name + msg_error
         raise CannotImportModuleException(msg_error)
     
-    imported_module = iu.module_from_spec(spec)
-
-    # on ajoute la fonction de décoration au module importé
-    setattr(imported_module, get_test_only_decorator_name(), test)  
-
-    workingdir = os.path.split(imported_module.__file__)
+    imported_source = iu.module_from_spec(spec)
+    
+    workingdir = os.path.split(imported_source.__file__)
     if (len(workingdir) > 0):
         basedir = workingdir[0]
         dirs = get_all_parent_directories(basedir)
         
         # ajout des packages parents au sys.path
         # on fait ça parce que on veut assurer les imports 
         # des fichiers contenant dans les packages parents
@@ -346,42 +347,23 @@
         # pour assurer les imports des fichiers contenant dans les sous packages
         sub_packages = get_sub_directories(basedir)
         [sys.path.append(basedir + os.sep + path) for path in sub_packages]
   
     try:
         # This line can raise an exception if the module contains compilation errors,
         # or if the module imports non existed modules
-        spec.loader.exec_module(imported_module) 
-        
-        return imported_module
+        spec.loader.exec_module(imported_source) 
+        return imported_source
     except BaseException as e:
         # the compilation error is catched and raised as a CompilationError
         # and the evaluation is interrupted(because we cannot parse a content
         # with compilation errors).
         error_info = sys.exc_info()
         formatted_error = get_last_exception(error_info)
         raise CompilationError(formatted_error) 
-    
-def test(func):
-    '''
-    This function returns a wrapper and it is used as a decorator to execute 
-    the tests of functions that have this decorator.
-    '''
-    def wrap(*args, **kwargs):
-        return func(*args, **kwargs)
-    return wrap
-
-def get_test_only_decorator_name(func=test) -> str:
-    """"Get the name of the decoration function.
-    The decoration function is passed by default to `func` parameter.
-
-    Returns:
-        str: return the name the given function
-    """
-    return func.__name__
 
 def get_all_parent_directories(dir_path:str):
     """
     For a given path of a directory returns all the parents directory from that path.
     
     Examples:
     >>> get_all_parent_directories('/home/stuff/src')
@@ -512,8 +494,52 @@
 def get_font_size_option():
     """Retrieves the value of the "font size" option from the "options" menu.
 
     Returns:
         int: The value of the setted font size.
     """
     workbench = thonny.get_workbench()
-    return workbench._guard_font_size(workbench.get_option("view.editor_font_size"))
+    return workbench._guard_font_size(workbench.get_option("view.editor_font_size"))
+
+def get_image_path(basename:str):
+    """Get the absolute path to the image in the /res directory
+
+    Args:
+        basename (str): just the name of the file inluding it's extension. 
+        For example: "icon.png"
+
+    Returns:
+        str: the absolute path to the image located in the docs/res directory
+    """
+    return os.path.join(os.path.abspath(os.path.dirname(__file__)), "docs", "res", basename)
+
+def get_photoImage(image_name:str):
+    """Returns a PhotoImage object from the given image path.
+
+    Args:
+        image_name (str): The basename of the image with its extension. 
+        The image must be located in the "docs/res" directory.   
+    Returns:
+        PhotoImage: A PhotoImage object.
+    """
+    # le chemin c'est par rapport au dossier du ce fichier 
+    # donc il faut remonter vers /thonnycontrib/ pour rentrer dans docs/res
+    icon_path = get_image_path(image_name)
+    return tk.PhotoImage(name=get_basename(icon_path), file=icon_path)
+
+def send_current_state(state:str, command_name=BACKEND_COMMAND, **options):
+    """
+    Sends the given state with given arg to the front(L1TestRunner).
+
+    Args:
+        state (str): The current state to send.
+        command_name (str, optional): The name of the command. Default is BACKEND_COMMAND.
+        **options: Other options to include in the message.
+
+    Raises:
+        AssertionError: If the backend is not initialized.
+    """
+    from thonny.common import InlineResponse
+    import thonnycontrib.backend.l1test_backend
+    backend = thonnycontrib.backend.l1test_backend.BACKEND
+    assert backend != None
+    backend.send_message(InlineResponse(command_name=command_name, state=state, **options))
```

