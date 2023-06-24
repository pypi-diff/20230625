# Comparing `tmp/mercury-sync-0.3.3.tar.gz` & `tmp/mercury-sync-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.3.tar", last modified: Sat Jun 24 21:43:40 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.4.tar", last modified: Sat Jun 24 22:48:45 2023, max compression
```

## Comparing `mercury-sync-0.3.3.tar` & `mercury-sync-0.3.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36297 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:48:45.251208 mercury-sync-0.3.4/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 22:48:45.000000 mercury-sync-0.3.4/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:48:45.255208 mercury-sync-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 22:48:38.000000 mercury-sync-0.3.4/setup.py
```

### Comparing `mercury-sync-0.3.3/LICENSE` & `mercury-sync-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/PKG-INFO` & `mercury-sync-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.3
+Version: 0.3.4
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.3/README.md` & `mercury-sync-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.4/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/env/env.py` & `mercury-sync-0.3.4/mercury_sync/env/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     MERCURY_SYNC_BOOT_WAIT: StrictStr='5s'
     MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD=3
     MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=7
     MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=10
     MERCURY_SYNC_INITIAL_NODES_COUNT: StrictInt=3
     MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='1s'
     MERCURY_SYNC_REGISTRATION_TIMEOUT: StrictStr='1m'
-    MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.2s'
+    MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.25s'
     MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=1
     MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
```

### Comparing `mercury-sync-0.3.3/mercury_sync/env/load_env.py` & `mercury-sync-0.3.4/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.4/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.4/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.4/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/service/controller.py` & `mercury-sync-0.3.4/mercury_sync/service/controller.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/service/monitor.py` & `mercury-sync-0.3.4/mercury_sync/service/monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,72 @@
         self._unhealthy_statuses = [
             'degraded',
             'suspect',
             'failed'
         ]
 
     @server()
+    async def update_node_status(
+        self,
+        shard_id: int,
+        healthcheck: HealthCheck
+    ) -> Call[HealthCheck]:
+        
+        source_host = healthcheck.source_host
+        source_port = healthcheck.source_port
+
+        self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+        return HealthCheck(
+            host=source_host,
+            port=source_port,
+            source_host=self.host,
+            source_port=self.port,
+            status=self.status
+        )
+
+    @server()
+    async def update_as_suspect(
+        self,
+        shard_id: int,
+        healthcheck: HealthCheck
+    ) -> Call[HealthCheck]:
+        
+        source_host = healthcheck.source_host
+        source_port = healthcheck.source_port
+
+        target_host = healthcheck.target_host
+        target_port = healthcheck.target_port
+
+        if self.status == 'healthy':
+            self._active_checks_queue.append(
+                asyncio.create_task(
+                    self.push_status_update(
+                        host=target_host,
+                        port=target_port,
+                        health_status=self.status,
+                        error_context=self.error_context
+                    )
+                )
+            )
+
+            self._local_health_multiplier = min(
+                self._local_health_multiplier + 1, 
+                self.max_suspect_multiplier
+            )
+
+        return HealthCheck(
+            host=source_host,
+            port=source_port,
+            source_host=self.host,
+            source_port=self.port,
+            status=self.status
+        )
+
+    @server()
     async def send_indirect_check(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
         source_host = healthcheck.source_host
@@ -175,46 +233,46 @@
         
     @server()
     async def register_new_node(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
-        host = healthcheck.source_host
-        port = healthcheck.source_port
+        source_host = healthcheck.source_host
+        source_port = healthcheck.source_port
 
-        not_self = host != self.host and port != self.port
+        not_self = source_host != self.host and source_port != self.port
         
         if not_self:
 
             suspect_tasks = dict(self._suspect_tasks)
-            suspect_task = suspect_tasks.get((host, port))
+            suspect_task = suspect_tasks.get((source_host, source_port))
 
             if suspect_task:
                 await cancel(suspect_task)
-                del suspect_tasks[(host, port)]
+                del suspect_tasks[(source_host, source_port)]
                 
                 self._suspect_tasks = suspect_tasks
 
-            self._node_statuses[(host, port)] =  'healthy'
+            self._node_statuses[(source_host, source_port)] =  'healthy'
             
             await self.extend_client(
                 HealthCheck(
-                    host=host,
-                    port=port,
+                    host=source_host,
+                    port=source_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
         return HealthCheck(
-            host=host,
-            port=port,
+            host=source_host,
+            port=source_port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
             status=self.status
         )
     
     @server()
@@ -340,44 +398,22 @@
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-        is_buddy = target_host is None and target_port is None
-
-        # Send our refutation
-        if local_node_status == 'suspect' and healthcheck.status == 'healthy' and is_buddy:
-
-            self._node_statuses[(source_host, source_port)] = 'healthy'
-            source_address = (source_host, source_port)
-            monitoring = [
-                address for address, status in self._node_statuses.items() if status in self._healthy_statuses and address != source_address
-            ]
-
-
-            self._active_checks_queue.extend([
-                asyncio.create_task(
-                    self._run_healthcheck(
-                        host,
-                        port,
-                        target_host=source_host,
-                        target_port=source_port
-                    )
-                ) for host, port in monitoring if host != source_host and port != source_port
-            ])
-
         self._node_statuses[(source_host, source_port)] = healthcheck.status
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
+            source_status=local_node_status,
             error=self.error_context,
             status=self.status
         )
 
     @client('register_health_update')
     async def push_health_update(
         self,
@@ -495,14 +531,52 @@
             target_status=self._node_statuses[(target_host, target_port)],
             source_host=self.host,
             source_port=self.port,
             error=error_context,
             status=health_status
         )
     
+    @client('update_node_status')
+    async def push_status_update(
+        self,
+        host: str,
+        port: int,
+        health_status: HealthStatus,
+        error_context: Optional[str]=None
+    ) -> Call[HealthCheck]:
+        return HealthCheck(
+            host=host,
+            port=port,
+            source_host=self.host,
+            source_port=self.port,
+            status=health_status,
+            error=error_context
+        )
+    
+    @client('update_as_suspect')
+    async def push_suspect_update(
+        self,
+        host: str,
+        port: int,
+        target_host: str,
+        target_port: int,
+        health_status: HealthStatus,
+        error_context: Optional[str]=None
+    ) -> Call[HealthCheck]:
+        return HealthCheck(
+            host=host,
+            port=port,
+            target_host=target_host,
+            target_port=target_port,
+            source_host=self.host,
+            source_port=self.port,
+            status=health_status,
+            error=error_context
+        )
+    
     async def start(self):
 
         await self.start_server()
         await asyncio.sleep(self.boot_wait)
 
     async def register(
         self,
@@ -712,14 +786,28 @@
                 next_health_multiplier, 
                 self.max_suspect_multiplier
             )
 
         if suspect_count >= len(confirmation_members):
 
             self._node_statuses[(suspect_host, suspect_port)] = 'suspect'
+
+            self._active_checks_queue.append(
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
             self._suspect_nodes.append((suspect_host, suspect_port))
 
             self._suspect_tasks[(suspect_host, suspect_port)] = asyncio.create_task(
                 self._start_suspect_monitor()
             )
 
         else:
@@ -919,14 +1007,27 @@
             confirmation_task.cancel()
 
         node_status = self._node_statuses[(suspect_host, suspect_port)]
 
         suspicion_timeout = self._calculate_suspicion_timeout(address)
 
         while elapsed < suspicion_timeout and node_status == 'suspect':
+
+            self._active_checks_queue.append(
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
                 
             confirmation_members = self._get_confirmation_members()
 
             healthchecks, suspect_count = await self._request_indirect_probe(
                 suspect_host,
                 suspect_port,
                 confirmation_members
@@ -981,14 +1082,40 @@
         
         if self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
             self._node_statuses[(suspect_host, suspect_port)] = 'failed'
             await self._propagate_state_update(
                     suspect_host,
                     suspect_port
                 )
+            
+    async def _push_suspect_update(
+        self,
+        host: str,
+        port: int,
+        target_host: str,
+        target_port: int,
+        health_status: HealthStatus,
+        error_context: Optional[str]=None
+    ):
+        
+        try:
+            await asyncio.wait_for(
+                self.push_suspect_update(
+                    host=host,
+                    port=port,
+                    target_host=target_host,
+                    target_port=target_port,
+                    health_status=health_status,
+                    error_context=error_context
+                ),
+                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+            )
+
+        except asyncio.TimeoutError:
+            pass
 
     async def cleanup_pending_checks(self):
 
         while self._running:
 
             for pending_check in list(self._active_checks_queue):
                 if pending_check.done() or pending_check.cancelled():
```

### Comparing `mercury-sync-0.3.3/mercury_sync/service/service.py` & `mercury-sync-0.3.4/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.4/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.4/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.4/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.3
+Version: 0.3.4
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.3/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.4/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.3/setup.py` & `mercury-sync-0.3.4/setup.py`

 * *Files identical despite different names*

