# Comparing `tmp/libre_fastapi_jwt-0.20.3.tar.gz` & `tmp/libre_fastapi_jwt-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.20.3.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.20.4.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.20.3.tar` & `libre_fastapi_jwt-0.20.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/LICENSE
--rw-r--r--   0        0        0     2091 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/README.md
--rw-r--r--   0        0        0      148 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5423 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    41338 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     4700 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1077 2023-06-18 04:26:14.677616 libre_fastapi_jwt-0.20.3/pyproject.toml
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 05:35:44.832738 libre_fastapi_jwt-0.20.4/LICENSE
+-rw-r--r--   0        0        0     2067 2023-06-25 05:35:44.832738 libre_fastapi_jwt-0.20.4/README.md
+-rw-r--r--   0        0        0      148 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5425 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    44570 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     4703 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1097 2023-06-25 05:35:44.836737 libre_fastapi_jwt-0.20.4/pyproject.toml
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.4/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.20.3/LICENSE` & `libre_fastapi_jwt-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.3/README.md` & `libre_fastapi_jwt-0.20.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   FastAPI JWT Auth
 </h1>
 
-[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
+[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
 [![PyPI version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-fastapi-jwt)
 [![Downloads](https://static.pepy.tech/personalized-badge/libre-fastapi-jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/libre-fastapi-jwt)
 
 ---
 <h3> BTW - The project is based on <a href="https://pypi.org/project/libre-fastapi-jwt/" target="_blank">Fastapi-jwt-auth</a> that is no longer maintained. </h3> 
 
 **Documentation**: <a href="https://LibreNZ.github.io/libre-fastapi-jwt" target="_blank">https://LibreNZ.github.io/libre-fastapi-jwt</a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 ****** FastAPI JWT Auth ******
 [![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/
-tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/
-actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://
-github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml) [![PyPI
-version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://
-badge.fury.io/py/libre-fastapi-jwt) [![Downloads](https://static.pepy.tech/
-personalized-badge/libre-fastapi-
+tests.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/
+workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/
+actions/workflows/codeql.yml/badge.svg)](https://github.com/LibreNZ/libre-
+fastapi-jwt/actions/workflows/codeql.yml) [![PyPI version](https://
+badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-
+fastapi-jwt) [![Downloads](https://static.pepy.tech/personalized-badge/libre-
+fastapi-
 jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/libre-fastapi-jwt) ---
 **** BTW - The project is based on Fastapi-jwt-auth that is no longer
 maintained. ****
 **Documentation**: https://LibreNZ.github.io/libre-fastapi-jwt **Source Code**:
 https://github.com/LibreNZ/libre-fastapi-jwt --- ## Features FastAPI extension
 that provides JWT Auth support (secure, easy to use and lightweight), if you
```

### Comparing `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,30 @@
     _decode_audience = None
     _denylist_enabled = False
     _denylist_token_checks = {"access", "refresh"}
     _header_name = "Authorization"
     _header_type = "Bearer"
     _token_in_denylist_callback = None
     _access_token_expires = timedelta(minutes=15)
-    _refresh_token_expires = timedelta(days=30)
+    _refresh_token_expires = timedelta(days=14)
 
     # option for create cookies
-    _access_cookie_key = "access_token_cookie"
-    _refresh_cookie_key = "refresh_token_cookie"
+    _access_cookie_key = "__Host-access_token"
+    _refresh_cookie_key = "__Host-refresh_token"
     _access_cookie_path = "/"
     _refresh_cookie_path = "/"
     _cookie_max_age = None
     _cookie_domain = None
     _cookie_secure = False
     _cookie_samesite = None
 
     # option for double submit csrf protection
     _cookie_csrf_protect = True
-    _access_csrf_cookie_key = "csrf_access_token"
-    _refresh_csrf_cookie_key = "csrf_refresh_token"
+    _access_csrf_cookie_key = "__Host-CSRF_access"
+    _refresh_csrf_cookie_key = "__Host-CSRF_refresh"
     _access_csrf_cookie_path = "/"
     _refresh_csrf_cookie_path = "/"
     _access_csrf_header_name = "X-CSRF-Token"
     _refresh_csrf_header_name = "X-CSRF-Token"
     _csrf_methods = {"POST", "PUT", "PATCH", "DELETE"}
 
     # options to adjust token's type claim
```

### Comparing `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/auth_jwt.py`

 * *Files 7% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
         expires_time: Optional[Union[timedelta, int, bool]] = None,
         audience: Optional[Union[str, Sequence[str]]] = None,
         user_claims: Optional[Dict] = {},
     ) -> str:
         """
-        Create a access token with 15 minutes for expired time (default),
+        Create a access token with X minutes for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
         return self._create_token(
             subject=subject,
             type_token="access",
@@ -337,15 +337,15 @@
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
         expires_time: Optional[Union[timedelta, int, bool]] = None,
         audience: Optional[Union[str, Sequence[str]]] = None,
         user_claims: Optional[Dict] = {},
     ) -> str:
         """
-        Create a refresh token with 30 days for expired time (default),
+        Create a refresh token with X days for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
         return self._create_token(
             subject=subject,
             type_token="refresh",
@@ -363,15 +363,15 @@
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
         expires_time: Optional[Union[timedelta, int, bool]] = None,
         audience: Optional[Union[str, Sequence[str]]] = None,
         user_claims: Optional[Dict] = {"aid": str(uuid4())},
     ) -> str:
         """
-        Create a refresh token with 30 days for expired time (default),
+        Create a refresh token with X days for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
 
         refresh = self._create_token(
             subject=subject,
@@ -502,17 +502,93 @@
                 path=self._refresh_csrf_cookie_path,
                 domain=self._cookie_domain,
                 secure=self._cookie_secure,
                 httponly=False,
                 samesite=self._cookie_samesite,
             )
 
+    def set_pair_cookies(
+        self,
+        encoded_pair_token: str,
+        response: Optional[Response] = None,
+        max_age: Optional[int] = None,
+    ) -> None:
+        """
+        Configures the response to set access AND refresh token in a cookie.
+        this will also set the CSRF double submit values in a separate cookie
+
+        :param encoded_pair_token: Both encoded tokens as returned from create_pair_token() to set in the cookies
+        :param response: The FastAPI response object to set the access cookies in
+        :param max_age: The max age of the cookie value should be the number of seconds (integer)
+        """
+        if not self.jwt_in_cookies:
+            raise RuntimeWarning(
+                "set_pair_cookies() called without 'authjwt_token_location' configured to use cookies"
+            )
+
+        if max_age and not isinstance(max_age, int):
+            raise TypeError("max_age must be a integer")
+        if response and not isinstance(response, Response):
+            raise TypeError("The response must be an object response FastAPI")
+
+        response = response or self._response
+
+        # Set the access JWT in the cookie
+        response.set_cookie(
+            self._access_cookie_key,
+            encoded_pair_token["access_token"],
+            max_age=max_age or self._cookie_max_age,
+            path=self._access_cookie_path,
+            domain=self._cookie_domain,
+            secure=self._cookie_secure,
+            httponly=True,
+            samesite=self._cookie_samesite,
+        )
+
+        # If enabled, set the csrf double submit access cookie
+        if self._cookie_csrf_protect:
+            response.set_cookie(
+                self._access_csrf_cookie_key,
+                self._get_csrf_token(encoded_pair_token["access_token"]),
+                max_age=max_age or self._cookie_max_age,
+                path=self._access_csrf_cookie_path,
+                domain=self._cookie_domain,
+                secure=self._cookie_secure,
+                httponly=False,
+                samesite=self._cookie_samesite,
+            )
+
+        # Set the refresh JWT in the cookie
+        response.set_cookie(
+            self._refresh_cookie_key,
+            encoded_pair_token["refresh_token"],
+            max_age=max_age or self._cookie_max_age,
+            path=self._refresh_cookie_path,
+            domain=self._cookie_domain,
+            secure=self._cookie_secure,
+            httponly=True,
+            samesite=self._cookie_samesite,
+        )
+
+        # If enabled, set the csrf double submit refresh cookie
+        if self._cookie_csrf_protect:
+            response.set_cookie(
+                self._refresh_csrf_cookie_key,
+                self._get_csrf_token(encoded_pair_token["refresh_token"]),
+                max_age=max_age or self._cookie_max_age,
+                path=self._refresh_csrf_cookie_path,
+                domain=self._cookie_domain,
+                secure=self._cookie_secure,
+                httponly=False,
+                samesite=self._cookie_samesite,
+            )
+
     def unset_jwt_cookies(self, response: Optional[Response] = None) -> None:
         """
-        Unset (delete) all jwt stored in a cookie
+        Unset (delete) all jwt tokens stored in a cookie
 
         :param response: The FastAPI response object to delete the JWT cookies in.
         """
         self.unset_access_cookies(response)
         self.unset_refresh_cookies(response)
 
     def unset_access_cookies(self, response: Optional[Response] = None) -> None:
@@ -587,17 +663,18 @@
 
     def _verify_and_get_jwt_optional_in_cookies(
         self,
         request: Union[Request, WebSocket],
         csrf_token: Optional[str] = None,
     ) -> "AuthJWT":
         """
-        Optionally check if cookies have a valid access token. if an access token present in
-        cookies, self._token will set. raises exception error when an access token is invalid
-        or doesn't match with CSRF token double submit
+        - Optionally check if cookies have a valid access token. If an access token is present in
+        cookies, self._token will be set. 
+        - Raise an exception error when an access token is invalid
+        or doesn't match the double submitted CSRF token.
 
         :param request: for identity get cookies from HTTP or WebSocket
         :param csrf_token: the CSRF double submit token
         """
         if not isinstance(request, (Request, WebSocket)):
             raise TypeError("request must be an instance of 'Request' or 'WebSocket'")
 
@@ -630,17 +707,18 @@
         self,
         type_token: str,
         request: Union[Request, WebSocket],
         csrf_token: Optional[str] = None,
         fresh: Optional[bool] = False,
     ) -> "AuthJWT":
         """
-        Check if cookies have a valid access or refresh token. if an token present in
-        cookies, self._token will set. raises exception error when an access or refresh token
-        is invalid or doesn't match with CSRF token double submit
+        - Check if cookies have a valid access or refresh token. If there is a token present in
+        cookies, self._token will be set.
+        - Raise an exception error when an access or refresh token
+        is invalid or doesn't match the double submitted CSRF token.
 
         :param type_token: indicate token is access or refresh token
         :param request: for identity get cookies from HTTP or WebSocket
         :param csrf_token: the CSRF double submit token
         :param fresh: check freshness token if True
         """
 
@@ -649,29 +727,29 @@
             raise ValueError("type_token must be between 'access' or 'refresh'")
         if not isinstance(request, (Request, WebSocket)):
             raise TypeError("request must be an instance of 'Request' or 'WebSocket'")
 
         # Initialize cookie_key with a default value
         cookie_key = None
 
-        # Get token type and CSRF token, set cookie_key
+        # Get token type and CSRF token, set cookie_key. If request does NOT comes from WebSocket, grab the CSRF value from the header.
         if type_token == "access":
             cookie_key = self._access_cookie_key
             if not isinstance(request, WebSocket):
                 csrf_token = request.headers.get(self._access_csrf_header_name)
         if type_token == "refresh":
             cookie_key = self._refresh_cookie_key
             if not isinstance(request, WebSocket):
                 csrf_token = request.headers.get(self._refresh_csrf_header_name)
 
         # Set cookie variable, validate it is not None (aka null/empty)
         cookie = request.cookies.get(cookie_key)
         if not cookie:
             raise MissingTokenError(
-                status_code=401, message="Missing cookie {}".format(cookie_key)
+                status_code=401, message="Missing or incorrect cookie. Expected: {}".format(cookie_key)
             )
 
         if self._cookie_csrf_protect and not csrf_token:
             if isinstance(request, WebSocket) or request.method in self._csrf_methods:
                 raise CSRFError(status_code=401, message="Missing CSRF Token")
 
         # set token from cookie and verify jwt
@@ -711,26 +789,26 @@
         self,
         token: str,
         type_token: str,
         token_from: str,
         fresh: Optional[bool] = False,
     ) -> None:
         """
-        Ensure that the requester has a valid token. this also check the freshness of the access token
+        Ensure that the requester has a valid token. This also check the freshness of the access token
 
         :param token: The encoded JWT
         :param type_token: indicate token is access or refresh token
         :param token_from: indicate token from headers cookies, websocket
         :param fresh: check freshness token if True
         """
         if type_token not in ["access", "refresh"]:
-            raise ValueError("type_token must be either 'access' or 'refresh'")
+            raise ValueError("type_token must be either: 'access' or 'refresh'")
         if token_from not in ["headers", "cookies", "websocket"]:
             raise ValueError(
-                "token_from must be between 'headers', 'cookies', 'websocket'"
+                "token_from must be either: 'headers', 'cookies' or 'websocket'"
             )
 
         if not token:
             if token_from == "headers":
                 raise MissingTokenError(
                     status_code=401,
                     message="Missing {} Header".format(self._header_name),
@@ -760,15 +838,15 @@
         if fresh and not raw_jwt["fresh"]:
             raise FreshTokenRequired(status_code=401, message="Fresh token required")
 
     def _verifying_token(
         self, encoded_token: str, issuer: Optional[str] = None
     ) -> None:
         """
-        Verified token and check if token is revoked
+        Verify for a valid token then verify is not revoked.
 
         :param encoded_token: token hash
         :param issuer: expected issuer in the JWT
         """
         raw_token = self._verified_token(encoded_token, issuer)
 
         if self._token_type_claim:
```

### Comparing `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     authjwt_decode_issuer: Optional[StrictStr] = None
     authjwt_decode_audience: Optional[Union[StrictStr,Sequence[StrictStr]]] = None
     authjwt_denylist_enabled: Optional[StrictBool] = False
     authjwt_denylist_token_checks: Optional[Sequence[StrictStr]] = {'access','refresh'}
     authjwt_header_name: Optional[StrictStr] = "Authorization"
     authjwt_header_type: Optional[StrictStr] = "Bearer"
     authjwt_access_token_expires: Optional[Union[StrictBool,StrictInt,timedelta]] = timedelta(minutes=15)
-    authjwt_refresh_token_expires: Optional[Union[StrictBool,StrictInt,timedelta]] = timedelta(days=30)
+    authjwt_refresh_token_expires: Optional[Union[StrictBool,StrictInt,timedelta]] = timedelta(days=14)
     # option for create cookies
-    authjwt_access_cookie_key: Optional[StrictStr] = "access_token_cookie"
-    authjwt_refresh_cookie_key: Optional[StrictStr] = "refresh_token_cookie"
+    authjwt_access_cookie_key: Optional[StrictStr] = "__Host-access_token"
+    authjwt_refresh_cookie_key: Optional[StrictStr] = "__Host-refresh_token"
     authjwt_access_cookie_path: Optional[StrictStr] = "/"
     authjwt_refresh_cookie_path: Optional[StrictStr] = "/"
-    authjwt_cookie_max_age: Optional[StrictInt] = None
+    authjwt_cookie_max_age: Optional[StrictInt] = 86400
     authjwt_cookie_domain: Optional[StrictStr] = None
-    authjwt_cookie_secure: Optional[StrictBool] = False
-    authjwt_cookie_samesite: Optional[StrictStr] = None
+    authjwt_cookie_secure: Optional[StrictBool] = True
+    authjwt_cookie_samesite: Optional[StrictStr] = "Lax"
     # option for double submit csrf protection
     authjwt_cookie_csrf_protect: Optional[StrictBool] = True
-    authjwt_access_csrf_cookie_key: Optional[StrictStr] = "csrf_access_token"
-    authjwt_refresh_csrf_cookie_key: Optional[StrictStr] = "csrf_refresh_token"
+    authjwt_access_csrf_cookie_key: Optional[StrictStr] = "__Host-CSRF_access"
+    authjwt_refresh_csrf_cookie_key: Optional[StrictStr] = "__Host-CSRF_refresh"
     authjwt_access_csrf_cookie_path: Optional[StrictStr] = "/"
     authjwt_refresh_csrf_cookie_path: Optional[StrictStr] = "/"
     authjwt_access_csrf_header_name: Optional[StrictStr] = "X-CSRF-Token"
     authjwt_refresh_csrf_header_name: Optional[StrictStr] = "X-CSRF-Token"
     authjwt_csrf_methods: Optional[Sequence[StrictStr]] = {'POST','PUT','PATCH','DELETE'}
     # options to adjust token's type claim
     authjwt_token_type_claim: Optional[StrictBool] = True
```

### Comparing `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.20.4/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.3/pyproject.toml` & `libre_fastapi_jwt-0.20.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.20.3"
+version = "0.20.4"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
@@ -27,11 +27,13 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 PyJWT = "^2.6.0"
 fastapi = ">=0.95.1"
 cryptography = ">=41.0.0"
 httpx = ">=0.14.0"
 
+
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 requests = "^2.27.1"
 pytest-cov = "^4.0.0"
+uvicorn = "^0.22.0"
```

### Comparing `libre_fastapi_jwt-0.20.3/PKG-INFO` & `libre_fastapi_jwt-0.20.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.20.3
+Version: 0.20.4
 Summary: Yet another fork of fast-jwt-auth
 Home-page: https://github.com/LibreNZ/libre-fastapi-jwt
 License: MIT
 Author: Libre NZ
 Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
@@ -25,16 +25,16 @@
 Project-URL: Repository, https://github.com/LibreNZ/libre-fastapi-jwt
 Description-Content-Type: text/markdown
 
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   FastAPI JWT Auth
 </h1>
 
-[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
+[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
 [![PyPI version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-fastapi-jwt)
 [![Downloads](https://static.pepy.tech/personalized-badge/libre-fastapi-jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/libre-fastapi-jwt)
 
 ---
 <h3> BTW - The project is based on <a href="https://pypi.org/project/libre-fastapi-jwt/" target="_blank">Fastapi-jwt-auth</a> that is no longer maintained. </h3> 
 
 **Documentation**: <a href="https://LibreNZ.github.io/libre-fastapi-jwt" target="_blank">https://LibreNZ.github.io/libre-fastapi-jwt</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.3 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.4 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -11,21 +11,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0) Requires-Dist: cryptography (>=41.0.0)
 Requires-Dist: fastapi (>=0.95.1) Requires-Dist: httpx (>=0.14.0) Project-URL:
 Repository, https://github.com/LibreNZ/libre-fastapi-jwt Description-Content-
 Type: text/markdown
 ****** FastAPI JWT Auth ******
 [![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/
-tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/
-actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://
-github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml) [![PyPI
-version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://
-badge.fury.io/py/libre-fastapi-jwt) [![Downloads](https://static.pepy.tech/
-personalized-badge/libre-fastapi-
+tests.yml/badge.svg)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/
+workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/
+actions/workflows/codeql.yml/badge.svg)](https://github.com/LibreNZ/libre-
+fastapi-jwt/actions/workflows/codeql.yml) [![PyPI version](https://
+badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-
+fastapi-jwt) [![Downloads](https://static.pepy.tech/personalized-badge/libre-
+fastapi-
 jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/libre-fastapi-jwt) ---
 **** BTW - The project is based on Fastapi-jwt-auth that is no longer
 maintained. ****
 **Documentation**: https://LibreNZ.github.io/libre-fastapi-jwt **Source Code**:
 https://github.com/LibreNZ/libre-fastapi-jwt --- ## Features FastAPI extension
 that provides JWT Auth support (secure, easy to use and lightweight), if you
```

