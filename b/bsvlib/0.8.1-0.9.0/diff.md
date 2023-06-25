# Comparing `tmp/bsvlib-0.8.1.tar.gz` & `tmp/bsvlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsvlib-0.8.1.tar", last modified: Tue Oct  4 08:46:53 2022, max compression
+gzip compressed data, was "bsvlib-0.9.0.tar", last modified: Fri Nov 25 14:49:55 2022, max compression
```

## Comparing `bsvlib-0.8.1.tar` & `bsvlib-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.640120 bsvlib-0.8.1/
--rw-r--r--   0 aaron67    (501) staff       (20)     1069 2022-04-01 14:15:37.000000 bsvlib-0.8.1/LICENSE
--rw-r--r--   0 aaron67    (501) staff       (20)     7760 2022-10-04 08:46:53.640242 bsvlib-0.8.1/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)     6945 2022-04-11 18:19:43.000000 bsvlib-0.8.1/README.md
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.634266 bsvlib-0.8.1/bsvlib/
--rw-r--r--   0 aaron67    (501) staff       (20)      231 2022-10-04 08:46:32.000000 bsvlib-0.8.1/bsvlib/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)      934 2022-01-20 12:33:26.000000 bsvlib-0.8.1/bsvlib/aes.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1529 2022-02-05 05:13:48.000000 bsvlib-0.8.1/bsvlib/base58.py
--rw-r--r--   0 aaron67    (501) staff       (20)     6602 2022-05-04 07:20:42.000000 bsvlib-0.8.1/bsvlib/constants.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2509 2022-01-28 20:24:48.000000 bsvlib-0.8.1/bsvlib/curve.py
--rw-r--r--   0 aaron67    (501) staff       (20)      343 2022-01-13 09:42:18.000000 bsvlib-0.8.1/bsvlib/hash.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.635959 bsvlib-0.8.1/bsvlib/hd/
--rw-r--r--   0 aaron67    (501) staff       (20)      227 2022-01-24 22:27:44.000000 bsvlib-0.8.1/bsvlib/hd/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     6941 2022-01-28 20:31:34.000000 bsvlib-0.8.1/bsvlib/hd/bip32.py
--rw-r--r--   0 aaron67    (501) staff       (20)     4039 2022-10-04 08:44:29.000000 bsvlib-0.8.1/bsvlib/hd/bip39.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1087 2022-01-25 06:42:15.000000 bsvlib-0.8.1/bsvlib/hd/bip44.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.636480 bsvlib-0.8.1/bsvlib/hd/wordlist/
--rw-r--r--   0 aaron67    (501) staff       (20)     8192 2022-01-24 22:27:44.000000 bsvlib-0.8.1/bsvlib/hd/wordlist/chinese_simplified.txt
--rw-r--r--   0 aaron67    (501) staff       (20)    15164 2022-01-24 22:27:44.000000 bsvlib-0.8.1/bsvlib/hd/wordlist/english.txt
--rw-r--r--   0 aaron67    (501) staff       (20)    13616 2022-03-30 16:09:31.000000 bsvlib-0.8.1/bsvlib/keys.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.637303 bsvlib-0.8.1/bsvlib/script/
--rw-r--r--   0 aaron67    (501) staff       (20)      152 2022-02-05 07:20:08.000000 bsvlib-0.8.1/bsvlib/script/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1193 2022-04-01 11:07:09.000000 bsvlib-0.8.1/bsvlib/script/script.py
--rw-r--r--   0 aaron67    (501) staff       (20)     6486 2022-02-05 07:59:40.000000 bsvlib-0.8.1/bsvlib/script/type.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.638913 bsvlib-0.8.1/bsvlib/service/
--rw-r--r--   0 aaron67    (501) staff       (20)      184 2022-04-11 16:59:57.000000 bsvlib-0.8.1/bsvlib/service/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2890 2022-04-11 17:16:15.000000 bsvlib-0.8.1/bsvlib/service/metasv.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2385 2022-04-11 17:15:40.000000 bsvlib-0.8.1/bsvlib/service/provider.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2657 2022-04-11 17:16:09.000000 bsvlib-0.8.1/bsvlib/service/sensiblequery.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1365 2022-04-11 16:58:20.000000 bsvlib-0.8.1/bsvlib/service/service.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1915 2022-04-11 17:16:05.000000 bsvlib-0.8.1/bsvlib/service/whatsonchain.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.639900 bsvlib-0.8.1/bsvlib/transaction/
--rw-r--r--   0 aaron67    (501) staff       (20)      124 2022-04-01 14:30:50.000000 bsvlib-0.8.1/bsvlib/transaction/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)    18712 2022-04-17 17:37:02.000000 bsvlib-0.8.1/bsvlib/transaction/transaction.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2720 2022-04-11 12:03:03.000000 bsvlib-0.8.1/bsvlib/transaction/unspent.py
--rw-r--r--   0 aaron67    (501) staff       (20)     9599 2022-04-01 13:23:30.000000 bsvlib-0.8.1/bsvlib/utils.py
--rw-r--r--   0 aaron67    (501) staff       (20)     6739 2022-04-11 17:50:34.000000 bsvlib-0.8.1/bsvlib/wallet.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-10-04 08:46:53.635079 bsvlib-0.8.1/bsvlib.egg-info/
--rw-r--r--   0 aaron67    (501) staff       (20)     7760 2022-10-04 08:46:53.000000 bsvlib-0.8.1/bsvlib.egg-info/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)      836 2022-10-04 08:46:53.000000 bsvlib-0.8.1/bsvlib.egg-info/SOURCES.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        1 2022-10-04 08:46:53.000000 bsvlib-0.8.1/bsvlib.egg-info/dependency_links.txt
--rw-r--r--   0 aaron67    (501) staff       (20)       51 2022-10-04 08:46:53.000000 bsvlib-0.8.1/bsvlib.egg-info/requires.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        7 2022-10-04 08:46:53.000000 bsvlib-0.8.1/bsvlib.egg-info/top_level.txt
--rw-r--r--   0 aaron67    (501) staff       (20)      104 2022-01-13 03:23:06.000000 bsvlib-0.8.1/pyproject.toml
--rw-r--r--   0 aaron67    (501) staff       (20)      984 2022-10-04 08:46:53.640617 bsvlib-0.8.1/setup.cfg
--rw-r--r--   0 aaron67    (501) staff       (20)      318 2022-01-13 10:03:26.000000 bsvlib-0.8.1/setup.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.387478 bsvlib-0.9.0/
+-rw-r--r--   0 aaron67    (501) staff       (20)     1069 2022-04-01 14:15:37.000000 bsvlib-0.9.0/LICENSE
+-rw-r--r--   0 aaron67    (501) staff       (20)     7834 2022-11-25 14:49:55.387608 bsvlib-0.9.0/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)     7019 2022-11-25 14:47:18.000000 bsvlib-0.9.0/README.md
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.382092 bsvlib-0.9.0/bsvlib/
+-rw-r--r--   0 aaron67    (501) staff       (20)      231 2022-11-25 14:49:19.000000 bsvlib-0.9.0/bsvlib/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      934 2022-01-20 12:33:26.000000 bsvlib-0.9.0/bsvlib/aes.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1529 2022-02-05 05:13:48.000000 bsvlib-0.9.0/bsvlib/base58.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     6671 2022-11-25 14:19:04.000000 bsvlib-0.9.0/bsvlib/constants.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2509 2022-01-28 20:24:48.000000 bsvlib-0.9.0/bsvlib/curve.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      343 2022-01-13 09:42:18.000000 bsvlib-0.9.0/bsvlib/hash.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.383686 bsvlib-0.9.0/bsvlib/hd/
+-rw-r--r--   0 aaron67    (501) staff       (20)      266 2022-11-25 14:00:26.000000 bsvlib-0.9.0/bsvlib/hd/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7023 2022-11-25 13:44:04.000000 bsvlib-0.9.0/bsvlib/hd/bip32.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     4015 2022-11-25 14:16:52.000000 bsvlib-0.9.0/bsvlib/hd/bip39.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1542 2022-11-25 14:17:34.000000 bsvlib-0.9.0/bsvlib/hd/bip44.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.384189 bsvlib-0.9.0/bsvlib/hd/wordlist/
+-rw-r--r--   0 aaron67    (501) staff       (20)     8192 2022-01-24 22:27:44.000000 bsvlib-0.9.0/bsvlib/hd/wordlist/chinese_simplified.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    15164 2022-01-24 22:27:44.000000 bsvlib-0.9.0/bsvlib/hd/wordlist/english.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    13780 2022-11-25 13:44:31.000000 bsvlib-0.9.0/bsvlib/keys.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.384967 bsvlib-0.9.0/bsvlib/script/
+-rw-r--r--   0 aaron67    (501) staff       (20)      152 2022-02-05 07:20:08.000000 bsvlib-0.9.0/bsvlib/script/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1275 2022-11-25 13:43:40.000000 bsvlib-0.9.0/bsvlib/script/script.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     6896 2022-11-25 13:45:24.000000 bsvlib-0.9.0/bsvlib/script/type.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.386356 bsvlib-0.9.0/bsvlib/service/
+-rw-r--r--   0 aaron67    (501) staff       (20)      143 2022-11-25 14:20:36.000000 bsvlib-0.9.0/bsvlib/service/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2977 2022-11-25 14:40:04.000000 bsvlib-0.9.0/bsvlib/service/metasv.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2493 2022-11-25 14:34:49.000000 bsvlib-0.9.0/bsvlib/service/provider.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1389 2022-11-25 13:52:08.000000 bsvlib-0.9.0/bsvlib/service/service.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1931 2022-11-25 14:39:30.000000 bsvlib-0.9.0/bsvlib/service/whatsonchain.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.387226 bsvlib-0.9.0/bsvlib/transaction/
+-rw-r--r--   0 aaron67    (501) staff       (20)      124 2022-04-01 14:30:50.000000 bsvlib-0.9.0/bsvlib/transaction/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    18833 2022-11-25 14:15:12.000000 bsvlib-0.9.0/bsvlib/transaction/transaction.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2802 2022-11-25 13:42:56.000000 bsvlib-0.9.0/bsvlib/transaction/unspent.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     9663 2022-11-25 14:12:52.000000 bsvlib-0.9.0/bsvlib/utils.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     6434 2022-11-25 14:06:25.000000 bsvlib-0.9.0/bsvlib/wallet.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2022-11-25 14:49:55.382863 bsvlib-0.9.0/bsvlib.egg-info/
+-rw-r--r--   0 aaron67    (501) staff       (20)     7834 2022-11-25 14:49:55.000000 bsvlib-0.9.0/bsvlib.egg-info/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)      804 2022-11-25 14:49:55.000000 bsvlib-0.9.0/bsvlib.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        1 2022-11-25 14:49:55.000000 bsvlib-0.9.0/bsvlib.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)       51 2022-11-25 14:49:55.000000 bsvlib-0.9.0/bsvlib.egg-info/requires.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        7 2022-11-25 14:49:55.000000 bsvlib-0.9.0/bsvlib.egg-info/top_level.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)      104 2022-01-13 03:23:06.000000 bsvlib-0.9.0/pyproject.toml
+-rw-r--r--   0 aaron67    (501) staff       (20)      984 2022-11-25 14:49:55.387996 bsvlib-0.9.0/setup.cfg
+-rw-r--r--   0 aaron67    (501) staff       (20)      318 2022-01-13 10:03:26.000000 bsvlib-0.9.0/setup.py
```

### Comparing `bsvlib-0.8.1/LICENSE` & `bsvlib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/PKG-INFO` & `bsvlib-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsvlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: Bitcoin SV (BSV) Python Library
 Home-page: https://github.com/gitzhou/bsvlib
 Author: aaron67
 Author-email: aaron67@aaron67.cc
 Project-URL: Bug Tracker, https://github.com/gitzhou/bsvlib/issues
 Keywords: bsv,bitcoin-sv,bitcoin sv,bitcoinsv,cryptocurrency,payments,tools,wallet
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 
 A Bitcoin SV (BSV) Python Library that is extremely simple to use but more.
 
 - MAINNET and TESTNET supported
 - P2PKH, P2PK, and bare-multisig supported
 - All the SIGHASH flags supported
 - Additional script types can be customized
-- [MetaSV](https://metasv.com/), [SensibleQuery](https://api.sensiblequery.com/swagger/index.html), and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
+- [MetaSV](https://metasv.com/) and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
 - Ability to adapt to different service providers
 - Fully ECDSA implementation
 - ECDH and Electrum ECIES (aka BIE1) implementation
 - HD implementation (BIP-32, BIP-39, BIP-44)
 
 👉 [Join our Telegram group for discussions or support](https://t.me/bsvlib).
 
@@ -51,15 +51,15 @@
 
 1. Send BSV in one line
 
 ```python
 from bsvlib import Wallet
 
 # Donate to aaron67!
-print(Wallet(['YOUR_WIF_GOES_HERE']).send_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]))
+print(Wallet(['YOUR_WIF']).create_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]).broadcast())
 ```
 
 2. Send unspent locked by different keys in one transaction, support OP_RETURN output as well
 
 ```python
 from bsvlib import Wallet
 from bsvlib.constants import Chain
@@ -68,36 +68,39 @@
 
 w.add_key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
 w.add_key('93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me')
 print(w.get_balance(refresh=True))
 
 outputs = [('mqBuyzdHfD87VfgxaYeM9pex3sJn4ihYHY', 724), ('mr1FHq6GwWzmD1y8Jxq6rNDGsiiQ9caF7r', 996)]
 pushdatas = ['hello', b'world']
-print(w.send_transaction(outputs=outputs, pushdatas=pushdatas, combine=True))
+print(w.create_transaction(outputs=outputs, pushdatas=pushdatas, combine=True).broadcast())
 ```
 
 3. Operate P2PK
 
 ```python
+import time
+
 from bsvlib import Wallet, TxOutput, Transaction
 from bsvlib.constants import Chain
 from bsvlib.keys import Key
 from bsvlib.script import P2pkScriptType
-from bsvlib.service import SensibleQuery
 
+chain = Chain.TEST
 k = Key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
-p = SensibleQuery(chain=Chain.TEST)
-unspents = Wallet(provider=p).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
+unspents = Wallet(chain=chain).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
 
-t = Transaction(provider=p)
-t.add_inputs(unspents)
+t = Transaction(chain=chain).add_inputs(unspents)
 t.add_output(TxOutput(P2pkScriptType.locking(k.public_key().serialize()), 996, P2pkScriptType()))
-t.add_change(k.address())
+t.add_change(k.address()).sign()
+print(t.broadcast())
 
-print(t.sign().broadcast())
+time.sleep(2)
+tt = Transaction(chain=chain).add_inputs(t.to_unspents(args=[{'private_keys': [k]}] * 2)).add_change(k.address()).sign()
+print(tt.broadcast())
 ```
 
 4. Operate bare-multisig
 
 ```python
 import time
 from typing import List, Union
@@ -189,26 +192,26 @@
 8. Process HD wallet derivation
 
 ![image](https://user-images.githubusercontent.com/1585505/150875831-2663e158-b00d-4089-8276-1ad72e335d28.png)
 
 ```python
 from typing import List
 
-from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_from_mnemonic
+from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_xprvs_from_mnemonic
 
 #
 # HD derivation
 #
 entropy = 'cd9b819d9c62f0027116c1849e7d497f'
 
 # snow swing guess decide congress abuse session subway loyal view false zebra
 mnemonic: str = mnemonic_from_entropy(entropy)
 print(mnemonic)
 
-keys: List[Xprv] = derive_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
+keys: List[Xprv] = derive_xprvs_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
 for key in keys:
     print(key.address(), key.private_key().wif())
 
 #
 # random mnemonic
 #
 print()
```

### Comparing `bsvlib-0.8.1/README.md` & `bsvlib-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 A Bitcoin SV (BSV) Python Library that is extremely simple to use but more.
 
 - MAINNET and TESTNET supported
 - P2PKH, P2PK, and bare-multisig supported
 - All the SIGHASH flags supported
 - Additional script types can be customized
-- [MetaSV](https://metasv.com/), [SensibleQuery](https://api.sensiblequery.com/swagger/index.html), and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
+- [MetaSV](https://metasv.com/) and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
 - Ability to adapt to different service providers
 - Fully ECDSA implementation
 - ECDH and Electrum ECIES (aka BIE1) implementation
 - HD implementation (BIP-32, BIP-39, BIP-44)
 
 👉 [Join our Telegram group for discussions or support](https://t.me/bsvlib).
 
@@ -30,15 +30,15 @@
 
 1. Send BSV in one line
 
 ```python
 from bsvlib import Wallet
 
 # Donate to aaron67!
-print(Wallet(['YOUR_WIF_GOES_HERE']).send_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]))
+print(Wallet(['YOUR_WIF']).create_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]).broadcast())
 ```
 
 2. Send unspent locked by different keys in one transaction, support OP_RETURN output as well
 
 ```python
 from bsvlib import Wallet
 from bsvlib.constants import Chain
@@ -47,36 +47,39 @@
 
 w.add_key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
 w.add_key('93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me')
 print(w.get_balance(refresh=True))
 
 outputs = [('mqBuyzdHfD87VfgxaYeM9pex3sJn4ihYHY', 724), ('mr1FHq6GwWzmD1y8Jxq6rNDGsiiQ9caF7r', 996)]
 pushdatas = ['hello', b'world']
-print(w.send_transaction(outputs=outputs, pushdatas=pushdatas, combine=True))
+print(w.create_transaction(outputs=outputs, pushdatas=pushdatas, combine=True).broadcast())
 ```
 
 3. Operate P2PK
 
 ```python
+import time
+
 from bsvlib import Wallet, TxOutput, Transaction
 from bsvlib.constants import Chain
 from bsvlib.keys import Key
 from bsvlib.script import P2pkScriptType
-from bsvlib.service import SensibleQuery
 
+chain = Chain.TEST
 k = Key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
-p = SensibleQuery(chain=Chain.TEST)
-unspents = Wallet(provider=p).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
+unspents = Wallet(chain=chain).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
 
-t = Transaction(provider=p)
-t.add_inputs(unspents)
+t = Transaction(chain=chain).add_inputs(unspents)
 t.add_output(TxOutput(P2pkScriptType.locking(k.public_key().serialize()), 996, P2pkScriptType()))
-t.add_change(k.address())
+t.add_change(k.address()).sign()
+print(t.broadcast())
 
-print(t.sign().broadcast())
+time.sleep(2)
+tt = Transaction(chain=chain).add_inputs(t.to_unspents(args=[{'private_keys': [k]}] * 2)).add_change(k.address()).sign()
+print(tt.broadcast())
 ```
 
 4. Operate bare-multisig
 
 ```python
 import time
 from typing import List, Union
@@ -168,26 +171,26 @@
 8. Process HD wallet derivation
 
 ![image](https://user-images.githubusercontent.com/1585505/150875831-2663e158-b00d-4089-8276-1ad72e335d28.png)
 
 ```python
 from typing import List
 
-from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_from_mnemonic
+from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_xprvs_from_mnemonic
 
 #
 # HD derivation
 #
 entropy = 'cd9b819d9c62f0027116c1849e7d497f'
 
 # snow swing guess decide congress abuse session subway loyal view false zebra
 mnemonic: str = mnemonic_from_entropy(entropy)
 print(mnemonic)
 
-keys: List[Xprv] = derive_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
+keys: List[Xprv] = derive_xprvs_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
 for key in keys:
     print(key.address(), key.private_key().wif())
 
 #
 # random mnemonic
 #
 print()
```

### Comparing `bsvlib-0.8.1/bsvlib/aes.py` & `bsvlib-0.9.0/bsvlib/aes.py`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/bsvlib/base58.py` & `bsvlib-0.9.0/bsvlib/base58.py`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/bsvlib/constants.py` & `bsvlib-0.9.0/bsvlib/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 TRANSACTION_SEQUENCE: int = int(os.getenv('BSVLIB_TRANSACTION_SEQUENCE') or 0xffffffff)
 TRANSACTION_VERSION: int = int(os.getenv('BSVLIB_TRANSACTION_VERSION') or 1)
 TRANSACTION_LOCKTIME: int = int(os.getenv('BSVLIB_TRANSACTION_LOCKTIME') or 0)
 TRANSACTION_FEE_RATE: float = float(os.getenv('BSVLIB_TRANSACTION_FEE_RATE') or 0.5)  # satoshi per byte
 P2PKH_DUST_LIMIT: int = int(os.getenv('BSVLIB_P2PKH_DUST_LIMIT') or 135)
 HTTP_REQUEST_TIMEOUT: int = int(os.getenv('BSVLIB_HTTP_REQUEST_TIMEOUT') or 30)
 THREAD_POOL_MAX_EXECUTORS: int = int(os.getenv('BSVLIB_THREAD_POOL_MAX_EXECUTORS') or 10)
-BIP39_ENTROPY_DEFAULT_BIT_LENGTH: int = int(os.getenv('BSVLIB_BIP39_ENTROPY_DEFAULT_BIT_LENGTH') or 128)
+BIP39_ENTROPY_BIT_LENGTH: int = int(os.getenv('BSVLIB_BIP39_ENTROPY_BIT_LENGTH') or 128)
+BIP44_DERIVATION_PATH = os.getenv('BSVLIB_BIP44_DERIVATION_PATH') or "m/44'/236'/0'"
 METASV_TOKEN: Optional[str] = os.getenv('BSVLIB_METASV_TOKEN') or os.getenv('METASV_TOKEN')
 
 
 class Chain(str, Enum):
     MAIN = 'main'
     TEST = 'test'
```

### Comparing `bsvlib-0.8.1/bsvlib/curve.py` & `bsvlib-0.9.0/bsvlib/curve.py`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/bsvlib/hd/bip32.py` & `bsvlib-0.9.0/bsvlib/hd/bip32.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         if isinstance(o, Xkey):
             return self.payload == o.payload
         return super().__eq__(o)  # pragma: no cover
 
     def __str__(self) -> str:
         return base58check_encode(self.payload)
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
 
 class Xpub(Xkey):
 
     def __init__(self, xpub: Union[str, bytes]):
         super().__init__(xpub)
         self.chain: Chain = XPUB_PREFIX_CHAIN_DICT.get(self.prefix)
         assert self.chain, 'unknown xpub prefix'
```

### Comparing `bsvlib-0.8.1/bsvlib/hd/bip39.py` & `bsvlib-0.9.0/bsvlib/hd/bip39.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from contextlib import suppress
 from hashlib import pbkdf2_hmac
 from secrets import randbits
 from typing import List, Dict, Union
 
-from ..constants import BIP39_ENTROPY_BIT_LENGTH_LIST, BIP39_ENTROPY_DEFAULT_BIT_LENGTH
+from ..constants import BIP39_ENTROPY_BIT_LENGTH_LIST, BIP39_ENTROPY_BIT_LENGTH
 from ..hash import sha256
 from ..utils import bytes_to_bits, bits_to_bytes
 
 
 class WordList:
     """
     BIP39 word list
@@ -62,15 +62,15 @@
 
 def mnemonic_from_entropy(entropy: Union[bytes, str, None] = None, lang: str = 'en') -> str:
     if entropy:
         assert type(entropy).__name__ in ['bytes', 'str'], 'unsupported entropy type'
         entropy_bytes = entropy if isinstance(entropy, bytes) else bytes.fromhex(entropy)
     else:
         # random a new entropy
-        entropy_bytes = randbits(BIP39_ENTROPY_DEFAULT_BIT_LENGTH).to_bytes(BIP39_ENTROPY_DEFAULT_BIT_LENGTH // 8, 'big')
+        entropy_bytes = randbits(BIP39_ENTROPY_BIT_LENGTH).to_bytes(BIP39_ENTROPY_BIT_LENGTH // 8, 'big')
     entropy_bits: str = bytes_to_bits(entropy_bytes)
     assert len(entropy_bits) in BIP39_ENTROPY_BIT_LENGTH_LIST, 'invalid entropy bit length'
     checksum_bits: str = bytes_to_bits(sha256(entropy_bytes))[:len(entropy_bits) // 32]
 
     bits: str = entropy_bits + checksum_bits
     indexes_bits: List[str] = [bits[i:i + 11] for i in range(0, len(bits), 11)]
     return ' '.join([WordList.get_word(bits_to_bytes(index_bits), lang) for index_bits in indexes_bits])
```

### Comparing `bsvlib-0.8.1/bsvlib/hd/wordlist/chinese_simplified.txt` & `bsvlib-0.9.0/bsvlib/hd/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/bsvlib/hd/wordlist/english.txt` & `bsvlib-0.9.0/bsvlib/hd/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bsvlib-0.8.1/bsvlib/keys.py` & `bsvlib-0.9.0/bsvlib/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,17 @@
         if isinstance(o, PublicKey):
             return self.key == o.key
         return super().__eq__(o)  # pragma: no cover
 
     def __str__(self) -> str:  # pragma: no cover
         return f'<PublicKey hex={self.hex()}>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
 
 class PrivateKey:
 
     def __init__(self, private_key: Union[str, int, bytes, CcPrivateKey, None] = None, chain: Optional[Chain] = None):
         """
         create private key from WIF (str), or int, or bytes, or CoinCurve private key
         random a new private key if None
@@ -274,14 +277,17 @@
         if isinstance(o, PrivateKey):
             return self.key == o.key
         return super().__eq__(o)  # pragma: no cover
 
     def __str__(self) -> str:  # pragma: no cover
         return f'<PrivateKey wif={self.wif()} int={self.int()}>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def from_hex(cls, octets: Union[str, bytes]) -> 'PrivateKey':
         b: bytes = octets if isinstance(octets, bytes) else bytes.fromhex(octets)
         return PrivateKey(CcPrivateKey(b))
 
     @classmethod
     def from_der(cls, octets: Union[str, bytes]) -> 'PrivateKey':  # pragma: no cover
```

### Comparing `bsvlib-0.8.1/bsvlib/script/script.py` & `bsvlib-0.9.0/bsvlib/script/script.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,7 +39,10 @@
     def __eq__(self, o: object) -> bool:
         if isinstance(o, Script):
             return self.script == o.script
         return super().__eq__(o)  # pragma: no cover
 
     def __str__(self) -> str:  # pragma: no cover
         return self.script.hex()
+
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
```

### Comparing `bsvlib-0.8.1/bsvlib/script/type.py` & `bsvlib-0.9.0/bsvlib/script/type.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,28 +43,34 @@
 
 
 class UnknownScriptType(ScriptType):  # pragma: no cover
 
     def __str__(self) -> str:
         return '<ScriptType:Unknown>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def unlocking(cls, **kwargs) -> Script:
         raise ValueError("don't know how to unlock for script of unknown type")
 
     @classmethod
     def estimated_unlocking_byte_length(cls, **kwargs) -> int:
         raise ValueError("don't know how to unlock for script of unknown type")
 
 
 class P2pkhScriptType(ScriptType):
 
     def __str__(self) -> str:  # pragma: no cover
         return '<ScriptType:P2PKH>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def locking(cls, value: Union[str, bytes]) -> Script:
         """
         from address (str) or public key hash160 (bytes)
         """
         if isinstance(value, str):
             pkh: bytes = address_to_public_key_hash(value)
@@ -88,14 +94,17 @@
 
 
 class OpReturnScriptType(ScriptType):
 
     def __str__(self) -> str:  # pragma: no cover
         return '<ScriptType:OP_RETURN>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def locking(cls, pushdatas: List[Union[str, bytes]]) -> Script:
         script: bytes = OP.OP_FALSE + OP.OP_RETURN
         for pushdata in pushdatas:
             if isinstance(pushdata, str):
                 pushdata_bytes: bytes = pushdata.encode('utf-8')
             elif isinstance(pushdata, bytes):
@@ -115,14 +124,17 @@
 
 
 class P2pkScriptType(ScriptType):
 
     def __str__(self) -> str:  # pragma: no cover
         return '<ScriptType:P2PK>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def locking(cls, public_key: Union[str, bytes]) -> Script:
         """
         from public key in format str or bytes
         """
         if isinstance(public_key, str):
             pk: bytes = bytes.fromhex(public_key)
@@ -145,14 +157,17 @@
 
 
 class BareMultisigScriptType(ScriptType):
 
     def __str__(self) -> str:  # pragma: no cover
         return '<ScriptType:BareMultisig>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def locking(cls, participants: List[Union[str, bytes]], threshold: int) -> Script:
         assert 1 <= threshold <= len(participants), 'bad threshold or number of participants'
         script: bytes = encode_int(threshold)
         for participant in participants:
             assert type(participant).__name__ in ['str', 'bytes'], 'unsupported public key type'
             if isinstance(participant, str):
```

### Comparing `bsvlib-0.8.1/bsvlib/service/metasv.py` & `bsvlib-0.9.0/bsvlib/service/metasv.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,48 +23,50 @@
             params = {}
             if flag:
                 params['flag'] = flag
             return self.get(url=f'{self.url}/address/{address}/utxo', params=params)
         return []
 
     def get_unspents(self, **kwargs) -> List[Dict]:
-        """
-        only P2PKH unspents
-        """
-        with suppress(Exception):
+        try:
             address, _, _ = self.parse_kwargs(**kwargs)
             # paging
             paged_unspents: List[Dict] = self._get_unspents(address)
             total_unspents: List[Dict] = paged_unspents
             while paged_unspents:
                 paged_unspents = self._get_unspents(address, paged_unspents[-1]['flag'])
                 total_unspents.extend(paged_unspents or [])
             # parsing
             unspents: List[Dict] = []
             for item in total_unspents:
                 unspent = {'txid': item['txid'], 'vout': item['outIndex'], 'satoshi': item['value'], 'height': item['height']}
                 unspent.update(kwargs)
                 unspents.append(unspent)
             return unspents
+        except Exception as e:
+            if kwargs.get('throw'):
+                raise e
         return []
 
     def get_balance(self, **kwargs) -> int:
-        with suppress(Exception):
+        try:
             address, _, _ = self.parse_kwargs(**kwargs)
             r: Dict = self.get(url=f'{self.url}/address/{address}/balance')
             return r.get('confirmed') + r.get('unconfirmed')
+        except Exception as e:
+            if kwargs.get('throw'):
+                raise e
         return 0
 
     def broadcast(self, raw: str) -> BroadcastResult:
         propagated, message = False, ''
         try:
             data = json.dumps({'hex': raw})
             _r = requests.post(f'{self.url}/tx/broadcast', headers=self.headers, data=data, timeout=self.timeout)
             _r.raise_for_status()
-
             r = _r.json()
             assert r, f'empty response {r}'
             if r.get('txid'):
                 propagated, message = True, r['txid']
             else:
                 propagated, message = False, r.get('message')
         except Exception as e:
```

### Comparing `bsvlib-0.8.1/bsvlib/service/provider.py` & `bsvlib-0.9.0/bsvlib/service/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,20 @@
         address: str = kwargs.get('address') or (public_key.address(chain=self.chain) if public_key else None)
         return address, public_key, private_key
 
     def get(self, **kwargs) -> Union[Dict, List[Dict]]:
         """
         HTTP GET wrapper
         """
-        r = requests.get(kwargs['url'], headers=self.headers, params=kwargs.get('params'), timeout=self.timeout)
+        r = requests.get(
+            kwargs['url'],
+            headers=kwargs.get('headers') or self.headers,
+            params=kwargs.get('params'),
+            timeout=kwargs.get('timeout') or self.timeout
+        )
         r.raise_for_status()
         return r.json()
 
     @abstractmethod
     def get_unspents(self, **kwargs) -> List[Dict]:
         """kwargs will pass the following at least
         {
```

### Comparing `bsvlib-0.8.1/bsvlib/service/service.py` & `bsvlib-0.9.0/bsvlib/service/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 from .whatsonchain import WhatsOnChain
 from ..constants import Chain, METASV_TOKEN
 
 
 class Service:
 
     def __init__(self, chain: Optional[Chain] = None, provider: Optional[Provider] = None):
-        chain = chain or Chain.MAIN
-        default_provider = MetaSV(token=METASV_TOKEN) if chain == Chain.MAIN and METASV_TOKEN else WhatsOnChain(chain)
-        self.provider = provider or default_provider
+        if provider:
+            self.provider = provider
+        else:
+            chain = chain or Chain.MAIN
+            self.provider = MetaSV(token=METASV_TOKEN) if chain == Chain.MAIN and METASV_TOKEN else WhatsOnChain(chain)
         self.chain = self.provider.chain
 
     def get_unspents(self, **kwargs) -> List[Dict]:
         """kwargs will pass the following at least
         {
             'private_keys': List[bsvlib.keys.PrivateKey],
         }
```

### Comparing `bsvlib-0.8.1/bsvlib/service/whatsonchain.py` & `bsvlib-0.9.0/bsvlib/service/whatsonchain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import json
-from contextlib import suppress
 from typing import List, Dict, Optional
 
 import requests
 
 from .provider import Provider, BroadcastResult
 from ..constants import Chain
 
 
-class WhatsOnChain(Provider):
+class WhatsOnChain(Provider):  # pragma: no cover
 
     def __init__(self, chain: Chain = Chain.MAIN, headers: Optional[Dict] = None, timeout: Optional[int] = None):
         super().__init__(chain, headers, timeout)
         self.url: str = 'https://api.whatsonchain.com/v1/bsv'
 
     def get_unspents(self, **kwargs) -> List[Dict]:
-        """
-        only P2PKH unspents
-        """
-        with suppress(Exception):
+        try:
             address, _, _ = self.parse_kwargs(**kwargs)
             r: Dict = self.get(url=f'{self.url}/{self.chain}/address/{address}/unspent')
             unspents: List[Dict] = []
             for item in r:  # pragma: no cover
                 unspent = {'txid': item['tx_hash'], 'vout': item['tx_pos'], 'satoshi': item['value'], 'height': item['height']}
                 unspent.update(kwargs)
                 unspents.append(unspent)
             return unspents
-        return []  # pragma: no cover
+        except Exception as e:
+            if kwargs.get('throw'):
+                raise e
+        return []
 
     def get_balance(self, **kwargs) -> int:
-        with suppress(Exception):
+        try:
             address, _, _ = self.parse_kwargs(**kwargs)
             r: Dict = self.get(url=f'{self.url}/{self.chain}/address/{address}/balance')
             return r.get('confirmed') + r.get('unconfirmed')
-        return 0  # pragma: no cover
+        except Exception as e:
+            if kwargs.get('throw'):
+                raise e
+        return 0
 
-    def broadcast(self, raw: str) -> BroadcastResult:  # pragma: no cover
+    def broadcast(self, raw: str) -> BroadcastResult:
         propagated, message = False, ''
         try:
             data = json.dumps({'txHex': raw})
             r = requests.post(f'{self.url}/{self.chain}/tx/raw', headers=self.headers, data=data, timeout=self.timeout)
             message = r.json()
             r.raise_for_status()
             propagated = True
```

### Comparing `bsvlib-0.8.1/bsvlib/transaction/transaction.py` & `bsvlib-0.9.0/bsvlib/transaction/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         stream.write(self.unlocking_script.serialize() if self.unlocking_script else b'')
         stream.write(self.sequence.to_bytes(4, 'little'))
         return stream.getvalue()
 
     def __str__(self) -> str:  # pragma: no cover
         return f'<TxInput outpoint={self.txid}:{self.vout} satoshi={self.satoshi} locking_script={self.locking_script}>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def from_hex(cls, stream: Union[str, bytes, TransactionBytesIO]) -> Optional['TxInput']:
         with suppress(Exception):
             stream = stream if isinstance(stream, TransactionBytesIO) else TransactionBytesIO(stream if isinstance(stream, bytes) else bytes.fromhex(stream))
             txid = stream.read_bytes(32)[::-1]
             assert len(txid) == 32
             vout = stream.read_int(4)
@@ -100,20 +103,17 @@
             assert sequence is not None
             return TxInput(unspent=Unspent(txid=txid.hex(), vout=vout, satoshi=0, locking_script=Script()), unlocking_script=Script(unlocking_script_bytes), sequence=sequence)
         return None
 
 
 class TxOutput:
 
-    def __init__(self, out: Union[str, List[Union[str, bytes]], Script, None] = None, satoshi: int = 0, script_type: ScriptType = UnknownScriptType()):
+    def __init__(self, out: Union[str, List[Union[str, bytes]], Script], satoshi: int = 0, script_type: ScriptType = UnknownScriptType()):
         self.satoshi = satoshi
-        if out is None:
-            self.locking_script: Script = Script()
-            self.script_type: ScriptType = UnknownScriptType()
-        elif isinstance(out, str):
+        if isinstance(out, str):
             # from address
             self.locking_script: Script = P2pkhScriptType.locking(out)
             self.script_type: ScriptType = P2pkhScriptType()
         elif isinstance(out, List):
             # from list of pushdata
             self.locking_script: Script = OpReturnScriptType.locking(out)
             self.script_type: ScriptType = OpReturnScriptType()
@@ -126,14 +126,17 @@
 
     def serialize(self) -> bytes:
         return self.satoshi.to_bytes(8, 'little') + self.locking_script.byte_length_varint() + self.locking_script.serialize()
 
     def __str__(self) -> str:  # pragma: no cover
         return f'<TxOutput satoshi={self.satoshi} locking_script={self.locking_script.hex()}>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     @classmethod
     def from_hex(cls, stream: Union[str, bytes, TransactionBytesIO]) -> Optional['TxOutput']:
         with suppress(Exception):
             stream = stream if isinstance(stream, TransactionBytesIO) else TransactionBytesIO(stream if isinstance(stream, bytes) else bytes.fromhex(stream))
             satoshi = stream.read_int(8)
             assert satoshi is not None
             script_length = stream.read_varint()
@@ -316,14 +319,15 @@
         return len(self.serialize())
 
     size = byte_length
 
     def estimated_byte_length(self, **kwargs) -> int:
         """
         :returns: estimated byte length of this transaction after signing
+        if transaction has already signed, it will return the same value as function byte_length
         """
         estimated_length = 4 + len(unsigned_to_varint(len(self.tx_inputs))) + len(unsigned_to_varint(len(self.tx_outputs))) + 4
         for tx_input in self.tx_inputs:
             if tx_input.unlocking_script is not None:
                 # unlocking script already set
                 estimated_length += len(tx_input.serialize())
             else:
@@ -357,17 +361,17 @@
                         break
             else:
                 change_output = TxOutput(out=change_address, satoshi=fee_overpaid)
             assert change_output, "can't parse any address from transaction inputs"
             self.add_output(change_output)
         return self
 
-    def broadcast(self) -> BroadcastResult:  # pragma: no cover
-        fee_expected = math.ceil(self.fee_rate * self.byte_length())
-        if self.fee() < fee_expected:
+    def broadcast(self, check_fee: bool = True) -> BroadcastResult:  # pragma: no cover
+        fee_expected = self.estimated_fee()
+        if check_fee and self.fee() < fee_expected:
             raise InsufficientFunds(f'require {self.satoshi_total_out() + fee_expected} satoshi but only {self.satoshi_total_in()}')
         return Service(self.chain, self.provider).broadcast(self.hex())
 
     def to_unspent(self, vout: int, **kwargs) -> Optional[Unspent]:
         assert 0 <= vout < len(self.tx_outputs), 'vout out of range'
         out = self.tx_outputs[vout]
         if out.script_type in [OpReturnScriptType()]:
```

### Comparing `bsvlib-0.8.1/bsvlib/transaction/unspent.py` & `bsvlib-0.9.0/bsvlib/transaction/unspent.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self.locking_script: Script = kwargs.get('locking_script') or (P2pkhScriptType.locking(self.address) if self.address else Script())
         # validate
         assert self.txid and len(self.txid) == 64 and self.vout is not None and self.satoshi is not None and self.locking_script, 'bad unspent'
 
     def __str__(self) -> str:  # pragma: no cover
         return f'<Unspent outpoint={self.txid}:{self.vout} satoshi={self.satoshi} script={self.locking_script}>'
 
+    def __repr__(self) -> str:  # pragma: no cover
+        return self.__str__()
+
     def __eq__(self, o: object) -> bool:  # pragma: no cover
         if isinstance(o, Unspent):
             return self.txid == o.txid and self.vout == o.vout
         return super().__eq__(o)
 
     def __hash__(self) -> int:  # pragma: no cover
         return f'{self.txid}:{self.vout}'.__hash__()
```

### Comparing `bsvlib-0.8.1/bsvlib/utils.py` & `bsvlib-0.9.0/bsvlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import re
 from base64 import b64encode, b64decode
 from contextlib import suppress
 from typing import Tuple, Optional, Union
 
 import requests
 from typing_extensions import Literal
@@ -27,15 +28,15 @@
         return b'\xff' + num.to_bytes(8, 'little')
 
 
 def unsigned_to_bytes(num: int, byteorder: Literal['big', 'little'] = 'big') -> bytes:
     """
     convert an unsigned int to the least number of bytes as possible.
     """
-    return num.to_bytes((num.bit_length() + 7) // 8 or 1, byteorder)
+    return num.to_bytes(math.ceil(num.bit_length() / 8) or 1, byteorder)
 
 
 def decode_address(address: str) -> Tuple[bytes, Chain]:
     """
     :returns: tuple (public_key_hash_bytes, chain)
     """
     if not re.match(r'^[1mn][a-km-zA-HJ-NP-Z1-9]{24,33}$', address):
@@ -264,10 +265,11 @@
     if len(bits) < len(b) * 8:
         bits = '0' * (len(b) * 8 - len(bits)) + bits
     return bits
 
 
 def bits_to_bytes(bits: str) -> bytes:
     """
-    convert binary 0/1 string to the least number of bytes
+    convert binary 0/1 string to bytes
     """
-    return unsigned_to_bytes(int(bits, 2))
+    byte_length = math.ceil(len(bits) / 8) or 1
+    return int(bits, 2).to_bytes(byte_length, byteorder='big')
```

### Comparing `bsvlib-0.8.1/bsvlib/wallet.py` & `bsvlib-0.9.0/bsvlib/wallet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from concurrent.futures import ThreadPoolExecutor
 from itertools import repeat
 from typing import Optional, List, Tuple, Union, Dict, Any
 
 from .constants import Chain, THREAD_POOL_MAX_EXECUTORS
 from .keys import PrivateKey
-from .service.provider import Provider, BroadcastResult
+from .service.provider import Provider
 from .service.service import Service
 from .transaction.transaction import Transaction, TxOutput, InsufficientFunds
 from .transaction.unspent import Unspent
 
 
 def get_unspents_wrapper(chain: Chain, provider: Provider, d: Dict) -> List['Unspent']:
     return Unspent.get_unspents(chain, provider, **d)
@@ -67,71 +67,64 @@
             chain: Chain = kwargs.pop('chain', None) or self.chain
             provider: Provider = kwargs.pop('provider', None) or self.provider
             with ThreadPoolExecutor(max_workers=THREAD_POOL_MAX_EXECUTORS) as executor:
                 args = [dict(private_keys=[key], **{**self.kwargs, **kwargs}) for key in self.keys]
                 return sum([r for r in executor.map(get_balance_wrapper, repeat(chain), repeat(provider), args)])
         return sum([unspent.satoshi for unspent in self.unspents])
 
-    def create_transaction(self, outputs: Optional[List[Tuple]] = None, leftover: Optional[str] = None,
-                           fee_rate: Optional[float] = None, unspents: Optional[List[Unspent]] = None,
+    def create_transaction(self, unspents: Optional[List[Unspent]] = None, outputs: Optional[List[Tuple]] = None,
+                           leftover: Optional[str] = None, fee_rate: Optional[float] = None,
                            combine: bool = False, pushdatas: Optional[List[Union[str, bytes]]] = None,
                            change: bool = True, sign: bool = True, **kwargs) -> Transaction:  # pragma: no cover
-        """create a signed transaction
+        """create a transaction
+        :param unspents: list of unspents, will refresh from service if None
         :param outputs: list of tuple (address, satoshi). if None then sweep all the unspents to leftover
         :param leftover: transaction change address
-        :param fee_rate: 0.5 satoshi per byte if None
-        :param unspents: list of unspents, will refresh from service if None
+        :param fee_rate: default fee rate if None
         :param combine: use all available unspents if True
         :param pushdatas: list of OP_RETURN pushdata
         :param change: automatically add a P2PKH change output if True
         :param sign: sign the transaction if True
         :param kwargs: passing to get unspents and create transaction
         """
         unspents: List[Unspent] = unspents or self.get_unspents(refresh=True, **{**self.kwargs, **kwargs})
-        if not unspents:
-            raise InsufficientFunds('transaction mush have at least one unspent')
+        return create_transaction(unspents, outputs, leftover, fee_rate, combine, pushdatas, change, sign, self.chain, self.provider, **{**self.kwargs, **kwargs})
 
-        t = Transaction(fee_rate=fee_rate, chain=self.chain, provider=self.provider, **{**self.kwargs, **kwargs})
-        if pushdatas:
-            t.add_output(TxOutput(pushdatas))
-        if outputs:
-            t.add_outputs([TxOutput(output[0], output[1]) for output in outputs])
-        # pick unspent
-        picked_unspents: List[Unspent] = []
-        if combine or not outputs:
-            picked_unspents = unspents
-            unspents = []
-            t.add_inputs([unspent for unspent in picked_unspents])
-        else:
-            unspent = unspents.pop()
-            picked_unspents.append(unspent)
-            t.add_input(unspent)
-            while t.fee() < t.estimated_fee() and unspents:
-                unspent = unspents.pop()
-                picked_unspents.append(unspent)
-                t.add_input(unspent)
-        if t.fee() < t.estimated_fee():
-            unspents.extend(picked_unspents)
-            raise InsufficientFunds(f'require {t.estimated_fee() + t.satoshi_total_out()} satoshi but only {t.satoshi_total_in()}')
-        else:
-            self.unspents = list(set(self.unspents) - set(picked_unspents))
-        if change:
-            t.add_change(leftover)
-        if sign:
-            t.sign()
-        return t
-
-    def send_transaction(self, outputs: Optional[List[Tuple]] = None, leftover: Optional[str] = None,
-                         fee_rate: Optional[float] = None, unspents: Optional[List[Unspent]] = None,
-                         combine: bool = False, pushdatas: Optional[List[Union[str, bytes]]] = None,
-                         **kwargs) -> BroadcastResult:  # pragma: no cover
-        """send a transaction
-        :param outputs: list of tuple (address, satoshi). if None then sweep all the unspents to leftover
-        :param leftover: transaction change address
-        :param fee_rate: 0.5 satoshi per byte if None
-        :param unspents: list of unspents, will refresh from service if None
-        :param combine: use all available unspents if True
-        :param pushdatas: list of OP_RETURN pushdata
-        :param kwargs: passing to get unspents and sign
-        :returns: txid if successfully otherwise None
-        """
-        return self.create_transaction(outputs, leftover, fee_rate, unspents, combine, pushdatas, True, True, **kwargs).broadcast()
+
+def create_transaction(unspents: List[Unspent], outputs: Optional[List[Tuple]] = None, leftover: Optional[str] = None,
+                       fee_rate: Optional[float] = None, combine: bool = False, pushdatas: Optional[List[Union[str, bytes]]] = None,
+                       change: bool = True, sign: bool = True, chain: Optional[Chain] = None, provider: Optional[Provider] = None,
+                       **kwargs) -> Transaction:  # pragma: no cover
+    """create a transaction
+    :param unspents: list of unspents, will refresh from service if None
+    :param outputs: list of tuple (address, satoshi). if None then sweep all the unspents to leftover
+    :param leftover: transaction change address
+    :param fee_rate: default fee rate if None
+    :param combine: use all available unspents if True
+    :param pushdatas: list of OP_RETURN pushdata
+    :param change: automatically add a P2PKH change output if True
+    :param sign: sign the transaction if True
+    :param chain: network chain
+    :param provider: service provider
+    :param kwargs: passing to get unspents and create transaction
+    """
+    if not unspents:
+        raise InsufficientFunds('transaction mush have at least one unspent')
+    t = Transaction(fee_rate=fee_rate, chain=chain, provider=provider, **kwargs)
+    if pushdatas:
+        t.add_output(TxOutput(pushdatas))
+    if outputs:
+        t.add_outputs([TxOutput(output[0], output[1]) for output in outputs])
+    # pick unspent
+    picked_unspents: List[Unspent] = []
+    while unspents and (combine or not outputs or t.fee() < t.estimated_fee()):
+        unspent = unspents.pop()
+        picked_unspents.append(unspent)
+        t.add_input(unspent)
+    if t.fee() < t.estimated_fee():
+        unspents.extend(picked_unspents)
+        raise InsufficientFunds(f'require {t.estimated_fee() + t.satoshi_total_out()} satoshi but only {t.satoshi_total_in()}')
+    if change:
+        t.add_change(leftover)
+    if sign:
+        t.sign()
+    return t
```

### Comparing `bsvlib-0.8.1/bsvlib.egg-info/PKG-INFO` & `bsvlib-0.9.0/bsvlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsvlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: Bitcoin SV (BSV) Python Library
 Home-page: https://github.com/gitzhou/bsvlib
 Author: aaron67
 Author-email: aaron67@aaron67.cc
 Project-URL: Bug Tracker, https://github.com/gitzhou/bsvlib/issues
 Keywords: bsv,bitcoin-sv,bitcoin sv,bitcoinsv,cryptocurrency,payments,tools,wallet
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 
 A Bitcoin SV (BSV) Python Library that is extremely simple to use but more.
 
 - MAINNET and TESTNET supported
 - P2PKH, P2PK, and bare-multisig supported
 - All the SIGHASH flags supported
 - Additional script types can be customized
-- [MetaSV](https://metasv.com/), [SensibleQuery](https://api.sensiblequery.com/swagger/index.html), and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
+- [MetaSV](https://metasv.com/) and [WhatsOnChain](https://developers.whatsonchain.com/) API integrated
 - Ability to adapt to different service providers
 - Fully ECDSA implementation
 - ECDH and Electrum ECIES (aka BIE1) implementation
 - HD implementation (BIP-32, BIP-39, BIP-44)
 
 👉 [Join our Telegram group for discussions or support](https://t.me/bsvlib).
 
@@ -51,15 +51,15 @@
 
 1. Send BSV in one line
 
 ```python
 from bsvlib import Wallet
 
 # Donate to aaron67!
-print(Wallet(['YOUR_WIF_GOES_HERE']).send_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]))
+print(Wallet(['YOUR_WIF']).create_transaction(outputs=[('1HYeFCE2KG4CW4Jwz5NmDqAZK9Q626ChmN', 724996)]).broadcast())
 ```
 
 2. Send unspent locked by different keys in one transaction, support OP_RETURN output as well
 
 ```python
 from bsvlib import Wallet
 from bsvlib.constants import Chain
@@ -68,36 +68,39 @@
 
 w.add_key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
 w.add_key('93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me')
 print(w.get_balance(refresh=True))
 
 outputs = [('mqBuyzdHfD87VfgxaYeM9pex3sJn4ihYHY', 724), ('mr1FHq6GwWzmD1y8Jxq6rNDGsiiQ9caF7r', 996)]
 pushdatas = ['hello', b'world']
-print(w.send_transaction(outputs=outputs, pushdatas=pushdatas, combine=True))
+print(w.create_transaction(outputs=outputs, pushdatas=pushdatas, combine=True).broadcast())
 ```
 
 3. Operate P2PK
 
 ```python
+import time
+
 from bsvlib import Wallet, TxOutput, Transaction
 from bsvlib.constants import Chain
 from bsvlib.keys import Key
 from bsvlib.script import P2pkScriptType
-from bsvlib.service import SensibleQuery
 
+chain = Chain.TEST
 k = Key('cVwfreZB3i8iv9JpdSStd9PWhZZGGJCFLS4rEKWfbkahibwhticA')
-p = SensibleQuery(chain=Chain.TEST)
-unspents = Wallet(provider=p).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
+unspents = Wallet(chain=chain).add_keys([k, '93UnxexmsTYCmDJdctz4zacuwxQd5prDmH6rfpEyKkQViAVA3me']).get_unspents(refresh=True)
 
-t = Transaction(provider=p)
-t.add_inputs(unspents)
+t = Transaction(chain=chain).add_inputs(unspents)
 t.add_output(TxOutput(P2pkScriptType.locking(k.public_key().serialize()), 996, P2pkScriptType()))
-t.add_change(k.address())
+t.add_change(k.address()).sign()
+print(t.broadcast())
 
-print(t.sign().broadcast())
+time.sleep(2)
+tt = Transaction(chain=chain).add_inputs(t.to_unspents(args=[{'private_keys': [k]}] * 2)).add_change(k.address()).sign()
+print(tt.broadcast())
 ```
 
 4. Operate bare-multisig
 
 ```python
 import time
 from typing import List, Union
@@ -189,26 +192,26 @@
 8. Process HD wallet derivation
 
 ![image](https://user-images.githubusercontent.com/1585505/150875831-2663e158-b00d-4089-8276-1ad72e335d28.png)
 
 ```python
 from typing import List
 
-from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_from_mnemonic
+from bsvlib.hd import mnemonic_from_entropy, Xprv, derive_xprvs_from_mnemonic
 
 #
 # HD derivation
 #
 entropy = 'cd9b819d9c62f0027116c1849e7d497f'
 
 # snow swing guess decide congress abuse session subway loyal view false zebra
 mnemonic: str = mnemonic_from_entropy(entropy)
 print(mnemonic)
 
-keys: List[Xprv] = derive_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
+keys: List[Xprv] = derive_xprvs_from_mnemonic(mnemonic, path="m/44'/0'/0'", change=1, index_start=0, index_end=5)
 for key in keys:
     print(key.address(), key.private_key().wif())
 
 #
 # random mnemonic
 #
 print()
```

### Comparing `bsvlib-0.8.1/bsvlib.egg-info/SOURCES.txt` & `bsvlib-0.9.0/bsvlib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,13 +25,12 @@
 bsvlib/hd/wordlist/english.txt
 bsvlib/script/__init__.py
 bsvlib/script/script.py
 bsvlib/script/type.py
 bsvlib/service/__init__.py
 bsvlib/service/metasv.py
 bsvlib/service/provider.py
-bsvlib/service/sensiblequery.py
 bsvlib/service/service.py
 bsvlib/service/whatsonchain.py
 bsvlib/transaction/__init__.py
 bsvlib/transaction/transaction.py
 bsvlib/transaction/unspent.py
```

### Comparing `bsvlib-0.8.1/setup.cfg` & `bsvlib-0.9.0/setup.cfg`

 * *Files identical despite different names*

