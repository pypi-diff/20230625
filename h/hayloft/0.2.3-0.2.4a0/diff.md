# Comparing `tmp/hayloft-0.2.3.tar.gz` & `tmp/hayloft-0.2.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.3.tar", max compression
+gzip compressed data, was "hayloft-0.2.4a0.tar", max compression
```

## Comparing `hayloft-0.2.3.tar` & `hayloft-0.2.4a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.3/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.3/hayloft/__init__.py
--rw-r--r--   0        0        0     3365 2023-06-22 15:54:28.929777 hayloft-0.2.3/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.3/hayloft/cors.py
--rw-r--r--   0        0        0      860 2023-06-22 12:45:37.075703 hayloft-0.2.3/hayloft/llama_index.py
--rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.3/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 12:45:37.079036 hayloft-0.2.3/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.3/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 12:45:37.079036 hayloft-0.2.3/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.3/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.3/hayloft/sse.py
--rw-r--r--   0        0        0      541 2023-06-22 15:55:08.073945 hayloft-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.4a0/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.4a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.4a0/hayloft/__init__.py
+-rw-r--r--   0        0        0     3599 2023-06-25 10:02:40.006427 hayloft-0.2.4a0/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.4a0/hayloft/cors.py
+-rw-r--r--   0        0        0      948 2023-06-25 09:53:28.322643 hayloft-0.2.4a0/hayloft/llama_index.py
+-rw-r--r--   0        0        0      687 2023-06-25 09:52:46.747777 hayloft-0.2.4a0/hayloft/logger.py
+-rw-r--r--   0        0        0    18224 2023-06-25 10:20:39.206080 hayloft-0.2.4a0/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0   175427 2023-06-25 10:20:39.206080 hayloft-0.2.4a0/hayloft/public/assets/index-76ea6d03.js
+-rw-r--r--   0        0        0      384 2023-06-25 10:20:43.475349 hayloft-0.2.4a0/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.4a0/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.4a0/hayloft/sse.py
+-rw-r--r--   0        0        0      543 2023-06-25 10:49:19.603407 hayloft-0.2.4a0/pyproject.toml
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 hayloft-0.2.4a0/PKG-INFO
```

### Comparing `hayloft-0.2.3/LICENSE` & `hayloft-0.2.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/README.md` & `hayloft-0.2.4a0/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/hayloft/app.py` & `hayloft-0.2.4a0/hayloft/app.py`

 * *Files 9% similar despite different names*

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
@@ -84,26 +86,28 @@
     yield 'retry: 500\n\n' 
     messages = sse.listen()
     
     while True:
         msg = messages.get()
         yield msg
 
-def start():
+def start(host="localhost", port=7000):
     db.connect()
     db.create_tables([Session, Event])
 
-    print(f'\033[96mHayloft {version(__package__)} starting up, open in your browser http://localhost:7000\033[0m')
+    print(f'\033[96mHayloft {version(__package__)} starting up, open in your browser http://{host}:{port}\033[0m')
     print("Hit Ctrl-C to quit.")
-    app.run(host='localhost', port=7000, server=GeventServer, quiet=True)
+    app.run(host=host, port=port, server=GeventServer, quiet=True)
 
 def cli():
     parser = argparse.ArgumentParser(description="Hayloft - UI tool for LLM frameworks")
     parser.add_argument("command", type=str, help="command to run", choices=["start"])
     parser.add_argument("-v", "--version", action="version", version=version(__package__))
+    parser.add_argument("--host", help="host of the hayloft server", default="localhost")
+    parser.add_argument("--port", help="port of the hayloft server", type=int, default=7000)
     args = parser.parse_args()
 
     if args.command == "start":
-        start()
+        start(host=args.host, port=args.port)
 
 if __name__ == '__main__':
     start()
```

### Comparing `hayloft-0.2.3/hayloft/cors.py` & `hayloft-0.2.4a0/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/hayloft/llama_index.py` & `hayloft-0.2.4a0/hayloft/llama_index.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from hayloft.logger import logger
 
 class HayloftLogger(logging.Handler):
-    def __init__(self):
+    def __init__(self, server="http://localhost:7000"):
         super().__init__()
-        self.log = logger()
+        self.log = logger(server=server)
     
     def emit(self, record):
         type = "info"
         if record.levelno == logging.ERROR or record.levelno == logging.CRITICAL:
             type = "error"
         elif record.levelno == logging.WARNING:
             type = "warning"
         elif record.name.startswith("llama_index.llm_predictor"):
             type = "completion"
         elif record.name.startswith("llama_index.indices.response"):
             type = "completion" if record.msg.find(" response: ") != -1 else "prompt"
 
         self.log(title=record.name, message=record.msg, type=type)
 
-def grab_logs():
+def grab_logs(server="http://localhost:7000"):
     logging.getLogger("llama_index").setLevel(logging.DEBUG)
-    logging.getLogger().addHandler(HayloftLogger())
+    logging.getLogger().addHandler(HayloftLogger(server=server))
```

### Comparing `hayloft-0.2.3/hayloft/logger.py` & `hayloft-0.2.4a0/hayloft/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from typing import Literal
 
 import requests
 from nanoid import generate
 
 main_logger = logging.getLogger(__name__)
 
-def logger():
+def logger(server="http://localhost:7000"):
     session = f"session-{generate(size=6)}"
 
     def log(
         title: str = "",
         message: str = "",
         type: Literal["info", "prompt", "completion", "warning", "error"] = "info",
     ) -> None:
         try:
             requests.post(
-                "http://localhost:7000/event",
+                f"{server}/event",
                 json={"session": session, "title": title, "message": message, "type": type},
             )
         except requests.exceptions.ConnectionError:
             main_logger.info("Hayloft didn't start")
 
     return log
```

### Comparing `hayloft-0.2.3/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.4a0/hayloft/public/assets/index-76ea6d03.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7137,15 +7137,15 @@
                 store: t,
                 mutateStore: n
             },
             children: e
         })
     },
     qi = () => q.useContext(zc),
-    Rc = "http://localhost:7000",
+    Rc = "",
     sa = async (e, t, n) => await fetch(`${Rc}${t}`, {
         method: e,
         headers: {
             "Content-Type": "application/json"
         },
         ...n && {
             body: JSON.stringify(n)
```

### Comparing `hayloft-0.2.3/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.4a0/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/hayloft/schema.py` & `hayloft-0.2.4a0/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/hayloft/sse.py` & `hayloft-0.2.4a0/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.3/pyproject.toml` & `hayloft-0.2.4a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.3"
+version = "0.2.4a0"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.3/PKG-INFO` & `hayloft-0.2.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.3
+Version: 0.2.4a0
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

