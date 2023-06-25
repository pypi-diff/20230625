# Comparing `tmp/speech_bot_helpers-0.1.0.tar.gz` & `tmp/speech_bot_helpers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_bot_helpers-0.1.0.tar", max compression
+gzip compressed data, was "speech_bot_helpers-0.1.1.tar", max compression
```

## Comparing `speech_bot_helpers-0.1.0.tar` & `speech_bot_helpers-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.1.0/README.md
--rw-r--r--   0        0        0      328 2023-06-25 11:26:44.675682 speech_bot_helpers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.1.0/speech_bot_helpers/__init__.py
--rw-r--r--   0        0        0       79 2023-06-25 11:34:06.560282 speech_bot_helpers-0.1.0/speech_bot_helpers/clients.py
--rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 speech_bot_helpers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.1.1/README.md
+-rw-r--r--   0        0        0      403 2023-06-25 12:16:40.106480 speech_bot_helpers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.1.1/speech_bot_helpers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-25 12:12:43.449535 speech_bot_helpers-0.1.1/speech_bot_helpers/clients.py
+-rw-r--r--   0        0        0       45 2023-06-25 11:57:14.602410 speech_bot_helpers-0.1.1/speech_bot_helpers/exceptions.py
+-rw-r--r--   0        0        0      638 2023-06-25 12:12:43.436940 speech_bot_helpers-0.1.1/speech_bot_helpers/wrappers.py
+-rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 speech_bot_helpers-0.1.1/PKG-INFO
```

