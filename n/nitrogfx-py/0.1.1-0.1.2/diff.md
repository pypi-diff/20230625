# Comparing `tmp/nitrogfx-py-0.1.1.tar.gz` & `tmp/nitrogfx-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrogfx-py-0.1.1.tar", last modified: Sat Jun 24 13:38:31 2023, max compression
+gzip compressed data, was "nitrogfx-py-0.1.2.tar", last modified: Sun Jun 25 17:09:35 2023, max compression
```

## Comparing `nitrogfx-py-0.1.1.tar` & `nitrogfx-py-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35150 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    41806 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 13:38:31.967492 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)    41806 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35150 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    41806 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.422729 nitrogfx-py-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.424729 nitrogfx-py-0.1.2/src/nitrogfx/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8702 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/ncer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6144 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/ncgr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/nclr.py
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/nscr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.425729 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    41806 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/top_level.txt
```

### Comparing `nitrogfx-py-0.1.1/LICENSE.txt` & `nitrogfx-py-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.1/PKG-INFO` & `nitrogfx-py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `nitrogfx-py-0.1.1/README.md` & `nitrogfx-py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.1/nitrogfx_py.egg-info/PKG-INFO` & `nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `nitrogfx-py-0.1.1/pyproject.toml` & `nitrogfx-py-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nitrogfx-py"
-version = "0.1.1"
+version = "0.1.2"
 keywords = ["NDS", "Nintendo DS", "NCGR", "NCLR", "NSCR"]
 authors = [
   { name="Fexean", email="3699814-Fexean@users.noreply.gitlab.com" },
 ]
 description = "Nintendo DS Graphic format library"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -14,16 +14,12 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	"Pillow==7.0.0"
 ]
 
-[build-system]
-requires = ["setuptools>=64.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
 
-[tool.setuptools]
-py-modules = ["nitrogfx"]
 
 [project.urls]
 "Homepage" = "https://gitlab/Fexean/ntrgfx-py"
+
```

