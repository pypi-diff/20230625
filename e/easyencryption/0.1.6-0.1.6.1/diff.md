# Comparing `tmp/easyencryption-0.1.6.tar.gz` & `tmp/easyencryption-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.6.tar", last modified: Sun Jun 25 21:43:19 2023, max compression
+gzip compressed data, was "easyencryption-0.1.6.1.tar", last modified: Sun Jun 25 21:45:44 2023, max compression
```

## Comparing `easyencryption-0.1.6.tar` & `easyencryption-0.1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.730664 easyencryption-0.1.6/
--rw-rw-rw-   0        0        0     3310 2023-06-25 21:43:19.730664 easyencryption-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2054 2023-06-25 21:41:37.000000 easyencryption-0.1.6/README.md
--rw-rw-rw-   0        0        0      723 2023-06-25 21:43:19.732666 easyencryption-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1992 2023-06-25 21:42:28.000000 easyencryption-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.686144 easyencryption-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.705153 easyencryption-0.1.6/src/easyencryption/
--rw-rw-rw-   0        0        0      606 2023-06-25 21:37:29.000000 easyencryption-0.1.6/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.6/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2034 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/pubprivate.py
--rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.6/src/easyencryption/sha.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:43:19.728664 easyencryption-0.1.6/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3310 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 21:43:19.000000 easyencryption-0.1.6/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 21:45:44.624129 easyencryption-0.1.6.1/
+-rw-rw-rw-   0        0        0     3330 2023-06-25 21:45:44.624129 easyencryption-0.1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2072 2023-06-25 21:45:24.000000 easyencryption-0.1.6.1/README.md
+-rw-rw-rw-   0        0        0      723 2023-06-25 21:45:44.628125 easyencryption-0.1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-06-25 21:45:33.000000 easyencryption-0.1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:45:44.601125 easyencryption-0.1.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 21:45:44.609129 easyencryption-0.1.6.1/src/easyencryption/
+-rw-rw-rw-   0        0        0      606 2023-06-25 21:37:29.000000 easyencryption-0.1.6.1/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-06-24 15:16:52.000000 easyencryption-0.1.6.1/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.6.1/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.6.1/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2034 2023-06-24 15:16:52.000000 easyencryption-0.1.6.1/src/easyencryption/pubprivate.py
+-rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.6.1/src/easyencryption/sha.py
+drwxrwxrwx   0        0        0        0 2023-06-25 21:45:44.623130 easyencryption-0.1.6.1/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-06-25 21:45:44.000000 easyencryption-0.1.6.1/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-25 21:45:44.000000 easyencryption-0.1.6.1/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 21:45:44.000000 easyencryption-0.1.6.1/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-25 21:45:44.000000 easyencryption-0.1.6.1/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 21:45:44.000000 easyencryption-0.1.6.1/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.6/PKG-INFO` & `easyencryption-0.1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -31,16 +31,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.6/README.md` & `easyencryption-0.1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.6/setup.cfg` & `easyencryption-0.1.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/setup.py` & `easyencryption-0.1.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.6"
+version = "0.1.6.1"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.6/src/easyencryption/__init__.py` & `easyencryption-0.1.6.1/src/easyencryption/__init__.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption/aes.py` & `easyencryption-0.1.6.1/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption/custom.py` & `easyencryption-0.1.6.1/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption/fernet.py` & `easyencryption-0.1.6.1/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption/pubprivate.py` & `easyencryption-0.1.6.1/src/easyencryption/pubprivate.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption/sha.py` & `easyencryption-0.1.6.1/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.6/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.6.1/src/easyencryption.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -31,16 +31,16 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

