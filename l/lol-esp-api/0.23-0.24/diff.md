# Comparing `tmp/lol-esp-api-0.23.tar.gz` & `tmp/lol-esp-api-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-esp-api-0.23.tar", last modified: Sun Jun 25 01:46:53 2023, max compression
+gzip compressed data, was "lol-esp-api-0.24.tar", last modified: Sun Jun 25 02:10:42 2023, max compression
```

## Comparing `lol-esp-api-0.23.tar` & `lol-esp-api-0.24.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 01:46:53.297943 lol-esp-api-0.23/
--rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.23/LICENSE
--rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 01:46:53.297943 lol-esp-api-0.23/PKG-INFO
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 01:46:53.297943 lol-esp-api-0.23/lol_esp_api/
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 01:46:53.297943 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/
--rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 01:46:53.000000 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      250 2023-06-25 01:46:53.000000 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/SOURCES.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 01:46:53.000000 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/dependency_links.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 01:46:53.000000 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/requires.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 01:46:53.000000 lol-esp-api-0.23/lol_esp_api/lol_esp_api.egg-info/top_level.txt
--rw-r--r--   0 madking   (1000) madking   (1000)       38 2023-06-25 01:46:53.297943 lol-esp-api-0.23/setup.cfg
--rw-r--r--   0 madking   (1000) madking   (1000)      433 2023-06-25 01:43:29.000000 lol-esp-api-0.23/setup.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/
+-rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24/LICENSE
+-rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 02:10:42.347840 lol-esp-api-0.24/PKG-INFO
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/lol_esp_api/
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/
+-rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      250 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/requires.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/top_level.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)       38 2023-06-25 02:10:42.347840 lol-esp-api-0.24/setup.cfg
+-rw-r--r--   0 madking   (1000) madking   (1000)      433 2023-06-25 02:05:16.000000 lol-esp-api-0.24/setup.py
```

### Comparing `lol-esp-api-0.23/LICENSE` & `lol-esp-api-0.24/LICENSE`

 * *Files identical despite different names*

