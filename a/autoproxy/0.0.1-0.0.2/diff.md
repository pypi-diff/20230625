# Comparing `tmp/autoproxy-0.0.1.tar.gz` & `tmp/autoproxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoproxy-0.0.1.tar", last modified: Sun Jun 25 17:17:59 2023, max compression
+gzip compressed data, was "autoproxy-0.0.2.tar", last modified: Sun Jun 25 17:28:10 2023, max compression
```

## Comparing `autoproxy-0.0.1.tar` & `autoproxy-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:17:59.636664 autoproxy-0.0.1/
--rw-rw-rw-   0        0        0     1050 2023-06-25 17:16:06.000000 autoproxy-0.0.1/LICENSES.txt
--rw-rw-rw-   0        0        0      682 2023-06-25 17:17:59.636664 autoproxy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-06-25 17:11:30.000000 autoproxy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 17:17:59.626856 autoproxy-0.0.1/autoproxy/
--rw-rw-rw-   0        0        0     1798 2023-06-25 17:09:07.000000 autoproxy-0.0.1/autoproxy/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-06-25 16:57:16.000000 autoproxy-0.0.1/autoproxy/__utils.py
--rw-rw-rw-   0        0        0     4326 2023-06-25 15:41:16.000000 autoproxy-0.0.1/autoproxy/sources.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:17:59.634691 autoproxy-0.0.1/autoproxy.egg-info/
--rw-rw-rw-   0        0        0      682 2023-06-25 17:17:59.000000 autoproxy-0.0.1/autoproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-25 17:17:59.000000 autoproxy-0.0.1/autoproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:17:59.000000 autoproxy-0.0.1/autoproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 17:17:59.000000 autoproxy-0.0.1/autoproxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-25 17:17:59.000000 autoproxy-0.0.1/autoproxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 17:17:59.636664 autoproxy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-06-25 17:16:25.000000 autoproxy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:28:10.754009 autoproxy-0.0.2/
+-rw-rw-rw-   0        0        0     1050 2023-06-25 17:16:06.000000 autoproxy-0.0.2/LICENSES.txt
+-rw-rw-rw-   0        0        0      682 2023-06-25 17:28:10.754009 autoproxy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-06-25 17:11:30.000000 autoproxy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 17:28:10.746155 autoproxy-0.0.2/autoproxy/
+-rw-rw-rw-   0        0        0     1818 2023-06-25 17:25:20.000000 autoproxy-0.0.2/autoproxy/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-06-25 16:57:16.000000 autoproxy-0.0.2/autoproxy/__utils.py
+-rw-rw-rw-   0        0        0     4326 2023-06-25 15:41:16.000000 autoproxy-0.0.2/autoproxy/sources.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:28:10.753010 autoproxy-0.0.2/autoproxy.egg-info/
+-rw-rw-rw-   0        0        0      682 2023-06-25 17:28:10.000000 autoproxy-0.0.2/autoproxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-25 17:28:10.000000 autoproxy-0.0.2/autoproxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:28:10.000000 autoproxy-0.0.2/autoproxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 17:28:10.000000 autoproxy-0.0.2/autoproxy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 17:28:10.000000 autoproxy-0.0.2/autoproxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:28:10.754009 autoproxy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-06-25 17:28:01.000000 autoproxy-0.0.2/setup.py
```

### Comparing `autoproxy-0.0.1/LICENSES.txt` & `autoproxy-0.0.2/LICENSES.txt`

 * *Files identical despite different names*

### Comparing `autoproxy-0.0.1/PKG-INFO` & `autoproxy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoproxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package give you auto proxies for your projects 
 Home-page: UNKNOWN
 Author: 01270
 Author-email: <mail@noemail.com>
 License: UNKNOWN
 Keywords: proxy,auto proxy,proxy scrapper
 Platform: UNKNOWN
```

### Comparing `autoproxy-0.0.1/autoproxy/__init__.py` & `autoproxy-0.0.2/autoproxy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from asyncio import run as async_run
-from __utils import proxyScraper
-from sources import sources
+from autoproxy.__utils import proxyScraper
+from autoproxy.sources import sources
 from random import choice
 
 class autoProxy:
     isInited: bool = False
     scrap_proxies: dict = {
         'http': [],
         'socks4': [],
```

### Comparing `autoproxy-0.0.1/autoproxy/__utils.py` & `autoproxy-0.0.2/autoproxy/__utils.py`

 * *Files identical despite different names*

### Comparing `autoproxy-0.0.1/autoproxy/sources.py` & `autoproxy-0.0.2/autoproxy/sources.py`

 * *Files identical despite different names*

### Comparing `autoproxy-0.0.1/autoproxy.egg-info/PKG-INFO` & `autoproxy-0.0.2/autoproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoproxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package give you auto proxies for your projects 
 Home-page: UNKNOWN
 Author: 01270
 Author-email: <mail@noemail.com>
 License: UNKNOWN
 Keywords: proxy,auto proxy,proxy scrapper
 Platform: UNKNOWN
```

### Comparing `autoproxy-0.0.1/setup.py` & `autoproxy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'This package give you auto proxies for your projects '
 LONG_DESCRIPTION = 'This package give you auto proxies for your projects'
 
 setup(
     name="autoproxy",
     version=VERSION,
     author="01270",
```

