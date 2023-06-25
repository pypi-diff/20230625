# Comparing `tmp/openai_function_calling-0.5.0.tar.gz` & `tmp/openai_function_calling-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-0.5.0.tar", max compression
+gzip compressed data, was "openai_function_calling-0.6.0.tar", max compression
```

## Comparing `openai_function_calling-0.5.0.tar` & `openai_function_calling-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2161 2023-06-24 18:57:10.088869 openai_function_calling-0.5.0/README.md
--rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.5.0/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     1756 2023-06-24 18:47:36.891394 openai_function_calling-0.5.0/openai_function_calling/function.py
--rw-r--r--   0        0        0      848 2023-06-24 18:35:53.411122 openai_function_calling-0.5.0/openai_function_calling/parameter.py
--rw-r--r--   0        0        0      571 2023-06-24 18:57:40.974266 openai_function_calling-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 openai_function_calling-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2161 2023-06-24 18:57:10.088869 openai_function_calling-0.6.0/README.md
+-rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.6.0/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     1756 2023-06-25 17:13:35.402170 openai_function_calling-0.6.0/openai_function_calling/function.py
+-rw-r--r--   0        0        0     2115 2023-06-25 18:01:57.838552 openai_function_calling-0.6.0/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0      571 2023-06-25 18:02:06.446555 openai_function_calling-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 openai_function_calling-0.6.0/PKG-INFO
```

### Comparing `openai_function_calling-0.5.0/README.md` & `openai_function_calling-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.5.0/openai_function_calling/function.py` & `openai_function_calling-0.6.0/openai_function_calling/function.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.5.0/pyproject.toml` & `openai_function_calling-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "0.5.0"
+version = "0.6.0"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `openai_function_calling-0.5.0/PKG-INFO` & `openai_function_calling-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-calling
-Version: 0.5.0
+Version: 0.6.0
 Summary: Helper functions to generate OpenAI GPT function calling requests.
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

