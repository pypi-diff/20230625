# Comparing `tmp/cryptoowl-0.0.6.tar.gz` & `tmp/cryptoowl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptoowl-0.0.6.tar", last modified: Sat Jun 24 22:42:46 2023, max compression
+gzip compressed data, was "cryptoowl-0.0.7.tar", last modified: Sun Jun 25 08:03:36 2023, max compression
```

## Comparing `cryptoowl-0.0.6.tar` & `cryptoowl-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/cryptoowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:42:46.000000 cryptoowl-0.0.6/cryptoowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:42:46.454944 cryptoowl-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 22:42:36.000000 cryptoowl-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:03:35.996545 cryptoowl-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-25 08:03:29.000000 cryptoowl-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 08:03:35.996545 cryptoowl-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 08:03:29.000000 cryptoowl-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:03:35.996545 cryptoowl-0.0.7/cryptoowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 08:03:35.000000 cryptoowl-0.0.7/cryptoowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-25 08:03:35.000000 cryptoowl-0.0.7/cryptoowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:03:35.000000 cryptoowl-0.0.7/cryptoowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 08:03:35.000000 cryptoowl-0.0.7/cryptoowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 08:03:35.000000 cryptoowl-0.0.7/cryptoowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:03:35.996545 cryptoowl-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-25 08:03:29.000000 cryptoowl-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:03:35.996545 cryptoowl-0.0.7/social/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:03:29.000000 cryptoowl-0.0.7/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 08:03:29.000000 cryptoowl-0.0.7/social/kitty.py
```

### Comparing `cryptoowl-0.0.6/LICENSE` & `cryptoowl-0.0.7/LICENSE`

 * *Files identical despite different names*

