# Comparing `tmp/lol-esp-api-0.24.2.tar.gz` & `tmp/lol-esp-api-0.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-esp-api-0.24.2.tar", last modified: Sun Jun 25 17:52:17 2023, max compression
+gzip compressed data, was "lol-esp-api-0.24.3.tar", last modified: Sun Jun 25 18:00:48 2023, max compression
```

## Comparing `lol-esp-api-0.24.2.tar` & `lol-esp-api-0.24.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/
--rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.2/LICENSE
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-06-25 17:52:17.197124 lol-esp-api-0.24.2/setup.cfg
--rw-r--r--   0 madking   (1000) madking   (1000)      419 2023-06-25 17:49:04.000000 lol-esp-api-0.24.2/setup.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/src/
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/src/lol_esp_api/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.24.2/src/lol_esp_api/__init__.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/src/lol_esp_api/apis/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/__init__.py
--rw-r--r--   0 madking   (1000) madking   (1000)      942 2023-06-25 17:51:39.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/eventsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)     2076 2023-06-25 17:51:39.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/leaguesAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      542 2023-06-25 17:51:39.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/matchAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-06-24 18:26:47.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/supfunc.py
--rw-r--r--   0 madking   (1000) madking   (1000)     1146 2023-06-25 17:51:39.000000 lol-esp-api-0.24.2/src/lol_esp_api/apis/teamsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      249 2023-06-25 17:51:43.000000 lol-esp-api-0.24.2/src/lol_esp_api/lol_esports_api.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 17:52:17.187124 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 17:52:17.000000 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-06-25 17:52:17.000000 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/SOURCES.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 17:52:17.000000 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/dependency_links.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 17:52:17.000000 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/requires.txt
--rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-06-25 17:52:17.000000 lol-esp-api-0.24.2/src/lol_esp_api.egg-info/top_level.txt
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/
+-rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.3/LICENSE
+-rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/setup.cfg
+-rw-r--r--   0 madking   (1000) madking   (1000)      419 2023-06-25 18:00:46.000000 lol-esp-api-0.24.3/setup.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.377112 lol-esp-api-0.24.3/src/
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.24.3/src/lol_esp_api/__init__.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api/apis/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/__init__.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      942 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/eventsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     2076 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/leaguesAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      542 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/matchAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-06-24 18:26:47.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/supfunc.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     1146 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/teamsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      249 2023-06-25 17:51:43.000000 lol-esp-api-0.24.3/src/lol_esp_api/lol_esports_api.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/
+-rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/requires.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/top_level.txt
```

### Comparing `lol-esp-api-0.24.2/LICENSE` & `lol-esp-api-0.24.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.2/src/lol_esp_api/apis/eventsAPI.py` & `lol-esp-api-0.24.3/src/lol_esp_api/apis/eventsAPI.py`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.2/src/lol_esp_api/apis/leaguesAPI.py` & `lol-esp-api-0.24.3/src/lol_esp_api/apis/leaguesAPI.py`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.2/src/lol_esp_api/apis/matchAPI.py` & `lol-esp-api-0.24.3/src/lol_esp_api/apis/matchAPI.py`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.2/src/lol_esp_api/apis/teamsAPI.py` & `lol-esp-api-0.24.3/src/lol_esp_api/apis/teamsAPI.py`

 * *Files identical despite different names*

