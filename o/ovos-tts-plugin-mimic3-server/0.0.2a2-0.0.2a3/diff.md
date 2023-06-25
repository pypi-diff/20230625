# Comparing `tmp/ovos_tts_plugin_mimic3_server-0.0.2a2-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic3_server-0.0.2a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13624 bytes, number of entries: 9
--rw-r--r--  2.0 unx    61039 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1141 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      232 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      932 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD
-9 files, 74993 bytes uncompressed, 11958 bytes compressed:  84.1%
+Zip file size: 13610 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    60995 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1141 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jun-25 15:27 ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/RECORD
+9 files, 74949 bytes uncompressed, 11944 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_tts_plugin_mimic3_server/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic3_server/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/zip-safe
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic3_server/__init__.py

```diff
@@ -17,16 +17,15 @@
 from ovos_utils.log import LOG
 
 
 class Mimic3ServerTTSPlugin(TTS):
     """Interface to Mimic3 Server TTS."""
     public_servers = [
         "http://mycroft.blue-systems.com:59125/api/tts",
-        "https://mimic3.ziggyai.online/api/tts",
-        "https://tts.smartgic.io/mimic3/api/tts"
+        "https://mimic3sample.ziggyai.online/api/tts"
     ]
     default_voices = {
         # TODO add default voice for every lang
         "en": "en_US/cmu-arctic_low",
         "en-uk": "en_UK/apope_low",
         "en-gb": "en_UK/apope_low",
         "de": "de_DE/thorsten_low",
```

## ovos_tts_plugin_mimic3_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE` & `ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA` & `ovos_tts_plugin_mimic3_server-0.0.2a3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic3-server
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: Mimic3 server plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic3-server
 Author: OpenVoiceOS
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Keywords: mycroft ovos plugin tts
 Platform: UNKNOWN
```

