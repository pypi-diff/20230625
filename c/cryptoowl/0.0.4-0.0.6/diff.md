# Comparing `tmp/cryptoowl-0.0.4.tar.gz` & `tmp/cryptoowl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptoowl-0.0.4.tar", last modified: Sat Jun 24 21:15:33 2023, max compression
+gzip compressed data, was "cryptoowl-0.0.6.tar", last modified: Sat Jun 24 22:42:46 2023, max compression
```

## Comparing `cryptoowl-0.0.4.tar` & `cryptoowl-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:33.329533 cryptoowl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-24 21:15:26.000000 cryptoowl-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 21:15:33.325533 cryptoowl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 21:15:26.000000 cryptoowl-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:33.325533 cryptoowl-0.0.4/cryptoowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 21:15:33.000000 cryptoowl-0.0.4/cryptoowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 21:15:33.000000 cryptoowl-0.0.4/cryptoowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:15:33.000000 cryptoowl-0.0.4/cryptoowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 21:15:33.000000 cryptoowl-0.0.4/cryptoowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:15:33.000000 cryptoowl-0.0.4/cryptoowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:15:33.329533 cryptoowl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 21:15:26.000000 cryptoowl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/cryptoowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/setup.py
```

### Comparing `cryptoowl-0.0.4/LICENSE` & `cryptoowl-0.0.6/LICENSE`

 * *Files identical despite different names*

