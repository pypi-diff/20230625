# Comparing `tmp/habitat_tools-0.1.9.tar.gz` & `tmp/habitat-tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habitat_tools-0.1.9.tar", max compression
+gzip compressed data, was "habitat-tools-0.2.0.tar", last modified: Sun Jun 25 19:18:20 2023, max compression
```

## Comparing `habitat_tools-0.1.9.tar` & `habitat-tools-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0       76 2022-05-27 16:37:30.287874 habitat_tools-0.1.9/habitat_tools/__init__.py
--rw-r--r--   0        0        0     3283 2022-07-10 16:20:09.211595 habitat_tools-0.1.9/habitat_tools/api_tools.py
--rw-r--r--   0        0        0      511 2022-07-10 16:14:57.268417 habitat_tools-0.1.9/habitat_tools/exceptions.py
--rw-r--r--   0        0        0      635 2022-06-28 23:17:28.552808 habitat_tools-0.1.9/habitat_tools/utils.py
--rw-r--r--   0        0        0      375 2022-07-10 16:20:15.932250 habitat_tools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      638 2022-07-10 16:20:26.766073 habitat_tools-0.1.9/setup.py
--rw-r--r--   0        0        0      510 2022-07-10 16:20:26.766548 habitat_tools-0.1.9/PKG-INFO
+drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2023-06-25 19:18:20.880284 habitat-tools-0.2.0/
+-rw-rw-r--   0 warren    (1000) warren    (1000)      268 2023-06-25 19:18:20.880284 habitat-tools-0.2.0/PKG-INFO
+-rw-rw-r--   0 warren    (1000) warren    (1000)       13 2023-06-25 18:30:34.000000 habitat-tools-0.2.0/README.md
+drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2023-06-25 19:18:20.880284 habitat-tools-0.2.0/api_tools/
+-rw-rw-r--   0 warren    (1000) warren    (1000)       61 2023-06-25 18:30:34.000000 habitat-tools-0.2.0/api_tools/__init__.py
+-rw-rw-r--   0 warren    (1000) warren    (1000)     1195 2023-06-25 18:30:34.000000 habitat-tools-0.2.0/api_tools/renderer.py
+-rw-rw-r--   0 warren    (1000) warren    (1000)     2927 2023-06-25 18:30:34.000000 habitat-tools-0.2.0/api_tools/tools.py
+drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2023-06-25 19:18:20.880284 habitat-tools-0.2.0/habitat_tools.egg-info/
+-rw-rw-r--   0 warren    (1000) warren    (1000)      268 2023-06-25 19:18:20.000000 habitat-tools-0.2.0/habitat_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 warren    (1000) warren    (1000)      229 2023-06-25 19:18:20.000000 habitat-tools-0.2.0/habitat_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 warren    (1000) warren    (1000)        1 2023-06-25 19:18:20.000000 habitat-tools-0.2.0/habitat_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 warren    (1000) warren    (1000)       10 2023-06-25 19:18:20.000000 habitat-tools-0.2.0/habitat_tools.egg-info/top_level.txt
+-rw-rw-r--   0 warren    (1000) warren    (1000)       38 2023-06-25 19:18:20.880284 habitat-tools-0.2.0/setup.cfg
+-rw-rw-r--   0 warren    (1000) warren    (1000)      430 2023-06-25 19:17:24.000000 habitat-tools-0.2.0/setup.py
```

