# Comparing `tmp/crypto-screening-1.0.2.tar.gz` & `tmp/crypto-screening-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.0.2.tar", last modified: Sun Jun 25 15:39:07 2023, max compression
+gzip compressed data, was "crypto-screening-1.0.3.tar", last modified: Sun Jun 25 16:31:23 2023, max compression
```

## Comparing `crypto-screening-1.0.2.tar` & `crypto-screening-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.889730 crypto-screening-1.0.2/
--rw-rw-rw-   0        0        0       98 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-25 15:39:07.888713 crypto-screening-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/build.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.870714 crypto-screening-1.0.2/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/base.py
--rw-rw-rw-   0        0        0    23575 2023-06-25 15:15:52.000000 crypto-screening-1.0.2/crypto_screening/collect.py
--rw-rw-rw-   0        0        0    12461 2023-06-25 15:33:45.000000 crypto-screening-1.0.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.0.2/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.0.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32685 2023-06-25 15:28:31.000000 crypto-screening-1.0.2/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.0.2/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2392 2023-06-25 15:15:52.000000 crypto-screening-1.0.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0    34516 2023-06-25 15:38:04.000000 crypto-screening-1.0.2/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9867 2023-06-25 14:09:42.000000 crypto-screening-1.0.2/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.887713 crypto-screening-1.0.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       73 2023-06-23 16:55:08.000000 crypto-screening-1.0.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 15:39:07.889730 crypto-screening-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-25 15:39:00.000000 crypto-screening-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:31:23.256883 crypto-screening-1.0.3/
+-rw-rw-rw-   0        0        0       98 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-25 16:31:23.256883 crypto-screening-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.0.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.0.3/build.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:31:23.243884 crypto-screening-1.0.3/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.0.3/crypto_screening/base.py
+-rw-rw-rw-   0        0        0    23575 2023-06-25 15:15:52.000000 crypto-screening-1.0.3/crypto_screening/collect.py
+-rw-rw-rw-   0        0        0    12461 2023-06-25 15:33:45.000000 crypto-screening-1.0.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.0.3/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.0.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.0.3/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.0.3/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32685 2023-06-25 15:28:31.000000 crypto-screening-1.0.3/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.0.3/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2392 2023-06-25 15:15:52.000000 crypto-screening-1.0.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    34516 2023-06-25 15:38:04.000000 crypto-screening-1.0.3/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.0.3/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:31:23.255885 crypto-screening-1.0.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-25 16:31:23.000000 crypto-screening-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       73 2023-06-23 16:55:08.000000 crypto-screening-1.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 16:31:23.256883 crypto-screening-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-25 16:31:13.000000 crypto-screening-1.0.3/setup.py
```

### Comparing `crypto-screening-1.0.2/PKG-INFO` & `crypto-screening-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.0.2
+Version: 1.0.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.0.2/README.md` & `crypto-screening-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/build.py` & `crypto-screening-1.0.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/base.py` & `crypto-screening-1.0.3/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/collect.py` & `crypto-screening-1.0.3/crypto_screening/collect.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/dataset.py` & `crypto-screening-1.0.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/document.py` & `crypto-screening-1.0.3/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/interval.py` & `crypto-screening-1.0.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/ohlcv.py` & `crypto-screening-1.0.3/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/orderbook.py` & `crypto-screening-1.0.3/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/process.py` & `crypto-screening-1.0.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/screener.py` & `crypto-screening-1.0.3/crypto_screening/screener.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/crypto_screening/symbols.py` & `crypto-screening-1.0.3/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,17 +247,17 @@
 
     :param symbol: The symbol to convert into a pair object.
     :param separator: The separator of the assets.
 
     :return: The symbol.
     """
 
-    return parts_to_symbol(
-        *symbol_to_parts(symbol=symbol, separator=separator)
-    )
+    base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
+    return parts_to_symbol(base=quote, quote=base)
 # end reverse_symbol
 
 def reverse_pair(pair: Pair, separator: Optional[str] = None) -> Pair:
     """
     Converts a pair of assets into a symbol.
 
     :param pair: The pair of assets.
```

### Comparing `crypto-screening-1.0.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.0.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.0.2
+Version: 1.0.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.0.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.0.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.2/pyproject.toml` & `crypto-screening-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.0.2'
+version = '1.0.3'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.0.2/setup.py` & `crypto-screening-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.0.2',
+        version='1.0.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

