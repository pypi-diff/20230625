# Comparing `tmp/hayloft-0.2.5.tar.gz` & `tmp/hayloft-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.5.tar", max compression
+gzip compressed data, was "hayloft-0.2.6.tar", max compression
```

## Comparing `hayloft-0.2.5.tar` & `hayloft-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.5/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.5/hayloft/__init__.py
--rw-r--r--   0        0        0     3599 2023-06-25 10:02:40.006427 hayloft-0.2.5/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.5/hayloft/cors.py
--rw-r--r--   0        0        0      948 2023-06-25 09:53:28.322643 hayloft-0.2.5/hayloft/llama_index.py
--rw-r--r--   0        0        0      687 2023-06-25 09:52:46.747777 hayloft-0.2.5/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.5/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.5/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.5/hayloft/sse.py
--rw-r--r--   0        0        0    28672 2023-06-22 09:44:37.007616 hayloft-0.2.5/hayloft/store.db
--rw-r--r--   0        0        0      541 2023-06-25 10:03:12.147621 hayloft-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.6/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.6/hayloft/__init__.py
+-rw-r--r--   0        0        0     3599 2023-06-25 10:02:40.006427 hayloft-0.2.6/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 12:45:37.075703 hayloft-0.2.6/hayloft/cors.py
+-rw-r--r--   0        0        0      948 2023-06-25 09:53:28.322643 hayloft-0.2.6/hayloft/llama_index.py
+-rw-r--r--   0        0        0      687 2023-06-25 09:52:46.747777 hayloft-0.2.6/hayloft/logger.py
+-rw-r--r--   0        0        0    18224 2023-06-25 10:20:39.206080 hayloft-0.2.6/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0   175427 2023-06-25 10:20:39.206080 hayloft-0.2.6/hayloft/public/assets/index-76ea6d03.js
+-rw-r--r--   0        0        0      384 2023-06-25 10:20:43.475349 hayloft-0.2.6/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-22 12:45:37.079036 hayloft-0.2.6/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.2.6/hayloft/sse.py
+-rw-r--r--   0        0        0      541 2023-06-25 10:21:48.225012 hayloft-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.6/PKG-INFO
```

### Comparing `hayloft-0.2.5/LICENSE` & `hayloft-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/README.md` & `hayloft-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/app.py` & `hayloft-0.2.6/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/cors.py` & `hayloft-0.2.6/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/llama_index.py` & `hayloft-0.2.6/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/logger.py` & `hayloft-0.2.6/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.6/hayloft/public/assets/index-76ea6d03.js`

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

### Comparing `hayloft-0.2.5/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.6/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/schema.py` & `hayloft-0.2.6/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/hayloft/sse.py` & `hayloft-0.2.6/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.5/pyproject.toml` & `hayloft-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.5"
+version = "0.2.6"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.5/PKG-INFO` & `hayloft-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.5
+Version: 0.2.6
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

