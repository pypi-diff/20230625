# Comparing `tmp/blaster-server-0.0.437.tar.gz` & `tmp/blaster-server-0.0.437b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.437.tar", last modified: Tue Jun 13 09:57:46 2023, max compression
+gzip compressed data, was "blaster-server-0.0.437b0.tar", last modified: Sun Jun 25 09:53:32 2023, max compression
```

## Comparing `blaster-server-0.0.437.tar` & `blaster-server-0.0.437b0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.437/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.437/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-13 09:57:46.099030 blaster-server-0.0.437/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.437/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.437/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.437/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.437/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.437/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.437/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.437/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38833 2023-06-09 14:07:27.000000 blaster-server-0.0.437/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    43823 2023-06-13 08:38:49.000000 blaster-server-0.0.437/blaster/tools/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.437/blaster/tools/sanitize_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.437/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3953 2023-06-06 19:29:14.000000 blaster-server-0.0.437/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.437/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.095029 blaster-server-0.0.437/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-13 09:57:46.000000 blaster-server-0.0.437/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-13 09:57:46.099030 blaster-server-0.0.437/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-06-09 14:09:20.000000 blaster-server-0.0.437/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-13 09:57:46.099030 blaster-server-0.0.437/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.437/test/test_command_line_parser.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.437/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.437/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.437/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.437/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.437b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.437b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.437b0/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.437b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-06-23 10:38:33.000000 blaster-server-0.0.437b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.437b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38833 2023-06-09 14:07:27.000000 blaster-server-0.0.437b0/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    43733 2023-06-24 12:52:51.000000 blaster-server-0.0.437b0/blaster/tools/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.437b0/blaster/tools/sanitize_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.437b0/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.437b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-17 08:57:19.000000 blaster-server-0.0.437b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.437b0/test/test_command_line_parser.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.437b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.437/LICENSE.txt` & `blaster-server-0.0.437b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/PKG-INFO` & `blaster-server-0.0.437b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.437
+Version: 0.0.437b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.437/README.md` & `blaster-server-0.0.437b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/__init__.py` & `blaster-server-0.0.437b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/cloud/analytics.py` & `blaster-server-0.0.437b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.437b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/cloud/push_tasks.py` & `blaster-server-0.0.437b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/cloud/storage.py` & `blaster-server-0.0.437b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/config.py` & `blaster-server-0.0.437b0/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/connection_pool.py` & `blaster-server-0.0.437b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/env.py` & `blaster-server-0.0.437b0/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/logging.py` & `blaster-server-0.0.437b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/mongo_orm.py` & `blaster-server-0.0.437b0/blaster/mongo_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1219,15 +1219,15 @@
 			handler(*obj)
 
 	def before_update(self):
 		pass
 
 	@property
 	def updated_at(self):
-		return self._original_doc.get("_")
+		return self._original_doc.get("_", 0)
 
 	def commit(
 		self, force=False, ignore_exceptions=None,
 		conditions=None, _transaction=None
 	):
 		cls = self.__class__
 		committed = False
@@ -1762,73 +1762,47 @@
 	IS_DEV \
 		and DEBUG_PRINT_LEVEL > 8 \
 		and print(
 			"\n\n#MONGO collection tracker key",
 			_Model._collection_tracker_key_
 		)
 
+	# FIND ALL DB NODES THIS TABLE IS SHARED TO
 	if(_Model not in [CollectionTracker]):
 		collection_tracker = CollectionTracker.get(_Model._collection_tracker_key_)
-		if(
-			not collection_tracker
-			or not collection_tracker.db_nodes
-			or not collection_tracker.primary_shard_key
-		):
-			print(
-				"\n\n#MONGOORM_IMPORTANT_INFO : "
-				"Collection tracker entry not present for '{:s}'.."
-				"creating table in control node for this time in database '{:s}'. "
-				"You may want to talk to dba to move to a proper node".format(
-					_Model.__name__, _Model._db_name_
-				)
+		if(collection_tracker):
+			_Model._db_nodes_ = tuple(
+				DatabaseNode(**_db_node)
+					for _db_node in collection_tracker.db_nodes
 			)
-
-			# check if the _Model already has _db_nodes_
-			_collection_tracker_node = CollectionTracker._db_nodes_[0]
-			db_node = {
-				"hosts": _collection_tracker_node.hosts,
-				"replicaset": _collection_tracker_node.replicaset,
-				"at": 0,
-				"username": _collection_tracker_node.username,
-				"password": _collection_tracker_node.password,
-				"db_name": _Model._db_name_
-			}
-
-			collection_tracker = CollectionTracker(
-				_id=_Model._collection_tracker_key_,
-				db_nodes=[db_node],
-				is_primary_shard=1 if not _Model._is_secondary_shard else 0,
-				primary_shard_key=_Model._shard_key_,
-				secondary_shard_keys=list(_Model._secondary_shards_.keys()),
-				pk_attrs=list(_Model._pk_attrs.keys()),
-				attrs=list(_Model._attrs_.keys())
-			).commit(force=True)
-
-		# version < 101 support
-		if(not collection_tracker.attrs):
-			collection_tracker.attrs = list(_Model._attrs_.keys())
-			collection_tracker.commit()
-
-		_Model._db_nodes_ = tuple(
-			DatabaseNode(**_db_node)
-			for _db_node in collection_tracker.db_nodes
-		)
-		# TODO: find new secondary shards by comparing 
-		# collection_tracker.secondary_shard_keys, _Model._secondary_shards_.keys()
-		# and create a job to create and reindex all data to secondary index
-		if(
-			not _Model._is_secondary_shard
-			and _Model._secondary_shards_
-			and collection_tracker.primary_shard_key != _Model._shard_key_
-		):
-			raise Exception(
-				"\n\n#MONGO_EXCEPTION: Primary shard key changed for ",
-				_Model, 
-				"It has secondary shards, that point to primary shard key. ",
-				"You will have to drop shard secondary shards and force reindex everything again. "
+			if(
+				not _Model._is_secondary_shard
+				and _Model._secondary_shards_
+				and collection_tracker.primary_shard_key != _Model._shard_key_
+			):
+				raise Exception(
+					"\n\n#MONGO_EXCEPTION: Primary shard key changed for ",
+					_Model,
+					"It has secondary shards, that point to primary shard key. ",
+					"You will have to drop shard secondary shards and force reindex everything again. "
+				)
+		else:
+			# just single db node, initialize on the default db node given
+			init_db_node = CollectionTracker._db_nodes_[0]
+			_Model._db_nodes_ = (  # tuple
+				DatabaseNode(
+					**{
+						"hosts": init_db_node.hosts,
+						"replicaset": init_db_node.replicaset,
+						"at": 0,
+						"username": init_db_node.username,
+						"password": init_db_node.password,
+						"db_name": _Model._db_name_
+					}
+				),
 			)
 
 		# check if new attribute added to secondary shard
 
 	# TODO: create or delete index using control jobs
 	# list existing indexes
 	existing_indexes = {}
@@ -1972,20 +1946,20 @@
 		db_nodes = [DatabaseNode(**db_nodes)]
 	elif(isinstance(db_nodes, list)):
 		db_nodes = [DatabaseNode(**db_node) for db_node in db_nodes]
 	else:
 		raise Exception(
 			f"argument must be a list of dicts, or a single dict, not {type(db_nodes)}"
 		)
-	# check connection to mongodb
+	# check connection to mongodbs
 	[db_node.mongo_client.server_info() for db_node in db_nodes]
 
 	# initialize control db
 	CollectionTracker._db_nodes_ = db_nodes
-	initialize_model([CollectionTracker])
+	initialize_model(CollectionTracker)
 
 	# set default db name for each class
 	for cls in all_subclasses(Model):
 		if(not getattr(cls, "_db_name_", None)):
 			cls._db_name_ = default_db_name
 		initialize_model(cls)
```

### Comparing `blaster-server-0.0.437/blaster/schema.py` & `blaster-server-0.0.437b0/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/server.py` & `blaster-server-0.0.437b0/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/tools/__init__.py` & `blaster-server-0.0.437b0/blaster/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,25 +196,22 @@
 	ret = cls()
 	for key in kwargs:
 		setattr(ret, key, kwargs[key])
 	return ret
 
 
 def get_by_key_list(d, key_list, default=None):
-	for key in key_list:
-		if(not d):
-			return default
-		if(isinstance(d, list)):
-			key = int(key)
-			if(key >= len(d) or key < 0):
-				return default  # dead end
+	try:
+		for key in key_list:
 			d = d[key]
-		else:
-			d = d.get(key, None)
-	return d
+		return d
+	except KeyError:
+		return default
+	except IndexError:
+		return default
 
 
 def set_by_key_list(d, key_list, value):
 	if(not key_list):
 		return
 	for key in key_list[0:-1]:
 		if(key not in d):
@@ -748,15 +745,15 @@
 	try:
 		return base64.b64decode(_value)
 	except Exception:
 		return None
 
 
 def hmac_hexdigest(secret, *parts) -> bytes:
-	hash = hmac.new(utf8(secret), digestmod=hashlib.sha1)
+	hash = hmac.new(utf8(secret), digestmod=hashlib.sha256)
 	for part in parts:
 		hash.update(utf8(part))
 	return utf8(hash.hexdigest())
 
 
 """Dependencies are expressed as a dictionary whose keys are items
 	and whose values are a set of dependent items. Output is a list of
@@ -1674,15 +1671,15 @@
 	)
 
 
 # print debugging info for networks request called with requests
 def debug_requests_on():
 	import logging
 	'''Switches on logging of the requests module.'''
-	HTTPConnection.debuglevel = 1
+	HTTPConnection.debuglevel = 3
 	logging.basicConfig()
 	logging.getLogger().setLevel(logging.DEBUG)
 	requests_log = logging.getLogger("requests.packages.urllib3")
 	requests_log.setLevel(logging.DEBUG)
 	requests_log.propagate = True
```

### Comparing `blaster-server-0.0.437/blaster/tools/sanitize_html.py` & `blaster-server-0.0.437b0/blaster/tools/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/data/countries.json` & `blaster-server-0.0.437b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/data/mime_types.json` & `blaster-server-0.0.437b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/data_utils.py` & `blaster-server-0.0.437b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/events.py` & `blaster-server-0.0.437b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/fork.py` & `blaster-server-0.0.437b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.437b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.437b0/blaster/utils/phone_number_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from .data_utils import COUNTRY_DATA
 
 
 NON_DIGITS = re.compile(r"[^0-9]")
 
-country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "256": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
+country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "256": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [9], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
 
 
 class SimpleTrie(dict):
 	end_obj = None
 
 
 country_code_num_digits_trie = SimpleTrie()
```

### Comparing `blaster-server-0.0.437/blaster/utils/xss_html.py` & `blaster-server-0.0.437b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/__init__.py` & `blaster-server-0.0.437b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_abnf.py` & `blaster-server-0.0.437b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_app.py` & `blaster-server-0.0.437b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_core.py` & `blaster-server-0.0.437b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_exceptions.py` & `blaster-server-0.0.437b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_handshake.py` & `blaster-server-0.0.437b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_http.py` & `blaster-server-0.0.437b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_logging.py` & `blaster-server-0.0.437b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_socket.py` & `blaster-server-0.0.437b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.437b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_url.py` & `blaster-server-0.0.437b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/_utils.py` & `blaster-server-0.0.437b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/server.py` & `blaster-server-0.0.437b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.437b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.437b0/blaster_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.437
+Version: 0.0.437b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.437/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.437b0/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/examples/gevent_wsgi_test.py` & `blaster-server-0.0.437b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/examples/mongo_ormexample.py` & `blaster-server-0.0.437b0/examples/mongo_ormexample.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 		self.updated_at = cur_ms()
 
 	_index_ = [
 				(company, agent_user_id),
 				(company, load, {"unique": False})
 			]
 
-
-
 #call this function after you import all mongo db classes/models
 def initialize_mongo():
 	nodes = []
 	if IS_DEV:
 		nodes.append(Connection(host="localhost", port=27017, db_name="xyz"))
 	else:
 		nodes.append(Connection(host="mongodb://mongo-0.mongo.default.svc/", port=27017, db_name="xyz"))
```

### Comparing `blaster-server-0.0.437/examples/simple_examples.py` & `blaster-server-0.0.437b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/examples/test_chat_room.py` & `blaster-server-0.0.437b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/examples/tornado_hello_world.py` & `blaster-server-0.0.437b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/examples/wheezy_hello.py` & `blaster-server-0.0.437b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/setup.py` & `blaster-server-0.0.437b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.437',
+	version='0.0.437b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.437/test/test_mongo_orm.py` & `blaster-server-0.0.437b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/test/test_phone_number_utils.py` & `blaster-server-0.0.437b0/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/test/test_schema.py` & `blaster-server-0.0.437b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/test/test_tools.py` & `blaster-server-0.0.437b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/test/test_utils.py` & `blaster-server-0.0.437b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437/test/timeit_snippets.py` & `blaster-server-0.0.437b0/test/timeit_snippets.py`

 * *Files identical despite different names*

