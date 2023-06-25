# Comparing `tmp/lol-esp-api-0.24.3.tar.gz` & `tmp/lol-esp-api-0.24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-esp-api-0.24.3.tar", last modified: Sun Jun 25 18:00:48 2023, max compression
+gzip compressed data, was "lol-esp-api-0.24.4.tar", last modified: Sun Jun 25 18:13:41 2023, max compression
```

## Comparing `lol-esp-api-0.24.3.tar` & `lol-esp-api-0.24.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/
--rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.3/LICENSE
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/setup.cfg
--rw-r--r--   0 madking   (1000) madking   (1000)      419 2023-06-25 18:00:46.000000 lol-esp-api-0.24.3/setup.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.377112 lol-esp-api-0.24.3/src/
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.24.3/src/lol_esp_api/__init__.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api/apis/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/__init__.py
--rw-r--r--   0 madking   (1000) madking   (1000)      942 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/eventsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)     2076 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/leaguesAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      542 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/matchAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-06-24 18:26:47.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/supfunc.py
--rw-r--r--   0 madking   (1000) madking   (1000)     1146 2023-06-25 17:51:39.000000 lol-esp-api-0.24.3/src/lol_esp_api/apis/teamsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      249 2023-06-25 17:51:43.000000 lol-esp-api-0.24.3/src/lol_esp_api/lol_esports_api.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:00:48.387112 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/SOURCES.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/dependency_links.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/requires.txt
--rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-06-25 18:00:48.000000 lol-esp-api-0.24.3/src/lol_esp_api.egg-info/top_level.txt
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/
+-rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.4/LICENSE
+-rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/setup.cfg
+-rw-r--r--   0 madking   (1000) madking   (1000)      419 2023-06-25 18:13:19.000000 lol-esp-api-0.24.4/setup.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/src/
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/src/lol_esp_api/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.24.4/src/lol_esp_api/__init__.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/src/lol_esp_api/apis/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/__init__.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      921 2023-06-25 18:12:40.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/eventsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     2055 2023-06-25 18:12:37.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/leaguesAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      520 2023-06-25 18:12:35.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/matchAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-06-24 18:26:47.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/supfunc.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     1119 2023-06-25 18:12:28.000000 lol-esp-api-0.24.4/src/lol_esp_api/apis/teamsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      185 2023-06-25 18:12:53.000000 lol-esp-api-0.24.4/src/lol_esp_api/lol_esports_api.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:13:41.457094 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/
+-rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:13:41.000000 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-06-25 18:13:41.000000 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 18:13:41.000000 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 18:13:41.000000 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/requires.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-06-25 18:13:41.000000 lol-esp-api-0.24.4/src/lol_esp_api.egg-info/top_level.txt
```

### Comparing `lol-esp-api-0.24.3/LICENSE` & `lol-esp-api-0.24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.3/src/lol_esp_api/apis/eventsAPI.py` & `lol-esp-api-0.24.4/src/lol_esp_api/apis/eventsAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.lol_esp_api.apis.supfunc import request
+from supfunc import request
 
 
 def getSchedule(leagueID, PageToken=""):
     url = (
         "https://esports-api.lolesports.com/persisted/gw/getSchedule?leagueId={0}&PageToken={1}"
         "&hl=en-US".format(leagueID, PageToken)
     )
```

### Comparing `lol-esp-api-0.24.3/src/lol_esp_api/apis/leaguesAPI.py` & `lol-esp-api-0.24.4/src/lol_esp_api/apis/leaguesAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.lol_esp_api.apis.supfunc import request
+from supfunc import request
 
 def getLeagues():
     url = "https://esports-api.lolesports.com/persisted/gw/getLeagues?hl=en-US"
 
     return request(url)
 
 def getLeagueBySlug(slug):
```

### Comparing `lol-esp-api-0.24.3/src/lol_esp_api/apis/matchAPI.py` & `lol-esp-api-0.24.4/src/lol_esp_api/apis/matchAPI.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.lol_esp_api.apis.supfunc import request
-
+from supfunc import request
 
 def getWindow(gameID="", startingTime="", participantIds=""):
     url = "https://feed.lolesports.com/livestats/v1/window/{0}?startingTime={1}&participentId={2}".format(
         gameID, startingTime, participantIds
     )
 
     return request(url)
```

### Comparing `lol-esp-api-0.24.3/src/lol_esp_api/apis/teamsAPI.py` & `lol-esp-api-0.24.4/src/lol_esp_api/apis/teamsAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import src.lol_esp_api.apis.supfunc as supfunc
+from supfunc import request
 
 
 # this works with either slug or team Id.
 def getTeams(slug=""):
     if slug == "":
         url = "https://esports-api.lolesports.com/persisted/gw/getTeams?hl=en-US"
     else:
         url = "https://esports-api.lolesports.com/persisted/gw/getTeams?id={}&hl=en-US".format(
             slug
         )
 
-    return supfunc.request(url)
+    return request(url)
 
 
 # this works with either slug or team Id.
 def getTeamPlayers(slug):
     response = getTeams(slug)
     players = response["data"]["teams"][0]["players"]
```

