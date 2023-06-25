# Comparing `tmp/easyencryption-0.1.5.1.tar.gz` & `tmp/easyencryption-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.5.1.tar", last modified: Mon Jun 19 16:46:48 2023, max compression
+gzip compressed data, was "easyencryption-0.1.6.tar", last modified: Sun Jun 25 21:43:19 2023, max compression
```

## Comparing `easyencryption-0.1.5.1.tar` & `easyencryption-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.870244 easyencryption-0.1.5.1/
--rw-rw-rw-   0        0        0     2810 2023-06-19 16:46:48.871286 easyencryption-0.1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1708 2023-06-19 16:45:47.000000 easyencryption-0.1.5.1/README.md
--rw-rw-rw-   0        0        0      723 2023-06-19 16:46:48.876241 easyencryption-0.1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1841 2023-06-19 16:46:10.000000 easyencryption-0.1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.787706 easyencryption-0.1.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.819240 easyencryption-0.1.5.1/src/easyencryption/
--rw-rw-rw-   0        0        0      456 2023-06-19 16:39:25.000000 easyencryption-0.1.5.1/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-06-17 21:41:40.000000 easyencryption-0.1.5.1/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1087 2023-06-17 21:41:44.000000 easyencryption-0.1.5.1/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2034 2023-06-17 21:41:48.000000 easyencryption-0.1.5.1/src/easyencryption/pubprivate.py
--rw-rw-rw-   0        0        0     2057 2023-06-19 16:36:12.000000 easyencryption-0.1.5.1/src/easyencryption/sha.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.867241 easyencryption-0.1.5.1/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     2810 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.730664 easyencryption-0.1.6/
+-rw-rw-rw-   0        0        0     3310 2023-06-25 21:43:19.730664 easyencryption-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2054 2023-06-25 21:41:37.000000 easyencryption-0.1.6/README.md
+-rw-rw-rw-   0        0        0      723 2023-06-25 21:43:19.732666 easyencryption-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1992 2023-06-25 21:42:28.000000 easyencryption-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.686144 easyencryption-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.705153 easyencryption-0.1.6/src/easyencryption/
+-rw-rw-rw-   0        0        0      606 2023-06-25 21:37:29.000000 easyencryption-0.1.6/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.6/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2034 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/pubprivate.py
+-rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/sha.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.728664 easyencryption-0.1.6/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3310 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.5.1/PKG-INFO` & `easyencryption-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.5.1
+Version: 0.1.6
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -13,14 +13,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -28,15 +31,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.5.1/README.md` & `easyencryption-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.5.1/setup.cfg` & `easyencryption-0.1.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6173 7965 6e63 7279 7074 696f   = easyencryptio
 00000020: 6e0d 0a76 6572 7369 6f6e 203d 2030 2e31  n..version = 0.1
-00000030: 2e35 0d0a 6175 7468 6f72 203d 2062 6c61  .5..author = bla
+00000030: 2e36 0d0a 6175 7468 6f72 203d 2062 6c61  .6..author = bla
 00000040: 7a65 6e0d 0a61 7574 686f 725f 656d 6169  zen..author_emai
 00000050: 6c20 3d20 636f 6e74 6163 7440 6669 7265  l = contact@fire
 00000060: 6261 6c6c 626f 742e 636f 6d0d 0a64 6573  ballbot.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2076 6572  cription = A ver
 00000080: 7920 6561 7379 2077 6179 2074 6f20 656e  y easy way to en
 00000090: 6372 7970 7420 6461 7461 0d0a 6c6f 6e67  crypt data..long
 000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `easyencryption-0.1.5.1/setup.py` & `easyencryption-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.5.1"
+version = "0.1.6"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -38,14 +38,17 @@
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities',
       ]
 )
 #© 2021 GitHub, Inc.
```

### Comparing `easyencryption-0.1.5.1/src/easyencryption/aes.py` & `easyencryption-0.1.6/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5.1/src/easyencryption/fernet.py` & `easyencryption-0.1.6/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5.1/src/easyencryption/pubprivate.py` & `easyencryption-0.1.6/src/easyencryption/pubprivate.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5.1/src/easyencryption/sha.py` & `easyencryption-0.1.6/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5.1/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.6/src/easyencryption.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.5.1
+Version: 0.1.6
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -13,14 +13,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -28,15 +31,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

