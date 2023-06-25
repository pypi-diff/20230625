# Comparing `tmp/fl-api-requester-1.0.0.tar.gz` & `tmp/fl-api-requester-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl-api-requester-1.0.0.tar", last modified: Sun Jun 25 21:02:52 2023, max compression
+gzip compressed data, was "fl-api-requester-1.0.1.tar", last modified: Sun Jun 25 21:18:41 2023, max compression
```

## Comparing `fl-api-requester-1.0.0.tar` & `fl-api-requester-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.814803 fl-api-requester-1.0.0/
--rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      412 2023-06-25 21:02:52.813815 fl-api-requester-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-06-25 20:58:36.000000 fl-api-requester-1.0.0/README.md
--rw-rw-rw-   0        0        0      544 2023-06-25 20:49:59.000000 fl-api-requester-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 21:02:52.814803 fl-api-requester-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.695774 fl-api-requester-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.735771 fl-api-requester-1.0.0/src/fl_api_requester/
--rw-rw-rw-   0        0        0     1856 2023-06-25 12:53:25.000000 fl-api-requester-1.0.0/src/fl_api_requester/FLAPIConnectionData.py
--rw-rw-rw-   0        0        0     9406 2023-06-25 20:27:55.000000 fl-api-requester-1.0.0/src/fl_api_requester/FLAPIRequester.py
--rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.0/src/fl_api_requester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.765770 fl-api-requester-1.0.0/src/fl_api_requester/dto/
--rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/DTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.701774 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.771771 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/alliance/
--rw-rw-rw-   0        0        0      173 2023-06-25 20:29:10.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
--rw-rw-rw-   0        0        0      179 2023-06-25 20:29:23.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.775297 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/authentication/
--rw-rw-rw-   0        0        0      229 2023-06-25 20:29:27.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.781285 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/discord/
--rw-rw-rw-   0        0        0      299 2023-06-25 20:29:32.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
--rw-rw-rw-   0        0        0      251 2023-06-25 20:29:34.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
--rw-rw-rw-   0        0        0      222 2023-06-25 20:29:37.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.790288 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/planet/
--rw-rw-rw-   0        0        0      279 2023-06-25 20:29:41.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
--rw-rw-rw-   0        0        0      233 2023-06-25 20:29:43.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
--rw-rw-rw-   0        0        0      295 2023-06-25 20:29:46.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.795287 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/player/
--rw-rw-rw-   0        0        0      178 2023-06-25 20:29:50.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
--rw-rw-rw-   0        0        0      186 2023-06-25 20:29:52.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
--rw-rw-rw-   0        0        0      239 2023-06-25 20:29:56.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
--rw-rw-rw-   0        0        0      281 2023-06-25 20:29:59.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.799285 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/war/
--rw-rw-rw-   0        0        0      178 2023-06-25 20:30:02.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/war/StartWarDTO.py
--rw-rw-rw-   0        0        0      176 2023-06-25 20:30:05.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/war/StopWarDTO.py
--rw-rw-rw-   0        0        0      336 2023-06-25 20:30:08.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.722771 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.802289 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/alliance/
--rw-rw-rw-   0        0        0      343 2023-06-25 20:30:36.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
--rw-rw-rw-   0        0        0      169 2023-06-25 20:30:44.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.804843 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/authentication/
--rw-rw-rw-   0        0        0      266 2023-06-25 20:30:48.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.806803 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/discord/
--rw-rw-rw-   0        0        0      321 2023-06-25 20:30:56.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/discord/DiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.808803 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/planet/
--rw-rw-rw-   0        0        0      268 2023-06-25 20:31:00.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/planet/PlanetDTO.py
--rw-rw-rw-   0        0        0      287 2023-06-25 20:31:07.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.809803 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/player/
--rw-rw-rw-   0        0        0      447 2023-06-25 20:31:17.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/player/PlayerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.811804 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/war/
--rw-rw-rw-   0        0        0      437 2023-06-25 20:31:27.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
--rw-rw-rw-   0        0        0      543 2023-06-25 20:31:33.000000 fl-api-requester-1.0.0/src/fl_api_requester/dto/response/war/WarDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.812803 fl-api-requester-1.0.0/src/fl_api_requester/exception/
--rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.0/src/fl_api_requester/exception/APIErrorException.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:02:52.764773 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/
--rw-rw-rw-   0        0        0      412 2023-06-25 21:02:52.000000 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2023-06-25 21:02:52.000000 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 21:02:52.000000 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 21:02:52.000000 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-25 21:02:52.000000 fl-api-requester-1.0.0/src/fl_api_requester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.364666 fl-api-requester-1.0.1/
+-rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1266 2023-06-25 21:18:41.363664 fl-api-requester-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2023-06-25 20:58:36.000000 fl-api-requester-1.0.1/README.md
+-rw-rw-rw-   0        0        0      596 2023-06-25 21:18:16.000000 fl-api-requester-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 21:18:41.365666 fl-api-requester-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.275661 fl-api-requester-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.296661 fl-api-requester-1.0.1/src/fl_api_requester/
+-rw-rw-rw-   0        0        0     1856 2023-06-25 12:53:25.000000 fl-api-requester-1.0.1/src/fl_api_requester/FLAPIConnectionData.py
+-rw-rw-rw-   0        0        0     9406 2023-06-25 20:27:55.000000 fl-api-requester-1.0.1/src/fl_api_requester/FLAPIRequester.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.1/src/fl_api_requester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.321662 fl-api-requester-1.0.1/src/fl_api_requester/dto/
+-rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/DTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.279661 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.324664 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/
+-rw-rw-rw-   0        0        0      173 2023-06-25 20:29:10.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
+-rw-rw-rw-   0        0        0      179 2023-06-25 20:29:23.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.326663 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/authentication/
+-rw-rw-rw-   0        0        0      229 2023-06-25 20:29:27.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.334662 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/
+-rw-rw-rw-   0        0        0      299 2023-06-25 20:29:32.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
+-rw-rw-rw-   0        0        0      251 2023-06-25 20:29:34.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
+-rw-rw-rw-   0        0        0      222 2023-06-25 20:29:37.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.338662 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/
+-rw-rw-rw-   0        0        0      279 2023-06-25 20:29:41.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
+-rw-rw-rw-   0        0        0      233 2023-06-25 20:29:43.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
+-rw-rw-rw-   0        0        0      295 2023-06-25 20:29:46.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.344663 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/
+-rw-rw-rw-   0        0        0      178 2023-06-25 20:29:50.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
+-rw-rw-rw-   0        0        0      186 2023-06-25 20:29:52.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
+-rw-rw-rw-   0        0        0      239 2023-06-25 20:29:56.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
+-rw-rw-rw-   0        0        0      281 2023-06-25 20:29:59.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.349430 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/
+-rw-rw-rw-   0        0        0      178 2023-06-25 20:30:02.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/StartWarDTO.py
+-rw-rw-rw-   0        0        0      176 2023-06-25 20:30:05.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/StopWarDTO.py
+-rw-rw-rw-   0        0        0      336 2023-06-25 20:30:08.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.289661 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.352664 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/
+-rw-rw-rw-   0        0        0      343 2023-06-25 20:30:36.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
+-rw-rw-rw-   0        0        0      169 2023-06-25 20:30:44.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.353663 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/authentication/
+-rw-rw-rw-   0        0        0      266 2023-06-25 20:30:48.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.354662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/discord/
+-rw-rw-rw-   0        0        0      321 2023-06-25 20:30:56.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/discord/DiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.356662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/
+-rw-rw-rw-   0        0        0      268 2023-06-25 20:31:00.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/PlanetDTO.py
+-rw-rw-rw-   0        0        0      287 2023-06-25 20:31:07.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.357662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/player/
+-rw-rw-rw-   0        0        0      447 2023-06-25 20:31:17.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/player/PlayerDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.360663 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/
+-rw-rw-rw-   0        0        0      437 2023-06-25 20:31:27.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
+-rw-rw-rw-   0        0        0      543 2023-06-25 20:31:33.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/WarDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.361663 fl-api-requester-1.0.1/src/fl_api_requester/exception/
+-rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.1/src/fl_api_requester/exception/APIErrorException.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.320661 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/
+-rw-rw-rw-   0        0        0     1266 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1956 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/top_level.txt
```

### Comparing `fl-api-requester-1.0.0/LICENSE` & `fl-api-requester-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/README.md` & `fl-api-requester-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/pyproject.toml` & `fl-api-requester-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fl-api-requester"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="FL-GL", email="franceleadergl@gmail.com" }
 ]
 description = "The France Leader API requester."
+readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 dependencies=[
     "munch", "requests"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
+"Homepage" = "https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester"
```

### Comparing `fl-api-requester-1.0.0/src/fl_api_requester/FLAPIConnectionData.py` & `fl-api-requester-1.0.1/src/fl_api_requester/FLAPIConnectionData.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/src/fl_api_requester/FLAPIRequester.py` & `fl-api-requester-1.0.1/src/fl_api_requester/FLAPIRequester.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/src/fl_api_requester/dto/response/war/WarDTO.py` & `fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/WarDTO.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/src/fl_api_requester/exception/APIErrorException.py` & `fl-api-requester-1.0.1/src/fl_api_requester/exception/APIErrorException.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.0/src/fl_api_requester.egg-info/SOURCES.txt` & `fl-api-requester-1.0.1/src/fl_api_requester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

