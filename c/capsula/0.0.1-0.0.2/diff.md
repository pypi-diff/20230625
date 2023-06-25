# Comparing `tmp/capsula-0.0.1.tar.gz` & `tmp/capsula-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsula-0.0.1.tar", max compression
+gzip compressed data, was "capsula-0.0.2.tar", max compression
```

## Comparing `capsula-0.0.1.tar` & `capsula-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-06-23 14:46:03.560678 capsula-0.0.1/LICENSE
--rw-r--r--   0        0        0       85 2023-06-23 14:54:58.750678 capsula-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 14:52:36.820678 capsula-0.0.1/capsula/__init__.py
--rw-r--r--   0        0        0      369 2023-06-23 14:54:08.740678 capsula-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 capsula-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-23 14:46:03.560678 capsula-0.0.2/LICENSE
+-rw-r--r--   0        0        0       81 2023-06-25 03:00:51.991804 capsula-0.0.2/README.md
+-rw-r--r--   0        0        0       48 2023-06-25 03:19:05.921800 capsula-0.0.2/capsula/__init__.py
+-rw-r--r--   0        0        0     1654 2023-06-25 03:00:51.991804 capsula-0.0.2/capsula/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-25 03:21:49.471792 capsula-0.0.2/capsula/_version.py
+-rw-r--r--   0        0        0     2829 2023-06-25 03:00:51.991804 capsula-0.0.2/capsula/capture.py
+-rw-r--r--   0        0        0     4487 2023-06-25 03:00:51.991804 capsula-0.0.2/capsula/context.py
+-rw-r--r--   0        0        0      849 2023-06-25 03:00:51.991804 capsula-0.0.2/capsula/hash.py
+-rw-r--r--   0        0        0     3436 2023-06-25 03:21:49.471792 capsula-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 capsula-0.0.2/PKG-INFO
```

### Comparing `capsula-0.0.1/LICENSE` & `capsula-0.0.2/LICENSE`

 * *Files identical despite different names*

