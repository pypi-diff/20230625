# Comparing `tmp/Pytdbot-0.8.4.dev2.tar.gz` & `tmp/Pytdbot-0.8.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytdbot-0.8.4.dev2.tar", last modified: Sat Jun 17 15:10:04 2023, max compression
+gzip compressed data, was "Pytdbot-0.8.4.dev3.tar", last modified: Sun Jun 25 06:41:56 2023, max compression
```

## Comparing `Pytdbot-0.8.4.dev2.tar` & `Pytdbot-0.8.4.dev3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 15:10:04.000000 Pytdbot-0.8.4.dev2/Pytdbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/pytdbot/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.530447 Pytdbot-0.8.4.dev2/pytdbot/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/generate_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   146553 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/handlers/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/methods/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57920 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/methods/tdlibfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/td_api.json
--rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/td_api.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/tdjson/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/tdjson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/tdjson/tdjson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/inline_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/remove_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/buttons/show_keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/result/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/result/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.534447 Pytdbot-0.8.4.dev2/pytdbot/types/update/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/chatActions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60488 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/types/update/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/pytdbot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/pytdbot/utils/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:10:04.538447 Pytdbot-0.8.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-17 15:10:02.000000 Pytdbot-0.8.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.629406 Pytdbot-0.8.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-25 06:41:56.629406 Pytdbot-0.8.4.dev3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.609406 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-25 06:41:56.000000 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-25 06:41:56.000000 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:41:56.000000 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 06:41:56.000000 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 06:41:56.000000 Pytdbot-0.8.4.dev3/Pytdbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.613406 Pytdbot-0.8.4.dev3/pytdbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42975 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.613406 Pytdbot-0.8.4.dev3/pytdbot/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/generate_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.613406 Pytdbot-0.8.4.dev3/pytdbot/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/handlers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146553 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/handlers/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.617406 Pytdbot-0.8.4.dev3/pytdbot/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57920 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/methods/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   444864 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/methods/tdlibfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1248427 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/td_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)   585705 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/td_api.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.617406 Pytdbot-0.8.4.dev3/pytdbot/tdjson/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/tdjson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/tdjson/tdjson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.617406 Pytdbot-0.8.4.dev3/pytdbot/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.621406 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/inline_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/remove_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/buttons/show_keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.621406 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.625406 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/log_stream_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/log_stream_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/logstream/log_stream_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.625406 Pytdbot-0.8.4.dev3/pytdbot/types/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.625406 Pytdbot-0.8.4.dev3/pytdbot/types/result/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/result/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.629406 Pytdbot-0.8.4.dev3/pytdbot/types/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/update/chatActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60488 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/types/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:41:56.629406 Pytdbot-0.8.4.dev3/pytdbot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/pytdbot/utils/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:41:56.629406 Pytdbot-0.8.4.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-25 06:41:54.000000 Pytdbot-0.8.4.dev3/setup.py
```

### Comparing `Pytdbot-0.8.4.dev2/LICENSE` & `Pytdbot-0.8.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/PKG-INFO` & `Pytdbot-0.8.4.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev2
+Version: 0.8.4.dev3
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
@@ -32,18 +32,19 @@
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
 
 ### Installation
 > For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
+You can install Pytdbot using pip:
 ```bash
 pip install pytdbot
 ```
-From github (dev version)
+To install the development version from Github, use the following command:
 ```bash
 pip install git+https://github.com/pytdbot/client.git
 ```
 
 ### Examples
 Basic example:
 ```python
```

### Comparing `Pytdbot-0.8.4.dev2/Pytdbot.egg-info/PKG-INFO` & `Pytdbot-0.8.4.dev3/Pytdbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytdbot
-Version: 0.8.4.dev2
+Version: 0.8.4.dev3
 Summary: Easy-to-use asynchronous TDLib wrapper for Python.
 Home-page: https://github.com/pytdbot/client
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/pytdbot/client
 Project-URL: Tracker, https://github.com/pytdbot/client/issues
@@ -32,18 +32,19 @@
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
 
 ### Installation
 > For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
+You can install Pytdbot using pip:
 ```bash
 pip install pytdbot
 ```
-From github (dev version)
+To install the development version from Github, use the following command:
 ```bash
 pip install git+https://github.com/pytdbot/client.git
 ```
 
 ### Examples
 Basic example:
 ```python
```

### Comparing `Pytdbot-0.8.4.dev2/Pytdbot.egg-info/SOURCES.txt` & `Pytdbot-0.8.4.dev3/Pytdbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/README.md` & `Pytdbot-0.8.4.dev3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 - Telegram [API key](https://my.telegram.org/apps)
 - [tdjson](https://github.com/tdlib/td#building)
 - [deepdiff](https://github.com/seperman/deepdiff)
 
 ### Installation
 > For better performance, it's recommended to install [orjson](https://github.com/ijl/orjson#install) or [ujson](https://github.com/ultrajson/ultrajson#ultrajson).
 
+You can install Pytdbot using pip:
 ```bash
 pip install pytdbot
 ```
-From github (dev version)
+To install the development version from Github, use the following command:
 ```bash
 pip install git+https://github.com/pytdbot/client.git
 ```
 
 ### Examples
 Basic example:
 ```python
```

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/client.py` & `Pytdbot-0.8.4.dev3/pytdbot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from getpass import getpass
 from importlib import import_module
 
 from typing import Callable, Union
 from logging import getLogger, DEBUG
 from base64 import b64encode
 from deepdiff import DeepDiff
-from concurrent.futures import ThreadPoolExecutor
-from threading import current_thread, main_thread
+from threading import current_thread, main_thread, Thread
 from json import dumps
 
 from .tdjson import TdJson
 from .handlers import Decorators, Handler
 from .methods import Methods
 from .types import Plugins, Result, LogStream, Update
 from .filters import Filter
@@ -90,15 +89,15 @@
             Pass key-value dictionary to set TDLib options. Check the list of available options at https://core.telegram.org/tdlib/options
 
         sleep_threshold (``int``, *optional*):
             Sleep threshold for all ``FLOOD_WAIT_X`` a.k.a ``Too Many Requests: retry after`` errors occur to this client.
             If any request is rate limited (flood waited) the client will repeat the request after sleeping the required amount of seconds returned by the error. If the ``retry after`` value is higher than ``sleep_threshold`` the error is returned. Defaults to ``None`` (Disabled)
 
         workers (``int``, *optional*):
-            Number of workers for handling updates. Defaults to ``5``
+            Number of workers to handle updates. Defaults to ``5``. If set to ``None``, updates will be immediately handled instead of being queued, which can impact performance.
 
         td_verbosity (``int``, *optional*):
             Verbosity level of TDLib. Defaults to ``2``
 
         td_log (:class:`~pytdbot.types.LogStream`, *optional*):
             Log stream. Defaults to ``None`` (Log to ``stdout``)
     """
@@ -136,15 +135,15 @@
         self.files_directory = files_directory
         self.lib_path = lib_path
         self.plugins = plugins
         self.update_class = update_class
         self.default_parse_mode = (
             default_parse_mode
             if isinstance(default_parse_mode, str)
-            and default_parse_mode in ["markdown", "markdownv2", "html"]
+            and default_parse_mode in ("markdown", "markdownv2", "html")
             else None
         )
         self.system_language_code = system_language_code
         self.device_model = device_model
         self.use_test_dc = use_test_dc
         self.use_file_database = use_file_database
         self.use_chat_info_database = use_chat_info_database
@@ -165,17 +164,17 @@
         self.options = {}
 
         self._check_init_args()
 
         self._handlers = {"initializer": [], "finalizer": []}
         self._results = {}
         self._tdjson = TdJson(lib_path, td_verbosity)
-        self._executor = ThreadPoolExecutor(5, "Pytdbot")
-        self._workers_tasks = None
         self._retry_after_prefex = "Too Many Requests: retry after "
+        self._workers_tasks = None
+        self.__listen_loop_thread = Thread(target=self.__listen_loop, daemon=True)
         self.__authorization_state = None
         self.__authorization = None
         self.__cache = {"is_coro_filter": {}}
         self.__login = False
         self.__is_closing = False
 
         self.loop = (
@@ -214,35 +213,40 @@
         Args:
             login (``bool``, *optional*):
                 Login after start. Defaults to ``True``
         """
         if not self.is_running:
             logger.info("Starting pytdbot client...")
 
-            self._workers_tasks = [
-                self.loop.create_task(self._update_worker(x + 1))
-                for x in range(self.workers)
-            ]
+            if isinstance(self.workers, int):
+                self._workers_tasks = [
+                    self.loop.create_task(self._queue_update_worker())
+                    for x in range(self.workers)
+                ]
+                self.__is_queue_worker = True
 
-            logger.info("Started with %s workers", self.workers)
+                logger.info("Started with %s workers", self.workers)
+            else:
+                self.__is_queue_worker = False
+                logger.info("Started with unlimited updates processes")
 
-            self.loop.create_task(self.__listen_loop())
+            self.__listen_loop_thread.start()
 
         if login:
             await self.login()
 
     async def login(self) -> None:
         """Login to Telegram."""
 
         if self.is_authenticated:
             return
 
         self.__login = True
 
-        await self.getOption("version")  # Ping TDLib to start authorization proccess
+        await self.getOption("version")  # Ping TDLib to start authorization process
 
         while self.authorization_state != "authorizationStateReady":
             await asyncio.sleep(0.1)
             if self.authorization_state == "authorizationStateClosed":
                 return
 
         if not self.is_running:
@@ -499,42 +503,35 @@
             logger.info("Instance closed")
 
             return True
 
     def __send(self, request: dict) -> None:
         return self._tdjson.send(
             request
-        )  # tdjson.send is asynchronous, So we don't need run_in_executor. This improves performance
-
-    async def __receive(self, timeout: float = 2.0) -> dict:
-        return await self.loop.run_in_executor(
-            self._executor, self._tdjson.receive, timeout
-        )
+        )  # tdjson.send is non-blocking method, So we don't need run_in_executor. This improves performance
 
     def _check_init_args(self):
         if not isinstance(self.__api_id, int):
             raise TypeError("api_id must be int")
         elif not isinstance(self.__api_hash, str):
             raise TypeError("api_hash must be str")
         elif not isinstance(self.__database_encryption_key, str) and not isinstance(
             self.__database_encryption_key, bytes
         ):
             raise TypeError("database_encryption_key must be str or bytes")
         elif not isinstance(self.files_directory, str):
             raise TypeError("files_directory must be str")
         elif not isinstance(self.td_verbosity, int):
             raise TypeError("td_verbosity must be int")
-        elif not isinstance(self.workers, int):
-            raise TypeError("workers must be int")
         elif type(Update) is not type(self.update_class):
             raise TypeError(
                 "update_class must be instance of class pytdbot.types.Update"
             )
 
-        if self.workers < 1:
+        if isinstance(self.workers, int) and self.workers < 1:
             raise ValueError("workers must be greater than 0")
 
     def get_retry_after_time(self, error_message: str) -> int:
         """Get the retry after time from flood wait error message
 
         Args:
             error_message (``str``):
@@ -585,21 +582,21 @@
         if func in self.__cache["is_coro_filter"]:
             return self.__cache["is_coro_filter"][func]
         else:
             is_coro = asyncio.iscoroutinefunction(func)
             self.__cache["is_coro_filter"][func] = is_coro
             return is_coro
 
-    async def __listen_loop(self):
+    def __listen_loop(self):
         try:
             self.is_running = True
             logger.info("Listening to updates...")
 
             while self.is_running:
-                update = await self.__receive(100000.0)  # seconds
+                update = self._tdjson.receive(100000.0)  # seconds
                 if update is None:
                     continue
                 self._process_update(update)
 
         except Exception:
             logger.exception("Exception in __listen_loop")
         finally:
@@ -620,27 +617,44 @@
             if update["@extra"]["id"] in self._results:
                 result: Result = self._results.pop(update["@extra"]["id"])
                 result.set_result(update)
             elif update["@type"] == "error" and "option" in update["@extra"]:
                 logger.error(f"{update['@extra']['option']}: {update['message']}")
         else:
             if update["@type"] == "updateAuthorizationState":
-                self.loop.create_task(self.__handle_authorization_state(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_authorization_state(update), loop=self.loop
+                )
             elif update["@type"] == "updateMessageSendSucceeded":
-                self.loop.create_task(self.__handle_update_message_succeeded(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_update_message_succeeded(update), loop=self.loop
+                )
             elif update["@type"] == "updateMessageSendFailed":
-                self.loop.create_task(self.__handle_update_message_failed(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_update_message_failed(update), loop=self.loop
+                )
             elif update["@type"] == "updateConnectionState":
-                self.loop.create_task(self.__handle_connection_state(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_connection_state(update), loop=self.loop
+                )
             elif update["@type"] == "updateOption":
-                self.loop.create_task(self.__handle_update_option(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_update_option(update), loop=self.loop
+                )
             elif update["@type"] == "updateUser":
-                self.loop.create_task(self.__handle_update_user(update))
+                asyncio.run_coroutine_threadsafe(
+                    self.__handle_update_user(update), loop=self.loop
+                )
 
-            self.queue.put_nowait(update)
+            if self.__is_queue_worker:
+                self.queue.put_nowait(update)
+            else:
+                asyncio.run_coroutine_threadsafe(
+                    self._handle_update(update), loop=self.loop
+                )
 
     async def __run_initializers(self, update):
         for initializer in self._handlers["initializer"]:
             try:
                 if initializer.filter is not None:
                     filter_func = initializer.filter.func
 
@@ -688,47 +702,43 @@
 
                 await finalizer.func(self, update)
             except StopHandlers as e:
                 raise e
             except Exception:
                 logger.exception(f"Finalizer {finalizer} failed")
 
-    async def _update_worker(self, worker_id: int):
-        self.is_running = True
-        while self.is_running:
-            try:
-                update = await self.queue.get()
-                if "@type" not in update:
-                    continue
+    async def _handle_update(self, update):
+        if (
+            logger.root.level >= DEBUG
+        ):  # dumping all updates can create performance issues
+            logger.debug(
+                f"Received: {dumps(update, indent=4)}",
+            )
 
-                if (
-                    logger.root.level >= DEBUG
-                ):  # dumping all updates can create performance issues
-                    logger.debug(
-                        f"w{worker_id}: Received: {dumps(update, indent=4)}",
-                    )
+        if update["@type"] in self._handlers:
+            update = self.update_class(self, update)
+            if (
+                update["@type"] == "updateNewMessage"
+                and update["message"]["is_outgoing"]
+                and "sending_state" in update["message"]
+            ):
+                return
 
-                if update["@type"] in self._handlers:
-                    update = self.update_class(self, update)
-                    if (
-                        update["@type"] == "updateNewMessage"
-                        and update["message"]["is_outgoing"]
-                        and "sending_state" in update["message"]
-                    ):
-                        continue
+            try:
+                await self.__run_initializers(update)
+                await self.__run_handlers(update)
+            except StopHandlers:
+                pass
+            finally:
+                await self.__run_finalizers(update)
 
-                    try:
-                        await self.__run_initializers(update)
-                        await self.__run_handlers(update)
-                    except StopHandlers:
-                        pass
-                    finally:
-                        await self.__run_finalizers(update)
-            except Exception:
-                logger.exception("Exception in _update_worker")
+    async def _queue_update_worker(self):
+        self.is_running = True
+        while self.is_running:
+            await self._handle_update(await self.queue.get())
 
     async def set_td_paramaters(self):
         """Make a call to :meth:`~pytdbot.Client.setTdlibParameters` with the current client init parameters
 
         Raises:
             `AuthorizationError`
         """
@@ -1010,16 +1020,15 @@
         if self.authorization_state != "authorizationStateWaitPassword":
             return
 
         if self.__authorization["password_hint"]:
             print(f"Your 2FA password hint is: {self.__authorization['password_hint']}")
 
         while self.is_running:
-            password = await self.loop.run_in_executor(
-                self._executor,
+            password = await asyncio.to_thread(
                 getpass,
                 "Enter your 2FA password {}: ".format(
                     "(empty to recover)"
                     if self.__authorization["has_recovery_email_address"]
                     else ""
                 ),
             )
@@ -1070,18 +1079,17 @@
                 else:
                     break
 
     def __stop_client(self) -> None:
         self.is_authenticated = False
         self.is_running = False
 
-        for worker_task in self._workers_tasks:
-            worker_task.cancel()
-
-        self._executor.shutdown(wait=False, cancel_futures=True)
+        if self.__is_queue_worker:
+            for worker_task in self._workers_tasks:
+                worker_task.cancel()
 
     def _register_signal_handlers(self):
         def _handle_signal():
             self.loop.create_task(self.stop())
             for sig in (
                 signal.SIGINT,
                 signal.SIGTERM,
@@ -1099,15 +1107,15 @@
                     signal.SIGSEGV,
                 ):
                     self.loop.add_signal_handler(sig, _handle_signal)
             except NotImplementedError:  # Windows dosen't support add_signal_handler
                 pass
 
     def __ainput(self, prompt: str):
-        return self.loop.run_in_executor(self._executor, input, prompt)
+        return asyncio.to_thread(input, prompt)
 
     def _print_welcome(self):
         print(f"Welcome to Pytdbot (v{pytdbot.__version__}). {pytdbot.__copyright__}")
         print(
             f"Pytdbot is free software and comes with ABSOLUTELY NO WARRANTY. Licensed under the terms of {pytdbot.__license__}.\n\n"
         )
```

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/filters.py` & `Pytdbot-0.8.4.dev3/pytdbot/filters.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/generate_files.py` & `Pytdbot-0.8.4.dev3/pytdbot/generate_files.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/generate_json.py` & `Pytdbot-0.8.4.dev3/pytdbot/generate_json.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/handlers/decorators.py` & `Pytdbot-0.8.4.dev3/pytdbot/handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/handlers/handler.py` & `Pytdbot-0.8.4.dev3/pytdbot/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/handlers/updates.py` & `Pytdbot-0.8.4.dev3/pytdbot/handlers/updates.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/methods/methods.py` & `Pytdbot-0.8.4.dev3/pytdbot/methods/methods.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/methods/tdlibfunctions.py` & `Pytdbot-0.8.4.dev3/pytdbot/methods/tdlibfunctions.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/td_api.json` & `Pytdbot-0.8.4.dev3/pytdbot/td_api.json`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/td_api.tl` & `Pytdbot-0.8.4.dev3/pytdbot/td_api.tl`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/tdjson/tdjson.py` & `Pytdbot-0.8.4.dev3/pytdbot/tdjson/tdjson.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/__init__.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/force_reply.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/buttons/force_reply.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/inline_keyboard.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/buttons/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/remove_keyboard.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/buttons/remove_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/buttons/show_keyboard.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/buttons/show_keyboard.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_generated.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_generated.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_local.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_local.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_file_remote.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_file_remote.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/inputfile/input_thumbnail.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/inputfile/input_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/logstream/log_stream_file.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/logstream/log_stream_file.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/result/result.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/result/result.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/update/chatActions.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/update/chatActions.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/types/update/update.py` & `Pytdbot-0.8.4.dev3/pytdbot/types/update/update.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/utils/escape.py` & `Pytdbot-0.8.4.dev3/pytdbot/utils/escape.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/pytdbot/utils/text_format.py` & `Pytdbot-0.8.4.dev3/pytdbot/utils/text_format.py`

 * *Files identical despite different names*

### Comparing `Pytdbot-0.8.4.dev2/setup.py` & `Pytdbot-0.8.4.dev3/setup.py`

 * *Files identical despite different names*

