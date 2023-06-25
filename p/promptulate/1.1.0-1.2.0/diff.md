# Comparing `tmp/promptulate-1.1.0.tar.gz` & `tmp/promptulate-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptulate-1.1.0.tar", last modified: Fri Jun 23 10:54:56 2023, max compression
+gzip compressed data, was "promptulate-1.2.0.tar", last modified: Sun Jun 25 15:18:29 2023, max compression
```

## Comparing `promptulate-1.1.0.tar` & `promptulate-1.2.0.tar`

### file list

```diff
@@ -1,72 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 10:54:43.000000 promptulate-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-23 10:54:56.457353 promptulate-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-06-23 10:54:43.000000 promptulate-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate/command/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/command/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/react/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/self_ask/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/self_ask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/local_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/preset_roles/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/provider/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/arxiv/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/duckduckgo/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/promptulate/tools/python_repl/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/promptulate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/core_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/openai_key_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:54:56.457353 promptulate-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-23 10:54:43.000000 promptulate-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.147642 promptulate-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 15:18:17.000000 promptulate-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 15:18:29.147642 promptulate-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-25 15:18:17.000000 promptulate-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/command/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/react/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/self_ask/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/self_ask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/local_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/preset_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/provider/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/duckduckgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/paper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/paper/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/python_repl/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/semantic_scholar/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.147642 promptulate-1.2.0/promptulate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/openai_key_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:18:29.147642 promptulate-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-25 15:18:17.000000 promptulate-1.2.0/setup.py
```

### Comparing `promptulate-1.1.0/LICENSE` & `promptulate-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/__init__.py` & `promptulate-1.2.0/promptulate/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/command/chat.py` & `promptulate-1.2.0/promptulate/command/chat.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/config.py` & `promptulate-1.2.0/promptulate/config.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/__init__.py` & `promptulate-1.2.0/promptulate/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/conversation/__init__.py` & `promptulate-1.2.0/promptulate/frameworks/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/conversation/conversation.py` & `promptulate-1.2.0/promptulate/frameworks/conversation/conversation.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
-from pydantic import Field
 from typing import Optional, Union
 
+from pydantic import Field
+
 from promptulate import utils
 from promptulate.config import Config
+from promptulate.frameworks.schema import BasePromptFramework
 from promptulate.llms import OpenAI
 from promptulate.llms.base import BaseLLM
 from promptulate.memory import BufferChatMemory
 from promptulate.memory.base import BaseChatMemory
-from promptulate.utils.core_utils import record_time
-from promptulate.tips import EmptyChatMessageHistoryTip
 from promptulate.preset_roles.roles import CustomPresetRole, get_preset_role_prompt
 from promptulate.provider.mixins import (
     SummarizerMixin,
     TranslatorMixin,
     DeriveHistoryMessageMixin,
 )
-from promptulate.frameworks.schema import BasePromptFramework
 from promptulate.schema import (
     LLMPrompt,
     AssistantMessage,
     ChatMessageHistory,
     init_chat_message_history,
 )
+from promptulate.tips import EmptyChatMessageHistoryTip
+from promptulate.utils.core_utils import record_time
 
 CFG = Config()
 logger = utils.get_logger()
 
 
 class Conversation(
     BasePromptFramework, SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin
@@ -81,18 +82,16 @@
             messages_history.add_user_message(message=prompt)
         except EmptyChatMessageHistoryTip as e:
             messages_history = init_chat_message_history(
                 get_preset_role_prompt(self.role), prompt
             )
             self.conversation_id = messages_history.conversation_id
             self.memory.save_conversation_to_memory(messages_history)
-        logger.debug(f"[promptulate Conversation] {messages_history.messages}")
-        logger.info(
-            f"[promptulate Conversation] ask: {messages_history.messages[-1].content}"
+        logger.debug(
+            f"[promptulate Conversation] conversation_id: <{self.conversation_id}> messages: <{messages_history.messages}>"
         )
         answer: AssistantMessage = self.llm.generate_prompt(
             LLMPrompt(messages=messages_history.messages)
         )
-        logger.info(f"[promptulate Conversation] answer: {answer}")
         messages_history.messages.append(answer)
         self.memory.save_conversation_to_memory(messages_history)
         return answer.content
```

### Comparing `promptulate-1.1.0/promptulate/frameworks/prompt.py` & `promptulate-1.2.0/promptulate/frameworks/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/react/__init__.py` & `promptulate-1.2.0/promptulate/frameworks/react/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/schema.py` & `promptulate-1.2.0/promptulate/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/frameworks/self_ask/__init__.py` & `promptulate-1.2.0/promptulate/frameworks/self_ask/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/llms/__init__.py` & `promptulate-1.2.0/promptulate/llms/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,10 +15,8 @@
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
 from promptulate.llms.openai import OpenAI
 
-__all__ = [
-    'OpenAI',
-]
+__all__ = ["OpenAI"]
```

### Comparing `promptulate-1.1.0/promptulate/llms/base.py` & `promptulate-1.2.0/promptulate/llms/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
+from abc import ABC, abstractmethod
 from typing import Any
+
 from pydantic import BaseModel, Extra
-from abc import ABC, abstractmethod
-from promptulate.schema import AssistantMessage
-from promptulate.schema import LLMPrompt
+
+from promptulate.schema import AssistantMessage, LLMPrompt
 
 
 class BaseLLM(BaseModel, ABC):
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
```

### Comparing `promptulate-1.1.0/promptulate/llms/openai.py` & `promptulate-1.2.0/promptulate/llms/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import json
+from typing import Optional, Any, Dict, List
+
 import requests
-from typing import List, Optional, Any, Dict
 
 from promptulate.config import Config
-from promptulate.utils import get_logger
 from promptulate.llms.base import BaseLLM
 from promptulate.preset_roles.prompt import PRESET_SYSTEM_PROMPT_ZH
 from promptulate.schema import (
     LLMPrompt,
     UserMessage,
     SystemMessage,
     AssistantMessage,
+    parse_llm_prompt_to_dict,
 )
+from promptulate.utils.logger import get_logger
 
 CFG = Config()
 logger = get_logger()
 
 
 class OpenAI(BaseLLM):
     """https://platform.openai.com/docs/api-reference/chat/create"""
@@ -51,27 +54,27 @@
     preset_description: str = ""
     """OpenAI system message"""
     enable_private_api_key = False
     """Enable to provide a separate api for openai llm """
     private_api_key: str = ""
     """Store private api key"""
     # todo finish enable retry
-    enable_retry: bool = False
+    enable_retry: bool = True
     """Retry if API failed to get response. You can enable retry when you have a rate limited API."""
     retry_times: int = 5
     """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained. You should
     enable retry if you want to use retry times."""
     retry_counter: int = 0
     """Used in conjunction with retry_times. Refresh when get data successfully."""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.retry_times = CFG.get_key_retry_times(self.model)
 
-    def __call__(self, prompt, *args, **kwargs) -> str:
+    def __call__(self, prompt: str, *args, **kwargs) -> str:
         system_message = (
             self.preset_description
             if self.preset_description != ""
             else PRESET_SYSTEM_PROMPT_ZH
         )
         llm_prompt = LLMPrompt(
             messages=[
@@ -84,31 +87,32 @@
     def generate_prompt(self, prompts: LLMPrompt) -> Optional[AssistantMessage]:
         api_key = self.api_key
         logger.debug(f"[promptulate openai key] {api_key}")
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {api_key}",
         }
-        body: Dict[str, Any] = self._build_api_dict(prompts)
+        body: Dict[str, Any] = self._build_api_params_dict(prompts)
 
         logger.debug(f"[promptulate openai params] body {body}")
         logger.debug(
             f"[promptulate openai request] url: {CFG.openai_request_url} proxies: {CFG.proxies}"
         )
         response = requests.post(
             url=CFG.openai_request_url, headers=headers, json=body, proxies=CFG.proxies
         )
         if response.status_code == 200:
             # todo enable stream mode
             # for chunk in response.iter_content(chunk_size=None):
             #     logger.debug(chunk)
             self.retry_counter = 0
             ret_data = response.json()
-            logger.debug(f"[promptulate response] {ret_data}")
+            logger.debug(f"[promptulate openai response] {json.dumps(ret_data)}")
             content = ret_data["choices"][0]["message"]["content"]
+            logger.debug(f"[promptulate openai answer] {content}")
             return AssistantMessage(content=content)
 
         logger.error(
             "[promptulate OpenAI] Failed to get data. Please check your network or api key."
         )
         logger.debug("[promptulate OpenAI] retry to get response")
         if self.enable_retry and self.retry_counter < self.retry_times:
@@ -123,23 +127,18 @@
             return self.private_api_key
         return CFG.get_openai_api_key(self.model)
 
     def set_private_api_key(self, value: str):
         self.enable_private_api_key = True
         self.private_api_key = value
 
-    def _build_api_dict(self, prompts: LLMPrompt) -> Dict[str, Any]:
+    def _build_api_params_dict(self, prompts: LLMPrompt) -> Dict[str, Any]:
         dic = {
             "messages": self._parse_prompt(prompts),
         }
         for key in self.api_param_keys:
             if key in self.__dict__:
                 dic.update({key: self.__dict__[key]})
         return dic
 
     def _parse_prompt(self, prompts: LLMPrompt) -> List[Dict]:
-        converted_messages: List[dict] = []
-        for message in prompts.messages:
-            converted_messages.append(
-                {"role": message.type, "content": message.content}
-            )
-        return converted_messages
+        return parse_llm_prompt_to_dict(prompts)
```

### Comparing `promptulate-1.1.0/promptulate/memory/__init__.py` & `promptulate-1.2.0/promptulate/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/memory/base.py` & `promptulate-1.2.0/promptulate/memory/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/memory/buffer.py` & `promptulate-1.2.0/promptulate/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/memory/local_cache.py` & `promptulate-1.2.0/promptulate/memory/local_cache.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/preset_roles/__init__.py` & `promptulate-1.2.0/promptulate/preset_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/preset_roles/prompt.py` & `promptulate-1.2.0/promptulate/preset_roles/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/preset_roles/roles.py` & `promptulate-1.2.0/promptulate/preset_roles/roles.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/provider/__init__.py` & `promptulate-1.2.0/promptulate/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/provider/mixins.py` & `promptulate-1.2.0/promptulate/provider/mixins.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/tips.py` & `promptulate-1.2.0/promptulate/tips.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
-__all__ = [
-    'EmptyChatMessageHistoryTip'
-]
+__all__ = ["EmptyChatMessageHistoryTip", "NetWorkError"]
 
 
 class EmptyChatMessageHistoryTip(Exception):
     pass
+
+
+class NetWorkError(Exception):
+    def __init__(self, origin: str):
+        super().__init__(f"<{origin}> could not get data")
```

### Comparing `promptulate-1.1.0/promptulate/tools/arxiv/api_wrapper.py` & `promptulate-1.2.0/promptulate/tools/arxiv/api_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             Common fields are: ["entry_id", "title", "authors", "summary", "published"]
         """
         search = self._query(keyword, id_list, num_results)
         if "specified_fields" in kwargs:
             return ArxivQuerySet.from_filter_result(
                 search, *kwargs["specified_fields"]
             ).all()
-        if "from_callback" in kwargs and kwargs["from_callback"] == "ArxivQueryTool":
+        if "from_callback" in kwargs and kwargs["from_callback"] == "arxiv-query":
             keys = ["entry_id", "title", "authors", "summary"]
             return ArxivQuerySet.from_filter_result(search, *keys).all()
         return ArxivQuerySet(search).all()
 
     def download_pdf(self, id_list: List[str]) -> str:
         paper = next(arxiv.Search(id_list=id_list).results())
         return paper.download_pdf()
```

### Comparing `promptulate-1.1.0/promptulate/tools/arxiv/tools.py` & `promptulate-1.2.0/promptulate/tools/arxiv/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 import time
-from pydantic import BaseModel, Field
-from typing import List, Dict, Optional, Union, Tuple
+from typing import List, Dict, Union
+
 from broadcast_service import broadcast_service
+from pydantic import Field
 
 from promptulate.llms.base import BaseLLM
 from promptulate.llms.openai import OpenAI
-from promptulate.utils.logger import get_logger
-from promptulate.utils.core_utils import record_time, listdict_to_string
-from promptulate.tools.base import BaseTool
 from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
+from promptulate.tools.base import BaseTool
+from promptulate.utils.core_utils import record_time, listdict_to_string
+from promptulate.utils.logger import get_logger
 
 logger = get_logger()
 
 
 class ArxivQueryTool(BaseTool):
     name = "arxiv-query"
     description = (
@@ -22,24 +23,40 @@
         "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
         "Electrical Engineering, and Economics "
         "from scientific articles on arxiv.org. "
         "Input should be a search query."
     )
     api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
 
-    def run(self, query: str, *args, **kwargs) -> str:
+    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        """Arxiv query tool
+
+        Args:
+            query: the paper keyword or arxiv id
+            **kwargs:
+                return_type(Optional(str)):  return string default. If you want to return List[Dict] type data,
+                you can set 'return_type'='original'
+                Moreover, you can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type or List[Dict] arxiv query result.
+        """
         kwargs.update({"from_callback": self.name})
-        return listdict_to_string(
-            self.api_wrapper.query(query, **kwargs), is_wrap=False
-        )
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            result = self.api_wrapper.query(id_list=[query], **kwargs)
+        else:
+            result = self.api_wrapper.query(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return listdict_to_string(result)
+        return result
 
 
 def _init_arxiv_reference_tool_llm():
-    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，并且遵循用户的指令输出。"
-    return OpenAI(preset_description=preset)
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return OpenAI(preset_description=preset, temperature=0)
 
 
 class ArxivReferenceTool(BaseTool):
     name = "arxiv-reference"
     description = (
         "Use this tool to find search related to the field."
         "Your input is a arxiv keyword query."
@@ -56,15 +73,15 @@
         Args:
             query(str): arxiv paper information
             *args: Nothing
             **kwargs:
                 return_type(Optional[str]): return string default. If you want to return List[Dict] type data,
                 you can set 'return_type'='original'
         Returns:
-            string type reference information
+            String type or List[Dict] reference information
         """
 
         @broadcast_service.on_listen("ArxivReferenceTool.get_relevant_paper_info")
         @record_time()
         def get_relevant_paper_info(keyword: str):
             """return paper related information from keyword"""
             arxiv_query_tool = ArxivQueryTool()
@@ -87,99 +104,116 @@
             for match in re.finditer(pattern, reference_string):
                 references.append({"title": match.group(2), "url": match.group(3)})
             return references
 
         self.reference_counter = 0
         prompt = (
             f"现在你需要根据其研究的具体内容，列出至少{self.max_reference_num}篇参考文献，你可以使用arxiv进行查询，你需要给我提供3个arxiv查询关键词，我将使用"
-            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。你的输出必须是三个查询词。\n"
-            "如 [query]: keyword1, keyword2, keyword3\n"
+            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。"
             f"用户输入:{query}"
+            "你的输出必须是三个查询词\n，如 [query]: keyword1, keyword2, keyword3\n"
         )
         keywords = analyze_query_string(self.llm(prompt))
         for keyword in keywords:
             broadcast_service.broadcast(
                 "ArxivReferenceTool.get_relevant_paper_info", keyword
             )
 
         while self.reference_counter < 3:
             time.sleep(0.2)
 
         prompt = (
             "现在你需要根据下面给出的论文，返回最合适的5篇参考文献\n"
             f"```{self.reference_string}```\n"
-            "你的输出格式必须为\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);除此之外，不能输出任何其他内容。"
+            "你的输出格式必须为\n参考文献:\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);"
         )
         # todo If there is a problem with the returned format and an error is reported, then ask LLM to format the data
         result = self.llm(prompt)
         logger.debug(f"[promptulate ArxivReferenceTool response] {result}")
         if "return_type" in kwargs and kwargs["return_type"] == "original":
             return analyze_reference_string(result)
         return result
 
 
-class ArxivSummaryTool(BaseTool):
-    """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
+def _init_arxiv_summary_tool_llm():
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return OpenAI(preset_description=preset, temperature=0)
 
-    Return:
-        - Summary of the paper
-        - List the key insights and lessons learned in the paper
-        - List at least 5 references related to the research field of the paper
-    """
 
+class ArxivSummaryTool(BaseTool):
     name = "arxiv-summary"
     description = (
         "A summary tool that can be used to obtain a paper summary, listing "
         "key insights and lessons learned in the paper, and references in the paper"
         "Your input is a arxiv keyword query."
     )
-    llm: BaseLLM = Field(default_factory=OpenAI)
+    llm: BaseLLM = Field(default_factory=_init_arxiv_summary_tool_llm)
     api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
     summary_string: str = ""
     summary_counter: int = 0
 
-    def run(self, query: str, *args, **kwargs) -> str:
-        @broadcast_service.on_listen("ArxivSummaryTool.summary")
+    def run(self, query: str, **kwargs) -> str:
+        """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
+
+        Args:
+            query: the keyword you want to query
+            **kwargs:
+                You can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type data, which contains:
+            - Summary of the paper
+            - List the key insights and lessons learned in the paper
+            - List at least 5 references related to the research field of the paper
+        """
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_opinion")
         def get_opinion():
             prompt = (
                 f"请就下面的论文摘要，列出论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
                 "你的输出格式为:\n关键见解:\n{分点给出关键见解}\n经验教训:\n{分点给出经验教训}，用`-`区分每点，用中文输出"
             )
-
             opinion = self.llm(prompt)
             self.summary_string += opinion + "\n"
-            logger.debug(f"[ArxivSummaryTool summary] {self.summary_string}")
             self.summary_counter += 1
 
-        @broadcast_service.on_listen("ArxivSummaryTool.summary")
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_references")
         def get_references():
             arxiv_referencer_tool = ArxivReferenceTool()
             references = arxiv_referencer_tool.run(paper_summary)
-            self.summary_string += references + "\n"
-            logger.debug(f"[ArxivSummaryTool summary] {self.summary_string}")
+            self.summary_string += references + "\n\n"
             self.summary_counter += 1
 
-        @broadcast_service.on_listen("ArxivSummaryTool.summary")
-        def get_opinion():
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_advice")
+        def get_advice():
             prompt = (
                 f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
                 "你的输出格式为:\n相关建议:\n{分点给出相关建议}，用`-`区分每点"
             )
             opinion = self.llm(prompt)
             self.summary_string += opinion + "\n"
-            logger.debug(f"[ArxivSummaryTool summary] {self.summary_string}")
             self.summary_counter += 1
 
-        paper_summary = listdict_to_string(
-            self.api_wrapper.query(
+        self.summary_counter = 0
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            paper_info = self.api_wrapper.query(
+                id_list=[query], num_results=1, specified_fields=["title", "summary"]
+            )
+        else:
+            paper_info = self.api_wrapper.query(
                 query, num_results=1, specified_fields=["title", "summary"]
-            ),
-            item_suffix="\n",
-        )
+            )
+            if len(paper_info) == 0:
+                return "Could not find relevant arxiv article."
+        paper_summary = listdict_to_string(paper_info, item_suffix="\n")
         self.summary_string = paper_summary
-        logger.debug(f"[ArxivSummaryTool summary] {self.summary_string}")
-        broadcast_service.publish("ArxivSummaryTool.summary")
+
+        broadcast_service.publish("ArxivSummaryTool.run.get_references")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_opinion")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_advice")
 
         while self.summary_counter < 3:
-            time.sleep(0.2)
+            time.sleep(0.1)
 
         return self.summary_string
```

### Comparing `promptulate-1.1.0/promptulate/tools/base.py` & `promptulate-1.2.0/promptulate/tools/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/tools/duckduckgo/api_wrapper.py` & `promptulate-1.2.0/promptulate/tools/duckduckgo/api_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List, Union, Any, Optional, Dict
-from promptulate.tools.base import BaseTool
+from typing import List, Optional, Dict
 
 from pydantic import BaseModel, Extra
 from pydantic.class_validators import root_validator
 
 
 class DuckDuckGoSearchAPIWrapper(BaseModel):
     """Wrapper for DuckDuckGo Search API. Free and does not require any setup."""
+
     region: Optional[str] = "cn-zh"
     safe_search: str = "moderate"
     time: Optional[str] = "y"
     max_num_of_results: int = 5
 
     class Config:
         """Configuration for this pydantic object."""
@@ -25,15 +25,17 @@
         except ImportError:
             raise ValueError(
                 "Could not import duckduckgo-search python package. "
                 "Please install it with `pip install duckduckgo-search`."
             )
         return values
 
-    def query(self, keyword: str, num_results: Optional[int] = None, **kwargs) -> List[str]:
+    def query(
+            self, keyword: str, num_results: Optional[int] = None, **kwargs
+    ) -> List[str]:
         """Run query through DuckDuckGo and return concatenated results."""
         from duckduckgo_search import DDGS
 
         if not num_results:
             num_results = self.max_num_of_results
 
         with DDGS() as ddgs:
```

### Comparing `promptulate-1.1.0/promptulate/tools/duckduckgo/tools.py` & `promptulate-1.2.0/promptulate/tools/duckduckgo/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/tools/duckduckgo.py` & `promptulate-1.2.0/promptulate/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/tools/python_repl/api_wrapper.py` & `promptulate-1.2.0/promptulate/tools/python_repl/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/tools/python_repl/tools.py` & `promptulate-1.2.0/promptulate/tools/python_repl/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/utils/__init__.py` & `promptulate-1.2.0/promptulate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/utils/core_utils.py` & `promptulate-1.2.0/promptulate/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/utils/logger.py` & `promptulate-1.2.0/promptulate/utils/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,41 +13,38 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
-import os
-import logging
 import datetime
-import platform
+import logging
+import os
+
 from promptulate import utils
 
 logger = logging.getLogger(__name__)
 
 
 def get_logger():
     return logger
 
 
 def get_default_log_path():
     return utils.get_default_storage_path("log")
 
 
-def _check_log_path():
+def get_log_name() -> str:
     log_path = get_default_log_path()
     if not os.path.exists(log_path):
         os.makedirs(log_path)
 
-
-def get_log_name() -> str:
-    _check_log_path()
     cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    return f"{utils.get_default_storage_path()}/log/log_{cur_time}.log"
+    return f"{log_path}/log_{cur_time}.log"
 
 
 def enable_log(level=logging.DEBUG):
     logging.basicConfig(
         level=level,
         format="[%(levelname)s] %(asctime)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
```

### Comparing `promptulate-1.1.0/promptulate/utils/openai_key_pool.py` & `promptulate-1.2.0/promptulate/utils/openai_key_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def delete(self, key: str, model: Optional[str] = None):
         if model:
             openai_key: OpenAIKey = (
                 self.cache.query(OpenAIKey).filter(key=key, model=model).first()
             )
         else:
-            openai_key: OpenAIKey = self.cache.query(OpenAIKey).filter(key=key).all()
+            openai_key: List[OpenAIKey] = self.cache.query(OpenAIKey).filter(key=key).all()
         self.cache.delete(openai_key)
 
     def get_num(self, model: str) -> int:
         return len(self.cache.query(OpenAIKey).filter(model=model).all())
 
 
 def export_openai_key_pool(keys: List[Dict[str, str]]):
```

### Comparing `promptulate-1.1.0/promptulate/utils/proxy.py` & `promptulate-1.2.0/promptulate/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate/utils/singleton.py` & `promptulate-1.2.0/promptulate/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.1.0/promptulate.egg-info/SOURCES.txt` & `promptulate-1.2.0/promptulate.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,21 @@
 promptulate/tools/arxiv/__init__.py
 promptulate/tools/arxiv/api_wrapper.py
 promptulate/tools/arxiv/toolkit.py
 promptulate/tools/arxiv/tools.py
 promptulate/tools/duckduckgo/__init__.py
 promptulate/tools/duckduckgo/api_wrapper.py
 promptulate/tools/duckduckgo/tools.py
+promptulate/tools/paper/__init__.py
+promptulate/tools/paper/tools.py
 promptulate/tools/python_repl/__init__.py
 promptulate/tools/python_repl/api_wrapper.py
 promptulate/tools/python_repl/tools.py
+promptulate/tools/semantic_scholar/__init__.py
+promptulate/tools/semantic_scholar/api_wrapper.py
+promptulate/tools/semantic_scholar/tools.py
 promptulate/utils/__init__.py
 promptulate/utils/core_utils.py
 promptulate/utils/logger.py
 promptulate/utils/openai_key_pool.py
 promptulate/utils/proxy.py
 promptulate/utils/singleton.py
```

### Comparing `promptulate-1.1.0/setup.py` & `promptulate-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/promptulate
 # Contact Email: zeeland@foxmail.com
 
-import setuptools
 import pathlib
 
+import setuptools
+
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="promptulate",
-    version="1.1.0",
+    version="1.2.0",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A powerful LLM Prompt Layer frameworks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/promptulate",
     packages=setuptools.find_packages(),
```

