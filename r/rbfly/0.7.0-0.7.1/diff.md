# Comparing `tmp/rbfly-0.7.0.tar.gz` & `tmp/rbfly-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfly-0.7.0.tar", last modified: Wed Jun 21 20:27:27 2023, max compression
+gzip compressed data, was "rbfly-0.7.1.tar", last modified: Sun Jun 25 18:55:01 2023, max compression
```

## Comparing `rbfly-0.7.0.tar` & `rbfly-0.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.231404 rbfly-0.7.0/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2023-01-11 23:13:37.000000 rbfly-0.7.0/COPYING
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-21 20:27:27.231404 rbfly-0.7.0/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-06-19 18:52:56.000000 rbfly-0.7.0/README
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      183 2023-06-09 14:43:29.000000 rbfly-0.7.0/pyproject.toml
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.228070 rbfly-0.7.0/rbfly/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      935 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   171073 2023-06-15 10:14:14.000000 rbfly-0.7.0/rbfly/_buffer.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1435 2023-01-16 12:48:43.000000 rbfly-0.7.0/rbfly/_buffer.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2023-06-15 10:13:38.000000 rbfly-0.7.0/rbfly/_buffer.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   160017 2023-06-15 10:14:14.000000 rbfly-0.7.0/rbfly/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/_codec.h
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2023-05-29 23:14:21.000000 rbfly-0.7.0/rbfly/_codec.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2023-06-15 10:13:38.000000 rbfly-0.7.0/rbfly/_codec.pyx
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.228070 rbfly-0.7.0/rbfly/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   677200 2023-06-16 12:22:42.000000 rbfly-0.7.0/rbfly/amqp/_message.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1617 2023-06-14 21:25:05.000000 rbfly-0.7.0/rbfly/amqp/_message.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1538 2023-06-15 21:01:28.000000 rbfly-0.7.0/rbfly/amqp/_message.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20434 2023-06-16 12:09:23.000000 rbfly-0.7.0/rbfly/amqp/_message.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3894 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/cm.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2023-01-30 14:42:53.000000 rbfly-0.7.0/rbfly/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/py.typed
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.231404 rbfly-0.7.0/rbfly/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1685 2023-06-15 16:46:02.000000 rbfly-0.7.0/rbfly/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1131466 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly/streams/_client.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2344 2023-06-18 11:23:29.000000 rbfly-0.7.0/rbfly/streams/_client.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15929 2023-06-18 19:34:29.000000 rbfly-0.7.0/rbfly/streams/_client.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   672712 2023-06-15 16:13:04.000000 rbfly-0.7.0/rbfly/streams/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1563 2023-06-10 19:30:42.000000 rbfly-0.7.0/rbfly/streams/_codec.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12460 2023-06-15 14:54:51.000000 rbfly-0.7.0/rbfly/streams/_codec.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   463176 2023-06-15 10:14:15.000000 rbfly-0.7.0/rbfly/streams/_mqueue.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2023-02-01 18:34:41.000000 rbfly-0.7.0/rbfly/streams/_mqueue.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3933 2023-06-15 10:13:38.000000 rbfly-0.7.0/rbfly/streams/_mqueue.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18040 2023-06-21 19:23:30.000000 rbfly-0.7.0/rbfly/streams/client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8690 2023-06-10 20:40:38.000000 rbfly-0.7.0/rbfly/streams/codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2023-02-01 15:06:50.000000 rbfly-0.7.0/rbfly/streams/const.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1103 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/streams/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5229 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/streams/offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    29111 2023-06-13 20:22:14.000000 rbfly-0.7.0/rbfly/streams/protocol.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1075 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/streams/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4004 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/streams/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.231404 rbfly-0.7.0/rbfly/tests/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/tests/__init__.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.231404 rbfly-0.7.0/rbfly/tests/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/tests/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10104 2023-06-16 12:13:33.000000 rbfly-0.7.0/rbfly/tests/amqp/test_message.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.231404 rbfly-0.7.0/rbfly/tests/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/tests/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    13944 2023-06-19 07:59:59.000000 rbfly-0.7.0/rbfly/tests/streams/test_client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    14725 2023-06-10 22:58:17.000000 rbfly-0.7.0/rbfly/tests/streams/test_codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2271 2023-02-01 15:02:22.000000 rbfly-0.7.0/rbfly/tests/streams/test_mqueue.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1344 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/tests/streams/test_offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/tests/test_util.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2287 2023-06-15 16:54:08.000000 rbfly-0.7.0/rbfly/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2023-01-11 23:13:37.000000 rbfly-0.7.0/rbfly/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-21 20:27:27.228070 rbfly-0.7.0/rbfly.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1235 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      216 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2023-06-21 20:27:27.000000 rbfly-0.7.0/rbfly.egg-info/top_level.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1422 2023-06-21 20:27:27.231404 rbfly-0.7.0/setup.cfg
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1705 2023-06-15 10:13:31.000000 rbfly-0.7.0/setup.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2023-01-11 23:13:37.000000 rbfly-0.7.1/COPYING
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-25 18:55:01.419360 rbfly-0.7.1/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-06-19 18:52:56.000000 rbfly-0.7.1/README
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      183 2023-06-09 14:43:29.000000 rbfly-0.7.1/pyproject.toml
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.406026 rbfly-0.7.1/rbfly/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      935 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   171073 2023-06-25 08:30:58.000000 rbfly-0.7.1/rbfly/_buffer.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1435 2023-01-16 12:48:43.000000 rbfly-0.7.1/rbfly/_buffer.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/_buffer.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   160017 2023-06-25 08:30:58.000000 rbfly-0.7.1/rbfly/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/_codec.h
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2023-05-29 23:14:21.000000 rbfly-0.7.1/rbfly/_codec.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/_codec.pyx
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.409360 rbfly-0.7.1/rbfly/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   677200 2023-06-25 08:30:59.000000 rbfly-0.7.1/rbfly/amqp/_message.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1617 2023-06-14 21:25:05.000000 rbfly-0.7.1/rbfly/amqp/_message.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1538 2023-06-15 21:01:28.000000 rbfly-0.7.1/rbfly/amqp/_message.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20434 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/amqp/_message.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3894 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/cm.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2023-01-30 14:42:53.000000 rbfly-0.7.1/rbfly/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/py.typed
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1685 2023-06-15 16:46:02.000000 rbfly-0.7.1/rbfly/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1168133 2023-06-25 08:30:59.000000 rbfly-0.7.1/rbfly/streams/_client.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2350 2023-06-25 07:47:11.000000 rbfly-0.7.1/rbfly/streams/_client.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15997 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_client.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   672712 2023-06-25 08:31:00.000000 rbfly-0.7.1/rbfly/streams/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1563 2023-06-10 19:30:42.000000 rbfly-0.7.1/rbfly/streams/_codec.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12460 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_codec.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   463176 2023-06-25 08:31:00.000000 rbfly-0.7.1/rbfly/streams/_mqueue.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2023-02-01 18:34:41.000000 rbfly-0.7.1/rbfly/streams/_mqueue.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3933 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_mqueue.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18064 2023-06-25 07:49:01.000000 rbfly-0.7.1/rbfly/streams/client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8690 2023-06-10 20:40:38.000000 rbfly-0.7.1/rbfly/streams/codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2023-02-01 15:06:50.000000 rbfly-0.7.1/rbfly/streams/const.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1103 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5229 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    29111 2023-06-13 20:22:14.000000 rbfly-0.7.1/rbfly/streams/protocol.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1075 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4004 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/__init__.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10104 2023-06-16 12:13:33.000000 rbfly-0.7.1/rbfly/tests/amqp/test_message.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    13944 2023-06-19 07:59:59.000000 rbfly-0.7.1/rbfly/tests/streams/test_client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    14725 2023-06-10 22:58:17.000000 rbfly-0.7.1/rbfly/tests/streams/test_codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2271 2023-02-01 15:02:22.000000 rbfly-0.7.1/rbfly/tests/streams/test_mqueue.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1344 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/streams/test_offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/test_util.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2287 2023-06-15 16:54:08.000000 rbfly-0.7.1/rbfly/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.406026 rbfly-0.7.1/rbfly.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1235 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      216 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/top_level.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1422 2023-06-25 18:55:01.422693 rbfly-0.7.1/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1705 2023-06-15 10:13:31.000000 rbfly-0.7.1/setup.py
```

### Comparing `rbfly-0.7.0/COPYING` & `rbfly-0.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/PKG-INFO` & `rbfly-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.7.0
+Version: 0.7.1
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
```

### Comparing `rbfly-0.7.0/README` & `rbfly-0.7.1/README`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/__init__.py` & `rbfly-0.7.1/rbfly/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_buffer.c` & `rbfly-0.7.1/rbfly/_buffer.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_buffer.pxd` & `rbfly-0.7.1/rbfly/_buffer.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_buffer.pyx` & `rbfly-0.7.1/rbfly/_buffer.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_codec.c` & `rbfly-0.7.1/rbfly/_codec.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_codec.h` & `rbfly-0.7.1/rbfly/_codec.h`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_codec.pxd` & `rbfly-0.7.1/rbfly/_codec.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/_codec.pyx` & `rbfly-0.7.1/rbfly/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/amqp/__init__.py` & `rbfly-0.7.1/rbfly/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/amqp/_message.c` & `rbfly-0.7.1/rbfly/amqp/_message.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/amqp/_message.pxd` & `rbfly-0.7.1/rbfly/amqp/_message.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/amqp/_message.pyi` & `rbfly-0.7.1/rbfly/amqp/_message.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/amqp/_message.pyx` & `rbfly-0.7.1/rbfly/amqp/_message.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/cm.py` & `rbfly-0.7.1/rbfly/cm.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/error.py` & `rbfly-0.7.1/rbfly/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/__init__.py` & `rbfly-0.7.1/rbfly/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_client.c` & `rbfly-0.7.1/rbfly/streams/_client.c`

 * *Files 1% similar despite different names*

```diff
@@ -1369,15 +1369,15 @@
   Py_ssize_t __pyx_v_count;
   PyObject *__pyx_v_data;
   struct __pyx_obj_5rbfly_7streams_7_client_PublisherBatchTrait *__pyx_v_publisher;
 };
 
 
 /* "rbfly/streams/_client.pyx":482
- *         self.message: MessageCtx | None = None
+ *         self._message: MessageCtx | None = None
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ {
   PyObject_HEAD
@@ -1529,21 +1529,21 @@
  * 
  * cdef class Subscriber:             # <<<<<<<<<<<<<<
  *     """
  *     RabbitMQ stream subscriber.
  */
 struct __pyx_obj_5rbfly_7streams_7_client_Subscriber {
   PyObject_HEAD
-  PyObject *client;
-  PyObject *stream;
-  uint8_t subscription_id;
-  PyObject *offset;
-  float timeout;
-  char amqp;
-  struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *message;
+  PyObject *_client;
+  PyObject *_stream;
+  uint8_t _subscription_id;
+  PyObject *_offset;
+  float _timeout;
+  char _amqp;
+  struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *_message;
 };
 
 
 /* "rbfly/streams/_client.pyx":98
  *         ...
  * 
  * cdef class PublisherTrait:             # <<<<<<<<<<<<<<
@@ -2595,14 +2595,17 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint8_t(uint8_t value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
@@ -2909,14 +2912,32 @@
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_12PublisherBin_5__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBin *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_batch(struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self, PyObject *__pyx_v_message); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_2flush(struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber___cinit__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_client, PyObject *__pyx_v_stream, PyObject *__pyx_v_subscription_id, PyObject *__pyx_v_offset, double __pyx_v_timeout, PyObject *__pyx_v_amqp); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_2__aiter__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_2_flush_messages(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5rbfly_7streams_7_client_PublisherBatchTrait *__pyx_v_publisher, PyObject *__pyx_v_data, PyObject *__pyx_v_amqp); /* proto */
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_6_flush(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_5_send(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -11146,15 +11167,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "rbfly/streams/_client.pyx":462
- *         MessageCtx message
+ *         public MessageCtx _message
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *             self,
  *             client,
  */
 
 /* Python wrapper */
@@ -11288,94 +11309,94 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "rbfly/streams/_client.pyx":474
  *         Create RabbitMQ stream subscriber.
  *         """
- *         self.client = client             # <<<<<<<<<<<<<<
- *         self.stream = stream
- *         self.subscription_id = subscription_id
+ *         self._client = client             # <<<<<<<<<<<<<<
+ *         self._stream = stream
+ *         self._subscription_id = subscription_id
  */
   __Pyx_INCREF(__pyx_v_client);
   __Pyx_GIVEREF(__pyx_v_client);
-  __Pyx_GOTREF(__pyx_v_self->client);
-  __Pyx_DECREF(__pyx_v_self->client);
-  __pyx_v_self->client = __pyx_v_client;
+  __Pyx_GOTREF(__pyx_v_self->_client);
+  __Pyx_DECREF(__pyx_v_self->_client);
+  __pyx_v_self->_client = __pyx_v_client;
 
   /* "rbfly/streams/_client.pyx":475
  *         """
- *         self.client = client
- *         self.stream = stream             # <<<<<<<<<<<<<<
- *         self.subscription_id = subscription_id
- *         self.offset = offset
+ *         self._client = client
+ *         self._stream = stream             # <<<<<<<<<<<<<<
+ *         self._subscription_id = subscription_id
+ *         self._offset = offset
  */
   __Pyx_INCREF(__pyx_v_stream);
   __Pyx_GIVEREF(__pyx_v_stream);
-  __Pyx_GOTREF(__pyx_v_self->stream);
-  __Pyx_DECREF(__pyx_v_self->stream);
-  __pyx_v_self->stream = __pyx_v_stream;
+  __Pyx_GOTREF(__pyx_v_self->_stream);
+  __Pyx_DECREF(__pyx_v_self->_stream);
+  __pyx_v_self->_stream = __pyx_v_stream;
 
   /* "rbfly/streams/_client.pyx":476
- *         self.client = client
- *         self.stream = stream
- *         self.subscription_id = subscription_id             # <<<<<<<<<<<<<<
- *         self.offset = offset
- *         self.timeout = timeout
+ *         self._client = client
+ *         self._stream = stream
+ *         self._subscription_id = subscription_id             # <<<<<<<<<<<<<<
+ *         self._offset = offset
+ *         self._timeout = timeout
  */
   __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_subscription_id); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 476, __pyx_L1_error)
-  __pyx_v_self->subscription_id = __pyx_t_1;
+  __pyx_v_self->_subscription_id = __pyx_t_1;
 
   /* "rbfly/streams/_client.pyx":477
- *         self.stream = stream
- *         self.subscription_id = subscription_id
- *         self.offset = offset             # <<<<<<<<<<<<<<
- *         self.timeout = timeout
- *         self.amqp = amqp
+ *         self._stream = stream
+ *         self._subscription_id = subscription_id
+ *         self._offset = offset             # <<<<<<<<<<<<<<
+ *         self._timeout = timeout
+ *         self._amqp = amqp
  */
   __Pyx_INCREF(__pyx_v_offset);
   __Pyx_GIVEREF(__pyx_v_offset);
-  __Pyx_GOTREF(__pyx_v_self->offset);
-  __Pyx_DECREF(__pyx_v_self->offset);
-  __pyx_v_self->offset = __pyx_v_offset;
+  __Pyx_GOTREF(__pyx_v_self->_offset);
+  __Pyx_DECREF(__pyx_v_self->_offset);
+  __pyx_v_self->_offset = __pyx_v_offset;
 
   /* "rbfly/streams/_client.pyx":478
- *         self.subscription_id = subscription_id
- *         self.offset = offset
- *         self.timeout = timeout             # <<<<<<<<<<<<<<
- *         self.amqp = amqp
- *         self.message: MessageCtx | None = None
+ *         self._subscription_id = subscription_id
+ *         self._offset = offset
+ *         self._timeout = timeout             # <<<<<<<<<<<<<<
+ *         self._amqp = amqp
+ *         self._message: MessageCtx | None = None
  */
-  __pyx_v_self->timeout = __pyx_v_timeout;
+  __pyx_v_self->_timeout = __pyx_v_timeout;
 
   /* "rbfly/streams/_client.pyx":479
- *         self.offset = offset
- *         self.timeout = timeout
- *         self.amqp = amqp             # <<<<<<<<<<<<<<
- *         self.message: MessageCtx | None = None
+ *         self._offset = offset
+ *         self._timeout = timeout
+ *         self._amqp = amqp             # <<<<<<<<<<<<<<
+ *         self._message: MessageCtx | None = None
  * 
  */
   __pyx_t_2 = __Pyx_PyInt_As_char(__pyx_v_amqp); if (unlikely((__pyx_t_2 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 479, __pyx_L1_error)
-  __pyx_v_self->amqp = __pyx_t_2;
+  __pyx_v_self->_amqp = __pyx_t_2;
 
   /* "rbfly/streams/_client.pyx":480
- *         self.timeout = timeout
- *         self.amqp = amqp
- *         self.message: MessageCtx | None = None             # <<<<<<<<<<<<<<
+ *         self._timeout = timeout
+ *         self._amqp = amqp
+ *         self._message: MessageCtx | None = None             # <<<<<<<<<<<<<<
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  __Pyx_GOTREF((PyObject *)__pyx_v_self->message);
-  __Pyx_DECREF((PyObject *)__pyx_v_self->message);
-  __pyx_v_self->message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None);
+  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
+  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
+  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None);
 
   /* "rbfly/streams/_client.pyx":462
- *         MessageCtx message
+ *         public MessageCtx _message
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *             self,
  *             client,
  */
 
   /* function exit code */
@@ -11387,15 +11408,15 @@
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_5rbfly_7streams_7_client_10Subscriber_4generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "rbfly/streams/_client.pyx":482
- *         self.message: MessageCtx | None = None
+ *         self._message: MessageCtx | None = None
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 
 /* Python wrapper */
@@ -11482,29 +11503,29 @@
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 482, __pyx_L1_error)
 
   /* "rbfly/streams/_client.pyx":487
  *         """
  *         cdef:
- *             float timeout = self.timeout             # <<<<<<<<<<<<<<
- *             object client = self.client
+ *             float timeout = self._timeout             # <<<<<<<<<<<<<<
+ *             object client = self._client
  *             object messages
  */
-  __pyx_t_1 = __pyx_cur_scope->__pyx_v_self->timeout;
+  __pyx_t_1 = __pyx_cur_scope->__pyx_v_self->_timeout;
   __pyx_cur_scope->__pyx_v_timeout = __pyx_t_1;
 
   /* "rbfly/streams/_client.pyx":488
  *         cdef:
- *             float timeout = self.timeout
- *             object client = self.client             # <<<<<<<<<<<<<<
+ *             float timeout = self._timeout
+ *             object client = self._client             # <<<<<<<<<<<<<<
  *             object messages
  *             object protocol
  */
-  __pyx_t_2 = __pyx_cur_scope->__pyx_v_self->client;
+  __pyx_t_2 = __pyx_cur_scope->__pyx_v_self->_client;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_client = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "rbfly/streams/_client.pyx":493
  *             object task
@@ -11516,28 +11537,28 @@
   while (1) {
 
     /* "rbfly/streams/_client.pyx":494
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  */
     {
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
         /* "rbfly/streams/_client.pyx":495
  *         while True:
  *             try:
  *                 protocol = await client.get_protocol()             # <<<<<<<<<<<<<<
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:
  */
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_client, __pyx_n_s_get_protocol); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
@@ -11595,21 +11616,21 @@
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_protocol, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_t_2 = 0;
 
         /* "rbfly/streams/_client.pyx":496
  *             try:
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)             # <<<<<<<<<<<<<<
+ *                 task = protocol.read_stream(self._subscription_id)             # <<<<<<<<<<<<<<
  *                 if timeout:
  *                     task = asyncio.wait_for(task, timeout)
  */
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_protocol, __pyx_n_s_read_stream); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 496, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_self->subscription_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 496, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 496, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_9 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11631,24 +11652,24 @@
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_task);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_task, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_t_2 = 0;
 
         /* "rbfly/streams/_client.pyx":497
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:             # <<<<<<<<<<<<<<
  *                     task = asyncio.wait_for(task, timeout)
  *                 messages = await task
  */
         __pyx_t_10 = (__pyx_cur_scope->__pyx_v_timeout != 0);
         if (__pyx_t_10) {
 
           /* "rbfly/streams/_client.pyx":498
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:
  *                     task = asyncio.wait_for(task, timeout)             # <<<<<<<<<<<<<<
  *                 messages = await task
  *             except ConnectionError:
  */
           __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_asyncio); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 498, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_6);
@@ -11681,15 +11702,15 @@
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_task);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_task, __pyx_t_2);
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
 
           /* "rbfly/streams/_client.pyx":497
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:             # <<<<<<<<<<<<<<
  *                     task = asyncio.wait_for(task, timeout)
  *                 messages = await task
  */
         }
 
         /* "rbfly/streams/_client.pyx":499
@@ -11737,35 +11758,35 @@
         __pyx_t_2 = 0;
 
         /* "rbfly/streams/_client.pyx":494
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  */
       }
 
       /* "rbfly/streams/_client.pyx":503
  *                 pass
  *             else:
  *                 while messages:             # <<<<<<<<<<<<<<
- *                     self.message = messages.popleft()
- *                     yield self.message
+ *                     self._message = messages.popleft()
+ *                     yield self._message
  */
       /*else:*/ {
         while (1) {
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_messages); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 503, __pyx_L8_except_error)
           if (!__pyx_t_10) break;
 
           /* "rbfly/streams/_client.pyx":504
  *             else:
  *                 while messages:
- *                     self.message = messages.popleft()             # <<<<<<<<<<<<<<
- *                     yield self.message
+ *                     self._message = messages.popleft()             # <<<<<<<<<<<<<<
+ *                     yield self._message
  * 
  */
           __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_messages, __pyx_n_s_popleft); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 504, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_7);
           __pyx_t_6 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
@@ -11784,28 +11805,28 @@
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
             if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 504, __pyx_L8_except_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
           if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 504, __pyx_L8_except_error)
           __Pyx_GIVEREF(__pyx_t_2);
-          __Pyx_GOTREF((PyObject *)__pyx_cur_scope->__pyx_v_self->message);
-          __Pyx_DECREF((PyObject *)__pyx_cur_scope->__pyx_v_self->message);
-          __pyx_cur_scope->__pyx_v_self->message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_2);
+          __Pyx_GOTREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
+          __Pyx_DECREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
+          __pyx_cur_scope->__pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_2);
           __pyx_t_2 = 0;
 
           /* "rbfly/streams/_client.pyx":505
  *                 while messages:
- *                     self.message = messages.popleft()
- *                     yield self.message             # <<<<<<<<<<<<<<
+ *                     self._message = messages.popleft()
+ *                     yield self._message             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  */
-          __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self->message);
-          __pyx_r = ((PyObject *)__pyx_cur_scope->__pyx_v_self->message);
+          __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
+          __pyx_r = ((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
           __Pyx_XGIVEREF(__pyx_t_3);
           __pyx_cur_scope->__pyx_t_0 = __pyx_t_3;
           __Pyx_XGIVEREF(__pyx_t_4);
           __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
           __Pyx_XGIVEREF(__pyx_t_5);
           __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
           __Pyx_XGIVEREF(__pyx_r);
@@ -11859,15 +11880,15 @@
       __pyx_L8_except_error:;
 
       /* "rbfly/streams/_client.pyx":494
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
- *                 task = protocol.read_stream(self.subscription_id)
+ *                 task = protocol.read_stream(self._subscription_id)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L1_error;
       __pyx_L7_exception_handled:;
@@ -11877,15 +11898,15 @@
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       __pyx_L13_try_end:;
     }
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* "rbfly/streams/_client.pyx":482
- *         self.message: MessageCtx | None = None
+ *         self._message: MessageCtx | None = None
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 
   /* function exit code */
@@ -11905,14 +11926,684 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "rbfly/streams/_client.pyx":454
+ *     """
+ *     cdef:
+ *         public object _client             # <<<<<<<<<<<<<<
+ *         public str _stream
+ *         public uint8_t _subscription_id
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_client);
+  __pyx_r = __pyx_v_self->_client;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_GIVEREF(__pyx_v_value);
+  __Pyx_GOTREF(__pyx_v_self->_client);
+  __Pyx_DECREF(__pyx_v_self->_client);
+  __pyx_v_self->_client = __pyx_v_value;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_5__del__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_client);
+  __Pyx_DECREF(__pyx_v_self->_client);
+  __pyx_v_self->_client = Py_None;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":455
+ *     cdef:
+ *         public object _client
+ *         public str _stream             # <<<<<<<<<<<<<<
+ *         public uint8_t _subscription_id
+ *         public object _offset
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_stream);
+  __pyx_r = __pyx_v_self->_stream;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(1, 455, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_value;
+  __Pyx_INCREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->_stream);
+  __Pyx_DECREF(__pyx_v_self->_stream);
+  __pyx_v_self->_stream = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._stream.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_5__del__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_stream);
+  __Pyx_DECREF(__pyx_v_self->_stream);
+  __pyx_v_self->_stream = ((PyObject*)Py_None);
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":456
+ *         public object _client
+ *         public str _stream
+ *         public uint8_t _subscription_id             # <<<<<<<<<<<<<<
+ *         public object _offset
+ *         public float _timeout
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 456, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._subscription_id.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  uint8_t __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 456, __pyx_L1_error)
+  __pyx_v_self->_subscription_id = __pyx_t_1;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._subscription_id.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":457
+ *         public str _stream
+ *         public uint8_t _subscription_id
+ *         public object _offset             # <<<<<<<<<<<<<<
+ *         public float _timeout
+ *         public char _amqp
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_offset);
+  __pyx_r = __pyx_v_self->_offset;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_GIVEREF(__pyx_v_value);
+  __Pyx_GOTREF(__pyx_v_self->_offset);
+  __Pyx_DECREF(__pyx_v_self->_offset);
+  __pyx_v_self->_offset = __pyx_v_value;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_5__del__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_offset);
+  __Pyx_DECREF(__pyx_v_self->_offset);
+  __pyx_v_self->_offset = Py_None;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":458
+ *         public uint8_t _subscription_id
+ *         public object _offset
+ *         public float _timeout             # <<<<<<<<<<<<<<
+ *         public char _amqp
+ *         public MessageCtx _message
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 458, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._timeout.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  float __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 458, __pyx_L1_error)
+  __pyx_v_self->_timeout = __pyx_t_1;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._timeout.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":459
+ *         public object _offset
+ *         public float _timeout
+ *         public char _amqp             # <<<<<<<<<<<<<<
+ *         public MessageCtx _message
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->_amqp); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 459, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._amqp.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  char __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __pyx_t_1 = __Pyx_PyInt_As_char(__pyx_v_value); if (unlikely((__pyx_t_1 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 459, __pyx_L1_error)
+  __pyx_v_self->_amqp = __pyx_t_1;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._amqp.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":460
+ *         public float _timeout
+ *         public char _amqp
+ *         public MessageCtx _message             # <<<<<<<<<<<<<<
+ * 
+ *     def __cinit__(
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_self->_message);
+  __pyx_r = ((PyObject *)__pyx_v_self->_message);
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 460, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_value;
+  __Pyx_INCREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
+  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
+  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._message.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
+  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
+  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None);
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
@@ -12089,15 +12780,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "rbfly/streams/_client.pyx":507
- *                     yield self.message
+ *                     yield self._message
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if not ctx.is_set_stream_publish_id:
  *         ctx.stream_publish_id = publisher.message_id
  */
 
 static CYTHON_INLINE void __pyx_f_5rbfly_7streams_7_client__before_ctx_publish(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_publisher, struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_v_ctx) {
@@ -12132,15 +12823,15 @@
  *     if not ctx.is_set_stream_publish_id:             # <<<<<<<<<<<<<<
  *         ctx.stream_publish_id = publisher.message_id
  * 
  */
   }
 
   /* "rbfly/streams/_client.pyx":507
- *                     yield self.message
+ *                     yield self._message
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if not ctx.is_set_stream_publish_id:
  *         ctx.stream_publish_id = publisher.message_id
  */
 
   /* function exit code */
@@ -14027,18 +14718,18 @@
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   #endif
   p = ((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o);
-  p->client = Py_None; Py_INCREF(Py_None);
-  p->stream = ((PyObject*)Py_None); Py_INCREF(Py_None);
-  p->offset = Py_None; Py_INCREF(Py_None);
-  p->message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
+  p->_client = Py_None; Py_INCREF(Py_None);
+  p->_stream = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  p->_offset = Py_None; Py_INCREF(Py_None);
+  p->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_5rbfly_7streams_7_client_10Subscriber_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
@@ -14048,69 +14739,175 @@
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client_Subscriber) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->client);
-  Py_CLEAR(p->stream);
-  Py_CLEAR(p->offset);
-  Py_CLEAR(p->message);
+  Py_CLEAR(p->_client);
+  Py_CLEAR(p->_stream);
+  Py_CLEAR(p->_offset);
+  Py_CLEAR(p->_message);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_5rbfly_7streams_7_client_Subscriber(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *p = (struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o;
-  if (p->client) {
-    e = (*v)(p->client, a); if (e) return e;
+  if (p->_client) {
+    e = (*v)(p->_client, a); if (e) return e;
   }
-  if (p->offset) {
-    e = (*v)(p->offset, a); if (e) return e;
+  if (p->_offset) {
+    e = (*v)(p->_offset, a); if (e) return e;
   }
-  if (p->message) {
-    e = (*v)(((PyObject *)p->message), a); if (e) return e;
+  if (p->_message) {
+    e = (*v)(((PyObject *)p->_message), a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_5rbfly_7streams_7_client_Subscriber(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *p = (struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o;
-  tmp = ((PyObject*)p->client);
-  p->client = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->_client);
+  p->_client = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->offset);
-  p->offset = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->_offset);
+  p->_offset = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->message);
-  p->message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->_message);
+  p->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__client(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__client(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_5__del__(o);
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__stream(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__stream(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_stream_5__del__(o);
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__subscription_id(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__subscription_id(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_16_subscription_id_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__offset(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__offset(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_offset_5__del__(o);
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__timeout(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__timeout(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__amqp(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__amqp(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__message(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__message(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(o);
+  }
+}
+
 static PyObject *__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
   return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(self);
 }
 
 static PyMethodDef __pyx_methods_5rbfly_7streams_7_client_Subscriber[] = {
   {"__aiter__", (PyCFunction)__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__, METH_NOARGS|METH_COEXIST, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_2__aiter__},
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__},
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__},
   {0, 0, 0, 0}
 };
+
+static struct PyGetSetDef __pyx_getsets_5rbfly_7streams_7_client_Subscriber[] = {
+  {(char *)"_client", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__client, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__client, (char *)PyDoc_STR("_client: object"), 0},
+  {(char *)"_stream", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__stream, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__stream, (char *)PyDoc_STR("_stream: unicode"), 0},
+  {(char *)"_subscription_id", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__subscription_id, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__subscription_id, (char *)PyDoc_STR("_subscription_id: 'uint8_t'"), 0},
+  {(char *)"_offset", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__offset, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__offset, (char *)PyDoc_STR("_offset: object"), 0},
+  {(char *)"_timeout", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__timeout, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__timeout, (char *)PyDoc_STR("_timeout: 'float'"), 0},
+  {(char *)"_amqp", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__amqp, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__amqp, (char *)PyDoc_STR("_amqp: 'char'"), 0},
+  {(char *)"_message", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__message, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__message, (char *)PyDoc_STR("_message: rbfly.amqp._message.MessageCtx"), 0},
+  {0, 0, 0, 0, 0}
+};
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_5rbfly_7streams_7_client_Subscriber_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_5rbfly_7streams_7_client_Subscriber},
   {Py_am_aiter, (void *)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__},
   {Py_tp_doc, (void *)PyDoc_STR("\n    RabbitMQ stream subscriber.\n\n    A stream subscriber holds information about RabbitMQ stream\n    subscription and is used to iterate over messages read from a stream.\n\n    :var client: RabbitMQ Streams client.\n    :var stream: RabbitMQ stream name.\n    :var subscription_id: RabbitMQ stream subscription id.\n    :var offset: RabbitMQ Streams offset specification.\n    :var timeout: Raise timeout error if no message within specified time\n        (in seconds).\n    :var message: Last received message or null.\n    :var amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP\n        decoding.\n    ")},
   {Py_tp_traverse, (void *)__pyx_tp_traverse_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_clear, (void *)__pyx_tp_clear_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_methods, (void *)__pyx_methods_5rbfly_7streams_7_client_Subscriber},
+  {Py_tp_getset, (void *)__pyx_getsets_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_new, (void *)__pyx_tp_new_5rbfly_7streams_7_client_Subscriber},
   {0, 0},
 };
 static PyType_Spec __pyx_type_5rbfly_7streams_7_client_Subscriber_spec = {
   "rbfly.streams._client.Subscriber",
   sizeof(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber),
   0,
@@ -14166,15 +14963,15 @@
   __pyx_tp_clear_5rbfly_7streams_7_client_Subscriber, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_5rbfly_7streams_7_client_Subscriber, /*tp_methods*/
   0, /*tp_members*/
-  0, /*tp_getset*/
+  __pyx_getsets_5rbfly_7streams_7_client_Subscriber, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
@@ -24104,14 +24901,52 @@
     return (char) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const char neg_one = (char) -1, const_zero = (char) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(char) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(char) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(char),
+                                     little, !is_unsigned);
+    }
+}
+
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
```

### Comparing `rbfly-0.7.0/rbfly/streams/_client.pyi` & `rbfly-0.7.1/rbfly/streams/_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     async def send(self, message: bytes) -> None: ...
 
 class PublisherBinBatch(PublisherBatchTrait):
     def batch(self, message: bytes) -> None: ...
     async def flush(self) -> None: ...
 
 class Subscriber:
-    stream: str
-    subscription_id: int
-    offset: Offset
-    timeout: float
-    amqp: bool
-    message: MessageCtx | None
+    _stream: str
+    _subscription_id: int
+    _offset: Offset
+    _timeout: float
+    _amqp: bool
+    _message: MessageCtx | None
 
     def __init__(
         self,
         client: StreamsClient,
         stream: str,
         subscription_id: int,
         offset: Offset,
```

### Comparing `rbfly-0.7.0/rbfly/streams/_client.pyx` & `rbfly-0.7.1/rbfly/streams/_client.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -447,66 +447,66 @@
     :var timeout: Raise timeout error if no message within specified time
         (in seconds).
     :var message: Last received message or null.
     :var amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP
         decoding.
     """
     cdef:
-        object client
-        str stream
-        uint8_t subscription_id
-        object offset
-        float timeout
-        char amqp
-        MessageCtx message
+        public object _client
+        public str _stream
+        public uint8_t _subscription_id
+        public object _offset
+        public float _timeout
+        public char _amqp
+        public MessageCtx _message
 
     def __cinit__(
             self,
             client,
             stream: str,
             subscription_id: int,
             offset: Offset,
             timeout: float,
             amqp: bool,
     ) -> None:
         """
         Create RabbitMQ stream subscriber.
         """
-        self.client = client
-        self.stream = stream
-        self.subscription_id = subscription_id
-        self.offset = offset
-        self.timeout = timeout
-        self.amqp = amqp
-        self.message: MessageCtx | None = None
+        self._client = client
+        self._stream = stream
+        self._subscription_id = subscription_id
+        self._offset = offset
+        self._timeout = timeout
+        self._amqp = amqp
+        self._message: MessageCtx | None = None
 
     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:
         """
         Iterate over messages read from a stream.
         """
         cdef:
-            float timeout = self.timeout
-            object client = self.client
+            float timeout = self._timeout
+            object client = self._client
             object messages
             object protocol
             object task
 
         while True:
             try:
                 protocol = await client.get_protocol()
-                task = protocol.read_stream(self.subscription_id)
+                task = protocol.read_stream(self._subscription_id)
                 if timeout:
                     task = asyncio.wait_for(task, timeout)
                 messages = await task
             except ConnectionError:
                 pass
             else:
                 while messages:
-                    self.message = messages.popleft()
-                    yield self.message
+                    self._message = messages.popleft()
+                    yield self._message
 
 cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
     if not ctx.is_set_stream_publish_id:
         ctx.stream_publish_id = publisher.message_id
 
 cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
     if ctx.is_set_stream_publish_id:
```

### Comparing `rbfly-0.7.0/rbfly/streams/_codec.c` & `rbfly-0.7.1/rbfly/streams/_codec.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_codec.pyi` & `rbfly-0.7.1/rbfly/streams/_codec.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_codec.pyx` & `rbfly-0.7.1/rbfly/streams/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_mqueue.c` & `rbfly-0.7.1/rbfly/streams/_mqueue.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_mqueue.pyi` & `rbfly-0.7.1/rbfly/streams/_mqueue.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/_mqueue.pyx` & `rbfly-0.7.1/rbfly/streams/_mqueue.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/client.py` & `rbfly-0.7.1/rbfly/streams/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,22 +126,24 @@
 
         for publisher in self._publishers.values():
             await self._create_publisher(
                 protocol, publisher.stream, publisher._id, publisher.name
             )
 
         for subscriber in self._subscribers.values():
-            msg = subscriber.message
-            proto_offset = subscriber.offset if msg is None else Offset.offset(msg.stream_offset + 1)
+            msg = subscriber._message
+            proto_offset = subscriber._offset if msg is None \
+                else Offset.offset(msg.stream_offset + 1)
+
             await self._subscribe(
                 protocol,
-                subscriber.stream,
-                subscriber.subscription_id,
+                subscriber._stream,
+                subscriber._subscription_id,
                 proto_offset,
-                subscriber.amqp
+                subscriber._amqp
             )
 
     async def _disconnect(self, protocol: RabbitMQStreamsProtocol) -> None:
         await protocol.send_close()
         logger.info(
             'rabbitmq streams client disconnected: {}'.format(self._cinfo)
         )
```

### Comparing `rbfly-0.7.0/rbfly/streams/codec.py` & `rbfly-0.7.1/rbfly/streams/codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/const.py` & `rbfly-0.7.1/rbfly/streams/const.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/error.py` & `rbfly-0.7.1/rbfly/streams/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/offset.py` & `rbfly-0.7.1/rbfly/streams/offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/protocol.py` & `rbfly-0.7.1/rbfly/streams/protocol.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/types.py` & `rbfly-0.7.1/rbfly/streams/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/streams/util.py` & `rbfly-0.7.1/rbfly/streams/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/__init__.py` & `rbfly-0.7.1/rbfly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/amqp/__init__.py` & `rbfly-0.7.1/rbfly/tests/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/amqp/test_message.py` & `rbfly-0.7.1/rbfly/tests/amqp/test_message.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/streams/__init__.py` & `rbfly-0.7.1/rbfly/tests/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/streams/test_client.py` & `rbfly-0.7.1/rbfly/tests/streams/test_client.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/streams/test_codec.py` & `rbfly-0.7.1/rbfly/tests/streams/test_codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/streams/test_mqueue.py` & `rbfly-0.7.1/rbfly/tests/streams/test_mqueue.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/streams/test_offset.py` & `rbfly-0.7.1/rbfly/tests/streams/test_offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/tests/test_util.py` & `rbfly-0.7.1/rbfly/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/types.py` & `rbfly-0.7.1/rbfly/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly/util.py` & `rbfly-0.7.1/rbfly/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/rbfly.egg-info/PKG-INFO` & `rbfly-0.7.1/rbfly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.7.0
+Version: 0.7.1
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
```

### Comparing `rbfly-0.7.0/rbfly.egg-info/SOURCES.txt` & `rbfly-0.7.1/rbfly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.0/setup.cfg` & `rbfly-0.7.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rbfly
-version = 0.7.0
+version = 0.7.1
 author = Artur Wroblewski
 author_email = wrobell@riseup.net
 license = GPLv3+
 description = RbFly - a library for RabbitMQ Streams using Python asyncio
 long_description = file: README
 long_description_content_type = text/x-rst
 url = https://wrobell.dcmod.org/rbfly/
```

### Comparing `rbfly-0.7.0/setup.py` & `rbfly-0.7.1/setup.py`

 * *Files identical despite different names*

