# Comparing `tmp/ringcentral-0.8.0.tar.gz` & `tmp/ringcentral-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringcentral-0.8.0.tar", last modified: Fri Jun  2 20:50:23 2023, max compression
+gzip compressed data, was "ringcentral-0.8.1.tar", last modified: Sun Jun 25 08:15:13 2023, max compression
```

## Comparing `ringcentral-0.8.0.tar` & `ringcentral-0.8.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.022863 ringcentral-0.8.0/
--rw-r--r--   0 tyler.liu   (502) staff       (20)     1088 2023-05-18 20:46:38.000000 ringcentral-0.8.0/LICENSE.md
--rw-r--r--   0 tyler.liu   (502) staff       (20)       42 2023-05-18 20:46:38.000000 ringcentral-0.8.0/MANIFEST.in
--rw-r--r--   0 tyler.liu   (502) staff       (20)      328 2023-06-02 20:50:23.022984 ringcentral-0.8.0/PKG-INFO
--rw-r--r--   0 tyler.liu   (502) staff       (20)     4593 2023-06-02 17:50:12.000000 ringcentral-0.8.0/README.md
--rw-r--r--   0 tyler.liu   (502) staff       (20)       78 2023-06-02 17:50:12.000000 ringcentral-0.8.0/requirements.txt
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.005001 ringcentral-0.8.0/ringcentral/
--rw-r--r--   0 tyler.liu   (502) staff       (20)       20 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/__init__.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.007639 ringcentral-0.8.0/ringcentral/core/
--rw-r--r--   0 tyler.liu   (502) staff       (20)      826 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/core/__init__.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.009861 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/
--rw-r--r--   0 tyler.liu   (502) staff       (20)       66 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/__init__.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      352 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/events.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     7076 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     5017 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription_test.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.015456 ringcentral-0.8.0/ringcentral/http/
--rw-r--r--   0 tyler.liu   (502) staff       (20)      153 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/__init__.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      654 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_exception.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      900 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_exception_test.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     3118 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/api_response.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     4649 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_response_test.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     2865 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/client.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     1405 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/client_test.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      794 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/json_object.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     1754 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/multipart_builder.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     1337 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/multipart_builder_test.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.018013 ringcentral-0.8.0/ringcentral/platform/
--rw-r--r--   0 tyler.liu   (502) staff       (20)       54 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/__init__.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     3450 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/auth.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      257 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/events.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     8362 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/platform/platform.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     5070 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/platform_test.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      861 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/sdk.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      342 2023-05-18 22:07:52.000000 ringcentral-0.8.0/ringcentral/sdk_test.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.020105 ringcentral-0.8.0/ringcentral/test/
--rw-r--r--   0 tyler.liu   (502) staff       (20)       52 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/test/__init__.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      164 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/test/spy.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     4378 2023-05-18 22:22:44.000000 ringcentral-0.8.0/ringcentral/test/testcase.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.022387 ringcentral-0.8.0/ringcentral/websocket/
--rw-r--r--   0 tyler.liu   (502) staff       (20)      143 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/__init__.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)      828 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/events.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     5406 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/web_socket_client.py
--rw-r--r--   0 tyler.liu   (502) staff       (20)     4557 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/web_socket_subscription.py
-drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.007255 ringcentral-0.8.0/ringcentral.egg-info/
--rw-r--r--   0 tyler.liu   (502) staff       (20)      328 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/PKG-INFO
--rw-r--r--   0 tyler.liu   (502) staff       (20)     1318 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/SOURCES.txt
--rw-r--r--   0 tyler.liu   (502) staff       (20)        1 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/dependency_links.txt
--rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/requires.txt
--rw-r--r--   0 tyler.liu   (502) staff       (20)       12 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/top_level.txt
--rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2023-06-02 20:50:23.023434 ringcentral-0.8.0/setup.cfg
--rw-r--r--   0 tyler.liu   (502) staff       (20)      557 2023-06-02 17:50:12.000000 ringcentral-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 08:14:32.000000 ringcentral-0.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-25 08:14:32.000000 ringcentral-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 08:15:13.058642 ringcentral-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-25 08:14:32.000000 ringcentral-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 08:14:32.000000 ringcentral-0.8.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/subscription_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/api_exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/api_response_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/multipart_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/http/multipart_builder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/platform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/platform/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/platform/platform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/sdk_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/test/spy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/test/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/websocket/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/websocket/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-25 08:14:32.000000 ringcentral-0.8.1/ringcentral/websocket/web_socket_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:15:13.054643 ringcentral-0.8.1/ringcentral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 08:15:13.000000 ringcentral-0.8.1/ringcentral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 08:15:13.000000 ringcentral-0.8.1/ringcentral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:15:13.000000 ringcentral-0.8.1/ringcentral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 08:15:13.000000 ringcentral-0.8.1/ringcentral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 08:15:13.000000 ringcentral-0.8.1/ringcentral.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 08:15:13.058642 ringcentral-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-25 08:14:32.000000 ringcentral-0.8.1/setup.py
```

### Comparing `ringcentral-0.8.0/LICENSE.md` & `ringcentral-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/README.md` & `ringcentral-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/core/__init__.py` & `ringcentral-0.8.1/ringcentral/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription.py` & `ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/subscription.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription_test.py` & `ringcentral-0.8.1/ringcentral/deprecated_pubnub_subscription/subscription_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/api_exception.py` & `ringcentral-0.8.1/ringcentral/http/api_exception.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/api_exception_test.py` & `ringcentral-0.8.1/ringcentral/http/api_exception_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/api_response.py` & `ringcentral-0.8.1/ringcentral/http/api_response.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/api_response_test.py` & `ringcentral-0.8.1/ringcentral/http/api_response_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/client.py` & `ringcentral-0.8.1/ringcentral/http/client.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/client_test.py` & `ringcentral-0.8.1/ringcentral/http/client_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/json_object.py` & `ringcentral-0.8.1/ringcentral/http/json_object.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/multipart_builder.py` & `ringcentral-0.8.1/ringcentral/http/multipart_builder.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/http/multipart_builder_test.py` & `ringcentral-0.8.1/ringcentral/http/multipart_builder_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/platform/auth.py` & `ringcentral-0.8.1/ringcentral/platform/auth.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/platform/platform.py` & `ringcentral-0.8.1/ringcentral/platform/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,14 +183,18 @@
         request = self._client.create_request('POST', url, query_params=query_params, headers=headers, body=body)
         return self.send_request(request, skip_auth_check=skip_auth_check)
 
     def put(self, url, body=None, query_params=None, headers=None, skip_auth_check=False):
         request = self._client.create_request('PUT', url, query_params=query_params, headers=headers, body=body)
         return self.send_request(request, skip_auth_check=skip_auth_check)
 
+    def patch(self, url, body=None, query_params=None, headers=None, skip_auth_check=False):
+        request = self._client.create_request('PATCH', url, query_params=query_params, headers=headers, body=body)
+        return self.send_request(request, skip_auth_check=skip_auth_check)
+
     def delete(self, url, query_params=None, headers=None, skip_auth_check=False):
         request = self._client.create_request('DELETE', url, query_params=query_params, headers=headers)
         return self.send_request(request, skip_auth_check=skip_auth_check)
 
     def _request_token(self, path='', body=None):
         headers = {
             'Authorization': 'Basic ' + self._api_key(),
```

### Comparing `ringcentral-0.8.0/ringcentral/platform/platform_test.py` & `ringcentral-0.8.1/ringcentral/platform/platform_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/sdk.py` & `ringcentral-0.8.1/ringcentral/sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._client = Client()
         self._platform = Platform(self._client, key, secret, server, name, version, redirect_uri, known_prefixes)
 
     def platform(self):
         return self._platform
 
     def create_subscription(self):
-        warnings.warn("PubNub subscription is deprecated, please use WebSocket subscription.")
+        warnings.warn("PubNub support is deprecated. Please migrate your application to WebSockets.")
         return Subscription(self._platform)
     
     def create_web_socket_client(self):
         return WebSocketClient(self._platform)
 
     def create_multipart_builder(self):
         return MultipartBuilder(self._platform)
```

### Comparing `ringcentral-0.8.0/ringcentral/test/testcase.py` & `ringcentral-0.8.1/ringcentral/test/testcase.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/websocket/events.py` & `ringcentral-0.8.1/ringcentral/websocket/events.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/websocket/web_socket_client.py` & `ringcentral-0.8.1/ringcentral/websocket/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral/websocket/web_socket_subscription.py` & `ringcentral-0.8.1/ringcentral/websocket/web_socket_subscription.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/ringcentral.egg-info/SOURCES.txt` & `ringcentral-0.8.1/ringcentral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.0/setup.py` & `ringcentral-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.8.0'
+VERSION = '0.8.1'
 
 setup(
     name='ringcentral',
     packages=find_packages(exclude=[]),
     version=VERSION,
     description='RingCentral Python SDK',
     author='Kirill Konshin',
```

