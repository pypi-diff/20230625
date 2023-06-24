# Comparing `tmp/usermgr-0.0.2.tar.gz` & `tmp/usermgr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usermgr-0.0.2.tar", max compression
+gzip compressed data, was "usermgr-0.1.0.tar", max compression
```

## Comparing `usermgr-0.0.2.tar` & `usermgr-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-01-21 23:53:55.483886 usermgr-0.0.2/LICENSE
--rw-r--r--   0        0        0      378 2023-01-22 03:06:09.113850 usermgr-0.0.2/README.md
--rw-r--r--   0        0        0      588 2023-01-26 07:03:35.859995 usermgr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      313 2023-01-22 01:04:56.253873 usermgr-0.0.2/usermgr/Factory.py
--rw-r--r--   0        0        0       22 2023-01-26 07:04:13.249995 usermgr-0.0.2/usermgr/__init__.py
--rw-r--r--   0        0        0      872 2023-01-26 06:51:06.379998 usermgr-0.0.2/usermgr/base.py
--rw-r--r--   0        0        0        0 2023-01-22 00:53:40.993875 usermgr-0.0.2/usermgr/providers/__init__.py
--rw-r--r--   0        0        0     3701 2023-01-26 07:00:08.129996 usermgr-0.0.2/usermgr/providers/cognito.py
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 usermgr-0.0.2/setup.py
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 usermgr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.0/LICENSE
+-rw-r--r--   0        0        0      396 2023-06-24 11:29:36.602405 usermgr-0.1.0/README.md
+-rw-r--r--   0        0        0      588 2023-06-24 23:23:06.135821 usermgr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.0/usermgr/Factory.py
+-rw-r--r--   0        0        0       22 2023-06-24 23:23:13.165818 usermgr-0.1.0/usermgr/__init__.py
+-rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.0/usermgr/base.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.0/usermgr/providers/__init__.py
+-rw-r--r--   0        0        0     3511 2023-06-24 23:22:03.885844 usermgr-0.1.0/usermgr/providers/cognito.py
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 usermgr-0.1.0/PKG-INFO
```

### Comparing `usermgr-0.0.2/LICENSE` & `usermgr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usermgr-0.0.2/pyproject.toml` & `usermgr-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usermgr"
-version = "0.0.2"
+version = "0.1.0"
 description = ""
 authors = ["tamuto <tamuto@infodb.jp>"]
 readme = "README.md"
 homepage = "https://github.com/tamuto/usermgr"
 repository = "https://github.com/tamuto/usermgr"
 
 packages = [
```

### Comparing `usermgr-0.0.2/usermgr/base.py` & `usermgr-0.1.0/usermgr/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 class UserManager(metaclass=ABCMeta):
 
     @abstractmethod
     def close(self):
         raise NotImplementedError()
 
     @abstractmethod
-    def add_user(self, username, password, **kwargs):
+    def add_user(self, username, password, attrs):
+        raise NotImplementedError()
+
+    @abstractmethod
+    def update_user(self, username, attrs):
+        raise NotImplementedError()
+
+    @abstractmethod
+    def set_password(self, username, password, permanent=False):
         raise NotImplementedError()
 
     @abstractmethod
     def delete_user(self, username):
         raise NotImplementedError()
 
     @abstractmethod
@@ -23,15 +31,11 @@
     @abstractmethod
     def add_user_to_group(self, username, groupname):
         raise NotImplementedError()
 
     @abstractmethod
     def add_group(self, groupname):
         raise NotImplementedError()
-    
-    @abstractmethod
-    def delete_group(self, groupname):
-        raise NotImplementedError()
 
     @abstractmethod
-    def list_users(self, groupname):
+    def delete_group(self, groupname):
         raise NotImplementedError()
```

### Comparing `usermgr-0.0.2/usermgr/providers/cognito.py` & `usermgr-0.1.0/usermgr/providers/cognito.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,76 +25,75 @@
 
     def _make_hash(self, username):
         return base64.b64encode(hmac.new(
             bytes(self.client_secret, 'utf-8'),
             bytes(username + self.client_id, 'utf-8'),
             digestmod=hashlib.sha256).digest()).decode()
 
-    def add_user(self, username, password, email, **kwargs):
-        # TODO ユーザ属性をどのように設定するか？
+    def add_user(self, username, password, attrs):
         response = self.idp.admin_create_user(
             UserPoolId=self.user_pool_id,
             Username=username,
             TemporaryPassword=password,
-            UserAttributes=[
-                {
-                    "Name": "email",
-                    "Value": email
-                },
-                {
-                    "Name": "email_verified",
-                    "Value": "true"
-                }
-            ],
+            UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
             MessageAction="SUPPRESS"
         )
-        print(response)
 
         response = self.idp.admin_initiate_auth(
             UserPoolId=self.user_pool_id,
             ClientId=self.client_id,
             AuthFlow='ADMIN_NO_SRP_AUTH',
             AuthParameters={
                 'USERNAME': username,
                 'PASSWORD': password,
                 'SECRET_HASH': self._make_hash(username)
             }
         )
 
-        print(response)
-
         session = response['Session']
 
         response = self.idp.admin_respond_to_auth_challenge(
             UserPoolId=self.user_pool_id,
             ClientId=self.client_id,
             ChallengeName='NEW_PASSWORD_REQUIRED',
             ChallengeResponses={
                 'USERNAME': username,
                 'NEW_PASSWORD': password,
                 'SECRET_HASH': self._make_hash(username)
             },
             Session=session
         )
-        print(response)
+
+    def update_user(self, username, attrs):
+        self.idp.admin_update_user_attributes(
+            UserPoolId=self.user_pool_id,
+            Username=username,
+            UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
+        )
+
+    def set_password(self, username, password, permanent=False):
+        self.idp.admin_set_user_password(
+            UserPoolId=self.user_pool_id,
+            Username=username,
+            Password=password,
+            Permanent=permanent
+        )
 
     def delete_user(self, username):
-        response = self.idp.admin_delete_user(
+        self.idp.admin_delete_user(
             UserPoolId=self.user_pool_id,
             Username=username
         )
-        print(response)
 
     def is_exist_user(self, username):
         try:
-            response = self.idp.admin_get_user(
+            self.idp.admin_get_user(
                 UserPoolId=self.user_pool_id,
                 Username=username
             )
-            print(response)
             return True
         except ClientError as e:
             if e.response['Error']['Code'] == 'UserNotFoundException':
                 return False
             raise
 
     def add_user_to_group(self, username, groupname):
@@ -112,16 +111,7 @@
         )
 
     def delete_group(self, groupname):
         self.idp.delete_group(
             UserPoolId=self.user_pool_id,
             GroupName=groupname
         )
-
-    def list_users(self, groupname, limit=60, nexttoken=''):
-        # TODO Paging対応する。
-        return self.idp.list_users_in_group(
-            UserPoolId=self.user_pool_id,
-            GroupName=groupname,
-            Limit=limit,
-            # NextToken=nexttoken
-        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `usermgr-0.0.2/PKG-INFO` & `usermgr-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usermgr
-Version: 0.0.2
+Version: 0.1.0
 Summary: 
 Home-page: https://github.com/tamuto/usermgr
 Author: tamuto
 Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,21 +20,22 @@
 ## Memo
 
 * unittest
 
   * prepare .env file
 
 ```
-AWS_ACCESS_KEY_ID=xxx
-AWS_SECRET_ACCESS_KEY=xxx
+AWS_ACCESS_KEY_ID=***
+AWS_SECRET_ACCESS_KEY=***
 or
-AWS_PROFILE=xxx
+AWS_PROFILE=***
 
-USER_POOL_ID=xxx
-CLIENT_ID=xxx
+USER_POOL_ID=***
+CLIENT_ID=***
+CLIENT_SECRET=***
 ```
 
   * run unittest
 
 ```
 poetry run dotenv run python -m unittest discover
 ```
```

