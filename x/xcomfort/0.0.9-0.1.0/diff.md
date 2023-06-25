# Comparing `tmp/xcomfort-0.0.9.tar.gz` & `tmp/xcomfort-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xcomfort-0.0.9.tar", last modified: Fri Jul 17 10:58:18 2020, max compression
+gzip compressed data, was "xcomfort-0.1.0.tar", last modified: Sun Jun 25 14:14:20 2023, max compression
```

## Comparing `xcomfort-0.0.9.tar` & `xcomfort-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-17 10:58:18.565326 xcomfort-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      709 2020-07-17 10:58:09.000000 xcomfort-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-17 10:58:18.565326 xcomfort-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      712 2020-07-17 10:58:09.000000 xcomfort-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/xcomfort/
--rw-r--r--   0 runner    (1001) docker     (116)       54 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3915 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/bridge.py
--rw-r--r--   0 runner    (1001) docker     (116)     7322 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/xcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      229 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:14:20.789410 xcomfort-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 14:14:11.000000 xcomfort-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 14:14:20.789410 xcomfort-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-25 14:14:11.000000 xcomfort-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 14:14:20.789410 xcomfort-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 14:14:11.000000 xcomfort-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:14:20.789410 xcomfort-0.1.0/xcomfort/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-25 14:14:11.000000 xcomfort-0.1.0/xcomfort/room.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:14:20.789410 xcomfort-0.1.0/xcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 14:14:20.000000 xcomfort-0.1.0/xcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 14:14:20.000000 xcomfort-0.1.0/xcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 14:14:20.000000 xcomfort-0.1.0/xcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 14:14:20.000000 xcomfort-0.1.0/xcomfort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 14:14:20.000000 xcomfort-0.1.0/xcomfort.egg-info/top_level.txt
```

### Comparing `xcomfort-0.0.9/setup.py` & `xcomfort-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xcomfort",
-    version="0.0.9",
+    version="0.1.0",
     author="Jan Kristian Bjerke",
     author_email="jan.bjerke@gmail.com",
     description="Integration with Eaton xComfort Bridge",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jankrib/xcomfort-python",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 2 - Pre-Alpha",
     ],
     python_requires='>=3.7',
+    install_requires=[
+        "aiohttp",
+        "rx",
+        "pycryptodome"
+    ],
 )
```

