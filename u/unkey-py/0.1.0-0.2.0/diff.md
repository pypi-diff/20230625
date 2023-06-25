# Comparing `tmp/unkey_py-0.1.0.tar.gz` & `tmp/unkey_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unkey_py-0.1.0.tar", max compression
+gzip compressed data, was "unkey_py-0.2.0.tar", max compression
```

## Comparing `unkey_py-0.1.0.tar` & `unkey_py-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-22 23:51:53.010504 unkey_py-0.1.0/LICENSE
--rw-r--r--   0        0        0      195 2023-06-22 23:51:53.010504 unkey_py-0.1.0/README.md
--rw-r--r--   0        0        0     2262 2023-06-22 23:51:53.010504 unkey_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      872 2023-06-22 23:51:53.090505 unkey_py-0.1.0/unkey/__init__.py
--rw-r--r--   0        0        0      643 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/__main__.py
--rw-r--r--   0        0        0       82 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/client.py
--rw-r--r--   0        0        0       46 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/models/__init__.py
--rw-r--r--   0        0        0      404 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/models/base.py
--rw-r--r--   0        0        0        0 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/py.typed
--rw-r--r--   0        0        0     1762 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/routes.py
--rw-r--r--   0        0        0       48 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/services/__init__.py
--rw-r--r--   0        0        0      113 2023-06-22 23:51:53.010504 unkey_py-0.1.0/unkey/services/base.py
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 unkey_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 00:52:34.797648 unkey_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1851 2023-06-25 00:52:34.797648 unkey_py-0.2.0/README.md
+-rw-r--r--   0        0        0     2262 2023-06-25 00:52:34.797648 unkey_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1399 2023-06-25 00:52:34.881647 unkey_py-0.2.0/unkey/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/__main__.py
+-rw-r--r--   0        0        0     2492 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/client.py
+-rw-r--r--   0        0        0      332 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/constants.py
+-rw-r--r--   0        0        0      434 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/errors.py
+-rw-r--r--   0        0        0      274 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/apis.py
+-rw-r--r--   0        0        0     1615 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/base.py
+-rw-r--r--   0        0        0      388 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/http.py
+-rw-r--r--   0        0        0     2393 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/keys.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/py.typed
+-rw-r--r--   0        0        0     2230 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/result.py
+-rw-r--r--   0        0        0     2089 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/routes.py
+-rw-r--r--   0        0        0     3445 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/serializer.py
+-rw-r--r--   0        0        0      151 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/__init__.py
+-rw-r--r--   0        0        0     1833 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/apis.py
+-rw-r--r--   0        0        0     1229 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/base.py
+-rw-r--r--   0        0        0     4331 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/http.py
+-rw-r--r--   0        0        0     3459 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/keys.py
+-rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 unkey_py-0.2.0/PKG-INFO
```

### Comparing `unkey_py-0.1.0/LICENSE` & `unkey_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unkey_py-0.1.0/pyproject.toml` & `unkey_py-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unkey.py"
-version = "0.1.0"
+version = "0.2.0"
 description = "An asynchronous Python SDK for unkey.dev."
 authors = ["Jonxslays"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/unkey.py"
 repository = "https://github.com/Jonxslays/unkey.py"
 packages = [
```

### Comparing `unkey_py-0.1.0/unkey/__main__.py` & `unkey_py-0.2.0/unkey/__main__.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.1.0/unkey/routes.py` & `unkey_py-0.2.0/unkey/routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import typing as t
 
 import attrs
 
+from unkey import constants as c
+
 __all__ = ("CompiledRoute", "Route")
 
 
 @attrs.define(weakref_slot=False)
 class CompiledRoute:
     """A route that has been compiled to include uri variables.
 
@@ -71,7 +73,17 @@
         """
         compiled = CompiledRoute(self, self.uri)
 
         for arg in args:
             compiled.uri = compiled.uri.replace(r"{}", str(arg), 1)
 
         return compiled
+
+
+# Keys
+CREATE_KEY: t.Final[Route] = Route(c.POST, "/keys")
+VERIFY_KEY: t.Final[Route] = Route(c.POST, "/keys/verify")
+REVOKE_KEY: t.Final[Route] = Route(c.DELETE, "/keys/{}")
+
+# Apis
+GET_API: t.Final[Route] = Route(c.GET, "/apis/{}")
+GET_KEYS: t.Final[Route] = Route(c.GET, "/apis/{}/keys")
```

