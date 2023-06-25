# Comparing `tmp/mycoinlib-1.2.tar.gz` & `tmp/mycoinlib-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-1.2.tar", last modified: Thu Jun 22 07:22:57 2023, max compression
+gzip compressed data, was "mycoinlib-1.4.tar", last modified: Sun Jun 25 03:40:48 2023, max compression
```

## Comparing `mycoinlib-1.2.tar` & `mycoinlib-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.713339 mycoinlib-1.2/
--rw-rw-rw-   0        0        0       54 2023-06-22 07:22:56.709360 mycoinlib-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.559835 mycoinlib-1.2/mycoinlib/
--rw-rw-rw-   0        0        0      130 2023-06-22 06:40:32.000000 mycoinlib-1.2/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0     1944 2023-06-22 07:21:56.000000 mycoinlib-1.2/mycoinlib/btc.py
--rw-rw-rw-   0        0        0     1990 2023-06-22 07:22:10.000000 mycoinlib-1.2/mycoinlib/eth.py
--rw-rw-rw-   0        0        0     2105 2023-06-22 07:22:19.000000 mycoinlib-1.2/mycoinlib/ltc.py
--rw-rw-rw-   0        0        0      637 2023-06-22 06:44:33.000000 mycoinlib-1.2/mycoinlib/mycoin.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.698433 mycoinlib-1.2/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-22 07:22:56.000000 mycoinlib-1.2/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:22:56.713339 mycoinlib-1.2/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-06-22 07:22:41.000000 mycoinlib-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 03:40:48.170617 mycoinlib-1.4/
+-rw-rw-rw-   0        0        0       54 2023-06-25 03:40:48.167636 mycoinlib-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 03:40:48.095582 mycoinlib-1.4/mycoinlib/
+-rw-rw-rw-   0        0        0      130 2023-06-22 06:40:32.000000 mycoinlib-1.4/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     1944 2023-06-22 07:21:56.000000 mycoinlib-1.4/mycoinlib/btc.py
+-rw-rw-rw-   0        0        0     2209 2023-06-25 03:40:07.000000 mycoinlib-1.4/mycoinlib/eth.py
+-rw-rw-rw-   0        0        0     2105 2023-06-22 07:22:19.000000 mycoinlib-1.4/mycoinlib/ltc.py
+-rw-rw-rw-   0        0        0      637 2023-06-22 06:44:33.000000 mycoinlib-1.4/mycoinlib/mycoin.py
+drwxrwxrwx   0        0        0        0 2023-06-25 03:40:48.165645 mycoinlib-1.4/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-25 03:40:47.000000 mycoinlib-1.4/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-25 03:40:47.000000 mycoinlib-1.4/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 03:40:47.000000 mycoinlib-1.4/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-25 03:40:47.000000 mycoinlib-1.4/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 03:40:47.000000 mycoinlib-1.4/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 03:40:48.170617 mycoinlib-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      278 2023-06-25 03:40:31.000000 mycoinlib-1.4/setup.py
```

### Comparing `mycoinlib-1.2/mycoinlib/btc.py` & `mycoinlib-1.4/mycoinlib/btc.py`

 * *Files identical despite different names*

### Comparing `mycoinlib-1.2/mycoinlib/eth.py` & `mycoinlib-1.4/mycoinlib/eth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 
 import requests
 from eth_account import Account
-
+from eth_keys import keys
+from eth_utils import decode_hex
 
 class ETH:
     # Create a new ETH wallet
     def create_wallet():
         account = Account.create()
         private_key = account._private_key.hex()
-        address = account.address
+        priv_key_bytes = decode_hex(private_key)
+        priv_key = keys.PrivateKey(priv_key_bytes)
+        pub_key = str(priv_key.public_key)
+        address = pub_key.to_checksum_address()
         info = {
             'crypto_type': 'ETH',
             'private_key': private_key,
-            'public_key': address,
+            'public_key': pub_key,
             'wallet_address': address
         }
         return info
 
 
     # retrieve current ETH price
     @staticmethod
```

### Comparing `mycoinlib-1.2/mycoinlib/ltc.py` & `mycoinlib-1.4/mycoinlib/ltc.py`

 * *Files identical despite different names*

### Comparing `mycoinlib-1.2/mycoinlib/mycoin.py` & `mycoinlib-1.4/mycoinlib/mycoin.py`

 * *Files identical despite different names*

