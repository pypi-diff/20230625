# Comparing `tmp/cm2py-0.2.0.tar.gz` & `tmp/cm2py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.2.0.tar", last modified: Wed May 31 02:13:37 2023, max compression
+gzip compressed data, was "cm2py-0.2.1.tar", last modified: Sun Jun 25 04:25:36 2023, max compression
```

## Comparing `cm2py-0.2.0.tar` & `cm2py-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.737789 cm2py-0.2.0/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-05-31 02:13:37.736789 cm2py-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-05-31 02:10:18.000000 cm2py-0.2.0/README.md
--rw-rw-rw-   0        0        0      687 2023-05-31 02:13:17.000000 cm2py-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 02:13:37.737789 cm2py-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.687788 cm2py-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.705789 cm2py-0.2.0/src/cm2py/
--rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.0/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6215 2023-05-31 02:13:21.000000 cm2py-0.2.0/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.729792 cm2py-0.2.0/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 02:13:37.000000 cm2py-0.2.0/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 02:13:37.732794 cm2py-0.2.0/tests/
--rw-rw-rw-   0        0        0     1671 2023-05-31 02:08:47.000000 cm2py-0.2.0/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.436139 cm2py-0.2.1/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-06-25 04:25:36.435139 cm2py-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-06-25 04:24:23.000000 cm2py-0.2.1/README.md
+-rw-rw-rw-   0        0        0      687 2023-06-25 04:24:27.000000 cm2py-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 04:25:36.437134 cm2py-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.356133 cm2py-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.380132 cm2py-0.2.1/src/cm2py/
+-rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.1/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6198 2023-06-25 04:24:27.000000 cm2py-0.2.1/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.426141 cm2py-0.2.1/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.431132 cm2py-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1671 2023-06-25 04:18:52.000000 cm2py-0.2.1/tests/test_app.py
```

### Comparing `cm2py-0.2.0/LICENSE` & `cm2py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.0/PKG-INFO` & `cm2py-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy 
@@ -50,15 +50,15 @@
 Basic program to generate a line of 8 looping OR gates:
 
 ```python
 import cm2py as cm2
 
 length = 8
 
-save = cm2.save()
+save = cm2.Save()
 
 blocks = []
 
 for i in range(length):
     blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
 
 ### Commented out for clarity.
```

### Comparing `cm2py-0.2.0/README.md` & `cm2py-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Basic program to generate a line of 8 looping OR gates:
 
 ```python
 import cm2py as cm2
 
 length = 8
 
-save = cm2.save()
+save = cm2.Save()
 
 blocks = []
 
 for i in range(length):
     blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
 
 ### Commented out for clarity.
```

### Comparing `cm2py-0.2.0/pyproject.toml` & `cm2py-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.2.0/src/cm2py/cm2py.py` & `cm2py-0.2.1/src/cm2py/cm2py.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 import re
 from uuid import UUID, uuid4
 import numpy as np
 
 
 class Save:
@@ -96,15 +96,15 @@
             and (isinstance(pos[0], float) or isinstance(pos[0], int))
             and (isinstance(pos[1], float) or isinstance(pos[1], int))
             and (isinstance(pos[2], float) or isinstance(pos[2], int))
         ), "pos must be a 3d tuple of integers"
         assert isinstance(state, bool), "state must be a boolean"
         assert isinstance(properties, list) or properties == None, "properties must be a list of numbers, or None"
         self.blockId = blockId
-        self.pos = tuple(np.round(pos))
+        self.pos = pos
         self.x = self.pos[0]
         self.y = self.pos[1]
         self.z = self.pos[2]
         self.state = state
         self.properties = properties
         self.uuid = uuid4()
```

### Comparing `cm2py-0.2.0/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.1/src/cm2py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy 
@@ -50,15 +50,15 @@
 Basic program to generate a line of 8 looping OR gates:
 
 ```python
 import cm2py as cm2
 
 length = 8
 
-save = cm2.save()
+save = cm2.Save()
 
 blocks = []
 
 for i in range(length):
     blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
 
 ### Commented out for clarity.
```

### Comparing `cm2py-0.2.0/tests/test_app.py` & `cm2py-0.2.1/tests/test_app.py`

 * *Files identical despite different names*

