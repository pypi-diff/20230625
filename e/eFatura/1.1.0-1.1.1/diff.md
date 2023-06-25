# Comparing `tmp/eFatura-1.1.0.tar.gz` & `tmp/eFatura-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.1.0.tar", last modified: Sun Jun 25 09:42:38 2023, max compression
+gzip compressed data, was "eFatura-1.1.1.tar", last modified: Sun Jun 25 09:49:11 2023, max compression
```

## Comparing `eFatura-1.1.0.tar` & `eFatura-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 09:42:10.000000 eFatura-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:42:38.022216 eFatura-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-25 09:42:10.000000 eFatura-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.018216 eFatura-1.1.0/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.018216 eFatura-1.1.0/eFatura/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:42:38.022216 eFatura-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-25 09:42:10.000000 eFatura-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 09:48:38.000000 eFatura-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:49:11.491297 eFatura-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-25 09:48:38.000000 eFatura-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.487296 eFatura-1.1.1/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-25 09:48:38.000000 eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 09:48:38.000000 eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 09:48:38.000000 eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.487296 eFatura-1.1.1/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 09:48:38.000000 eFatura-1.1.1/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:49:11.491297 eFatura-1.1.1/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:49:11.000000 eFatura-1.1.1/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:49:11.491297 eFatura-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-25 09:48:38.000000 eFatura-1.1.1/setup.py
```

### Comparing `eFatura-1.1.0/PKG-INFO` & `eFatura-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.1.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.1.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.1.0/README.md` & `eFatura-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.1.0" date="2023-6-25">
+    <release version="1.1.1" date="2023-6-25">
       <description>
         <p>Çeşitli iyileştirmeler yapıldı..</p>
       </description>
     </release>
     <release version="1.0.5" date="2023-5-23"/>
     <release version="0.0.1" date="2022-8-13"/>
   </releases>
```

### Comparing `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.svg` & `eFatura-1.1.1/Shared/org.KekikAkademi.eFatura.svg`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura/Assets/logo.png` & `eFatura-1.1.1/eFatura/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura/Core/__init__.py` & `eFatura-1.1.1/eFatura/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura/GUI/__init__.py` & `eFatura-1.1.1/eFatura/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura/Libs/Oturum.py` & `eFatura-1.1.1/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura/konsol.py` & `eFatura-1.1.1/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/eFatura.egg-info/PKG-INFO` & `eFatura-1.1.1/eFatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.1.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.1.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.1.0/eFatura.egg-info/SOURCES.txt` & `eFatura-1.1.1/eFatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFatura-1.1.0/setup.py` & `eFatura-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.1.0",
+    version      = "1.1.1",
     url          = "https://github.com/keyiflerolsun/eFatura",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

