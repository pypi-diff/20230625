# Comparing `tmp/mercury-sync-0.3.4.tar.gz` & `tmp/mercury-sync-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.4.tar", last modified: Sat Jun 24 22:48:45 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.5.tar", last modified: Sun Jun 25 08:00:16 2023, max compression
```

## Comparing `mercury-sync-0.3.4.tar` & `mercury-sync-0.3.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    36297 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41512 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:00:16.136694 mercury-sync-0.3.5/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 08:00:16.000000 mercury-sync-0.3.5/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:00:16.140694 mercury-sync-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-25 08:00:12.000000 mercury-sync-0.3.5/setup.py
```

### Comparing `mercury-sync-0.3.4/LICENSE` & `mercury-sync-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/PKG-INFO` & `mercury-sync-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.4/README.md` & `mercury-sync-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.5/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         self._semaphore: Union[asyncio.Semaphore, None] = None
         self._compressor: Union[zstandard.ZstdCompressor, None] = None
         self._decompressor: Union[zstandard.ZstdDecompressor, None] = None
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
+        self._tcp_connect_retries = env.MERCURY_SYNC_TCP_CONNECT_RETRIES
 
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         worker_socket: Optional[socket.socket]=None
     ):
@@ -165,24 +166,20 @@
                 key_path=key_path
             ) 
 
         if self.connected is False and worker_socket is None:
             self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
-            while True:
+            try:
+                self._server_socket.bind((self.host, self.port))
 
-                try:
+            except Exception:
+                pass
 
-                    self._server_socket.bind((self.host, self.port))
-                    break
-
-                except Exception:
-                    self.port += 1
- 
 
             self._server_socket
 
             self._server_socket.setblocking(False)
 
         elif self.connected is False:
             self._server_socket = worker_socket
@@ -246,25 +243,39 @@
 
         tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         tcp_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         await self._loop.run_in_executor(None, tcp_socket.connect, address)
 
         tcp_socket.setblocking(False)
 
-        client_transport, _ = await self._loop.create_connection(
-            lambda: MercurySyncTCPClientProtocol(
-                self.read
-            ),
-            sock=tcp_socket,
-            ssl=self._client_ssl_context
-        )
+        last_error: Union[Exception, None] = None
+
+        for _ in range(self._tcp_connect_retries):
+
+            try:
+
+                client_transport, _ = await self._loop.create_connection(
+                    lambda: MercurySyncTCPClientProtocol(
+                        self.read
+                    ),
+                    sock=tcp_socket,
+                    ssl=self._client_ssl_context
+                )
+
+                self._client_transports[address] = client_transport
+
+                return client_transport
+            
+            except ConnectionRefusedError as connection_error:
+                last_error = connection_error
 
-        self._client_transports[address] = client_transport
+            await asyncio.sleep(1)
 
-        return client_transport
+        if last_error:
+            raise last_error
     
     def _create_client_ssl_context(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> ssl.SSLContext:
```

### Comparing `mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.5/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.5/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.5/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.5/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/env/env.py` & `mercury-sync-0.3.5/mercury_sync/env/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,30 +11,36 @@
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
-    MERCURY_SYNC_BOOT_WAIT: StrictStr='5s'
+    MERCURY_SYNC_TCP_CONNECT_RETRIES: StrictInt=3
+    MERCURY_SYNC_BOOT_WAIT: StrictStr='3s'
+    MERCURY_SYNC_MAX_TIME_IDLE: StrictStr='10s'
+    MERCURY_SYNC_IDLE_REBOOT_TIMEOUT: StrictStr='10s'
     MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD=3
-    MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=7
-    MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=10
+    MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=2
+    MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=7
     MERCURY_SYNC_INITIAL_NODES_COUNT: StrictInt=3
-    MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='1s'
+    MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='0.2s'
     MERCURY_SYNC_REGISTRATION_TIMEOUT: StrictStr='1m'
-    MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.25s'
-    MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=1
+    MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.2s'
+    MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=3
     MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
+            'MERCURY_SYNC_TCP_CONNECT_RETRIES': int,
+            'MERCURY_SYNC_MAX_TIME_IDLE': str,
+            'MERCURY_SYNC_IDLE_REBOOT_TIMEOUT': str,
             'MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD': int,
             'MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER': int,
             'MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER': int,
             'MERCURY_SYNC_INITIAL_NODES_COUNT': int,
             'MERCURY_SYNC_BOOT_WAIT': str,
             'MERCURY_SYNC_REGISTRATION_TIMEOUT': str,
             'MERCURY_SYNC_HEALTH_POLL_INTERVAL': str,
```

### Comparing `mercury-sync-0.3.4/mercury_sync/env/load_env.py` & `mercury-sync-0.3.5/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.5/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.5/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.5/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/service/controller.py` & `mercury-sync-0.3.5/mercury_sync/service/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,16 +516,20 @@
             connection: MercurySyncUDPConnection = await existing_udp_connections.get()
             await connection.close()
 
         while existing_tcp_connections.empty() is False:
             connection: MercurySyncUDPConnection = await existing_tcp_connections.get()
             await connection.close()
 
-        del self._udp_queue[(remote.host, remote.port)]
-        del self._tcp_queue[(remote.host, remote.port)]
+        if self._udp_queue.get((remote.host, remote.port)):
+            del self._udp_queue[(remote.host, remote.port)]
+
+        
+        if self._tcp_queue.get((remote.host, remote.port)):
+            del self._tcp_queue[(remote.host, remote.port)]
 
     async def send(
         self,
         event_name: str,
         message: Message
     ):
         connection: MercurySyncUDPConnection = await self._udp_queue[(message.host, message.port)].get()
```

### Comparing `mercury-sync-0.3.4/mercury_sync/service/monitor.py` & `mercury-sync-0.3.5/mercury_sync/service/monitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
 import math
 import random
 import time
+import traceback
 from collections import defaultdict, deque
 from mercury_sync.env import Env, load_env
 from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.hooks.client_hook import client
 from mercury_sync.hooks.server_hook import server
 from mercury_sync.models.healthcheck import HealthCheck, HealthStatus
 from mercury_sync.models.ticket import Ticket
+from mercury_sync.snowflake import Snowflake
 from mercury_sync.types import Call
 from typing import Optional, Dict, Tuple, List, Deque, Union
 from .controller import Controller
 
 
 async def cancel(pending_item: asyncio.Task) -> None:
     pending_item.cancel()
@@ -58,41 +60,55 @@
 
         self.status: HealthStatus = 'initializing'
         
 
         self.error_context: Optional[str] = None
         self.registration_timeout = TimeParser(env.MERCURY_SYNC_REGISTRATION_TIMEOUT).time
         self.boot_wait = TimeParser(env.MERCURY_SYNC_BOOT_WAIT).time
-
+        
         self._healthchecks: Dict[str, asyncio.Task] = {}
         self._registered: Dict[int, Tuple[str, int]] = {}
         self._running = False
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._poll_interval = TimeParser(env.MERCURY_SYNC_HEALTH_POLL_INTERVAL).time
         self._poll_timeout = TimeParser(env.MERCURY_SYNC_HEALTH_CHECK_TIMEOUT).time
+        self._reboot_timeout = TimeParser(env.MERCURY_SYNC_IDLE_REBOOT_TIMEOUT).time
+        self._max_time_idle = TimeParser(env.MERCURY_SYNC_MAX_TIME_IDLE).time
+        self._tcp_sync_interval = 1
+        self._sync_interval = 1
+
         self._check_nodes_count = env.MERCURY_SYNC_INDIRECT_CHECK_NODES
 
         self.min_suspect_multiplier = env.MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER
         self.max_suspect_multiplier = env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER 
         self._min_suspect_node_count = env.MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD
-        self._local_health_multiplier = self.max_suspect_multiplier
-
-        self._local_health_monitor: Optional[asyncio.Task] = None
+        self._local_health_multiplier = 0
         self._confirmed_suspicions: Dict[Tuple[str, int], int] = {}
         self._waiter: Optional[asyncio.Future] = None
-        self._active_checks_queue: Deque[asyncio.Task] = deque()
+
+        self._tasks_queue: Deque[asyncio.Task] = deque()
         self._degraded_nodes: Deque[Tuple[str, int]] = deque()
         self._suspect_nodes: Deque[Tuple[str, int]] = deque()
 
-        self._failed_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
+        self._degraded_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._suspect_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
+
+        self._local_health_monitor: Union[asyncio.Task, None] = None
+        self._udp_sync_task: Union[asyncio.Task, None] = None
+        self._tcp_sync_task: Union[asyncio.Task, None] = None
+
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._investigating_nodes: Dict[Tuple[str, int], Dict[Tuple[str, int]]] = defaultdict(dict)
         self._node_statuses: Dict[Tuple[str, int], HealthStatus] = {}
+
+        self.bootstrap_host: Union[str, None] = None
+        self.bootstrap_port: Union[int, None] = None
+
         self._healthy_statuses = [
+            'waiting',
             'healthy'
         ]
 
         self._unhealthy_statuses = [
             'degraded',
             'suspect',
             'failed'
@@ -100,23 +116,53 @@
 
     @server()
     async def update_node_status(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
+    
+        update_node_host = healthcheck.source_host
+        update_node_port = healthcheck.source_port
+        update_status = healthcheck.status
+
+        if healthcheck.target_host and healthcheck.target_port:
+            update_node_host = healthcheck.target_host
+            update_node_port = healthcheck.target_port
+
+        if healthcheck.target_status:
+            update_status = healthcheck.target_status
         
-        source_host = healthcheck.source_host
-        source_port = healthcheck.source_port
+        node_exists = self._node_statuses.get((
+            update_node_host,
+            update_node_port
+        )) is not None
 
-        self._node_statuses[(source_host, source_port)] = healthcheck.status
+        if update_node_host != self.host and update_node_port != self.port and node_exists:
+
+            self._node_statuses[(update_node_host, update_node_port)] = update_status
+
+        elif update_node_host != self.host and update_node_port != self.port:
+
+            await self.extend_client(
+                HealthCheck(
+                    host=update_node_host,
+                    port=update_node_port,
+                    source_host=self.host,
+                    source_port=self.port,
+                    status=self.status,
+                    error=healthcheck.error
+                )
+            )
+
+            self._node_statuses[(update_node_host, update_node_port)] = update_status
 
         return HealthCheck(
-            host=source_host,
-            port=source_port,
+            host=healthcheck.source_host,
+            port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             status=self.status
         )
 
     @server()
     async def update_as_suspect(
@@ -128,15 +174,15 @@
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
 
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
 
         if self.status == 'healthy':
-            self._active_checks_queue.append(
+            self._tasks_queue.append(
                 asyncio.create_task(
                     self.push_status_update(
                         host=target_host,
                         port=target_port,
                         health_status=self.status,
                         error_context=self.error_context
                     )
@@ -175,16 +221,14 @@
                 source_host,
                 source_port,
                 target_host,
                 target_port
             )
 
 
-            self._node_statuses[(target_host, target_port)] = healthcheck.target_status
-
             indirect_probe = asyncio.wait_for(
                 self.push_health_update(
                     target_host,
                     target_port,
                     self.status,
                     error_context=healthcheck.error
                 ),
@@ -195,21 +239,21 @@
                 investigation_update,
                 indirect_probe
             ]):
                 result: Union[Tuple[int, HealthCheck], None] = await task
 
                 if isinstance(result, tuple):
 
-                    _, response = result
-
                     self._local_health_multiplier = max(
-                        0, 
-                        self._local_health_multiplier - 1
+                        self._local_health_multiplier - 1, 
+                        0
                     )
 
+                    _, response = result
+
                     self._node_statuses[(target_host, target_port)]  = response.status
 
                     # We've received a refutation
                     return HealthCheck(
                         host=healthcheck.source_host,
                         port=healthcheck.source_port,
                         target_status=response.status,   
@@ -217,14 +261,33 @@
                         source_port=response.source_port,
                         status=response.status,
                         error=response.error
                     )
 
         except asyncio.TimeoutError:
 
+            self._local_health_multiplier = min(
+                self._local_health_multiplier + 1, 
+                self.max_suspect_multiplier
+            )
+
+            node_status = self._node_statuses.get((target_host, target_port)) 
+
+            if node_status not in self._unhealthy_statuses or node_status is None:
+                self._node_statuses[(target_host, target_port)] = 'degraded'
+
+                self._degraded_nodes.append((
+                    target_host,
+                    target_port
+                ))
+
+                self._degraded_tasks[(target_host, target_port)] = asyncio.create_task(
+                    self._probe_timed_out_node()
+                )
+
             # Our suspicion is correct!
             return HealthCheck(
                 host=healthcheck.source_host,
                 port=healthcheck.source_port,
                 source_host=target_host,
                 source_port=target_port,
                 target_status=healthcheck.status, 
@@ -249,26 +312,31 @@
 
             if suspect_task:
                 await cancel(suspect_task)
                 del suspect_tasks[(source_host, source_port)]
                 
                 self._suspect_tasks = suspect_tasks
 
-            self._node_statuses[(source_host, source_port)] =  'healthy'
+
+            local_node_status = self._node_statuses.get((source_host, source_port))
+
+            if local_node_status is None:
             
-            await self.extend_client(
-                HealthCheck(
-                    host=source_host,
-                    port=source_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=healthcheck.status,
-                    error=healthcheck.error
+                await self.extend_client(
+                    HealthCheck(
+                        host=source_host,
+                        port=source_port,
+                        source_host=self.host,
+                        source_port=self.port,
+                        status=healthcheck.status,
+                        error=healthcheck.error
+                    )
                 )
-            )
+
+            self._node_statuses[(source_host, source_port)] =  'healthy'
 
         return HealthCheck(
             host=source_host,
             port=source_port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
@@ -321,38 +389,14 @@
         suspect_task = suspect_tasks.pop((source_host, source_port), None)
 
         if suspect_task:
             await cancel(suspect_task)
 
             self._suspect_tasks = suspect_tasks
 
-            
-        if healthcheck.target_status == 'suspect' or healthcheck.target_status == 'degraded':
-
-            self._local_health_multiplier = min(
-                self._local_health_multiplier + 1,
-                self.max_suspect_multiplier
-            )
-
-            monitoring = [
-                address for address, status in self._node_statuses.items() if status in self._healthy_statuses
-            ]
-
-            # Send our refutation
-            self._active_checks_queue.extend([
-                asyncio.create_task(
-                    self._run_healthcheck(
-                        host,
-                        port,
-                        target_host=healthcheck.target_host,
-                        target_port=healthcheck.target_port
-                    )
-                ) for host, port in monitoring
-            ])
-
         status_unhealthy = local_node_status == 'failed' or local_node_status == 'suspect'
             
         if local_node_status is None or status_unhealthy:
             
             monitoring = [
                 address for address, status in self._node_statuses.items() if status == 'healthy'
             ]
@@ -364,48 +408,27 @@
                     source_host,
                     source_port,
                     healthcheck.status,
                     error_context=healthcheck.error
                 ) for host, port in monitoring
             ])
 
-            self._active_checks_queue.extend([
-                asyncio.create_task(
-                    self._run_healthcheck(
-                        host,
-                        port,
-                    )
-                ) for host, port in monitoring
-            ])
-
         if local_node_status is None:
 
             await self.extend_client(
                 HealthCheck(
                     host=source_host,
                     port=source_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-        elif status_unhealthy:
-            await self.refresh_clients(
-                HealthCheck(
-                    host=source_host,
-                    port=source_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=healthcheck.status,
-                    error=healthcheck.error
-                )
-            )
-
         self._node_statuses[(source_host, source_port)] = healthcheck.status
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
@@ -421,17 +444,17 @@
         port: int,
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[str]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         
-        target_status = self._node_statuses[(host, port)]
+        target_status: Union[HealthCheck, None] = None
         if target_host and target_port:
-            target_status = self._node_statuses[(target_host, target_port)]
+            target_status = self._node_statuses.get((target_host, target_port))
 
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
@@ -448,17 +471,17 @@
         port: int,
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[str]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         
-        target_status = self._node_statuses[(host, port)]
+        target_status: Union[HealthCheck, None] = None
         if target_host and target_port:
-            target_status = self._node_statuses[(target_host, target_port)]
+            target_status = self._node_statuses.get((target_host, target_port))
 
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
@@ -537,21 +560,58 @@
     
     @client('update_node_status')
     async def push_status_update(
         self,
         host: str,
         port: int,
         health_status: HealthStatus,
+        target_host: Optional[str]=None,
+        target_port: Optional[int]=None,
+        error_context: Optional[str]=None
+    ) -> Call[HealthCheck]:
+        
+        target_status: Union[HealthStatus, None] = None
+        if target_host and target_port:
+            target_status = self._node_statuses.get((target_host, target_port))
+
+        return HealthCheck(
+            host=host,
+            port=port,
+            source_host=self.host,
+            source_port=self.port,
+            target_host=target_host,
+            target_port=target_port,
+            target_status=target_status,
+            status=health_status,
+            error=error_context
+        )
+    
+    @client('update_node_status', as_tcp=True)
+    async def push_tcp_status_update(
+        self,
+        host: str,
+        port: int,
+        health_status: HealthStatus,
+        target_host: Optional[str]=None,
+        target_port: Optional[int]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
+        
+        target_status: Union[HealthStatus, None] = None
+        if target_host and target_port:
+            target_status = self._node_statuses.get((target_host, target_port))
+
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
+            target_host=target_host,
+            target_port=target_port,
+            target_status=target_status,
             status=health_status,
             error=error_context
         )
     
     @client('update_as_suspect')
     async def push_suspect_update(
         self,
@@ -580,14 +640,17 @@
 
     async def register(
         self,
         host: str,
         port: int
     ) -> Call[Ticket]:
         
+        self.bootstrap_host = host
+        self.bootstrap_port = port
+        
         await asyncio.wait_for(
             asyncio.create_task(
                 self.start_client(
                     HealthCheck(
                         host=host,
                         port=port,
                         source_host=self.host,
@@ -610,29 +673,35 @@
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
 
+        self._udp_sync_task = asyncio.create_task(
+            self._run_state_sync()
+        )
+
     def _calculate_min_suspect_timeout(self):
         nodes_count = len({
             address: status for address, status in self._node_statuses.items() if status != 'failed'
         }) + 1
 
+        poll_timeout = self._poll_timeout * (self._local_health_multiplier + 1)
+
         return round(
-            self.min_suspect_multiplier * math.log10(nodes_count) * self._poll_interval,
-            2
+            self.min_suspect_multiplier * math.log10(nodes_count) * poll_timeout,
+            4
         )
 
     def _calculate_max_suspect_timeout(self, min_suspect_timeout: float):
         
         return round(
             self.max_suspect_multiplier * min_suspect_timeout,
-            2
+            4
         )
 
     def _calculate_suspicion_timeout(
         self,
         suspect_node_address: Tuple[str, int]
     ):
 
@@ -691,23 +760,25 @@
 
         except asyncio.TimeoutError:
             self._local_health_multiplier = min(
                 self._local_health_multiplier + 1, 
                 self.max_suspect_multiplier
             )
 
-            if self._node_statuses[(host, port)] not in self._unhealthy_statuses:
+            node_status = self._node_statuses.get((host, port)) 
+
+            if node_status and node_status not in self._unhealthy_statuses:
                 self._node_statuses[(host, port)] = 'degraded'
 
                 self._degraded_nodes.append((
                     host,
                     port
                 ))
 
-                self._failed_tasks[(host, port)] = asyncio.create_task(
+                self._degraded_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
 
     async def _run_healthcheck(
         self, 
         host: str, 
         port: int,
@@ -749,15 +820,15 @@
                 self._node_statuses[(host, port)] = 'degraded'
 
                 self._degraded_nodes.append((
                     host,
                     port
                 ))
 
-                self._failed_tasks[(host, port)] = asyncio.create_task(
+                self._degraded_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
 
     async def _probe_timed_out_node(self):
         
         suspect_host, suspect_port = self._degraded_nodes.pop()
         
@@ -770,32 +841,39 @@
         )
 
         self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
             check for _, check in healthchecks if check.target_status == 'suspect'
         ])
 
         indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+        self._local_health_multiplier = max(
+            0,
+            self._local_health_multiplier - indirect_ack_count
+        )
+
 
         missing_ack_count = len(confirmation_members) - indirect_ack_count
         
         next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
         if next_health_multiplier < 0:
             self._local_health_multiplier = 0
 
         else:
             self._local_health_multiplier = min(
                 next_health_multiplier, 
                 self.max_suspect_multiplier
             )
 
-        if suspect_count >= len(confirmation_members):
+        confirmation_members_count = len(confirmation_members)
+
+        if suspect_count >= confirmation_members_count:
 
             self._node_statuses[(suspect_host, suspect_port)] = 'suspect'
 
-            self._active_checks_queue.append(
+            self._tasks_queue.append(
                 asyncio.create_task(
                     self._push_suspect_update(
                         host=suspect_host,
                         port=suspect_port,
                         target_host=suspect_host,
                         target_port=suspect_port,
                         health_status=self.status,
@@ -812,28 +890,118 @@
 
         else:
             self._node_statuses[(suspect_host, suspect_port)] = 'healthy' 
             self.status = 'healthy'
 
         if self._investigating_nodes.get((suspect_host, suspect_port)):
             del self._investigating_nodes[(suspect_host, suspect_port)]
+
+    async def _start_suspect_monitor(self):
+
+        elapsed = 0
+        start = time.monotonic()
+
+    
+        if len(self._suspect_nodes) < 1:
+            return
+        
+        address = self._suspect_nodes.pop()
+        suspect_host, suspect_port = address
+
+        confirmation_task = self._degraded_tasks.get((suspect_host, suspect_port))
+        if confirmation_task:
+            await cancel(confirmation_task)
+            confirmation_task.cancel()
+
+        node_status = self._node_statuses[(suspect_host, suspect_port)]
+        
+        suspicion_timeout = self._calculate_suspicion_timeout(address)
+
+        while elapsed < suspicion_timeout and node_status == 'suspect':
+
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self._push_suspect_update(
+                        host=suspect_host,
+                        port=suspect_port,
+                        target_host=suspect_host,
+                        target_port=suspect_port,
+                        health_status=self.status,
+                        error_context=self.error_context
+                    )
+                )
+            )
+                
+            confirmation_members = self._get_confirmation_members()
+
+            healthchecks, suspect_count = await self._request_indirect_probe(
+                suspect_host,
+                suspect_port,
+                confirmation_members
+            )
+
+            self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
+                check for _, check in healthchecks if check.target_status == 'suspect'
+            ])
+            
+            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+            self._local_health_multiplier = max(
+                0,
+                self._local_health_multiplier - indirect_ack_count
+            )
+
+
+            missing_ack_count = len(confirmation_members) - indirect_ack_count
+            
+            next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
+            if next_health_multiplier < 0:
+                self._local_health_multiplier = 0
+
+            else:
+                self._local_health_multiplier = min(
+                    next_health_multiplier, 
+                    self.max_suspect_multiplier
+                )
+
+            confirmation_members_count = len(confirmation_members)
+
+            if suspect_count < confirmation_members_count:
+                # We had a majority confirmation the node was healthy.
+
+                self._node_statuses[(suspect_host, suspect_port)] = 'healthy'
+
+                await self._propagate_state_update(
+                    suspect_host,
+                    suspect_port
+                )
+
+            if self._investigating_nodes.get((suspect_host, suspect_port)):
+                del self._investigating_nodes[(suspect_host, suspect_port)]
+
+            await asyncio.sleep(
+                self._poll_interval * (self._local_health_multiplier + 1)
+            ) 
+
+            elapsed = time.monotonic() - start
+
+            suspicion_timeout = self._calculate_suspicion_timeout(address)
+
+        if self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
+            self._node_statuses[(suspect_host, suspect_port)] = 'failed'
             
     def _get_confirmation_members(self) -> List[Tuple[str, int]]:
         confirmation_members = [
             address for address, status in self._node_statuses.items() if status in self._healthy_statuses
         ]
 
-        confirmation_candidates_count = len(confirmation_members) 
-
-        if confirmation_candidates_count < self._check_nodes_count:
-            self._check_nodes_count = confirmation_candidates_count
+        confirmation_members_count = len(confirmation_members)
 
         confirmation_members = random.sample(
             confirmation_members, 
-            self._check_nodes_count
+            confirmation_members_count
         )
 
         return confirmation_members
 
     async def _request_indirect_probe(
         self,
         host: str,
@@ -882,18 +1050,19 @@
             requested_checks, 
             timeout=self._poll_timeout * (self._local_health_multiplier + 1)
         )
 
         completed, pending = check_tasks
 
         healthchecks: List[Call[HealthCheck]]  = await asyncio.gather(*completed)
-
         sorted_checks: List[Call[HealthCheck]] = list(sorted(
             healthchecks,
-            key=lambda check: check[0]
+            key=lambda check: Snowflake.parse(
+                Snowflake.parse(check[0]).timestamp
+            ).timestamp
         ))
 
         suspect = [
             (
                 shard_id,
                 check
             ) for shard_id, check in sorted_checks if check.target_status == 'suspect'
@@ -959,138 +1128,155 @@
             monitors = [
                 address for address, status in self._node_statuses.items() if status == 'healthy'
             ]
 
             host: Union[str, None] = None
             port: Union[int, None] = None
 
-            if len(monitors) > 0:
+            monitors_count = len(monitors)
+
+            if monitors_count > 0:
 
-                monitors_count = len(monitors)
                 monitor_idx = monitor_idx%monitors_count
                 host, port = monitors[monitor_idx]
 
             if self._node_statuses.get((host, port)):
         
-                self._active_checks_queue.append(
+                self._tasks_queue.append(
                     asyncio.create_task(
                         self._run_healthcheck(
                             host,
                             port
                         )
                     )
                 )
 
-            if monitor_idx%monitors_count == 0:
-                self.status = 'healthy'
-
             monitor_idx += 1
 
             await asyncio.sleep(
                 self._poll_interval * (self._local_health_multiplier + 1)
-            )      
+            )
 
-    async def _start_suspect_monitor(self):
+    async def _run_state_sync(self):
+        while self._running:
 
-        elapsed = 0
-        start = time.monotonic()
+            monitors = [
+                address for address, status in self._node_statuses.items() if status in self._healthy_statuses
+            ]
 
-    
-        if len(self._suspect_nodes) < 1:
-            return
-        
-        address = self._suspect_nodes.pop()
-        suspect_host, suspect_port = address
+            active_nodes_count = len(monitors)
 
-        confirmation_task = self._failed_tasks.get((suspect_host, suspect_port))
-        if confirmation_task:
-            await cancel(confirmation_task)
-            confirmation_task.cancel()
+            if active_nodes_count > 0:
 
-        node_status = self._node_statuses[(suspect_host, suspect_port)]
+                self._tasks_queue.extend([
+                    asyncio.create_task(
+                        self._push_state_to_node(
+                            host=host,
+                            port=port
+                        )
+                    ) for host, port in monitors
+                ])
 
-        suspicion_timeout = self._calculate_suspicion_timeout(address)
+                self._tasks_queue.extend([
+                    asyncio.create_task(
+                        self._push_state_to_node_tcp(
+                            host=host,
+                            port=port
+                        )
+                    ) for host, port in monitors
+                ])
 
-        while elapsed < suspicion_timeout and node_status == 'suspect':
+                self._sync_interval = round(
+                    math.log10(active_nodes_count + 1),
+                    2
+                ) * (active_nodes_count + 1)
 
-            self._active_checks_queue.append(
-                asyncio.create_task(
-                    self._push_suspect_update(
-                        host=suspect_host,
-                        port=suspect_port,
-                        target_host=suspect_host,
-                        target_port=suspect_port,
-                        health_status=self.status,
-                        error_context=self.error_context
-                    )
+            await asyncio.sleep(
+                max(
+                    self._sync_interval,
+                    1
                 )
             )
-                
-            confirmation_members = self._get_confirmation_members()
-
-            healthchecks, suspect_count = await self._request_indirect_probe(
-                suspect_host,
-                suspect_port,
-                confirmation_members
-            )
 
-            self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
-                check for _, check in healthchecks if check.target_status == 'suspect'
-            ])
-
-            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
-
-            missing_ack_count = len(confirmation_members) - indirect_ack_count
-            
-            next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
-            if next_health_multiplier < 0:
-                self._local_health_multiplier = 0
+    async def _push_state_to_node(
+        self,
+        host: str,
+        port: int
+    ):
+        await asyncio.gather(*[
+            self._push_status_update(
+                host=host,
+                port=port,
+                target_host=node_host,
+                target_port=node_port
+            ) for node_host, node_port in self._node_statuses
+        ])
 
-            else:
-                self._local_health_multiplier = min(
-                    next_health_multiplier, 
-                    self.max_suspect_multiplier
-                )
+    async def _push_state_to_node_tcp(
+        self,
+        host: str,
+        port: int
+    ):
+        await asyncio.gather(*[
+            self._push_tcp_status_update(
+                host=host,
+                port=port,
+                target_host=node_host,
+                target_port=node_port
+            ) for node_host, node_port in self._node_statuses
+        ])
 
-            if suspect_count < len(confirmation_members):
-                # We had a majority confirmation the node was healthy.
+    async def _push_status_update(
+        self,
+        host: str,
+        port: int,
+        target_host: Optional[str]=None,
+        target_port: Optional[int]=None
+    ):
+        
+        try:
 
-                self._node_statuses[(suspect_host, suspect_port)] = 'healthy'
+            await asyncio.wait_for(
+                self.push_status_update(
+                    host=host,
+                    port=port,
+                    target_host=target_host,
+                    target_port=target_port,
+                    health_status=self.status
+                ),
+                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+            )
 
-                await self._propagate_state_update(
-                    suspect_host,
-                    suspect_port
-                )
+        except asyncio.TimeoutError:
+            pass
 
-                await self.refresh_clients(
-                    HealthCheck(
-                        host=suspect_host,
-                        port=suspect_port,
-                        source_host=self.host,
-                        source_port=self.port,
-                        status=self.status
-                    )
-                )
+    async def _push_tcp_status_update(
+        self,
+        host: str,
+        port: int,
+        target_host: Optional[str]=None,
+        target_port: Optional[int]=None
+    ):
+        
+        try:
 
-            if self._investigating_nodes.get((suspect_host, suspect_port)):
-                del self._investigating_nodes[(suspect_host, suspect_port)]
+            await asyncio.wait_for(
+                self.push_tcp_status_update(
+                    host=host,
+                    port=port,
+                    target_host=target_host,
+                    target_port=target_port,
+                    health_status=self.status
+                ),
+                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+            )
 
-            await asyncio.sleep(
-                self._poll_interval * (self._local_health_multiplier + 1)
-            ) 
+        except asyncio.TimeoutError:
+            pass
 
-            elapsed = time.monotonic() - start
-        
-        if self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
-            self._node_statuses[(suspect_host, suspect_port)] = 'failed'
-            await self._propagate_state_update(
-                    suspect_host,
-                    suspect_port
-                )
-            
     async def _push_suspect_update(
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int,
         health_status: HealthStatus,
@@ -1113,53 +1299,46 @@
         except asyncio.TimeoutError:
             pass
 
     async def cleanup_pending_checks(self):
 
         while self._running:
 
-            for pending_check in list(self._active_checks_queue):
+            for pending_check in list(self._tasks_queue):
                 if pending_check.done() or pending_check.cancelled():
-                    self._active_checks_queue.remove(pending_check)
-
-            failed_nodes = [
-                address for address, status in self._node_statuses.items() if status == 'failed'
-            ]
-
-            for host, port in failed_nodes:
-
-                await self.remove_clients(
-                    HealthCheck(
-                        host=host,
-                        port=port,
-                        source_host=self.host,
-                        source_port=self.port,
-                        status='failed'
-                    )
-                )
+                    self._tasks_queue.remove(pending_check)
 
             await asyncio.sleep(self._cleanup_interval)
     
     async def shutdown(self):
         self._running = False
         self._local_health_monitor.cancel()
 
         await asyncio.gather(*[
-            cancel(check) for check in self._active_checks_queue
+            cancel(check) for check in self._tasks_queue
         ])
 
         await asyncio.gather(*[
             cancel(remote_check) for remote_check in self._healthchecks.values()
         ])
 
         await cancel(self._local_health_monitor)
         
         await cancel(self._cleanup_task)
 
+        await cancel(self._udp_sync_task)
+
         await self.close()
+
+    async def soft_shutdown(self):
+        await asyncio.gather(*[
+            cancel(check) for check in self._tasks_queue
+        ])
+
+
```

### Comparing `mercury-sync-0.3.4/mercury_sync/service/service.py` & `mercury-sync-0.3.5/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.5/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.5/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.5/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.4/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.5/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.4/setup.py` & `mercury-sync-0.3.5/setup.py`

 * *Files identical despite different names*

