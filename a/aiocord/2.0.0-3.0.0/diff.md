# Comparing `tmp/aiocord-2.0.0.tar.gz` & `tmp/aiocord-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocord-2.0.0.tar", last modified: Sun Jun 25 08:40:34 2023, max compression
+gzip compressed data, was "aiocord-3.0.0.tar", last modified: Sun Jun 25 08:43:07 2023, max compression
```

## Comparing `aiocord-2.0.0.tar` & `aiocord-3.0.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.497523 aiocord-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.481523 aiocord-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.485523 aiocord-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-25 08:40:23.000000 aiocord-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-25 08:40:23.000000 aiocord-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 08:40:23.000000 aiocord-2.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 08:40:23.000000 aiocord-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-25 08:40:34.497523 aiocord-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-25 08:40:23.000000 aiocord-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.485523 aiocord-2.0.0/aiocord/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   264433 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.489523 aiocord-2.0.0/aiocord/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/gateway/vital.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.489523 aiocord-2.0.0/aiocord/http/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/http/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/http/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34793 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/http/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/aiocord/model/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29482 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)   208686 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/aiocord/voice/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/voice/vital.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-25 08:40:23.000000 aiocord-2.0.0/aiocord/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.489523 aiocord-2.0.0/aiocord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 08:40:34.000000 aiocord-2.0.0/aiocord.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/_static/images/github-mark-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/_static/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/_templates/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.493523 aiocord-2.0.0/docs/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:40:34.497523 aiocord-2.0.0/docs/pages/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/interact.naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/interact.smart.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/voice.data.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/voice.file.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-25 08:40:23.000000 aiocord-2.0.0/docs/pages/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:40:34.497523 aiocord-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 08:40:23.000000 aiocord-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.478567 aiocord-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.470567 aiocord-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.470567 aiocord-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-25 08:42:55.000000 aiocord-3.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-25 08:42:55.000000 aiocord-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 08:42:55.000000 aiocord-3.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 08:42:55.000000 aiocord-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-25 08:43:07.478567 aiocord-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-25 08:42:55.000000 aiocord-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.470567 aiocord-3.0.0/aiocord/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264433 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/aiocord/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/gateway/vital.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/aiocord/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/http/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34793 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/http/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/aiocord/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29482 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208686 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/aiocord/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/voice/vital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-25 08:42:55.000000 aiocord-3.0.0/aiocord/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.470567 aiocord-3.0.0/aiocord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 08:43:07.000000 aiocord-3.0.0/aiocord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/_static/images/github-mark-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/_static/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/_templates/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:43:07.474567 aiocord-3.0.0/docs/pages/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/interact.naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/interact.smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/voice.data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/voice.file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-25 08:42:55.000000 aiocord-3.0.0/docs/pages/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:43:07.478567 aiocord-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 08:42:55.000000 aiocord-3.0.0/setup.py
```

### Comparing `aiocord-2.0.0/.github/workflows/publish.yml` & `aiocord-3.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/.gitignore` & `aiocord-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/LICENSE` & `aiocord-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/PKG-INFO` & `aiocord-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocord
-Version: 2.0.0
+Version: 3.0.0
 Summary: A modern API wrapper for Discord.
 Home-page: https://github.com/Exahilosys/aiocord
 License: MIT
 Requires: yarl    (>= 1.9.1, < 2.0.0)
 Requires: aiohttp (>= 3.8.4, < 4.0.0)
 Requires: vessel  (>= 4.2.0, < 5.0.0)
 Requires: pynacl  (>= 1.5.0, < 2.0.0)
```

### Comparing `aiocord-2.0.0/README.rst` & `aiocord-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/client.py` & `aiocord-3.0.0/aiocord/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/enums.py` & `aiocord-3.0.0/aiocord/enums.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/events.py` & `aiocord-3.0.0/aiocord/events.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/gateway/client.py` & `aiocord-3.0.0/aiocord/gateway/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/gateway/errors.py` & `aiocord-3.0.0/aiocord/gateway/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/gateway/vital.py` & `aiocord-3.0.0/aiocord/gateway/vital.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/helpers.py` & `aiocord-3.0.0/aiocord/helpers.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/http/client.py` & `aiocord-3.0.0/aiocord/http/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/http/errors.py` & `aiocord-3.0.0/aiocord/http/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/http/helpers.py` & `aiocord-3.0.0/aiocord/http/helpers.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/http/routes.py` & `aiocord-3.0.0/aiocord/http/routes.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/enums.py` & `aiocord-3.0.0/aiocord/model/enums.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/images.py` & `aiocord-3.0.0/aiocord/model/images.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/mentions.py` & `aiocord-3.0.0/aiocord/model/mentions.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/objects.py` & `aiocord-3.0.0/aiocord/model/objects.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/protocols.py` & `aiocord-3.0.0/aiocord/model/protocols.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/responses.py` & `aiocord-3.0.0/aiocord/model/responses.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/model/types.py` & `aiocord-3.0.0/aiocord/model/types.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/utils.py` & `aiocord-3.0.0/aiocord/utils.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/vendor.py` & `aiocord-3.0.0/aiocord/vendor.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/audio.py` & `aiocord-3.0.0/aiocord/voice/audio.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/client.py` & `aiocord-3.0.0/aiocord/voice/client.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/errors.py` & `aiocord-3.0.0/aiocord/voice/errors.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/player.py` & `aiocord-3.0.0/aiocord/voice/player.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/stream.py` & `aiocord-3.0.0/aiocord/voice/stream.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/voice/vital.py` & `aiocord-3.0.0/aiocord/voice/vital.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord/widget.py` & `aiocord-3.0.0/aiocord/widget.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/aiocord.egg-info/PKG-INFO` & `aiocord-3.0.0/aiocord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocord
-Version: 2.0.0
+Version: 3.0.0
 Summary: A modern API wrapper for Discord.
 Home-page: https://github.com/Exahilosys/aiocord
 License: MIT
 Requires: yarl    (>= 1.9.1, < 2.0.0)
 Requires: aiohttp (>= 3.8.4, < 4.0.0)
 Requires: vessel  (>= 4.2.0, < 5.0.0)
 Requires: pynacl  (>= 1.5.0, < 2.0.0)
```

### Comparing `aiocord-2.0.0/aiocord.egg-info/SOURCES.txt` & `aiocord-3.0.0/aiocord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/Makefile` & `aiocord-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/_static/images/github-mark-white.png` & `aiocord-3.0.0/docs/_static/images/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/_static/main.css` & `aiocord-3.0.0/docs/_static/main.css`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/_templates/layout.html` & `aiocord-3.0.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/conf.py` & `aiocord-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/index.rst` & `aiocord-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/make.bat` & `aiocord-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples/interact.naive.py` & `aiocord-3.0.0/docs/pages/examples/interact.naive.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples/interact.smart.py` & `aiocord-3.0.0/docs/pages/examples/interact.smart.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples/voice.data.py` & `aiocord-3.0.0/docs/pages/examples/voice.data.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples/voice.file.py` & `aiocord-3.0.0/docs/pages/examples/voice.file.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples/widget.py` & `aiocord-3.0.0/docs/pages/examples/widget.py`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/examples.rst` & `aiocord-3.0.0/docs/pages/examples.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/docs/pages/reference.rst` & `aiocord-3.0.0/docs/pages/reference.rst`

 * *Files identical despite different names*

### Comparing `aiocord-2.0.0/setup.py` & `aiocord-3.0.0/setup.py`

 * *Files identical despite different names*

