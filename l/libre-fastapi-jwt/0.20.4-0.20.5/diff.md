# Comparing `tmp/libre_fastapi_jwt-0.20.4.tar.gz` & `tmp/libre_fastapi_jwt-0.20.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.20.4.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.20.5.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.20.4.tar` & `libre_fastapi_jwt-0.20.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-25 05:35:44.832738 libre_fastapi_jwt-0.20.4/LICENSE
--rw-r--r--   0        0        0     2067 2023-06-25 05:35:44.832738 libre_fastapi_jwt-0.20.4/README.md
--rw-r--r--   0        0        0      148 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5425 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    44570 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     4703 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1097 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/pyproject.toml
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 06:09:07.709343 libre_fastapi_jwt-0.20.5/LICENSE
+-rw-r--r--   0        0        0     2067 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/README.md
+-rw-r--r--   0        0        0      148 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5425 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    44625 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     4703 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2023-06-25 06:09:07.713343 libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1054 2023-06-25 06:09:07.717343 libre_fastapi_jwt-0.20.5/pyproject.toml
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.5/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.20.4/LICENSE` & `libre_fastapi_jwt-0.20.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.4/README.md` & `libre_fastapi_jwt-0.20.5/README.md`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/auth_config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/auth_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,14 @@
             "jti": self._get_jwt_identifier(),
         }
         token_types = {
             "access": self._access_token_type,
             "refresh": self._refresh_token_type,
         }
 
-        # TODO: Check if we still need this (ToroNZ)
-        # custom_claims = {"type_token": type_token}
-
         if self._token_type_claim:
             custom_claims = {self._token_type_claim_name: token_types[type_token]}
         else:
             custom_claims = {}
 
         # for access_token only fresh needed
         if type_token == "access":
@@ -360,41 +357,43 @@
         self,
         subject: Union[str, int],
         fresh: Optional[bool] = False,
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
         expires_time: Optional[Union[timedelta, int, bool]] = None,
         audience: Optional[Union[str, Sequence[str]]] = None,
-        user_claims: Optional[Dict] = {"aid": str(uuid4())},
+        user_claims: Optional[Dict] = {},
     ) -> str:
         """
         Create a refresh token with X days for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
+        # Create a unique identifier to allow consumers to associate both tokens created as pair
+        pair_identifier = {"aid": str(uuid4())}
 
         refresh = self._create_token(
             subject=subject,
             type_token="refresh",
             exp_time=self._get_expired_time("refresh", expires_time),
             algorithm=algorithm,
             headers=headers,
             audience=audience,
-            user_claims=user_claims,
+            user_claims=user_claims | pair_identifier,
         )
         access = self._create_token(
             subject=subject,
             type_token="access",
             exp_time=self._get_expired_time("access", expires_time),
             fresh=fresh,
             algorithm=algorithm,
             headers=headers,
             audience=audience,
-            user_claims=user_claims,
+            user_claims=user_claims | pair_identifier,
             issuer=self._encode_issuer,
         )
         return {"access_token": access, "refresh_token": refresh}
 
     def _get_csrf_token(self, encoded_token: str) -> str:
         """
         Returns the CSRF double submit token from an encoded JWT.
```

### Comparing `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.20.5/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.4/pyproject.toml` & `libre_fastapi_jwt-0.20.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.20.4"
+version = "0.20.5"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `libre_fastapi_jwt-0.20.4/PKG-INFO` & `libre_fastapi_jwt-0.20.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.20.4
+Version: 0.20.5
 Summary: Yet another fork of fast-jwt-auth
 Home-page: https://github.com/LibreNZ/libre-fastapi-jwt
 License: MIT
 Author: Libre NZ
 Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.4 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.5 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

