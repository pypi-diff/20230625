# Comparing `tmp/jplaw-0.1.1.tar.gz` & `tmp/jplaw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.1.tar", last modified: Sat Jun 24 06:05:51 2023, max compression
+gzip compressed data, was "jplaw-0.1.2.tar", last modified: Sat Jun 24 22:36:58 2023, max compression
```

## Comparing `jplaw-0.1.1.tar` & `jplaw-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:05:51.252832 jplaw-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-24 06:05:41.000000 jplaw-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-24 06:05:51.252832 jplaw-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-24 06:05:41.000000 jplaw-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:05:51.252832 jplaw-0.1.1/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-24 06:05:41.000000 jplaw-0.1.1/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:05:51.252832 jplaw-0.1.1/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-24 06:05:51.000000 jplaw-0.1.1/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-24 06:05:51.000000 jplaw-0.1.1/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:05:51.000000 jplaw-0.1.1/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 06:05:51.000000 jplaw-0.1.1/jplaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 06:05:51.000000 jplaw-0.1.1/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-24 06:05:41.000000 jplaw-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:05:51.252832 jplaw-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-24 06:05:41.000000 jplaw-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-24 22:36:48.000000 jplaw-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 22:36:58.513698 jplaw-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-24 22:36:48.000000 jplaw-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-24 22:36:48.000000 jplaw-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:36:58.513698 jplaw-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-24 22:36:48.000000 jplaw-0.1.2/setup.py
```

### Comparing `jplaw-0.1.1/LICENSE` & `jplaw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.1/PKG-INFO` & `jplaw-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
@@ -16,7 +16,11 @@
 
 # Python Lemmy API Wrapper
 Like PRAW but for Lemmy
 
 Written using the [Lemmy TS library](https://github.com/LemmyNet/lemmy-js-client) for reference.
 
 Forked from benja810's plaw
+
+Currently, most of the API functions are implemented, but there are likely quite a few bugs. It is a bit difficult to test at the moment without spinning up a new instance. 
+
+If you find any bugs, let me know on the [issues page](https://github.com/amarpersaud/python-jplaw/issues)
```

### Comparing `jplaw-0.1.1/jplaw/lemmy.py` & `jplaw-0.1.2/jplaw/lemmy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .requestor import Requestor, HttpType
 from enum import *
 from .comment import Comment
 from .community import Community
 from .post import Post
 from .user import User
 from .site import Site
+from .private_message import PrivateMessage
 
 class Lemmy:
     Post: Post
     Community: Community
     Comment: Comment
     User: User
     Site: Site
+    PrivateMessage: PrivateMessage
     
     def __enter__(self):
         """Handle the context manager open."""
         return self
     
     def __exit__(self, *_args):
         """Handle the context manager close."""
@@ -27,14 +29,15 @@
         self._req = Requestor(instance=instance, username=username, password=password, headers={})
         
         self.Post = Post(self._req)
         self.Community = Community(self._req)
         self.Comment = Comment(self._req)
         self.User = User(self._req)
         self.Site = Site(self._req)
+        self.PrivateMessage = PrivateMessage(self._req)
         # print(self._req.headers.get("Authorization"))
         
     def resolveObject(self, obj, instance=None, auth_token=None):
         form={
             "q": obj
         }
         res = self._req.lemmyRequest(HttpType.GET, "resolveObject", instance=instance, form=form, auth_token=auth_token)
```

### Comparing `jplaw-0.1.1/jplaw/requestor.py` & `jplaw-0.1.2/jplaw/requestor.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.1/jplaw/site.py` & `jplaw-0.1.2/jplaw/private_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 from .requestor import Requestor
 from .api_paths import *
-from typing import List
 
-class Site():
+
+class PrivateMessage():
     def __init__(self, _req: Requestor):
         self._req = _req
     
-    def getSite(self, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getPrivateMessages(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
         form = {}
-        res = self._req.lemmyRequest("getSite", instance=instance, form=form, auth=auth, auth_token=auth_token)
-        return res
-    
-    def createSite(self, instance:str=None, auth_token:str=None, form={}):
-        res = self._req.lemmyRequest("createSite", instance=instance, form=form, auth=True, auth_token=auth_token)
-        return res
-    
-    def editSite(self, instance:str=None, auth_token:str=None, form={}):
-        res = self._req.lemmyRequest("editSite", instance=instance, form=form, auth=True, auth_token=auth_token)
-        return res
-        
-    def getFederatedInstances(self, instance:str=None, auth:bool=True, auth_token:str=None):
-        res = self._req.lemmyRequest("federated_instances", instance=instance, auth=auth, auth_token=auth_token)
+        optional={
+            "unread_only": unread_only,
+            "page": page,
+            "limit": limit,
+            }
+        res = self._req.lemmyRequest("getPrivateMessages", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
-        
-    def createCustomEmoji(self, category:str, shortcode:str, image_url:str, alt_text:str, keywords:List[str], instance:str=None, auth_token:str=None):
-        form={
-            "category": category,
-            "shortcode": shortcode,
-            "image_url": image_url,
-            "alt_text": alt_text,
-            "keywords": keywords
+    def createPrivateMessage(self, content:str, recipient_id:int, instance:str=None, auth_token:str=None):
+        form = {
+            "content": content,
+            "recipient_id": recipient_id,
             }
-        res = self._req.lemmyRequest("createCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def editCustomEmoji(self, emoji_id:int, category:str=None, image_url:str=None, alt_text:str=None, keywords:List[str]=None, instance:str=None, auth_token:str=None):
-        form={
-            "id": emoji_id,
-            "category": category,
-            "image_url": image_url,
-            "alt_text": alt_text,
-            "keywords": keywords
+    def createPrivateMessageReport(self, private_message_id:int, reason:str, instance:str=None, auth_token:str=None):
+        form = {
+            "private_message_id": private_message_id,
+            "reason": reason,
             }
-        res = self._req.lemmyRequest("editCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPrivateMessageReport", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def deleteCustomEmoji(self, emoji_id:int, instance:str=None, auth_token:str=None):
-        form={
-            "id": emoji_id
+    def editPrivateMessage(self, private_message_id:int, content:str, instance:str=None, auth_token:str=None):
+        form = {
+            "private_message_id": private_message_id,
+            "content": content,
             }
-        res = self._req.lemmyRequest("deleteCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("editPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
-
-    def addAdmin(self, person_id:int, added:bool, instance:str=None, auth_token:str=None):
-        form={
-            "person_id": person_id,
-            "added": added
+        
+    def deletePrivateMessage(self, private_message_id:int, instance:str=None, auth_token:str=None):
+        form = {
+            "private_message_id": private_message_id,
             }
-        res = self._req.lemmyRequest("addAdmin", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deletePrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def getUnreadRegistrationApplicationCount(self, instance:str=None, auth_token=None):
+    def markPrivateMessageAsRead(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
         form={}
-        res = self._req.lemmyRequest("getUnreadRegistrationApplicationCount", instance=instance, form=form, auth=True, auth_token=auth_token)
+        optional = {
+            "unread_only": unread_only,
+            "page": page,
+            "limit": limit,
+            }
+        res = self._req.lemmyRequest("markPrivateMessageAsRead", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
         
-    def listRegistrationApplications(self, unread_only:bool=None, page:int=None, limit:str=None, instance:str=None, auth_token=None):
-        form={}
-        optional={
+    def listPrivateMessageReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, instance:str=None, auth_token:str=None):
+        form = {}
+        optional = {
             "page": page,
             "limit": limit,
-            "unread_only": unread_only
+            "unresolved_only": unresolved_only,
+            }
+        res = self._req.lemmyRequest("listPrivateMessageReports", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        return res
+    def resolvePrivateMessageReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+        form = {
+            "report_id"  : report_id ,
+            "resolved"   : resolved  ,
             }
-        res = self._req.lemmyRequest("listRegistrationApplications", instance=instance, form=form, auth=True, auth_token=auth_token)
-        return res
+        res = self._req.lemmyRequest("resolvePrivateMessageReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        return
```

### Comparing `jplaw-0.1.1/jplaw/user.py` & `jplaw-0.1.2/jplaw/user.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.1/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.2/jplaw.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
@@ -16,7 +16,11 @@
 
 # Python Lemmy API Wrapper
 Like PRAW but for Lemmy
 
 Written using the [Lemmy TS library](https://github.com/LemmyNet/lemmy-js-client) for reference.
 
 Forked from benja810's plaw
+
+Currently, most of the API functions are implemented, but there are likely quite a few bugs. It is a bit difficult to test at the moment without spinning up a new instance. 
+
+If you find any bugs, let me know on the [issues page](https://github.com/amarpersaud/python-jplaw/issues)
```

### Comparing `jplaw-0.1.1/pyproject.toml` & `jplaw-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jplaw"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Amar Persaud", email="tehspartaa@gmail.com" },
 ]
 description = "A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jplaw-0.1.1/setup.py` & `jplaw-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jplaw',
-    version='0.1.1',
+    version='0.1.2',
     packages=['jplaw'],
     description='A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)',
     author='Amar Persaud',
     author_email='amar.d.persaud@gmail.com',
     install_requires=["requests >=2.6.0, <3.0"],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

