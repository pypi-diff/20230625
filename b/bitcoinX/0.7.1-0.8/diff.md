# Comparing `tmp/bitcoinX-0.7.1.tar.gz` & `tmp/bitcoinX-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoinX-0.7.1.tar", last modified: Mon Dec 12 09:36:34 2022, max compression
+gzip compressed data, was "bitcoinX-0.8.tar", last modified: Sun Jun 25 12:17:25 2023, max compression
```

## Comparing `bitcoinX-0.7.1.tar` & `bitcoinX-0.8.tar`

### file list

```diff
@@ -1,42 +1,40 @@
-drwxr-xr-x   0 neil       (501) staff       (20)        0 2022-12-12 09:36:34.981306 bitcoinX-0.7.1/
--rw-r--r--   0 neil       (501) staff       (20)     1698 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/LICENCE
--rw-r--r--   0 neil       (501) staff       (20)       68 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/MANIFEST.in
--rw-r--r--   0 neil       (501) staff       (20)      782 2022-12-12 09:36:34.981176 bitcoinX-0.7.1/PKG-INFO
--rw-r--r--   0 neil       (501) staff       (20)     2655 2022-12-12 09:26:56.000000 bitcoinX-0.7.1/README.rst
-drwxr-xr-x   0 neil       (501) staff       (20)        0 2022-12-12 09:36:34.977217 bitcoinX-0.7.1/bitcoinX.egg-info/
--rw-r--r--   0 neil       (501) staff       (20)      782 2022-12-12 09:36:34.000000 bitcoinX-0.7.1/bitcoinX.egg-info/PKG-INFO
--rw-r--r--   0 neil       (501) staff       (20)      771 2022-12-12 09:36:34.000000 bitcoinX-0.7.1/bitcoinX.egg-info/SOURCES.txt
--rw-r--r--   0 neil       (501) staff       (20)        1 2022-12-12 09:36:34.000000 bitcoinX-0.7.1/bitcoinX.egg-info/dependency_links.txt
--rw-r--r--   0 neil       (501) staff       (20)       41 2022-12-12 09:36:34.000000 bitcoinX-0.7.1/bitcoinX.egg-info/requires.txt
--rw-r--r--   0 neil       (501) staff       (20)        9 2022-12-12 09:36:34.000000 bitcoinX-0.7.1/bitcoinX.egg-info/top_level.txt
-drwxr-xr-x   0 neil       (501) staff       (20)        0 2022-12-12 09:36:34.980031 bitcoinX-0.7.1/bitcoinx/
--rw-r--r--   0 neil       (501) staff       (20)      866 2022-12-12 09:36:08.000000 bitcoinX-0.7.1/bitcoinx/__init__.py
--rw-r--r--   0 neil       (501) staff       (20)     7149 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/address.py
--rw-r--r--   0 neil       (501) staff       (20)     1071 2022-06-01 09:34:34.000000 bitcoinX-0.7.1/bitcoinx/aes.py
--rw-r--r--   0 neil       (501) staff       (20)     2648 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/base58.py
--rw-r--r--   0 neil       (501) staff       (20)    10487 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/bip32.py
--rw-r--r--   0 neil       (501) staff       (20)      165 2022-11-13 20:52:26.000000 bitcoinX-0.7.1/bitcoinx/bsor.py
--rw-r--r--   0 neil       (501) staff       (20)     5664 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/cashaddr.py
--rw-r--r--   0 neil       (501) staff       (20)    17458 2022-12-12 09:25:02.000000 bitcoinX-0.7.1/bitcoinx/chain.py
--rw-r--r--   0 neil       (501) staff       (20)     1419 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/consts.py
-drwxr-xr-x   0 neil       (501) staff       (20)        0 2022-12-12 09:36:34.980664 bitcoinX-0.7.1/bitcoinx/data/
--rw-r--r--   0 neil       (501) staff       (20)     8192 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/bitcoinx/data/chinese_simplified.txt
--rw-r--r--   0 neil       (501) staff       (20)    10593 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/bitcoinx/data/electrum_old.txt
--rw-r--r--   0 neil       (501) staff       (20)    13116 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/bitcoinx/data/english.txt
--rw-r--r--   0 neil       (501) staff       (20)    24287 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/bitcoinx/data/japanese.txt
--rw-r--r--   0 neil       (501) staff       (20)    13659 2021-02-20 08:58:17.000000 bitcoinX-0.7.1/bitcoinx/data/spanish.txt
--rw-r--r--   0 neil       (501) staff       (20)     6432 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/errors.py
--rw-r--r--   0 neil       (501) staff       (20)     2499 2022-06-01 10:04:39.000000 bitcoinX-0.7.1/bitcoinx/hashes.py
--rw-r--r--   0 neil       (501) staff       (20)    45689 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/interpreter.py
--rw-r--r--   0 neil       (501) staff       (20)    22309 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/keys.py
--rw-r--r--   0 neil       (501) staff       (20)     2878 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/limited_stack.py
--rw-r--r--   0 neil       (501) staff       (20)     2146 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/misc.py
--rw-r--r--   0 neil       (501) staff       (20)    13120 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/mnemonic.py
--rw-r--r--   0 neil       (501) staff       (20)     7345 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/networks.py
--rw-r--r--   0 neil       (501) staff       (20)     5569 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/packing.py
--rw-r--r--   0 neil       (501) staff       (20)    22715 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/script.py
--rw-r--r--   0 neil       (501) staff       (20)    12959 2021-02-28 17:11:03.000000 bitcoinX-0.7.1/bitcoinx/signature.py
--rw-r--r--   0 neil       (501) staff       (20)    13593 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/tx.py
--rw-r--r--   0 neil       (501) staff       (20)     6625 2021-09-29 11:32:26.000000 bitcoinX-0.7.1/bitcoinx/work.py
--rw-r--r--   0 neil       (501) staff       (20)       38 2022-12-12 09:36:34.981349 bitcoinX-0.7.1/setup.cfg
--rw-r--r--   0 neil       (501) staff       (20)     1520 2022-06-01 09:33:22.000000 bitcoinX-0.7.1/setup.py
+drwxr-xr-x   0 neil       (501) staff       (20)        0 2023-06-25 12:17:25.229747 bitcoinX-0.8/
+-rw-r--r--   0 neil       (501) staff       (20)     1698 2021-02-20 08:58:17.000000 bitcoinX-0.8/LICENCE
+-rw-r--r--   0 neil       (501) staff       (20)       68 2021-02-20 08:58:17.000000 bitcoinX-0.8/MANIFEST.in
+-rw-r--r--   0 neil       (501) staff       (20)      778 2023-06-25 12:17:25.229643 bitcoinX-0.8/PKG-INFO
+-rw-r--r--   0 neil       (501) staff       (20)     1170 2023-06-25 12:16:36.000000 bitcoinX-0.8/README.rst
+drwxr-xr-x   0 neil       (501) staff       (20)        0 2023-06-25 12:17:25.226291 bitcoinX-0.8/bitcoinX.egg-info/
+-rw-r--r--   0 neil       (501) staff       (20)      778 2023-06-25 12:17:24.000000 bitcoinX-0.8/bitcoinX.egg-info/PKG-INFO
+-rw-r--r--   0 neil       (501) staff       (20)      735 2023-06-25 12:17:25.000000 bitcoinX-0.8/bitcoinX.egg-info/SOURCES.txt
+-rw-r--r--   0 neil       (501) staff       (20)        1 2023-06-25 12:17:25.000000 bitcoinX-0.8/bitcoinX.egg-info/dependency_links.txt
+-rw-r--r--   0 neil       (501) staff       (20)       41 2023-06-25 12:17:25.000000 bitcoinX-0.8/bitcoinX.egg-info/requires.txt
+-rw-r--r--   0 neil       (501) staff       (20)        9 2023-06-25 12:17:25.000000 bitcoinX-0.8/bitcoinX.egg-info/top_level.txt
+drwxr-xr-x   0 neil       (501) staff       (20)        0 2023-06-25 12:17:25.228573 bitcoinX-0.8/bitcoinx/
+-rw-r--r--   0 neil       (501) staff       (20)      822 2023-06-25 12:16:08.000000 bitcoinX-0.8/bitcoinx/__init__.py
+-rw-r--r--   0 neil       (501) staff       (20)     7148 2023-04-30 06:32:49.000000 bitcoinX-0.8/bitcoinx/address.py
+-rw-r--r--   0 neil       (501) staff       (20)     1071 2022-06-01 09:34:34.000000 bitcoinX-0.8/bitcoinx/aes.py
+-rw-r--r--   0 neil       (501) staff       (20)     2648 2021-02-28 17:11:03.000000 bitcoinX-0.8/bitcoinx/base58.py
+-rw-r--r--   0 neil       (501) staff       (20)    10486 2023-04-30 06:32:49.000000 bitcoinX-0.8/bitcoinx/bip32.py
+-rw-r--r--   0 neil       (501) staff       (20)     5664 2021-09-29 11:32:26.000000 bitcoinX-0.8/bitcoinx/cashaddr.py
+-rw-r--r--   0 neil       (501) staff       (20)     1419 2021-02-28 17:11:03.000000 bitcoinX-0.8/bitcoinx/consts.py
+drwxr-xr-x   0 neil       (501) staff       (20)        0 2023-06-25 12:17:25.229465 bitcoinX-0.8/bitcoinx/data/
+-rw-r--r--   0 neil       (501) staff       (20)     8192 2021-02-20 08:58:17.000000 bitcoinX-0.8/bitcoinx/data/chinese_simplified.txt
+-rw-r--r--   0 neil       (501) staff       (20)    10593 2021-02-20 08:58:17.000000 bitcoinX-0.8/bitcoinx/data/electrum_old.txt
+-rw-r--r--   0 neil       (501) staff       (20)    13116 2021-02-20 08:58:17.000000 bitcoinX-0.8/bitcoinx/data/english.txt
+-rw-r--r--   0 neil       (501) staff       (20)    24287 2021-02-20 08:58:17.000000 bitcoinX-0.8/bitcoinx/data/japanese.txt
+-rw-r--r--   0 neil       (501) staff       (20)    13659 2021-02-20 08:58:17.000000 bitcoinX-0.8/bitcoinx/data/spanish.txt
+-rw-r--r--   0 neil       (501) staff       (20)     6432 2023-06-25 12:13:24.000000 bitcoinX-0.8/bitcoinx/errors.py
+-rw-r--r--   0 neil       (501) staff       (20)     2499 2022-06-01 10:04:39.000000 bitcoinX-0.8/bitcoinx/hashes.py
+-rw-r--r--   0 neil       (501) staff       (20)    22661 2023-06-25 12:15:02.000000 bitcoinX-0.8/bitcoinx/headers.py
+-rw-r--r--   0 neil       (501) staff       (20)    45689 2021-02-28 17:11:03.000000 bitcoinX-0.8/bitcoinx/interpreter.py
+-rw-r--r--   0 neil       (501) staff       (20)    22369 2023-04-30 06:32:49.000000 bitcoinX-0.8/bitcoinx/keys.py
+-rw-r--r--   0 neil       (501) staff       (20)     2878 2021-02-28 17:11:03.000000 bitcoinX-0.8/bitcoinx/limited_stack.py
+-rw-r--r--   0 neil       (501) staff       (20)     2146 2023-06-25 12:13:24.000000 bitcoinX-0.8/bitcoinx/misc.py
+-rw-r--r--   0 neil       (501) staff       (20)    13120 2021-09-29 11:32:26.000000 bitcoinX-0.8/bitcoinx/mnemonic.py
+-rw-r--r--   0 neil       (501) staff       (20)     5569 2021-09-29 11:32:26.000000 bitcoinX-0.8/bitcoinx/packing.py
+-rw-r--r--   0 neil       (501) staff       (20)    22715 2021-09-29 11:32:26.000000 bitcoinX-0.8/bitcoinx/script.py
+-rw-r--r--   0 neil       (501) staff       (20)    12959 2021-02-28 17:11:03.000000 bitcoinX-0.8/bitcoinx/signature.py
+-rw-r--r--   0 neil       (501) staff       (20)    13593 2021-09-29 11:32:26.000000 bitcoinX-0.8/bitcoinx/tx.py
+-rw-r--r--   0 neil       (501) staff       (20)     2076 2023-04-30 06:32:49.000000 bitcoinX-0.8/bitcoinx/work.py
+-rw-r--r--   0 neil       (501) staff       (20)       38 2023-06-25 12:17:25.229782 bitcoinX-0.8/setup.cfg
+-rw-r--r--   0 neil       (501) staff       (20)     1520 2023-06-25 12:14:21.000000 bitcoinX-0.8/setup.py
```

### Comparing `bitcoinX-0.7.1/LICENCE` & `bitcoinX-0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/PKG-INFO` & `bitcoinX-0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bitcoinX
-Version: 0.7.1
+Version: 0.8
 Summary: Library of Bitcoin functions
 Home-page: https://github.com/kyuupichan/bitcoinX
-Download-URL: https://github.com/kyuupichan/bitcoinX/archive/0.7.1.tar.gz
+Download-URL: https://github.com/kyuupichan/bitcoinX/archive/0.8.tar.gz
 Author: Neil Booth
 Author-email: kyuupichan@gmail.com
 License: MIT Licence
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENCE
 
 Library of Bitcoin functions covering network protocol, consensus, transactions, scripting and signing.
```

### Comparing `bitcoinX-0.7.1/bitcoinX.egg-info/PKG-INFO` & `bitcoinX-0.8/bitcoinX.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bitcoinX
-Version: 0.7.1
+Version: 0.8
 Summary: Library of Bitcoin functions
 Home-page: https://github.com/kyuupichan/bitcoinX
-Download-URL: https://github.com/kyuupichan/bitcoinX/archive/0.7.1.tar.gz
+Download-URL: https://github.com/kyuupichan/bitcoinX/archive/0.8.tar.gz
 Author: Neil Booth
 Author-email: kyuupichan@gmail.com
 License: MIT Licence
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENCE
 
 Library of Bitcoin functions covering network protocol, consensus, transactions, scripting and signing.
```

### Comparing `bitcoinX-0.7.1/bitcoinX.egg-info/SOURCES.txt` & `bitcoinX-0.8/bitcoinX.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 bitcoinX.egg-info/requires.txt
 bitcoinX.egg-info/top_level.txt
 bitcoinx/__init__.py
 bitcoinx/address.py
 bitcoinx/aes.py
 bitcoinx/base58.py
 bitcoinx/bip32.py
-bitcoinx/bsor.py
 bitcoinx/cashaddr.py
-bitcoinx/chain.py
 bitcoinx/consts.py
 bitcoinx/errors.py
 bitcoinx/hashes.py
+bitcoinx/headers.py
 bitcoinx/interpreter.py
 bitcoinx/keys.py
 bitcoinx/limited_stack.py
 bitcoinx/misc.py
 bitcoinx/mnemonic.py
-bitcoinx/networks.py
 bitcoinx/packing.py
 bitcoinx/script.py
 bitcoinx/signature.py
 bitcoinx/tx.py
 bitcoinx/work.py
 bitcoinx/data/chinese_simplified.txt
 bitcoinx/data/electrum_old.txt
```

### Comparing `bitcoinX-0.7.1/bitcoinx/__init__.py` & `bitcoinX-0.8/bitcoinx/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from .address import *
 from .aes import *
 from .base58 import *
 from .bip32 import *
-from .chain import *
 from .consts import *
 from .errors import *
 from .hashes import *
+from .headers import *
 from .interpreter import *
 from .keys import *
 from .misc import *
 from .mnemonic import *
-from .networks import *
 from .packing import *
 from .script import *
 from .signature import *
 from .tx import *
 from .work import *
 
-_version_str = '0.7.1'
+_version_str = '0.8'
 _version = tuple(int(part) for part in _version_str.split('.'))
 
 __all__ = sum((
     address.__all__,
     aes.__all__,
     base58.__all__,
     bip32.__all__,
-    chain.__all__,
     consts.__all__,
     errors.__all__,
     hashes.__all__,
+    headers.__all__,
     interpreter.__all__,
     keys.__all__,
     misc.__all__,
     mnemonic.__all__,
-    networks.__all__,
     packing.__all__,
     script.__all__,
     signature.__all__,
     tx.__all__,
     work.__all__,
 ), ())
```

### Comparing `bitcoinX-0.7.1/bitcoinx/address.py` & `bitcoinX-0.8/bitcoinx/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 from abc import ABC, abstractmethod
 
 from bitcoinx import cashaddr
 from .hashes import hash160 as calc_hash160
 from .base58 import base58_decode_check, base58_encode_check
-from .networks import Bitcoin
+from .headers import Bitcoin
 from .packing import pack_byte
 from .script import Script, Ops, push_item, push_int, item_to_int
 
 
 class Address(ABC):
 
     def __init__(self, network):
```

### Comparing `bitcoinX-0.7.1/bitcoinx/aes.py` & `bitcoinX-0.8/bitcoinx/aes.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/base58.py` & `bitcoinX-0.8/bitcoinx/base58.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/bip32.py` & `bitcoinX-0.8/bitcoinx/bip32.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from os import urandom
 import re
 
 import attr
 
 from .base58 import base58_decode_check, base58_encode_check
 from .hashes import hmac_sha512_halves, hash160
+from .headers import Bitcoin, Network
 from .keys import PrivateKey, PublicKey
 from .misc import cachedproperty
-from .networks import Bitcoin, Network
 from .packing import pack_be_uint32, unpack_be_uint32, pack_byte
 
 HARDENED = 1 << 31
 PART_REGEX = re.compile("([0-9]+)'?$")
 
 
 @attr.s(slots=True, frozen=True, repr=False)
```

### Comparing `bitcoinX-0.7.1/bitcoinx/cashaddr.py` & `bitcoinX-0.8/bitcoinx/cashaddr.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/consts.py` & `bitcoinX-0.8/bitcoinx/consts.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/data/chinese_simplified.txt` & `bitcoinX-0.8/bitcoinx/data/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/data/electrum_old.txt` & `bitcoinX-0.8/bitcoinx/data/electrum_old.txt`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/data/english.txt` & `bitcoinX-0.8/bitcoinx/data/english.txt`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/data/japanese.txt` & `bitcoinX-0.8/bitcoinx/data/japanese.txt`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/data/spanish.txt` & `bitcoinX-0.8/bitcoinx/data/spanish.txt`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/errors.py` & `bitcoinX-0.8/bitcoinx/errors.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/hashes.py` & `bitcoinX-0.8/bitcoinx/hashes.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/interpreter.py` & `bitcoinX-0.8/bitcoinx/interpreter.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/keys.py` & `bitcoinX-0.8/bitcoinx/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 from .address import P2PKH_Address, P2PK_Output
 from .aes import aes_encrypt_with_iv, aes_decrypt_with_iv
 from .base58 import base58_encode_check, base58_decode_check, is_minikey
 from .consts import CURVE_ORDER
 from .errors import DecryptionError, InvalidSignature
 from .hashes import sha256, sha512, double_sha256, hash160 as calc_hash160, hmac_digest, _sha256
+from .headers import Bitcoin, Network
 from .misc import be_bytes_to_int, int_to_be_bytes, CONTEXT, cachedproperty
-from .networks import Bitcoin, Network
 from .packing import pack_byte, pack_signed_message
 from .signature import (
     sign_der, sign_recoverable, verify_der_signature, verify_recoverable_signature,
     public_key_from_recoverable_signature, to_message_signature, to_recoverable_signature,
 )
 
 EC_COMPRESSED = lib.SECP256K1_EC_COMPRESSED
@@ -327,14 +327,18 @@
     def __str__(self):
         return self.to_hex()
 
     def network(self):
         '''The implied network.'''
         return self._network
 
+    @property
+    def public_key(self):
+        return self
+
     def is_compressed(self):
         '''Return true if it serializes to 33 bytes.'''
         return self._compressed
 
     def to_bytes(self, *, compressed=None):
         '''Serialize a PublicKey to bytes.'''
         if (self._compressed if compressed is None else compressed):
```

### Comparing `bitcoinX-0.7.1/bitcoinx/limited_stack.py` & `bitcoinX-0.8/bitcoinx/limited_stack.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/misc.py` & `bitcoinX-0.8/bitcoinx/misc.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/mnemonic.py` & `bitcoinX-0.8/bitcoinx/mnemonic.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/packing.py` & `bitcoinX-0.8/bitcoinx/packing.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/script.py` & `bitcoinX-0.8/bitcoinx/script.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/signature.py` & `bitcoinX-0.8/bitcoinx/signature.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/bitcoinx/tx.py` & `bitcoinX-0.8/bitcoinx/tx.py`

 * *Files identical despite different names*

### Comparing `bitcoinX-0.7.1/setup.py` & `bitcoinX-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 tld = os.path.abspath(os.path.dirname(__file__))
 version = find_version(os.path.join(tld, 'bitcoinx', '__init__.py'))
 
 
 setuptools.setup(
     name='bitcoinX',
     version=version,
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=['attrs', 'pycryptodomex', 'electrumsv-secp256k1'],
     packages=['bitcoinx'],
     description='Library of Bitcoin functions',
     author='Neil Booth',
     author_email='kyuupichan@gmail.com',
     license='MIT Licence',
     # Tell setuptools to include data files specified by MANIFEST.in.
@@ -36,12 +36,12 @@
         'transactions, scripting and signing.'
     ),
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.8",
         'Topic :: Internet',
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

