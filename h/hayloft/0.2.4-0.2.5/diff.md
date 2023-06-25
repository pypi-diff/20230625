# Comparing `tmp/hayloft-0.2.4.tar.gz` & `tmp/hayloft-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.4.tar", max compression
+gzip compressed data, was "hayloft-0.2.5.tar", max compression
```

## Comparing `hayloft-0.2.4.tar` & `hayloft-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.4/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.4/hayloft/__init__.py
--rw-r--r--   0        0        0     3609 2023-06-25 09:56:43.893210 hayloft-0.2.4/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.4/hayloft/cors.py
--rw-r--r--   0        0        0      948 2023-06-25 09:53:28.322643 hayloft-0.2.4/hayloft/llama_index.py
--rw-r--r--   0        0        0      687 2023-06-25 09:52:46.747777 hayloft-0.2.4/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 12:45:37.079036 hayloft-0.2.4/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.4/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 12:45:37.079036 hayloft-0.2.4/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.4/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.4/hayloft/sse.py
--rw-r--r--   0        0        0    28672 2023-06-22 09:44:37.007616 hayloft-0.2.4/hayloft/store.db
--rw-r--r--   0        0        0      541 2023-06-25 09:58:15.419936 hayloft-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.5/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.5/hayloft/__init__.py
+-rw-r--r--   0        0        0     3599 2023-06-25 10:02:40.006427 hayloft-0.2.5/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.5/hayloft/cors.py
+-rw-r--r--   0        0        0      948 2023-06-25 09:53:28.322643 hayloft-0.2.5/hayloft/llama_index.py
+-rw-r--r--   0        0        0      687 2023-06-25 09:52:46.747777 hayloft-0.2.5/hayloft/logger.py
+-rw-r--r--   0        0        0   175448 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/public/assets/index-0cc0a4d1.js
+-rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.5/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0      384 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.5/hayloft/sse.py
+-rw-r--r--   0        0        0    28672 2023-06-22 09:44:37.007616 hayloft-0.2.5/hayloft/store.db
+-rw-r--r--   0        0        0      541 2023-06-25 10:03:12.147621 hayloft-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.5/PKG-INFO
```

### Comparing `hayloft-0.2.4/LICENSE` & `hayloft-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/README.md` & `hayloft-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/app.py` & `hayloft-0.2.5/hayloft/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from gevent import monkey; monkey.patch_all()
-from bottle import app, static_file, request, response, GeventServer
-from hayloft.schema import db, Session, Event
-from hayloft.cors import EnableCors
-from hayloft.sse import sse
+import argparse
+import time
 from importlib.metadata import version
 from pathlib import Path
 from typing import Dict
-import argparse
-import time
+
+from bottle import GeventServer, app, request, response, static_file
+
+from hayloft.cors import EnableCors
+from hayloft.schema import Event, Session, db
+from hayloft.sse import sse
 
 app = app()
 app.install(EnableCors()) 
 path = str(Path(__file__).parent.resolve()) 
 
 @app.get("/")
 def index():
@@ -96,16 +98,16 @@
     print("Hit Ctrl-C to quit.")
     app.run(host=host, port=port, server=GeventServer, quiet=True)
 
 def cli():
     parser = argparse.ArgumentParser(description="Hayloft - UI tool for LLM frameworks")
     parser.add_argument("command", type=str, help="command to run", choices=["start"])
     parser.add_argument("-v", "--version", action="version", version=version(__package__))
-    parser.add_argument("-h", "--host", help="host of the hayloft server", default="localhost")
-    parser.add_argument("-p", "--port", help="port of the hayloft server", type=int, default=7000)
+    parser.add_argument("--host", help="host of the hayloft server", default="localhost")
+    parser.add_argument("--port", help="port of the hayloft server", type=int, default=7000)
     args = parser.parse_args()
 
     if args.command == "start":
         start(host=args.host, port=args.port)
 
 if __name__ == '__main__':
     start()
```

### Comparing `hayloft-0.2.4/hayloft/cors.py` & `hayloft-0.2.5/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/llama_index.py` & `hayloft-0.2.5/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/logger.py` & `hayloft-0.2.5/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.5/hayloft/public/assets/index-0cc0a4d1.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.5/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/schema.py` & `hayloft-0.2.5/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/sse.py` & `hayloft-0.2.5/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/hayloft/store.db` & `hayloft-0.2.5/hayloft/store.db`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.4/pyproject.toml` & `hayloft-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.4"
+version = "0.2.5"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.4/PKG-INFO` & `hayloft-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.4
+Version: 0.2.5
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

