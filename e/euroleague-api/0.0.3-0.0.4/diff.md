# Comparing `tmp/euroleague_api-0.0.3.tar.gz` & `tmp/euroleague_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euroleague_api-0.0.3.tar", last modified: Sun Jun 18 19:47:57 2023, max compression
+gzip compressed data, was "euroleague_api-0.0.4.tar", last modified: Sun Jun 25 20:51:45 2023, max compression
```

## Comparing `euroleague_api-0.0.3.tar` & `euroleague_api-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 19:47:57.411955 euroleague_api-0.0.3/
--rw-rw-rw-   0        0        0     1097 2023-06-13 23:32:02.000000 euroleague_api-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2030 2023-06-18 19:47:57.411955 euroleague_api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2023-06-18 19:16:51.000000 euroleague_api-0.0.3/README.md
--rw-rw-rw-   0        0        0       88 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      711 2023-06-18 19:47:57.414247 euroleague_api-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 19:47:57.376179 euroleague_api-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 19:47:57.392887 euroleague_api-0.0.3/src/euroleague_api/
--rw-rw-rw-   0        0        0      277 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/__init__.py
--rw-rw-rw-   0        0        0     4413 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/game_stats.py
--rw-rw-rw-   0        0        0    10352 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/player_stats.py
--rw-rw-rw-   0        0        0     2466 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/shot_data.py
--rw-rw-rw-   0        0        0     1323 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/standings.py
--rw-rw-rw-   0        0        0     3804 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/team_stats.py
--rw-rw-rw-   0        0        0    17871 2023-06-13 23:33:55.000000 euroleague_api-0.0.3/src/euroleague_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 19:47:57.404442 euroleague_api-0.0.3/src/euroleague_api.egg-info/
--rw-rw-rw-   0        0        0     2030 2023-06-18 19:47:57.000000 euroleague_api-0.0.3/src/euroleague_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-06-18 19:47:57.000000 euroleague_api-0.0.3/src/euroleague_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 19:47:57.000000 euroleague_api-0.0.3/src/euroleague_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-18 19:47:57.000000 euroleague_api-0.0.3/src/euroleague_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 19:47:57.000000 euroleague_api-0.0.3/src/euroleague_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 20:51:45.306268 euroleague_api-0.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-06-13 23:32:02.000000 euroleague_api-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2209 2023-06-25 20:51:45.306268 euroleague_api-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2023-06-25 20:38:17.000000 euroleague_api-0.0.4/README.md
+-rw-rw-rw-   0        0        0       88 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      711 2023-06-25 20:51:45.309819 euroleague_api-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 20:51:45.252755 euroleague_api-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 20:51:45.274192 euroleague_api-0.0.4/src/euroleague_api/
+-rw-rw-rw-   0        0        0      277 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/__init__.py
+-rw-rw-rw-   0        0        0     4413 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/game_stats.py
+-rw-rw-rw-   0        0        0     2697 2023-06-25 20:29:49.000000 euroleague_api-0.0.4/src/euroleague_api/play_by_play_data.py
+-rw-rw-rw-   0        0        0    10352 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/player_stats.py
+-rw-rw-rw-   0        0        0     2470 2023-06-25 20:30:16.000000 euroleague_api-0.0.4/src/euroleague_api/shot_data.py
+-rw-rw-rw-   0        0        0     1323 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/standings.py
+-rw-rw-rw-   0        0        0     3804 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/team_stats.py
+-rw-rw-rw-   0        0        0    17871 2023-06-13 23:33:55.000000 euroleague_api-0.0.4/src/euroleague_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:51:45.305450 euroleague_api-0.0.4/src/euroleague_api.egg-info/
+-rw-rw-rw-   0        0        0     2209 2023-06-25 20:51:45.000000 euroleague_api-0.0.4/src/euroleague_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-25 20:51:45.000000 euroleague_api-0.0.4/src/euroleague_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:51:45.000000 euroleague_api-0.0.4/src/euroleague_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-25 20:51:45.000000 euroleague_api-0.0.4/src/euroleague_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 20:51:45.000000 euroleague_api-0.0.4/src/euroleague_api.egg-info/top_level.txt
```

### Comparing `euroleague_api-0.0.3/LICENSE` & `euroleague_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/PKG-INFO` & `euroleague_api-0.0.4/src/euroleague_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: euroleague_api
-Version: 0.0.3
+Name: euroleague-api
+Version: 0.0.4
 Summary: A Python wrapper of the Euroleague API
 Home-page: https://github.com/giasemidis/euroleague_api
-Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.4.tar.gz
 Author: Georgios Giasemidis
 Author-email: g.giasemidis@gmail.com
 Keywords: euroleague,api,basketball
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,14 +44,17 @@
 
 ### Standings
 [standings.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/standings.html)
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
+### Play-by-play data
+[play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

### Comparing `euroleague_api-0.0.3/README.md` & `euroleague_api-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 ### Standings
 [standings.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/standings.html)
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
+### Play-by-play data
+[play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

### Comparing `euroleague_api-0.0.3/setup.cfg` & `euroleague_api-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7572 6f6c 6561 6775 655f 6170   = euroleague_ap
 00000020: 690d 0a76 6572 7369 6f6e 203d 2030 2e30  i..version = 0.0
-00000030: 2e33 0d0a 6175 7468 6f72 203d 2047 656f  .3..author = Geo
+00000030: 2e34 0d0a 6175 7468 6f72 203d 2047 656f  .4..author = Geo
 00000040: 7267 696f 7320 4769 6173 656d 6964 6973  rgios Giasemidis
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2067 2e67 6961 7365 6d69 6469 7340 676d   g.giasemidis@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000090: 7772 6170 7065 7220 6f66 2074 6865 2045  wrapper of the E
 000000a0: 7572 6f6c 6561 6775 6520 4150 490d 0a64  uroleague API..d
@@ -22,15 +22,15 @@
 00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000160: 2f67 6961 7365 6d69 6469 732f 6575 726f  /giasemidis/euro
 00000170: 6c65 6167 7565 5f61 7069 0d0a 646f 776e  league_api..down
 00000180: 6c6f 6164 5f75 726c 203d 2068 7474 7073  load_url = https
 00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6769  ://github.com/gi
 000001a0: 6173 656d 6964 6973 2f65 7572 6f6c 6561  asemidis/eurolea
 000001b0: 6775 655f 6170 692f 6172 6368 6976 652f  gue_api/archive/
-000001c0: 7265 6673 2f74 6167 732f 7630 2e30 2e33  refs/tags/v0.0.3
+000001c0: 7265 6673 2f74 6167 732f 7630 2e30 2e34  refs/tags/v0.0.4
 000001d0: 2e74 6172 2e67 7a0d 0a0d 0a5b 6f70 7469  .tar.gz....[opti
 000001e0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
 000001f0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
 00000200: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 00000220: 3d20 3e3d 332e 360d 0a69 6e73 7461 6c6c  = >=3.6..install
 00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
```

### Comparing `euroleague_api-0.0.3/src/euroleague_api/game_stats.py` & `euroleague_api-0.0.4/src/euroleague_api/game_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/src/euroleague_api/player_stats.py` & `euroleague_api-0.0.4/src/euroleague_api/player_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/src/euroleague_api/shot_data.py` & `euroleague_api-0.0.4/src/euroleague_api/shot_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     shots_df['ID_PLAYER'] = shots_df['ID_PLAYER'].str.strip()
     shots_df['ID_ACTION'] = shots_df['ID_ACTION'].str.strip()
     shots_df.insert(0, 'Season', season)
     shots_df.insert(1, 'Gamecode', gamecode)
     return shots_df
 
 
-def get_game_reports_single_season(season: int) -> pd.DataFrame:
+def get_game_shot_data_single_season(season: int) -> pd.DataFrame:
     """
     A function that gets the shot data of *all* games in a single season
 
     Args:
 
         season (int): The start year of the season
 
@@ -58,15 +58,15 @@
         pd.DataFrame: A dataframe with the shot data of all games in a single
             season
     """
     data_df = get_season_data_from_game_data(season, get_game_shot_data)
     return data_df
 
 
-def get_game_reports_multiple_seasons(
+def get_game_shot_data_multiple_seasons(
     start_season: int, end_season: int
 ) -> pd.DataFrame:
     """
     A function that gets the shot data of *all* games in a range of seasons
 
     Args:
```

### Comparing `euroleague_api-0.0.3/src/euroleague_api/standings.py` & `euroleague_api-0.0.4/src/euroleague_api/standings.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/src/euroleague_api/team_stats.py` & `euroleague_api-0.0.4/src/euroleague_api/team_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/src/euroleague_api/utils.py` & `euroleague_api-0.0.4/src/euroleague_api/utils.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.3/src/euroleague_api.egg-info/PKG-INFO` & `euroleague_api-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: euroleague-api
-Version: 0.0.3
+Name: euroleague_api
+Version: 0.0.4
 Summary: A Python wrapper of the Euroleague API
 Home-page: https://github.com/giasemidis/euroleague_api
-Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.4.tar.gz
 Author: Georgios Giasemidis
 Author-email: g.giasemidis@gmail.com
 Keywords: euroleague,api,basketball
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,14 +44,17 @@
 
 ### Standings
 [standings.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/standings.html)
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
+### Play-by-play data
+[play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

