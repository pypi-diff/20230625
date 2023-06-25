# Comparing `tmp/py_multiauth-2.0.0rc2.tar.gz` & `tmp/py_multiauth-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_multiauth-2.0.0rc2.tar", max compression
+gzip compressed data, was "py_multiauth-2.0.0rc3.tar", max compression
```

## Comparing `py_multiauth-2.0.0rc2.tar` & `py_multiauth-2.0.0rc3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1117 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2572 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/README.md
--rw-r--r--   0        0        0      152 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/__init__.py
--rw-r--r--   0        0        0       94 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/__main__.py
--rw-r--r--   0        0        0     2088 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/cli.py
--rw-r--r--   0        0        0       40 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/__init__.py
--rw-r--r--   0        0        0      598 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/errors.py
--rw-r--r--   0        0        0      474 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/http.py
--rw-r--r--   0        0        0     2250 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/interfaces.py
--rw-r--r--   0        0        0     3101 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/main.py
--rw-r--r--   0        0        0        0 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/__init__.py
--rw-r--r--   0        0        0     1719 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/aws.py
--rw-r--r--   0        0        0      830 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/graphql.py
--rw-r--r--   0        0        0     1575 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/oauth.py
--rw-r--r--   0        0        0      632 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/rest.py
--rw-r--r--   0        0        0      511 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/utils.py
--rw-r--r--   0        0        0     7876 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/generator.py
--rw-r--r--   0        0        0     3381 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/handlers.py
--rw-r--r--   0        0        0    13730 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/helpers.py
--rw-r--r--   0        0        0    10409 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/main.py
--rw-r--r--   0        0        0     6462 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/manager.py
--rw-r--r--   0        0        0      599 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/__init__.py
--rw-r--r--   0        0        0     3198 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/apikey.py
--rw-r--r--   0        0        0    15633 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/aws.py
--rw-r--r--   0        0        0     1590 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/basic.py
--rw-r--r--   0        0        0     9003 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/digest.py
--rw-r--r--   0        0        0    14577 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/graphql.py
--rw-r--r--   0        0        0     1067 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/manual.py
--rw-r--r--   0        0        0    15749 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/oauth.py
--rw-r--r--   0        0        0     9672 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/rest.py
--rw-r--r--   0        0        0        0 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/py.typed
--rw-r--r--   0        0        0        0 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/static/__init__.py
--rw-r--r--   0        0        0    44688 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/static/auth_schema.json
--rw-r--r--   0        0        0     5361 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/utils.py
--rw-r--r--   0        0        0     1514 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-06-25 21:43:42.190253 py_multiauth-2.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     2572 2023-06-25 21:43:42.190253 py_multiauth-2.0.0rc3/README.md
+-rw-r--r--   0        0        0      152 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/__main__.py
+-rw-r--r--   0        0        0     2088 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/cli.py
+-rw-r--r--   0        0        0       40 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/__init__.py
+-rw-r--r--   0        0        0      598 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/errors.py
+-rw-r--r--   0        0        0      474 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/http.py
+-rw-r--r--   0        0        0     2250 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/interfaces.py
+-rw-r--r--   0        0        0     3101 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/main.py
+-rw-r--r--   0        0        0        0 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/providers/__init__.py
+-rw-r--r--   0        0        0     1719 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/providers/aws.py
+-rw-r--r--   0        0        0      830 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/providers/graphql.py
+-rw-r--r--   0        0        0     1575 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/providers/oauth.py
+-rw-r--r--   0        0        0      632 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/providers/rest.py
+-rw-r--r--   0        0        0      511 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/entities/utils.py
+-rw-r--r--   0        0        0     7876 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/generator.py
+-rw-r--r--   0        0        0     3381 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/handlers.py
+-rw-r--r--   0        0        0    13759 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/helpers.py
+-rw-r--r--   0        0        0    10409 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/main.py
+-rw-r--r--   0        0        0     6462 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/manager.py
+-rw-r--r--   0        0        0      599 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/apikey.py
+-rw-r--r--   0        0        0    15633 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/aws.py
+-rw-r--r--   0        0        0     1590 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/basic.py
+-rw-r--r--   0        0        0     9003 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/digest.py
+-rw-r--r--   0        0        0    14577 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/graphql.py
+-rw-r--r--   0        0        0     1067 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/manual.py
+-rw-r--r--   0        0        0    15749 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/oauth.py
+-rw-r--r--   0        0        0     9672 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/providers/rest.py
+-rw-r--r--   0        0        0        0 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/py.typed
+-rw-r--r--   0        0        0        0 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/static/__init__.py
+-rw-r--r--   0        0        0    44688 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/static/auth_schema.json
+-rw-r--r--   0        0        0     5361 2023-06-25 21:43:42.194253 py_multiauth-2.0.0rc3/multiauth/utils.py
+-rw-r--r--   0        0        0     1514 2023-06-25 21:43:42.198253 py_multiauth-2.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc3/PKG-INFO
```

### Comparing `py_multiauth-2.0.0rc2/LICENSE` & `py_multiauth-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/README.md` & `py_multiauth-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/cli.py` & `py_multiauth-2.0.0rc3/multiauth/cli.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/errors.py` & `py_multiauth-2.0.0rc3/multiauth/entities/errors.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/interfaces.py` & `py_multiauth-2.0.0rc3/multiauth/entities/interfaces.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/main.py` & `py_multiauth-2.0.0rc3/multiauth/entities/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/providers/aws.py` & `py_multiauth-2.0.0rc3/multiauth/entities/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/providers/graphql.py` & `py_multiauth-2.0.0rc3/multiauth/entities/providers/graphql.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/providers/oauth.py` & `py_multiauth-2.0.0rc3/multiauth/entities/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/entities/providers/rest.py` & `py_multiauth-2.0.0rc3/multiauth/entities/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/generator.py` & `py_multiauth-2.0.0rc3/multiauth/generator.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/handlers.py` & `py_multiauth-2.0.0rc3/multiauth/handlers.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/helpers.py` & `py_multiauth-2.0.0rc3/multiauth/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,23 +110,23 @@
             input_data = input_data.encode('utf-8')
         return hashlib.sha512(input_data).hexdigest()
 
     return ''
 
 
 def token_endpoint_auth_method(auth_location: AuthOAuthlocation) -> str:
-    """This function takes the authorization location that is provided in the configuration and determines which token endpoint authentication method should be
-    used by the session."""
+    """This function takes the authorization location that is provided in the configuration
+    and determines which token endpoint authentication method should be used by the session."""
 
     if auth_location == AuthOAuthlocation.BODY:
         return 'client_secret_post'
     if auth_location == AuthOAuthlocation.BASIC:
         return 'client_secret_basic'
 
-    return ''
+    return ''  # type: ignore[unreachable]
 
 
 def get_secret_hash(
     username: str,
     client_id: str,
     client_secret: str,
 ) -> str:
```

### Comparing `py_multiauth-2.0.0rc2/multiauth/main.py` & `py_multiauth-2.0.0rc3/multiauth/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/manager.py` & `py_multiauth-2.0.0rc3/multiauth/manager.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/__init__.py` & `py_multiauth-2.0.0rc3/multiauth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/apikey.py` & `py_multiauth-2.0.0rc3/multiauth/providers/apikey.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/aws.py` & `py_multiauth-2.0.0rc3/multiauth/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/basic.py` & `py_multiauth-2.0.0rc3/multiauth/providers/basic.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/digest.py` & `py_multiauth-2.0.0rc3/multiauth/providers/digest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/graphql.py` & `py_multiauth-2.0.0rc3/multiauth/providers/graphql.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/manual.py` & `py_multiauth-2.0.0rc3/multiauth/providers/manual.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/oauth.py` & `py_multiauth-2.0.0rc3/multiauth/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/providers/rest.py` & `py_multiauth-2.0.0rc3/multiauth/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/static/auth_schema.json` & `py_multiauth-2.0.0rc3/multiauth/static/auth_schema.json`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/multiauth/utils.py` & `py_multiauth-2.0.0rc3/multiauth/utils.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc2/pyproject.toml` & `py_multiauth-2.0.0rc3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-multiauth"
-version = "2.0.0-rc.2"
+version = "2.0.0-rc.3"
 description = "Python package to interact with multiple authentication services"
 authors = ["Escape Technologies SAS <ping@escape.tech>"]
 maintainers = [
     "Antoine Carossio <antoine@escape.tech>",
     "Swan <swan@escape.tech>"
 ]
 license = "MIT"
@@ -33,15 +33,15 @@
 [tool.mypy]
 files = ["multiauth", "tests"]
 
 [tool.poetry.dependencies]
 Authlib = "^1.2.0"
 graphql-core = "^3.2.3"
 pycognito = "^2022.12.0"
-pydash = "^6.0.0"
+pydash = "^7.0.0"
 PyJWT = "^2.6.0"
 python = ">=3.8,<4.0"
 jsonschema = "^4.17.3"
 urllib3 = "<1.27"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^2.0.1"
```

### Comparing `py_multiauth-2.0.0rc2/PKG-INFO` & `py_multiauth-2.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-multiauth
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Python package to interact with multiple authentication services
 Home-page: https://escape.tech/
 License: MIT
 Author: Escape Technologies SAS
 Author-email: ping@escape.tech
 Maintainer: Antoine Carossio
 Maintainer-email: antoine@escape.tech
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Authlib (>=1.2.0,<2.0.0)
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: pycognito (>=2022.12.0,<2023.0.0)
-Requires-Dist: pydash (>=6.0.0,<7.0.0)
+Requires-Dist: pydash (>=7.0.0,<8.0.0)
 Requires-Dist: urllib3 (<1.27)
 Project-URL: Bug Tracker, https://github.com/Escape-Technologies/py-multiauth/issues
 Project-URL: Repository, https://github.com/Escape-Technologies/py-multiauth
 Description-Content-Type: text/markdown
 
 # py-multiauth ![PyPI](https://img.shields.io/pypi/v/py-multiauth) [![CI](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml) [![CD](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml) [![codecov](https://codecov.io/gh/Escape-Technologies/py-multiauth/branch/main/graph/badge.svg?token=NL148MNKAE)](https://codecov.io/gh/Escape-Technologies/py-multiauth)
```

