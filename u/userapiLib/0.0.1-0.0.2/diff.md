# Comparing `tmp/userapiLib-0.0.1.tar.gz` & `tmp/userapiLib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userapiLib-0.0.1.tar", last modified: Sun Jun 25 14:34:32 2023, max compression
+gzip compressed data, was "userapiLib-0.0.2.tar", last modified: Sun Jun 25 14:42:41 2023, max compression
```

## Comparing `userapiLib-0.0.1.tar` & `userapiLib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:34:32.558224 userapiLib-0.0.1/
--rw-r--r--   0 amo       (1000) amo       (1001)     1063 2023-06-25 13:56:03.000000 userapiLib-0.0.1/LICENSE
--rw-r--r--   0 amo       (1000) amo       (1001)     2601 2023-06-25 14:34:32.554890 userapiLib-0.0.1/PKG-INFO
--rw-r--r--   0 amo       (1000) amo       (1001)     1768 2023-06-25 14:34:03.000000 userapiLib-0.0.1/README.md
--rw-r--r--   0 amo       (1000) amo       (1001)       38 2023-06-25 14:34:32.558224 userapiLib-0.0.1/setup.cfg
--rw-r--r--   0 amo       (1000) amo       (1001)     1391 2023-06-25 14:25:00.000000 userapiLib-0.0.1/setup.py
-drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:34:32.488222 userapiLib-0.0.1/userapiLib.egg-info/
--rw-r--r--   0 amo       (1000) amo       (1001)     2601 2023-06-25 14:34:32.000000 userapiLib-0.0.1/userapiLib.egg-info/PKG-INFO
--rw-r--r--   0 amo       (1000) amo       (1001)      286 2023-06-25 14:34:32.000000 userapiLib-0.0.1/userapiLib.egg-info/SOURCES.txt
--rw-r--r--   0 amo       (1000) amo       (1001)        1 2023-06-25 14:34:32.000000 userapiLib-0.0.1/userapiLib.egg-info/dependency_links.txt
--rw-r--r--   0 amo       (1000) amo       (1001)       31 2023-06-25 14:34:32.000000 userapiLib-0.0.1/userapiLib.egg-info/requires.txt
--rw-r--r--   0 amo       (1000) amo       (1001)       11 2023-06-25 14:34:32.000000 userapiLib-0.0.1/userapiLib.egg-info/top_level.txt
-drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:34:32.534890 userapiLib-0.0.1/userapilib/
--rw-rw-rw-   0 amo       (1000) amo       (1001)      712 2023-06-25 13:51:38.000000 userapiLib-0.0.1/userapilib/__init__.py
--rw-r--r--   0 amo       (1000) amo       (1001)      975 2023-06-25 00:11:27.000000 userapiLib-0.0.1/userapilib/exception.py
--rw-r--r--   0 amo       (1000) amo       (1001)     5957 2023-06-24 12:08:29.000000 userapiLib-0.0.1/userapilib/testapi.py
--rw-r--r--   0 amo       (1000) amo       (1001)    13764 2023-06-25 14:06:51.000000 userapiLib-0.0.1/userapilib/userapi.py
+drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:42:41.021782 userapiLib-0.0.2/
+-rw-r--r--   0 amo       (1000) amo       (1001)     1063 2023-06-25 13:56:03.000000 userapiLib-0.0.2/LICENSE
+-rw-r--r--   0 amo       (1000) amo       (1001)     2618 2023-06-25 14:42:41.018448 userapiLib-0.0.2/PKG-INFO
+-rw-r--r--   0 amo       (1000) amo       (1001)     1785 2023-06-25 14:41:43.000000 userapiLib-0.0.2/README.md
+-rw-r--r--   0 amo       (1000) amo       (1001)       38 2023-06-25 14:42:41.021782 userapiLib-0.0.2/setup.cfg
+-rw-r--r--   0 amo       (1000) amo       (1001)     1394 2023-06-25 14:41:10.000000 userapiLib-0.0.2/setup.py
+drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:42:40.951779 userapiLib-0.0.2/userapiLib.egg-info/
+-rw-r--r--   0 amo       (1000) amo       (1001)     2618 2023-06-25 14:42:40.000000 userapiLib-0.0.2/userapiLib.egg-info/PKG-INFO
+-rw-r--r--   0 amo       (1000) amo       (1001)      286 2023-06-25 14:42:40.000000 userapiLib-0.0.2/userapiLib.egg-info/SOURCES.txt
+-rw-r--r--   0 amo       (1000) amo       (1001)        1 2023-06-25 14:42:40.000000 userapiLib-0.0.2/userapiLib.egg-info/dependency_links.txt
+-rw-r--r--   0 amo       (1000) amo       (1001)       34 2023-06-25 14:42:40.000000 userapiLib-0.0.2/userapiLib.egg-info/requires.txt
+-rw-r--r--   0 amo       (1000) amo       (1001)       11 2023-06-25 14:42:40.000000 userapiLib-0.0.2/userapiLib.egg-info/top_level.txt
+drwxr-xr-x   0 amo       (1000) amo       (1001)        0 2023-06-25 14:42:41.001781 userapiLib-0.0.2/userapilib/
+-rw-rw-rw-   0 amo       (1000) amo       (1001)      712 2023-06-25 13:51:38.000000 userapiLib-0.0.2/userapilib/__init__.py
+-rw-r--r--   0 amo       (1000) amo       (1001)      975 2023-06-25 00:11:27.000000 userapiLib-0.0.2/userapilib/exception.py
+-rw-r--r--   0 amo       (1000) amo       (1001)     5957 2023-06-24 12:08:29.000000 userapiLib-0.0.2/userapilib/testapi.py
+-rw-r--r--   0 amo       (1000) amo       (1001)    13764 2023-06-25 14:06:51.000000 userapiLib-0.0.2/userapilib/userapi.py
```

### Comparing `userapiLib-0.0.1/LICENSE` & `userapiLib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `userapiLib-0.0.1/PKG-INFO` & `userapiLib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userapiLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: With This Package Can You GET Info Username And Checking 
 Home-page: https://github.com/muamelAmeer/userapi
 Author: Muamel Ameer
 Author-email: amowallet@gmail.com
 Project-URL: Source, https://github.com/muamelAmeer/userapi
 Project-URL: Dev Lib, https://github.com/muamelAmeer
 Project-URL: Documentation, https://github.com/muamelAmeer/userApi/tree/main#example
@@ -15,16 +15,16 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# UserApi [![Version](https://img.shields.io/pypi/v/UserApi?style=flat&logo=pypi)](https://pypi.org/project/UserAPi)
-### UserApi
+# UserApilib [![Version](https://img.shields.io/pypi/v/UserApilib?style=flat&logo=pypi)](https://pypi.org/project/UserAPilib) 
+### UserApilib
 ```
 This Semple Pkg For Telegram UserNames
 Advantages :
     Check-UserName . Get-Info-UserName 
 
 ```
 ### Features
@@ -61,15 +61,15 @@
 
 print(info().auction(user))  #To Get Information UserName If in 'Fragment.com' , Result >>> Json Data
 
 print(info().fragment(user)) #To Get Status UserName in 'Fragment.com' , Result >>> Onauction - Sold - For Sell - ect...
 
 print(info().fragment(user,proxy='123.123.123')) #To Get Status UserName in 'Fragment.com' With Proxis! , Result >>> Onauction - Sold - For Sell - ect...
 
-print(info().Nft()) #To Get Information UserName If is 'NFT' , Result >>> Json Data
+print(info().Nft(user)) #To Get Information UserName If is 'NFT' , Result >>> Json Data
 
 
 
 ```
 For examples, check the [examples](https://github.com/muamelameer/userapi/test.py).
 
 # Thanks to
```

### Comparing `userapiLib-0.0.1/README.md` & `userapiLib-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# UserApi [![Version](https://img.shields.io/pypi/v/UserApi?style=flat&logo=pypi)](https://pypi.org/project/UserAPi)
-### UserApi
+# UserApilib [![Version](https://img.shields.io/pypi/v/UserApilib?style=flat&logo=pypi)](https://pypi.org/project/UserAPilib) 
+### UserApilib
 ```
 This Semple Pkg For Telegram UserNames
 Advantages :
     Check-UserName . Get-Info-UserName 
 
 ```
 ### Features
@@ -40,15 +40,15 @@
 
 print(info().auction(user))  #To Get Information UserName If in 'Fragment.com' , Result >>> Json Data
 
 print(info().fragment(user)) #To Get Status UserName in 'Fragment.com' , Result >>> Onauction - Sold - For Sell - ect...
 
 print(info().fragment(user,proxy='123.123.123')) #To Get Status UserName in 'Fragment.com' With Proxis! , Result >>> Onauction - Sold - For Sell - ect...
 
-print(info().Nft()) #To Get Information UserName If is 'NFT' , Result >>> Json Data
+print(info().Nft(user)) #To Get Information UserName If is 'NFT' , Result >>> Json Data
 
 
 
 ```
 For examples, check the [examples](https://github.com/muamelameer/userapi/test.py).
 
 # Thanks to
```

### Comparing `userapiLib-0.0.1/setup.py` & `userapiLib-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'With This Package Can You GET Info Username And Checking '
 LONG_DESCRIPTION = 'This PKG for checker telegram usernames .'
 
 # Setting up
 setup(
     name="userapiLib",
     version=VERSION,
     author="Muamel Ameer",
     author_email="amowallet@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['requests','fake_useragent','re','bs4'],
+    install_requires=['requests','fake_useragent','regex','bs4'],
     keywords=['telegram','username','checker','fragment','api','telegram-username'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `userapiLib-0.0.1/userapiLib.egg-info/PKG-INFO` & `userapiLib-0.0.2/userapiLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userapiLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: With This Package Can You GET Info Username And Checking 
 Home-page: https://github.com/muamelAmeer/userapi
 Author: Muamel Ameer
 Author-email: amowallet@gmail.com
 Project-URL: Source, https://github.com/muamelAmeer/userapi
 Project-URL: Dev Lib, https://github.com/muamelAmeer
 Project-URL: Documentation, https://github.com/muamelAmeer/userApi/tree/main#example
@@ -15,16 +15,16 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# UserApi [![Version](https://img.shields.io/pypi/v/UserApi?style=flat&logo=pypi)](https://pypi.org/project/UserAPi)
-### UserApi
+# UserApilib [![Version](https://img.shields.io/pypi/v/UserApilib?style=flat&logo=pypi)](https://pypi.org/project/UserAPilib) 
+### UserApilib
 ```
 This Semple Pkg For Telegram UserNames
 Advantages :
     Check-UserName . Get-Info-UserName 
 
 ```
 ### Features
@@ -61,15 +61,15 @@
 
 print(info().auction(user))  #To Get Information UserName If in 'Fragment.com' , Result >>> Json Data
 
 print(info().fragment(user)) #To Get Status UserName in 'Fragment.com' , Result >>> Onauction - Sold - For Sell - ect...
 
 print(info().fragment(user,proxy='123.123.123')) #To Get Status UserName in 'Fragment.com' With Proxis! , Result >>> Onauction - Sold - For Sell - ect...
 
-print(info().Nft()) #To Get Information UserName If is 'NFT' , Result >>> Json Data
+print(info().Nft(user)) #To Get Information UserName If is 'NFT' , Result >>> Json Data
 
 
 
 ```
 For examples, check the [examples](https://github.com/muamelameer/userapi/test.py).
 
 # Thanks to
```

### Comparing `userapiLib-0.0.1/userapilib/__init__.py` & `userapiLib-0.0.2/userapilib/__init__.py`

 * *Files identical despite different names*

### Comparing `userapiLib-0.0.1/userapilib/exception.py` & `userapiLib-0.0.2/userapilib/exception.py`

 * *Files identical despite different names*

### Comparing `userapiLib-0.0.1/userapilib/testapi.py` & `userapiLib-0.0.2/userapilib/testapi.py`

 * *Files identical despite different names*

### Comparing `userapiLib-0.0.1/userapilib/userapi.py` & `userapiLib-0.0.2/userapilib/userapi.py`

 * *Files identical despite different names*

