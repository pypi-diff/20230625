# Comparing `tmp/vcorelib-2.0.0.tar.gz` & `tmp/vcorelib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-2.0.0.tar", last modified: Wed Jun 21 07:45:27 2023, max compression
+gzip compressed data, was "vcorelib-2.0.1.tar", last modified: Sun Jun 25 00:55:37 2023, max compression
```

## Comparing `vcorelib-2.0.0.tar` & `vcorelib-2.0.1.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.932766 vcorelib-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 07:44:04.000000 vcorelib-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-21 07:45:27.932766 vcorelib-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-21 07:44:04.000000 vcorelib-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-21 07:44:04.000000 vcorelib-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:45:27.932766 vcorelib-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 07:44:04.000000 vcorelib-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.920765 vcorelib-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-21 07:44:04.000000 vcorelib-2.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 07:44:04.000000 vcorelib-2.0.0/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-21 07:44:04.000000 vcorelib-2.0.0/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.920765 vcorelib-2.0.0/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.928765 vcorelib-2.0.0/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.932766 vcorelib-2.0.0/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-21 07:44:04.000000 vcorelib-2.0.0/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:45:27.924765 vcorelib-2.0.0/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-21 07:45:27.000000 vcorelib-2.0.0/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-21 07:45:27.000000 vcorelib-2.0.0/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:45:27.000000 vcorelib-2.0.0/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:45:27.000000 vcorelib-2.0.0/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 07:45:27.000000 vcorelib-2.0.0/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 00:54:18.000000 vcorelib-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-25 00:55:37.791426 vcorelib-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-25 00:54:18.000000 vcorelib-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 00:54:18.000000 vcorelib-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 00:55:37.791426 vcorelib-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-25 00:54:18.000000 vcorelib-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.783426 vcorelib-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-25 00:54:18.000000 vcorelib-2.0.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-25 00:54:18.000000 vcorelib-2.0.1/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-25 00:54:18.000000 vcorelib-2.0.1/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.783426 vcorelib-2.0.1/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.791426 vcorelib-2.0.1/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-25 00:54:18.000000 vcorelib-2.0.1/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:55:37.787426 vcorelib-2.0.1/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-25 00:55:37.000000 vcorelib-2.0.1/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-25 00:55:37.000000 vcorelib-2.0.1/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:55:37.000000 vcorelib-2.0.1/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-25 00:55:37.000000 vcorelib-2.0.1/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 00:55:37.000000 vcorelib-2.0.1/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-2.0.0/LICENSE` & `vcorelib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/PKG-INFO` & `vcorelib-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.0.0
+Version: 2.0.1
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e2335154489804baac80ff4fa5703aed
+    hash=b62c8c800bcc6195e61d7492ca560a0e
     =====================================
 -->
 
-# vcorelib ([2.0.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.0.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
 
@@ -43,15 +42,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vcorelib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vcorelib-2.0.0/README.md` & `vcorelib-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e2335154489804baac80ff4fa5703aed
+    hash=b62c8c800bcc6195e61d7492ca560a0e
     =====================================
 -->
 
-# vcorelib ([2.0.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.0.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
 
@@ -19,15 +19,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vcorelib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vcorelib-2.0.0/pyproject.toml` & `vcorelib-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "2.0.0"
+version = "2.0.1"
 description = "A collection of core Python utilities."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
```

### Comparing `vcorelib-2.0.0/setup.py` & `vcorelib-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=2f5e369319178caaf8b067b6862054a7
+# hash=aa3f8de4be97b3a228df7e69c5398da6
 # =====================================
 
 """
 vcorelib - Package definition for distribution.
 """
 
 # third-party
@@ -24,15 +24,14 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.7",
         "3.8",
         "3.9",
         "3.10",
         "3.11",
     ],
 }
 setup(
```

### Comparing `vcorelib-2.0.0/tests/test_logging.py` & `vcorelib-2.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/tests/test_names.py` & `vcorelib-2.0.1/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/tests/test_namespace.py` & `vcorelib-2.0.1/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/args/__init__.py` & `vcorelib-2.0.1/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/args/newline.py` & `vcorelib-2.0.1/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/asyncio/__init__.py` & `vcorelib-2.0.1/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/asyncio/cli.py` & `vcorelib-2.0.1/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/asyncio/subprocess.py` & `vcorelib-2.0.1/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/dict/__init__.py` & `vcorelib-2.0.1/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/dict/cache.py` & `vcorelib-2.0.1/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/dict/codec.py` & `vcorelib-2.0.1/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/dict/config.py` & `vcorelib-2.0.1/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/dict/env.py` & `vcorelib-2.0.1/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/graph/__init__.py` & `vcorelib-2.0.1/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/graph/abc.py` & `vcorelib-2.0.1/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/graph/edge.py` & `vcorelib-2.0.1/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/graph/node.py` & `vcorelib-2.0.1/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/graph/port.py` & `vcorelib-2.0.1/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/__init__.py` & `vcorelib-2.0.1/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/abc.py` & `vcorelib-2.0.1/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/arbiter/base.py` & `vcorelib-2.0.1/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/arbiter/context.py` & `vcorelib-2.0.1/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/arbiter/directory.py` & `vcorelib-2.0.1/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/archive/__init__.py` & `vcorelib-2.0.1/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/cache.py` & `vcorelib-2.0.1/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/decode.py` & `vcorelib-2.0.1/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/encode.py` & `vcorelib-2.0.1/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/mapping.py` & `vcorelib-2.0.1/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/io/types.py` & `vcorelib-2.0.1/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/logging.py` & `vcorelib-2.0.1/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/math/__init__.py` & `vcorelib-2.0.1/vcorelib/math/unit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Math utilities.
+A module for working with units.
 """
 
 # built-in
 import typing
 
 
 class UnitSystem(typing.NamedTuple):
```

### Comparing `vcorelib-2.0.0/vcorelib/math/analysis/average.py` & `vcorelib-2.0.1/vcorelib/math/analysis/average.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 A module for working with averages.
 """
 
 # built-in
 from typing import List as _List
 
+DEFAULT_DEPTH = 10
+
 
 class MovingAverage:  # pylint: disable=too-many-instance-attributes
     """A class for managing a moving average of floats."""
 
-    def __init__(self, depth: int = 10, initial: float = 0.0) -> None:
+    def __init__(
+        self, depth: int = DEFAULT_DEPTH, initial: float = 0.0
+    ) -> None:
         """Initialize this moving average."""
 
         self._index: int = 0
         self._data: _List[float] = []
         self._sum: float = initial
 
         # Intentionally public members.
```

### Comparing `vcorelib-2.0.0/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-2.0.1/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-2.0.1/vcorelib/math/analysis/rate/limiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 A module for simplifying limiting the rate of a function call or hot loop.
 """
 
 # built-in
 from typing import Callable as _Callable
 
 # internal
-from vcorelib.math.analysis.rate import RateTracker
+from vcorelib.math.analysis.rate import RateTracker as _RateTracker
 from vcorelib.math.time import default_time_ns as _default_time_ns
 
 
 class RateLimiter:
     """A class for limiting the rate of runtime work."""
 
     def __init__(self, period_ns: int, **kwargs) -> None:
         """Initialize this rate-limiter."""
 
         assert period_ns >= 0
         self.period_ns = period_ns
         self.prev_time_ns: int = 0
-        self.rate = RateTracker(**kwargs)
+        self.rate = _RateTracker(**kwargs)
 
     @property
     def rate_hz(self) -> float:
         """
         Get the underlying rate that this limiter is governing. This is useful
         to determine if the rate limitation is or isn't impacting the rate of
         some task.
```

### Comparing `vcorelib-2.0.0/vcorelib/math/time.py` & `vcorelib-2.0.1/vcorelib/math/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from time import time_ns as _time_ns
 from typing import Dict as _Dict
 from typing import Iterator as _Iterator
 from typing import Tuple as _Tuple
 from typing import Union as _Union
 
 # internal
-from vcorelib.math import KIBI_UNITS as _KIBI_UNITS
-from vcorelib.math import SI_UNITS as _SI_UNITS
-from vcorelib.math import UnitSystem as _UnitSystem
-from vcorelib.math import unit_traverse as _unit_traverse
+from vcorelib.math.unit import KIBI_UNITS as _KIBI_UNITS
+from vcorelib.math.unit import SI_UNITS as _SI_UNITS
+from vcorelib.math.unit import UnitSystem as _UnitSystem
+from vcorelib.math.unit import unit_traverse as _unit_traverse
 
 
 def default_time_ns() -> int:
     """Get a timestamp value using a default method."""
     return _time_ns()
```

### Comparing `vcorelib-2.0.0/vcorelib/names.py` & `vcorelib-2.0.1/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/namespace.py` & `vcorelib-2.0.1/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/paths/__init__.py` & `vcorelib-2.0.1/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/paths/context.py` & `vcorelib-2.0.1/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/paths/info.py` & `vcorelib-2.0.1/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/paths/info_cache.py` & `vcorelib-2.0.1/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/platform/__init__.py` & `vcorelib-2.0.1/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/schemas/__init__.py` & `vcorelib-2.0.1/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/schemas/base.py` & `vcorelib-2.0.1/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/schemas/json.py` & `vcorelib-2.0.1/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/schemas/mixins.py` & `vcorelib-2.0.1/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/script/__init__.py` & `vcorelib-2.0.1/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/target/__init__.py` & `vcorelib-2.0.1/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/target/evaluation.py` & `vcorelib-2.0.1/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/target/expression.py` & `vcorelib-2.0.1/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/target/resolver.py` & `vcorelib-2.0.1/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/task/__init__.py` & `vcorelib-2.0.1/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/task/dict/melder.py` & `vcorelib-2.0.1/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/task/manager.py` & `vcorelib-2.0.1/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/task/subprocess/run.py` & `vcorelib-2.0.1/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib/task/time/sleep.py` & `vcorelib-2.0.1/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.0.0/vcorelib.egg-info/PKG-INFO` & `vcorelib-2.0.1/vcorelib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.0.0
+Version: 2.0.1
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e2335154489804baac80ff4fa5703aed
+    hash=b62c8c800bcc6195e61d7492ca560a0e
     =====================================
 -->
 
-# vcorelib ([2.0.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.0.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
 
@@ -43,15 +42,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vcorelib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vcorelib-2.0.0/vcorelib.egg-info/SOURCES.txt` & `vcorelib-2.0.1/vcorelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 vcorelib/io/arbiter/__init__.py
 vcorelib/io/arbiter/base.py
 vcorelib/io/arbiter/context.py
 vcorelib/io/arbiter/directory.py
 vcorelib/io/archive/__init__.py
 vcorelib/math/__init__.py
 vcorelib/math/time.py
+vcorelib/math/unit.py
 vcorelib/math/analysis/__init__.py
 vcorelib/math/analysis/average.py
 vcorelib/math/analysis/rate/__init__.py
 vcorelib/math/analysis/rate/limiter.py
 vcorelib/paths/__init__.py
 vcorelib/paths/context.py
 vcorelib/paths/info.py
```

