# Comparing `tmp/SpLFastlyWrite-1.0.4.tar.gz` & `tmp/SpLFastlyWrite-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpLFastlyWrite-1.0.4.tar", last modified: Sun Jun 25 03:32:21 2023, max compression
+gzip compressed data, was "SpLFastlyWrite-1.0.5.tar", last modified: Sun Jun 25 04:16:08 2023, max compression
```

## Comparing `SpLFastlyWrite-1.0.4.tar` & `SpLFastlyWrite-1.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.388923 SpLFastlyWrite-1.0.4/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-25 03:29:18.000000 SpLFastlyWrite-1.0.4/LICENSE
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 03:32:21.388923 SpLFastlyWrite-1.0.4/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-25 03:29:19.000000 SpLFastlyWrite-1.0.4/README.md
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.381923 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 03:32:21.000000 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-06-25 03:32:21.000000 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/SOURCES.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 03:32:21.000000 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/dependency_links.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 03:32:21.000000 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/not-zip-safe
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-25 03:32:21.000000 SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/top_level.txt
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.381923 SpLFastlyWrite-1.0.4/Spoiled/
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.383923 SpLFastlyWrite-1.0.4/Spoiled/Database/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-06-25 03:29:26.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-25 03:29:25.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/chat_words.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-25 03:29:25.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/chats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-25 03:29:25.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-25 03:29:25.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/completed.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-25 03:29:25.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/global_stats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-25 03:29:26.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/privacy.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-25 03:29:26.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/record.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-25 03:29:26.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/user_chat_info.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-25 03:29:26.000000 SpLFastlyWrite-1.0.4/Spoiled/Database/users.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.384923 SpLFastlyWrite-1.0.4/Spoiled/Shannu/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-06-25 03:29:24.000000 SpLFastlyWrite-1.0.4/Spoiled/Shannu/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-06-25 03:29:24.000000 SpLFastlyWrite-1.0.4/Spoiled/Shannu/alpha.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1327 2023-06-25 03:29:24.000000 SpLFastlyWrite-1.0.4/Spoiled/Shannu/config.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1276 2023-06-25 03:29:24.000000 SpLFastlyWrite-1.0.4/Spoiled/Shannu/shivi.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-06-25 03:29:24.000000 SpLFastlyWrite-1.0.4/Spoiled/Shannu/words.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 03:32:21.387923 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-25 03:29:23.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8189 2023-06-25 03:29:21.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/callbacks.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      585 2023-06-25 03:29:21.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-25 03:29:21.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/eval.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2824 2023-06-25 03:29:21.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/fw.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1139 2023-06-25 03:29:21.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/help.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-06-25 03:29:22.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/image.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1410 2023-06-25 03:29:22.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/inline.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      831 2023-06-25 03:29:22.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/leaderboard.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      876 2023-06-25 03:29:22.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/served.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3720 2023-06-25 03:29:23.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/start.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-25 03:29:23.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/templates.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-25 03:29:23.000000 SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/watchers.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-25 03:29:20.000000 SpLFastlyWrite-1.0.4/Spoiled/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-25 03:32:21.388923 SpLFastlyWrite-1.0.4/setup.cfg
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-25 03:32:11.000000 SpLFastlyWrite-1.0.4/setup.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.931705 SpLFastlyWrite-1.0.5/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-25 04:12:25.000000 SpLFastlyWrite-1.0.5/LICENSE
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:16:08.930705 SpLFastlyWrite-1.0.5/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.5/README.md
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.924704 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/SOURCES.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/dependency_links.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/not-zip-safe
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/top_level.txt
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.924704 SpLFastlyWrite-1.0.5/Spoiled/
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.927704 SpLFastlyWrite-1.0.5/Spoiled/Database/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/chat_words.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/chats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/completed.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/global_stats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/privacy.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/record.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/user_chat_info.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/users.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.928705 SpLFastlyWrite-1.0.5/Spoiled/Shannu/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/alpha.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1327 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/config.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1264 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/shivi.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/words.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.930705 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8156 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/callbacks.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/eval.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2831 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/fw.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/help.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/image.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/inline.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/leaderboard.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/served.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3727 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/start.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/templates.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/watchers.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-25 04:12:27.000000 SpLFastlyWrite-1.0.5/Spoiled/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-25 04:16:08.931705 SpLFastlyWrite-1.0.5/setup.cfg
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.5/setup.py
```

### Comparing `SpLFastlyWrite-1.0.4/LICENSE` & `SpLFastlyWrite-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/PKG-INFO` & `SpLFastlyWrite-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.4
+Version: 1.0.5
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/PKG-INFO` & `SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.4
+Version: 1.0.5
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.4/SpLFastlyWrite.egg-info/SOURCES.txt` & `SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/chat_words.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/chat_words.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/chats.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/chats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/coins.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/completed.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/completed.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/global_stats.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/global_stats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/privacy.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/privacy.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/user_chat_info.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/user_chat_info.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Database/users.py` & `SpLFastlyWrite-1.0.5/Spoiled/Database/users.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Shannu/config.py` & `SpLFastlyWrite-1.0.5/Spoiled/Shannu/config.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/Shannu/shivi.py` & `SpLFastlyWrite-1.0.5/Spoiled/Shannu/shivi.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,17 +19,17 @@
   except:
     pass
   with open("Images/bg.jpg", "wb") as f:
     f.write(g.content)
 
 try:
   if API_ID and API_HASH:
-    alpha = Alpha("SpLFW", api_id=API_ID, api_hash=API_HASH, bot_token=BOT_TOKEN, plugins=dict(root='Spoiled/SpoiledPlugins'))
+    alpha = Alpha("SpLFW", api_id=API_ID, api_hash=API_HASH, bot_token=BOT_TOKEN, plugins=dict(root='./SpoiledPlugins'))
   else:
-    alpha = Alpha("SpLFW", bot_token=BOT_TOKEN, plugins=dict(root='Spoiled/SpoiledPlugins'))
+    alpha = Alpha("SpLFW", bot_token=BOT_TOKEN, plugins=dict(root='./SpoiledPlugins'))
 except Exception as e:
   print(e)
   sys.exit()
 
 def __initialize__():  
   try:
     database()
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/__init__.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/callbacks.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from . import capsify, _sort, mention, title
 from alphagram.types import IKM, IKB
-from alphagram import filters
+from alphagram import Alpha, filters
 from ..Database.privacy import *
 from ..Database.chats import get_served_chats
 from ..Database.users import get_served_users
 from ..Database.global_stats import get_users_dic, get_chats_dic
 from ..Database.chat_words import get_top_chat_users
 from ..Database.user_chat_info import get_user_info, get_chat_info
 from ..Database.coins import _get, _get_chat
 from .templates import info_template
 from Spoiled import CODE_OWNER_ID
-from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_callback_query(filters.regex('leaderboard'))
+@Alpha.on_callback_query(filters.regex('leaderboard'))
 async def leaderboard_cbq(_, q):
   markup = IKM(
     [
       [
         IKB(capsify('users'), callback_data='users'),
         IKB(capsify('chats'), callback_data='chats')
       ],
@@ -24,15 +23,15 @@
         IKB(capsify("back"), callback_data="backtostart")
       ]
     ]
   )
   await q.answer()
   await q.edit_message_text(capsify('» private accounts will be hidden.') + '\n\n' + capsify('choose from below !'), reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('info'))
+@Alpha.on_callback_query(filters.regex('info'))
 async def info_cbq(_, q):
   chats = str(len(await get_served_chats()))
   users = str(len(await get_served_users()))
   txt = info_template(chats, users)
   markup = IKM(
     [
       [
@@ -47,15 +46,15 @@
         IKB(capsify('back'), callback_data='backtostart')
       ]
     ]
   )
   await q.answer()
   await q.edit_message_text(txt, reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('settings'))
+@Alpha.on_callback_query(filters.regex('settings'))
 async def settings_cbq(_, q):
   user_id = q.from_user.id
   x = await get_private_users()
   priv = True if user_id in x else False
   enab = capsify("enabled 🔘") if priv else capsify("enabled")
   disab = capsify("disabled") if priv else capsify("disabled 🔘")
   markup = IKM(
@@ -75,20 +74,20 @@
   txt = capsify('⚙️ settings') + '\n\n'
   txt += capsify('privacy enabled » your profile will be private.') + '\n'
   txt += capsify('privacy disabled » your profile will be public.') + '\n\n'
   txt += capsify('choose from below !')
   await q.answer()
   await q.edit_message_text(txt, reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('privacy_answer'))
+@Alpha.on_callback_query(filters.regex('privacy_answer'))
 async def privacy_answer_cbq(_, q):
   txt = 'use buttons below to toggle private mode !'
   await q.answer(capsify(txt), show_alert=True)
 
-@alpha.on_callback_query(filters.regex('users') | filters.regex('users_'))
+@Alpha.on_callback_query(filters.regex('users') | filters.regex('users_'))
 async def users(_, q):
   if q.data == 'users':
     x = await get_private_users()
     dic = await get_users_dic()
     dic = _sort(dic)
     a = 1
     txt = capsify('top users by words') + "\n\n"
@@ -135,15 +134,15 @@
           IKB(capsify('back'), callback_data='leaderboard')
         ]
       ]
     )
     await q.answer()
     await q.edit_message_text(txt, reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('chats') | filters.regex('chats_'))
+@Alpha.on_callback_query(filters.regex('chats') | filters.regex('chats_'))
 async def chats(_, q):
   if q.data == 'chats':
     dic = await get_chats_dic()
     dic = _sort(dic)
     a = 1
     txt = capsify('top chats by words') + "\n\n"
     for y in dic:
@@ -184,15 +183,15 @@
           IKB(capsify('back'), callback_data='leaderboard')
         ]
       ]
     )
     await q.answer()
     await q.edit_message_text(txt, reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('enable') | filters.regex('disable'))
+@Alpha.on_callback_query(filters.regex('enable') | filters.regex('disable'))
 async def enab_priv(_, q):
   user_id = q.from_user.id
   data = q.data
   x = await get_private_users()
   if q.data == 'enable':
     if user_id in x:
       return await q.answer(capsify('private mode is already enabled !'), show_alert=True)
@@ -218,15 +217,15 @@
         IKB(capsify('back'), callback_data='backtostart')
       ]
     ]
   )
   await q.answer()
   await q.edit_message_reply_markup(reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('topby_'))
+@Alpha.on_callback_query(filters.regex('topby_'))
 async def topby(_, q):
   data = q.data.split('_')[1]
   await q.answer()
   if data == 'coins':
     await q.edit_message_text(capsify('sorting top by coins, please wait...'))
     get = await _get()
     sor = _sort(get)
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/coins.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/coins.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from alphagram import filters
+from alphagram import Alpha, filters
 from ..Database.coins import get_coins
 from . import capsify
-from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_message(filters.command('coins') & filters.group)
+@Alpha.on_message(filters.command('coins') & filters.group)
 async def coins(_, m):
   user_id = m.from_user.id
   chat_id = m.chat.id
   title = m.chat.title
   this_coins = await get_coins(user_id, chat_id=chat_id)
   global_coins = await get_coins(user_id)
   txt = capsify("coins in") + '\n\n'
   txt += f'{title} : `{this_coins}`\n'
   txt += f'{capsify("global")} : `{global_coins}`'
   await m.reply(txt)
-                                  
+
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/eval.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/eval.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/fw.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/fw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from . import _sort, capsify, get_readable_time
-from alphagram import filters
+from alphagram import Alpha, filters
 from alphagram.types import IKM, IKB
 from ..Database.chats import get_served_chats
 from ..Database.completed import incr_word
 from ..Database.chat_words import incr_chat_word
 from ..Database.coins import add_coins
 from ..Database.global_stats import *
 from ..Database.record import update_record
 from Spoiled.Shannu.config import SUPPORT_GROUP, WORD_SPAWN_TIME
 from .watchers import fw_watcher
 import words
-from Spoiled.Shannu.shivi import alpha
+from Spoiled.Shannu.alpha import alpha
 from .image import make_image
 import asyncio
 import time
 
 dic = {} # status dict
 last_sent = {} # queue dict
 
@@ -31,15 +31,15 @@
     return 10
   if t <= 10:
     return 8
   if t <= 60:
     return 5
   return 3
 
-@alpha.on_message(filters.group, group=fw_watcher)
+@Alpha.on_message(filters.group, group=fw_watcher)
 async def cwf(_, m):
   global dic
   if not m.chat:
     return
   chat_id = m.chat.id
   if chat_id not in dic:
     return
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/help.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from alphagram import filters
+from alphagram import Alpha, filters
 from config import OWNER_ID, SUPPORT_GROUP, SUPPORT_CHANNEL
 from Spoiled import CODE_OWNER_ID
 from . import capsify
 from alphagram.types import IKM, IKB
-from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_message(filters.command('help') & filters.private)
+@Alpha.on_message(filters.command('help') & filters.private)
 async def help(_, m):
   txt = f'**{capsify("commands")}**\n\n'
   txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
   txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
   txt += '\n'
   txt += f'**{capsify("bot owner contact")}**\n\n'
   group = capsify('group')
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/image.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/image.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/inline.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/inline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from ..Database.coins import get_coins
 from . import capsify, get_readable_time, title
 from Spoiled.Database.completed import get_top_chat, get_completed_words
 from Spoiled.Database.record import get_record
-from alphagram import filters
-from Spoiled.Shannu.alpha import alpha
+from alphagram import Alpha, filters
 from alphagram.types import InlineQueryResultArticle as IQRA, InputTextMessageContent as ITMC, IKM, IKB
 
 
-@alpha.on_inline_query()
+@Alpha.on_inline_query()
 async def inline(_, i):
   query = i.query
   if query == 'share':
     user_id = i.from_user.id
     cns = await get_coins(user_id)
     txt = capsify('👤 User Profile')
     txt += '\n\n'
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/leaderboard.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/leaderboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from alphagram import filters
+from alphagram import Alpha, filters
 from ..Database.chat_words import get_top_chat_users
 from alphagram.types import IKM, IKB
 from . import capsify, mention, title
-from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_message(filters.command('leaderboard') & filters.group)
+@Alpha.on_message(filters.command('leaderboard') & filters.group)
 async def leaderboard(_, m):
   ok = await m.reply(capsify('getting leaderboard...'))
   chat_id = m.chat.id
   chat_title = m.chat.title
   x = await get_top_chat_users(chat_id)
   txt = capsify('top word completers in {}') + '\n\n'
   txt = txt.format(chat_title)
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/served.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/served.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .watchers import served_watcher
 from alphagram import Alpha, filters
 from ..Database.chats import add_served_chat
 from ..Database.users import add_served_user
 from ..Database.user_chat_info import update_chat_info, update_user_info
-from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_message(group=served_watcher)
+@Alpha.on_message(group=served_watcher)
 async def cwf(_, m):
   if m.from_user:
     await add_served_user(m.from_user.id)
     details = {}
     details["first_name"] = m.from_user.first_name
     details["last_name"] = m.from_user.last_name if m.from_user.last_name else None
     details["username"] = m.from_user.username if m.from_user.username else None
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/start.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from alphagram import filters
+from alphagram import Alpha, filters
 from alphagram.types import IKM, IKB
 from config import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
 from Spoiled.Database.users import add_served_user
 from Spoiled.Database.coins import get_coins
 from Spoiled.Database.completed import get_top_chat, get_completed_words
 from Spoiled.Database.record import get_record
 from . import capsify, get_readable_time, title
 from Spoiled.Shannu.alpha import alpha
 
-@alpha.on_message(filters.command('start') & filters.private)
+@Alpha.on_message(filters.command('start') & filters.private)
 async def start(_, m):
   await add_served_user(m.from_user.id)
   txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
   id = _.me.id
   un = _.me.username
   fn = _.me.first_name
   user_first_name = m.from_user.first_name
@@ -33,15 +33,15 @@
               IKB(capsify("Info ℹ️"), callback_data='info'),
               IKB(capsify("Settings ⚙️"), callback_data='settings')
           ]
       ]
   )
   await m.reply(txt.format(user_first_name, fn), reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('backtostart'))
+@Alpha.on_callback_query(filters.regex('backtostart'))
 async def backtostart(_, q):
   txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
   id = _.me.id
   un = _.me.username
   fn = _.me.first_name
   user_first_name = q.from_user.first_name
   markup = IKM(
@@ -62,15 +62,15 @@
               IKB(capsify("Settings ⚙️"), callback_data='settings')
           ]
       ]
   )
   await q.answer()
   await q.edit_message_text(txt.format(user_first_name, fn), reply_markup=markup)
 
-@alpha.on_callback_query(filters.regex('profile'))
+@Alpha.on_callback_query(filters.regex('profile'))
 async def profile_cbq(_, q):
   await q.answer()
   await q.edit_message_text(capsify('getting your profile, please wait...'))
   user_id = q.from_user.id
   cns = await get_coins(user_id)
   txt = capsify('👤 User Profile')
   txt += '\n\n'
```

### Comparing `SpLFastlyWrite-1.0.4/Spoiled/SpoiledPlugins/templates.py` & `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/templates.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.4/setup.py` & `SpLFastlyWrite-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="SpLFastlyWrite",
-    version="1.0.4",
+    version="1.0.5",
     description="SpLFastlyWrite",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ShutupKeshav/SpLFastlyWrite",
     download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
     author="ShutupKeshav",
     author_email="keshavatripathi@yahoo.com",
```

