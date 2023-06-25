# Comparing `tmp/lol-esp-api-0.24.tar.gz` & `tmp/lol-esp-api-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-esp-api-0.24.tar", last modified: Sun Jun 25 02:10:42 2023, max compression
+gzip compressed data, was "lol-esp-api-0.24.1.tar", last modified: Sun Jun 25 17:06:15 2023, max compression
```

## Comparing `lol-esp-api-0.24.tar` & `lol-esp-api-0.24.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/
--rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24/LICENSE
--rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 02:10:42.347840 lol-esp-api-0.24/PKG-INFO
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/lol_esp_api/
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 02:10:42.347840 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/
--rw-r--r--   0 madking   (1000) madking   (1000)      295 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      250 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/SOURCES.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/dependency_links.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/requires.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 02:10:42.000000 lol-esp-api-0.24/lol_esp_api/lol_esp_api.egg-info/top_level.txt
--rw-r--r--   0 madking   (1000) madking   (1000)       38 2023-06-25 02:10:42.347840 lol-esp-api-0.24/setup.cfg
--rw-r--r--   0 madking   (1000) madking   (1000)      433 2023-06-25 02:05:16.000000 lol-esp-api-0.24/setup.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:06:15.251677 lol-esp-api-0.24.1/
+-rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.1/LICENSE
+-rw-r--r--   0 madking   (1000) madking   (1000)      297 2023-06-25 17:06:15.251677 lol-esp-api-0.24.1/PKG-INFO
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:06:15.251677 lol-esp-api-0.24.1/lol_esp_api/
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:06:15.251677 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/
+-rw-r--r--   0 madking   (1000) madking   (1000)      297 2023-06-25 17:06:15.000000 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      250 2023-06-25 17:06:15.000000 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 17:06:15.000000 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 17:06:15.000000 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/requires.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 17:06:15.000000 lol-esp-api-0.24.1/lol_esp_api/lol_esp_api.egg-info/top_level.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)       38 2023-06-25 17:06:15.251677 lol-esp-api-0.24.1/setup.cfg
+-rw-r--r--   0 madking   (1000) madking   (1000)      435 2023-06-25 16:42:29.000000 lol-esp-api-0.24.1/setup.py
```

### Comparing `lol-esp-api-0.24/LICENSE` & `lol-esp-api-0.24.1/LICENSE`

 * *Files identical despite different names*

