# Comparing `tmp/SpLFastlyWrite-1.0.5.tar.gz` & `tmp/SpLFastlyWrite-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpLFastlyWrite-1.0.5.tar", last modified: Sun Jun 25 04:16:08 2023, max compression
+gzip compressed data, was "SpLFastlyWrite-1.0.6.tar", last modified: Sun Jun 25 04:38:01 2023, max compression
```

## Comparing `SpLFastlyWrite-1.0.5.tar` & `SpLFastlyWrite-1.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.931705 SpLFastlyWrite-1.0.5/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-25 04:12:25.000000 SpLFastlyWrite-1.0.5/LICENSE
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:16:08.930705 SpLFastlyWrite-1.0.5/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.5/README.md
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.924704 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/SOURCES.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/dependency_links.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/not-zip-safe
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/top_level.txt
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.924704 SpLFastlyWrite-1.0.5/Spoiled/
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.927704 SpLFastlyWrite-1.0.5/Spoiled/Database/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/chat_words.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/chats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/completed.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/global_stats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/privacy.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/record.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/user_chat_info.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.5/Spoiled/Database/users.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.928705 SpLFastlyWrite-1.0.5/Spoiled/Shannu/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/alpha.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1327 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/config.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1264 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/shivi.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.5/Spoiled/Shannu/words.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:16:08.930705 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8156 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/callbacks.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/eval.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2831 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/fw.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/help.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/image.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/inline.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/leaderboard.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/served.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3727 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/start.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/templates.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/watchers.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-25 04:12:27.000000 SpLFastlyWrite-1.0.5/Spoiled/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-25 04:16:08.931705 SpLFastlyWrite-1.0.5/setup.cfg
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.5/setup.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.312514 SpLFastlyWrite-1.0.6/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-25 04:12:25.000000 SpLFastlyWrite-1.0.6/LICENSE
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:38:01.312514 SpLFastlyWrite-1.0.6/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.6/README.md
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.303513 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:38:01.000000 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-06-25 04:38:01.000000 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/SOURCES.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:38:01.000000 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/dependency_links.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/not-zip-safe
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-25 04:38:01.000000 SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/top_level.txt
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.303513 SpLFastlyWrite-1.0.6/Spoiled/
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.306513 SpLFastlyWrite-1.0.6/Spoiled/Database/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/chat_words.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/chats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/completed.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/global_stats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/privacy.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/record.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/user_chat_info.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.6/Spoiled/Database/users.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.308513 SpLFastlyWrite-1.0.6/Spoiled/Shannu/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.6/Spoiled/Shannu/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.6/Spoiled/Shannu/alpha.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1327 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.6/Spoiled/Shannu/config.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1264 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.6/Spoiled/Shannu/shivi.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.6/Spoiled/Shannu/words.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:38:01.312514 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8156 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/callbacks.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/eval.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2876 2023-06-25 04:37:02.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/fw.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/help.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/image.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/inline.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/leaderboard.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/served.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3727 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/start.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/templates.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/watchers.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-25 04:12:27.000000 SpLFastlyWrite-1.0.6/Spoiled/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-25 04:38:01.313514 SpLFastlyWrite-1.0.6/setup.cfg
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-25 04:37:22.000000 SpLFastlyWrite-1.0.6/setup.py
```

### Comparing `SpLFastlyWrite-1.0.5/LICENSE` & `SpLFastlyWrite-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/PKG-INFO` & `SpLFastlyWrite-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.5
+Version: 1.0.6
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/PKG-INFO` & `SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.5
+Version: 1.0.6
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.5/SpLFastlyWrite.egg-info/SOURCES.txt` & `SpLFastlyWrite-1.0.6/SpLFastlyWrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/chat_words.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/chat_words.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/chats.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/chats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/coins.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/completed.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/completed.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/global_stats.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/global_stats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/privacy.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/privacy.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/user_chat_info.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/user_chat_info.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Database/users.py` & `SpLFastlyWrite-1.0.6/Spoiled/Database/users.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Shannu/config.py` & `SpLFastlyWrite-1.0.6/Spoiled/Shannu/config.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/Shannu/shivi.py` & `SpLFastlyWrite-1.0.6/Spoiled/Shannu/shivi.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/__init__.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/callbacks.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/coins.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/eval.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/eval.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/fw.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/fw.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,18 @@
   await update_record(user_id, tt)
   await add_coins(user_id, int(rew), chat_id)
 
 async def send():
   global last_sent, dic
   _ = alpha
   while True:
-    un = _.me.username
+    try:
+        un = _.me.username
+    except:
+        continue
     chats = await get_served_chats()
     for x in chats:
       if x in last_sent:
         diff = int(time.time() - last_sent[x])
         if diff >= WORD_SPAWN_TIME:
           w = words.Word()
           im = make_image(w, un)
```

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/help.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/help.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/image.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/image.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/inline.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/inline.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/leaderboard.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/leaderboard.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/served.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/served.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/start.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/start.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/Spoiled/SpoiledPlugins/templates.py` & `SpLFastlyWrite-1.0.6/Spoiled/SpoiledPlugins/templates.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.5/setup.py` & `SpLFastlyWrite-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="SpLFastlyWrite",
-    version="1.0.5",
+    version="1.0.6",
     description="SpLFastlyWrite",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ShutupKeshav/SpLFastlyWrite",
     download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
     author="ShutupKeshav",
     author_email="keshavatripathi@yahoo.com",
```

