# Comparing `tmp/specialStr-0.0.2.tar.gz` & `tmp/specialStr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialStr-0.0.2.tar", last modified: Sat Jun 17 15:01:33 2023, max compression
+gzip compressed data, was "specialStr-0.0.3.tar", last modified: Sun Jun 25 16:34:23 2023, max compression
```

## Comparing `specialStr-0.0.2.tar` & `specialStr-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.730479 specialStr-0.0.2/
--rw-rw-rw-   0        0        0      819 2023-06-17 15:01:33.730479 specialStr-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-06-11 10:43:10.000000 specialStr-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-17 15:01:33.730479 specialStr-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-06-17 15:01:27.000000 specialStr-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.720478 specialStr-0.0.2/specialStr/
--rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.0.2/specialStr/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-06-17 15:01:09.000000 specialStr-0.0.2/specialStr/checker.py
--rw-rw-rw-   0        0        0     6266 2023-06-11 11:58:05.000000 specialStr-0.0.2/specialStr/main.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.728480 specialStr-0.0.2/specialStr.egg-info/
--rw-rw-rw-   0        0        0      819 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.926436 specialStr-0.0.3/
+-rw-rw-rw-   0        0        0     1170 2023-06-25 16:34:23.926436 specialStr-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-06-25 16:32:05.000000 specialStr-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-25 16:34:23.926436 specialStr-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-06-25 16:33:52.000000 specialStr-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.919437 specialStr-0.0.3/specialStr/
+-rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.0.3/specialStr/__init__.py
+-rw-rw-rw-   0        0        0     2494 2023-06-25 16:10:29.000000 specialStr-0.0.3/specialStr/checker.py
+-rw-rw-rw-   0        0        0     6770 2023-06-25 16:10:04.000000 specialStr-0.0.3/specialStr/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.925435 specialStr-0.0.3/specialStr.egg-info/
+-rw-rw-rw-   0        0        0     1170 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/top_level.txt
```

### Comparing `specialStr-0.0.2/PKG-INFO` & `specialStr-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
@@ -20,10 +20,34 @@
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 Richer strings
 ==============
 
 Provide more strings for specific purposes
 
--  url
+-  `url <https://developer.mozilla.org/docs/Web/API/URL>`__
+
+   -  shame
+   -  domain
+   -  port
+   -  path
+   -  paramstr
+   -  anchor
+
 -  email
+
+   -  user
+   -  domain
+
 -  path
+
+   -  driver
+   -  path
+   -  (something more about path)
+
+-  `version <https://semver.org/>`__
+
+   -  major
+   -  minor
+   -  patch
+   -  preRelease
+   -  buildMetadata
```

### Comparing `specialStr-0.0.2/setup.py` & `specialStr-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'specialStr',
-    version = '0.0.2',
+    version = '0.0.3',
     keywords = ['string'],
     description = 'Manage strings more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

### Comparing `specialStr-0.0.2/specialStr/__init__.py` & `specialStr-0.0.3/specialStr/__init__.py`

 * *Files identical despite different names*

### Comparing `specialStr-0.0.2/specialStr/checker.py` & `specialStr-0.0.3/specialStr/checker.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
 import re
 from typing import List,Dict,Tuple
-__all__=["UrlChecker","PathChecker","EmailChecker","Checker"]
+__all__=["UrlChecker","PathChecker","EmailChecker","Checker","VersionChecker"]
 class Checker(object):
     tester=[] #type: List[re.Pattern]
     finder={} #type: Dict[Tuple[str,...],re.Pattern]
     
 class UrlChecker(Checker):
     tester=[re.compile(r"^[^/\\\.&\?\#]*://(?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+(?::[0-9]+)?(?:(?:/[^/\\&\?\#]+)*/?)(?:\?(?:(?:[^/\\\.&\?\#]+=[^/\\\.&\?\#]*)&?)+)?(?:#[^&\?\#]*)?$")]
     finder={
@@ -36,7 +36,14 @@
 class EmailChecker(Checker):
     tester=[re.compile(r"^[\w.%+-]+@(?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+$")]
     finder={
         (
             "user","domain"
         ):re.compile(r"^([\w.%+-]+)@((?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+)$")
     }
+class VersionChecker(Checker):
+    tester=[re.compile(r"^(?:0|[1-9]\d*)\.(?:0|[1-9]\d*)\.(?:0|[1-9]\d*)(?:-(?:(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?:[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$")]
+    finder={
+        (
+            "major","minor","patch","preRelease","buildMetadata"
+        ):re.compile(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$")
+    }
```

### Comparing `specialStr-0.0.2/specialStr/main.py` & `specialStr-0.0.3/specialStr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 See the Mulan PSL v2 for more details.
 """
 import os
 from .checker import *
 from typing import Any, Dict,List,Union,Tuple,Union
 from typing_extensions import Literal
 import copy
-__all__=["Url","Path","Email"]
+__all__=["Url","Path","Email","Version"]
 class SpecialStr(str):
     checker=Checker() #type: Checker
     def __new__(cls, value):
         var=str(value)
         if not all([i.match(var)!=None for i in cls.checker.tester]):
             raise ValueError("\"%s\" does not appear to be a legal %s"%(var,cls.__name__.lower()))
         return super().__new__(cls, var)
@@ -125,8 +125,24 @@
     ## Represents a email address. It can be used as same as a str, but it has more function about path.
     Attributes:
         - user (str): The user of the address.
         - domain (str): The doomain of address.
     """
     checker=EmailChecker()
     user="" #type: str
-    domain="" #type: str
+    domain="" #type: str
+class Version(SpecialStr):
+    """
+    ## Represents a semantic version(see https://semver.org/)
+    Attributes:
+        - major: The major version
+        - minor: The minor version
+        - patch: The patch version
+        - preRelease: The pre-release version
+        - buildMetadata: The build metadata
+    """
+    checker=VersionChecker()
+    major="" #type: str
+    minor="" #type: str
+    patch="" #type: str
+    preRelease="" #type: str
+    buildMetadata="" #type: str
```

### Comparing `specialStr-0.0.2/specialStr.egg-info/PKG-INFO` & `specialStr-0.0.3/specialStr.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
@@ -20,10 +20,34 @@
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 Richer strings
 ==============
 
 Provide more strings for specific purposes
 
--  url
+-  `url <https://developer.mozilla.org/docs/Web/API/URL>`__
+
+   -  shame
+   -  domain
+   -  port
+   -  path
+   -  paramstr
+   -  anchor
+
 -  email
+
+   -  user
+   -  domain
+
 -  path
+
+   -  driver
+   -  path
+   -  (something more about path)
+
+-  `version <https://semver.org/>`__
+
+   -  major
+   -  minor
+   -  patch
+   -  preRelease
+   -  buildMetadata
```

