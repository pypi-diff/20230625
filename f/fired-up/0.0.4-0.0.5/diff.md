# Comparing `tmp/fired-up-0.0.4.tar.gz` & `tmp/fired-up-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fired-up-0.0.4.tar", last modified: Fri Jun 23 13:46:10 2023, max compression
+gzip compressed data, was "fired-up-0.0.5.tar", last modified: Sun Jun 25 07:09:45 2023, max compression
```

## Comparing `fired-up-0.0.4.tar` & `fired-up-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.024715 fired-up-0.0.4/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.023804 fired-up-0.0.4/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     5174 2023-06-23 13:44:41.000000 fired-up-0.0.4/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.4/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.4/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     7177 2023-06-23 13:46:10.024601 fired-up-0.0.4/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.023921 fired-up-0.0.4/fired_up/
--rw-r--r--   0 xtof       (501) staff       (20)     3043 2023-06-23 13:44:51.000000 fired-up-0.0.4/fired_up/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.024436 fired-up-0.0.4/fired_up.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     7177 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-23 13:46:10.000000 fired-up-0.0.4/fired_up.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-23 13:46:10.024751 fired-up-0.0.4/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.4/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474934 fired-up-0.0.5/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474027 fired-up-0.0.5/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     5171 2023-06-25 07:00:13.000000 fired-up-0.0.5/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.5/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.5/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     7174 2023-06-25 07:09:45.474818 fired-up-0.0.5/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474141 fired-up-0.0.5/fired_up/
+-rw-r--r--   0 xtof       (501) staff       (20)     3039 2023-06-25 06:57:57.000000 fired-up-0.0.5/fired_up/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474643 fired-up-0.0.5/fired_up.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     7174 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-25 07:09:45.474975 fired-up-0.0.5/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.5/setup.py
```

### Comparing `fired-up-0.0.4/.github/README.md` & `fired-up-0.0.5/.github/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 > conventions and supporting tools for using Fire in a more natural-ish style
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
 [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
 
 
-## A command line DSL using Fire
+## Your Fired Up Command Line
 
 `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
 
 ### Minimal Survival Command
 
 ```console
 % pip install fired-up
```

### Comparing `fired-up-0.0.4/LICENSE.txt` & `fired-up-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fired-up-0.0.4/PKG-INFO` & `fired-up-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.4
+Version: 0.0.5
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         
-        ## A command line DSL using Fire
+        ## Your Fired Up Command Line
         
         `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
         
         ### Minimal Survival Command
         
         ```console
         % pip install fired-up
```

### Comparing `fired-up-0.0.4/fired_up/__init__.py` & `fired-up-0.0.5/fired_up/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 
   conventions and supporting tools for using Fire in a more natural-ish
   language style
 
 """
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 import sys
 import functools
 
 import fire
 
 class Group():
@@ -99,15 +99,15 @@
         clazz, args = clazz
       else:
         args = {}
       # only handle classes, objects are used verbatim
       if isinstance(clazz, type):
         # make sure all public methods return self to allow for chaining
         for attr in clazz.__dict__:
-          if callable(getattr(clazz, attr)) and attr != "__init__":
+          if callable(getattr(clazz, attr)) and attr[0] != "_":
             setattr(clazz, attr, keep(getattr(clazz, attr)))
         self.__dict__[group] = clazz(_parent=self, **args)
       elif isinstance(clazz, Menu):
         # handle "sub"menu's, which are already created and need a ref to the
         # shared
         self.__dict__[group] = clazz
         clazz._parent = self
@@ -118,20 +118,20 @@
   """
   
   the FiredUp class is the root-menu and holds the shared globals and clipboard
   
   """
   
   def __init__(self, name=None, **kwargs):
-    super().__init__(**kwargs)
     self._actual_shared = {
       "clipboard" : Clipboards(),
       "globals"   : {},
       "exit"      : self
     }
+    super().__init__(**kwargs)
     try:
       fire.Fire(self, name=name, serialize=paste_result)
     except KeyboardInterrupt:
       pass
 
   @property
   def _shared(self):
```

### Comparing `fired-up-0.0.4/fired_up.egg-info/PKG-INFO` & `fired-up-0.0.5/fired_up.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.4
+Version: 0.0.5
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/fired-up.svg)](https://pypi.python.org/pypi/fired-up/)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         
-        ## A command line DSL using Fire
+        ## Your Fired Up Command Line
         
         `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
         
         ### Minimal Survival Command
         
         ```console
         % pip install fired-up
```

### Comparing `fired-up-0.0.4/setup.py` & `fired-up-0.0.5/setup.py`

 * *Files identical despite different names*

