# Comparing `tmp/bittrade_luno_websocket-0.1.6.tar.gz` & `tmp/bittrade_luno_websocket-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_luno_websocket-0.1.6.tar", max compression
+gzip compressed data, was "bittrade_luno_websocket-0.1.7.tar", max compression
```

## Comparing `bittrade_luno_websocket-0.1.6.tar` & `bittrade_luno_websocket-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0        0 2023-02-07 04:39:10.926618 bittrade_luno_websocket-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-02-07 04:39:10.926618 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 04:54:38.094803 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/channels/__init__.py
--rw-r--r--   0        0        0    13101 2023-06-19 01:37:18.734165 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/channels/orderbook.py
--rw-r--r--   0        0        0     1735 2023-04-19 06:22:14.941257 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/channels/user_stream.py
--rw-r--r--   0        0        0        0 2023-03-10 01:38:28.536176 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/__init__.py
--rw-r--r--   0        0        0     1374 2023-03-12 01:34:13.037369 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/authenticate.py
--rw-r--r--   0        0        0     3525 2023-03-12 05:38:45.786365 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/generic.py
--rw-r--r--   0        0        0     2296 2023-04-23 05:37:33.190506 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/http.py
--rw-r--r--   0        0        0      720 2023-03-12 06:46:01.623584 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/public.py
--rw-r--r--   0        0        0      102 2023-03-13 08:27:34.679675 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/__init__.py
--rw-r--r--   0        0        0      344 2023-06-17 03:41:54.472758 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/endpoints.py
--rw-r--r--   0        0        0      690 2023-03-10 02:44:12.318417 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0      203 2023-03-13 03:15:50.329774 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/orderbook.py
--rw-r--r--   0        0        0      398 2023-03-13 08:34:59.946557 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/request.py
--rw-r--r--   0        0        0      847 2023-03-13 08:14:41.380022 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/response_message.py
--rw-r--r--   0        0        0        0 2023-03-13 08:20:30.323385 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0      470 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/balance.py
--rw-r--r--   0        0        0      129 2023-06-17 03:41:00.170711 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/fee.py
--rw-r--r--   0        0        0     1100 2023-03-16 08:02:48.834747 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/get_order.py
--rw-r--r--   0        0        0     1236 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/order.py
--rw-r--r--   0        0        0      512 2023-05-01 05:24:59.858547 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/transfer.py
--rw-r--r--   0        0        0     1034 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/balance.py
--rw-r--r--   0        0        0      580 2023-03-15 08:30:08.583232 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_book.py
--rw-r--r--   0        0        0      875 2023-06-17 03:47:22.503861 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_fee_info.py
--rw-r--r--   0        0        0      621 2023-03-16 08:05:10.479544 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_order.py
--rw-r--r--   0        0        0     1876 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/order.py
--rw-r--r--   0        0        0      367 2023-03-13 08:59:54.685549 bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/signing/__init__.py
--rw-r--r--   0        0        0     1070 2023-06-19 01:38:26.897419 bittrade_luno_websocket-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.6/setup.py
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566521 bittrade_luno_websocket-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566632 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566732 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/channels/__init__.py
+-rw-r--r--   0        0        0    13101 2023-06-25 00:00:08.940533 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/channels/orderbook.py
+-rw-r--r--   0        0        0     1701 2023-06-25 00:37:44.884815 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/channels/user_stream.py
+-rw-r--r--   0        0        0        0 2023-03-11 21:05:54.544362 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/__init__.py
+-rw-r--r--   0        0        0     1374 2023-03-11 21:05:54.545267 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/authenticate.py
+-rw-r--r--   0        0        0     3525 2023-03-13 09:43:24.335646 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2296 2023-06-25 00:00:08.942671 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/http.py
+-rw-r--r--   0        0        0      720 2023-03-13 09:43:24.336282 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/public.py
+-rw-r--r--   0        0        0      102 2023-03-13 09:43:24.336634 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-25 00:34:39.427579 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/endpoints.py
+-rw-r--r--   0        0        0      690 2023-03-11 21:05:54.548298 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0      203 2023-03-13 09:43:24.337178 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/orderbook.py
+-rw-r--r--   0        0        0      398 2023-03-13 09:43:24.337444 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/request.py
+-rw-r--r--   0        0        0      847 2023-03-13 09:43:24.337668 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/response_message.py
+-rw-r--r--   0        0        0        0 2023-03-13 09:43:24.337809 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-16 20:12:18.269435 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/balance.py
+-rw-r--r--   0        0        0      129 2023-06-25 00:00:08.943811 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/fee.py
+-rw-r--r--   0        0        0     1100 2023-03-23 09:08:33.509055 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/get_order.py
+-rw-r--r--   0        0        0     1236 2023-04-16 20:00:08.620775 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/order.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:31:53.255950 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/receive_address.py
+-rw-r--r--   0        0        0      512 2023-06-25 00:00:08.944095 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/transfer.py
+-rw-r--r--   0        0        0     1034 2023-04-17 04:25:05.453554 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/balance.py
+-rw-r--r--   0        0        0      580 2023-03-23 09:08:33.509444 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_book.py
+-rw-r--r--   0        0        0      875 2023-06-25 00:00:08.944285 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_fee_info.py
+-rw-r--r--   0        0        0      621 2023-03-23 09:08:33.509626 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_order.py
+-rw-r--r--   0        0        0      881 2023-06-25 00:35:30.914817 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_receive_address.py
+-rw-r--r--   0        0        0     1876 2023-04-17 04:24:16.695673 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/order.py
+-rw-r--r--   0        0        0      367 2023-03-13 09:43:24.340924 bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/signing/__init__.py
+-rw-r--r--   0        0        0     1070 2023-06-25 00:46:01.749152 bittrade_luno_websocket-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.7/setup.py
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.7/PKG-INFO
```

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/channels/orderbook.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/channels/orderbook.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/channels/user_stream.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/channels/user_stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     abc,
     operators,
     disposable,
     observer,
     throw,
 )
 from reactivex.scheduler import ThreadPoolScheduler
-from returns import result, maybe
 
 logger = logging.getLogger(__name__)
 
 
 class UserStreamMessage(TypedDict):
     type: Literal["order_status", "order_fill", "balance_update"]
     order_status_update: dict
```

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/authenticate.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/authenticate.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/generic.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/http.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/connection/public.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/connection/public.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/enhanced_websocket.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/response_message.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/response_message.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/get_order.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/order.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/models/rest/transfer.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/models/rest/transfer.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/balance.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/balance.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_book.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_book.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_fee_info.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_fee_info.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/get_order.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/bittrade_luno_websocket/rest/order.py` & `bittrade_luno_websocket-0.1.7/bittrade_luno_websocket/rest/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.6/pyproject.toml` & `bittrade_luno_websocket-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-luno-websocket"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Matt <matt@techspace.asia>"]
 readme = "README.md"
 packages = [{ include = "bittrade_luno_websocket" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bittrade_luno_websocket-0.1.6/setup.py` & `bittrade_luno_websocket-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'reactivex>=4.0.4,<5.0.0',
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'bittrade-luno-websocket',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': '',
     'author': 'Matt',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bittrade_luno_websocket-0.1.6/PKG-INFO` & `bittrade_luno_websocket-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-luno-websocket
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Matt
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ccxt (>=2.7.91,<3.0.0)
```

