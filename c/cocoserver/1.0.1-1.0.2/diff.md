# Comparing `tmp/cocoserver-1.0.1.tar.gz` & `tmp/cocoserver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoserver-1.0.1.tar", last modified: Sat Jun 24 14:31:50 2023, max compression
+gzip compressed data, was "cocoserver-1.0.2.tar", last modified: Sun Jun 25 03:30:41 2023, max compression
```

## Comparing `cocoserver-1.0.1.tar` & `cocoserver-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.699493 cocoserver-1.0.1/
--rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.1/LICENSE
--rw-r--r--   0 culler     (501) staff       (20)     2138 2023-06-24 14:31:50.699116 cocoserver-1.0.1/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)     1971 2023-06-24 14:27:51.000000 cocoserver-1.0.1/README.rst
--rw-r--r--   0 culler     (501) staff       (20)     1132 2023-06-24 13:39:31.000000 cocoserver-1.0.1/pyproject.toml
--rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-24 14:31:50.699596 cocoserver-1.0.1/setup.cfg
--rw-r--r--   0 culler     (501) staff       (20)      434 2023-06-24 13:39:31.000000 cocoserver-1.0.1/setup.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.693984 cocoserver-1.0.1/src/
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.696362 cocoserver-1.0.1/src/cocoserver/
--rw-r--r--   0 culler     (501) staff       (20)     5963 2023-06-24 14:31:27.000000 cocoserver-1.0.1/src/cocoserver/__init__.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.698516 cocoserver-1.0.1/src/cocoserver.egg-info/
--rw-r--r--   0 culler     (501) staff       (20)     2138 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)      221 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/SOURCES.txt
--rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/dependency_links.txt
--rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/top_level.txt
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-25 03:30:41.297571 cocoserver-1.0.2/
+-rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.2/LICENSE
+-rw-r--r--   0 culler     (501) staff       (20)     2139 2023-06-25 03:30:41.297151 cocoserver-1.0.2/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)     1972 2023-06-25 03:29:09.000000 cocoserver-1.0.2/README.rst
+-rw-r--r--   0 culler     (501) staff       (20)     1132 2023-06-24 13:39:31.000000 cocoserver-1.0.2/pyproject.toml
+-rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-25 03:30:41.297711 cocoserver-1.0.2/setup.cfg
+-rw-r--r--   0 culler     (501) staff       (20)      434 2023-06-24 13:39:31.000000 cocoserver-1.0.2/setup.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-25 03:30:41.292222 cocoserver-1.0.2/src/
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-25 03:30:41.294550 cocoserver-1.0.2/src/cocoserver/
+-rw-r--r--   0 culler     (501) staff       (20)     5963 2023-06-25 03:30:25.000000 cocoserver-1.0.2/src/cocoserver/__init__.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-25 03:30:41.296459 cocoserver-1.0.2/src/cocoserver.egg-info/
+-rw-r--r--   0 culler     (501) staff       (20)     2139 2023-06-25 03:30:41.000000 cocoserver-1.0.2/src/cocoserver.egg-info/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)      221 2023-06-25 03:30:41.000000 cocoserver-1.0.2/src/cocoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-25 03:30:41.000000 cocoserver-1.0.2/src/cocoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-25 03:30:41.000000 cocoserver-1.0.2/src/cocoserver.egg-info/top_level.txt
```

### Comparing `cocoserver-1.0.1/LICENSE` & `cocoserver-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.1/PKG-INFO` & `cocoserver-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.1
+Version: 1.0.2
 Summary: A local HTTP server for compressed content.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 A Simple HTTP Server for Static Content
 =======================================
 
-This Python module provides a modified version of the ThreadedHTTPServer
+This Python module provides a modified version of the ThreadingHTTPServer
 class from the http.server module in the standard library.  This server
 is designed to serve a static web site, such as documentation for a
 python project generated by Sphinx and installed with the software.  It
 serves the files locally, on a random port of the loopback interface,
 and hence works off line.  The server runs in its own daemon thread
 of the python process, so it terminates when the python program exits
 and thus will not leave zombie processes running.
```

### Comparing `cocoserver-1.0.1/README.rst` & `cocoserver-1.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 A Simple HTTP Server for Static Content
 =======================================
 
-This Python module provides a modified version of the ThreadedHTTPServer
+This Python module provides a modified version of the ThreadingHTTPServer
 class from the http.server module in the standard library.  This server
 is designed to serve a static web site, such as documentation for a
 python project generated by Sphinx and installed with the software.  It
 serves the files locally, on a random port of the loopback interface,
 and hence works off line.  The server runs in its own daemon thread
 of the python process, so it terminates when the python program exits
 and thus will not leave zombie processes running.
```

### Comparing `cocoserver-1.0.1/pyproject.toml` & `cocoserver-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.1/src/cocoserver/__init__.py` & `cocoserver-1.0.2/src/cocoserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import email
 import shutil
 import datetime
 import webbrowser
 import urllib.parse
 import importlib.metadata
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 class GzipHTTPRequestHandler(SimpleHTTPRequestHandler):
 
     def log_message(self, format, *args):
         # We have no place for the log messages to go.
         pass
```

### Comparing `cocoserver-1.0.1/src/cocoserver.egg-info/PKG-INFO` & `cocoserver-1.0.2/src/cocoserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.1
+Version: 1.0.2
 Summary: A local HTTP server for compressed content.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 A Simple HTTP Server for Static Content
 =======================================
 
-This Python module provides a modified version of the ThreadedHTTPServer
+This Python module provides a modified version of the ThreadingHTTPServer
 class from the http.server module in the standard library.  This server
 is designed to serve a static web site, such as documentation for a
 python project generated by Sphinx and installed with the software.  It
 serves the files locally, on a random port of the loopback interface,
 and hence works off line.  The server runs in its own daemon thread
 of the python process, so it terminates when the python program exits
 and thus will not leave zombie processes running.
```

