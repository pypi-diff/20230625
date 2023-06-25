# Comparing `tmp/speech_bot_helpers-0.2.2.tar.gz` & `tmp/speech_bot_helpers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_bot_helpers-0.2.2.tar", max compression
+gzip compressed data, was "speech_bot_helpers-0.2.3.tar", max compression
```

## Comparing `speech_bot_helpers-0.2.2.tar` & `speech_bot_helpers-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.2.2/README.md
--rw-r--r--   0        0        0      403 2023-06-25 14:08:45.845203 speech_bot_helpers-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.2.2/speech_bot_helpers/__init__.py
--rw-r--r--   0        0        0     2660 2023-06-25 12:12:43.449535 speech_bot_helpers-0.2.2/speech_bot_helpers/clients.py
--rw-r--r--   0        0        0       45 2023-06-25 11:57:14.602410 speech_bot_helpers-0.2.2/speech_bot_helpers/exceptions.py
--rw-r--r--   0        0        0      340 2023-06-25 14:07:27.538452 speech_bot_helpers-0.2.2/speech_bot_helpers/wrappers.py
--rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 speech_bot_helpers-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.2.3/README.md
+-rw-r--r--   0        0        0      421 2023-06-25 20:51:49.460386 speech_bot_helpers-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.2.3/speech_bot_helpers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-25 12:12:43.449535 speech_bot_helpers-0.2.3/speech_bot_helpers/clients.py
+-rw-r--r--   0        0        0       45 2023-06-25 11:57:14.602410 speech_bot_helpers-0.2.3/speech_bot_helpers/exceptions.py
+-rw-r--r--   0        0        0      490 2023-06-25 20:51:11.349830 speech_bot_helpers-0.2.3/speech_bot_helpers/wrappers.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 speech_bot_helpers-0.2.3/PKG-INFO
```

### Comparing `speech_bot_helpers-0.2.2/speech_bot_helpers/clients.py` & `speech_bot_helpers-0.2.3/speech_bot_helpers/clients.py`

 * *Files identical despite different names*

