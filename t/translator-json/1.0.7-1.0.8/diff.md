# Comparing `tmp/translator_json-1.0.7.tar.gz` & `tmp/translator_json-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_json-1.0.7.tar", last modified: Sat Oct 15 12:35:25 2022, max compression
+gzip compressed data, was "translator_json-1.0.8.tar", last modified: Sun Jun 25 05:08:19 2023, max compression
```

## Comparing `translator_json-1.0.7.tar` & `translator_json-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-15 12:35:25.053420 translator_json-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-10-15 12:35:11.000000 translator_json-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2180 2022-10-15 12:35:25.053420 translator_json-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1641 2022-10-15 12:35:11.000000 translator_json-1.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-10-15 12:35:11.000000 translator_json-1.0.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      198 2022-10-15 12:35:25.053420 translator_json-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-10-15 12:35:11.000000 translator_json-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-15 12:35:25.054420 translator_json-1.0.7/translator/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-15 12:35:11.000000 translator_json-1.0.7/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-10-15 12:35:25.054420 translator_json-1.0.7/translator/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2022-10-15 12:35:11.000000 translator_json-1.0.7/translator/translate_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-15 12:35:25.053420 translator_json-1.0.7/translator_json.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2180 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      126 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-10-15 12:35:25.000000 translator_json-1.0.7/translator_json.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-10-15 12:35:11.000000 translator_json-1.0.7/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.524297 translator_json-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-25 05:08:07.000000 translator_json-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-25 05:08:19.525297 translator_json-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2023-06-25 05:08:07.000000 translator_json-1.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-25 05:08:07.000000 translator_json-1.0.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-25 05:08:19.525297 translator_json-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-25 05:08:07.000000 translator_json-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.525297 translator_json-1.0.8/translator/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-25 05:08:07.000000 translator_json-1.0.8/translator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-25 05:08:19.525297 translator_json-1.0.8/translator/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-25 05:08:07.000000 translator_json-1.0.8/translator/translate_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.524297 translator_json-1.0.8/translator_json.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-06-25 05:08:07.000000 translator_json-1.0.8/versioneer.py
```

### Comparing `translator_json-1.0.7/PKG-INFO` & `translator_json-1.0.8/translator_json.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: translator_json
-Version: 1.0.7
+Name: translator-json
+Version: 1.0.8
 Summary: A translator for Json info
 Home-page: https://gitlab.com/FlorentSimonnot1/translator
 Author: Florent Simonnot
 Author-email: contact@gwanly.fr
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/FlorentSimonnot1/translator
 Platform: UNKNOWN
@@ -20,14 +20,19 @@
 
 When you create a multi language website, it's very long to translate all your sentences.
 
 With json_translator, you can translate a json file to many languages.
 
 The plugin will create the json file in according to the language you want to translate.
 
+google-cloud-translate==3.8.4
+google-auth==1.35.0
+google-api-core==2.8.0
+protobuf==3.19.5
+
 ## Pre required
 
 To use json_translator plugin you have to create a Google Cloud account.
 
 See : https://cloud.google.com
 
 Please verify in your apis dashboard that cloud translation API service is enable.
```

### Comparing `translator_json-1.0.7/README.md` & `translator_json-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 When you create a multi language website, it's very long to translate all your sentences.
 
 With json_translator, you can translate a json file to many languages.
 
 The plugin will create the json file in according to the language you want to translate.
 
+google-cloud-translate==3.8.4
+google-auth==1.35.0
+google-api-core==2.8.0
+protobuf==3.19.5
+
 ## Pre required
 
 To use json_translator plugin you have to create a Google Cloud account.
 
 See : https://cloud.google.com
 
 Please verify in your apis dashboard that cloud translation API service is enable.
```

### Comparing `translator_json-1.0.7/setup.py` & `translator_json-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `translator_json-1.0.7/translator_json.egg-info/PKG-INFO` & `translator_json-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: translator-json
-Version: 1.0.7
+Name: translator_json
+Version: 1.0.8
 Summary: A translator for Json info
 Home-page: https://gitlab.com/FlorentSimonnot1/translator
 Author: Florent Simonnot
 Author-email: contact@gwanly.fr
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/FlorentSimonnot1/translator
 Platform: UNKNOWN
@@ -20,14 +20,19 @@
 
 When you create a multi language website, it's very long to translate all your sentences.
 
 With json_translator, you can translate a json file to many languages.
 
 The plugin will create the json file in according to the language you want to translate.
 
+google-cloud-translate==3.8.4
+google-auth==1.35.0
+google-api-core==2.8.0
+protobuf==3.19.5
+
 ## Pre required
 
 To use json_translator plugin you have to create a Google Cloud account.
 
 See : https://cloud.google.com
 
 Please verify in your apis dashboard that cloud translation API service is enable.
```

### Comparing `translator_json-1.0.7/versioneer.py` & `translator_json-1.0.8/versioneer.py`

 * *Files identical despite different names*

