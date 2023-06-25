# Comparing `tmp/jplaw-0.1.2.tar.gz` & `tmp/jplaw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.2.tar", last modified: Sat Jun 24 22:36:58 2023, max compression
+gzip compressed data, was "jplaw-0.1.3.tar", last modified: Sun Jun 25 21:08:58 2023, max compression
```

## Comparing `jplaw-0.1.2.tar` & `jplaw-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-24 22:36:48.000000 jplaw-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 22:36:58.513698 jplaw-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-24 22:36:48.000000 jplaw-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-24 22:36:48.000000 jplaw-0.1.2/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:36:58.513698 jplaw-0.1.2/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 22:36:58.000000 jplaw-0.1.2/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-24 22:36:48.000000 jplaw-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:36:58.513698 jplaw-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-24 22:36:48.000000 jplaw-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-25 21:08:48.000000 jplaw-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 21:08:58.949240 jplaw-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-25 21:08:48.000000 jplaw-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.945240 jplaw-0.1.3/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-25 21:08:48.000000 jplaw-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:08:58.949240 jplaw-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-25 21:08:48.000000 jplaw-0.1.3/setup.py
```

### Comparing `jplaw-0.1.2/LICENSE` & `jplaw-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.2/PKG-INFO` & `jplaw-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jplaw-0.1.2/jplaw/api_paths.py` & `jplaw-0.1.3/jplaw/api_paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .http_type import HttpType
+from .types.http_type import HttpType
 
 API_VERSION = "/api/v3"
 API_PATH = {
     "login" :                               { "method": HttpType.POST    , "path": "/user/login"                            },
     "getPost" :                             { "method": HttpType.GET     , "path": "/post"                                  },
     "getCommunity" :                        { "method": HttpType.GET     , "path": "/community"                             },
     "listCommunities" :                     { "method": HttpType.GET     , "path": "/community/list"                        },
```

### Comparing `jplaw-0.1.2/jplaw/comment.py` & `jplaw-0.1.3/jplaw/comment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 from .requestor import Requestor
 from .api_paths import *
-from .listing_type import ListingType
-from .comment_sort_type import CommentSortType
+from .types.listing_type import ListingType
+from .types.comment_sort_type import CommentSortType
 
 class Comment():
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def createComment(self, post_id:int, content:str, parent_id:int=None, language_id:str=None, instance:str=None, auth_token:str=None):
+    def create(self, post_id:int, content:str, parent_id:int=None, language_id:str=None, instance:str=None, auth_token:str=None):
         form = {
             "content": content,
             "post_id": post_id,
         }
         optional={
             "language_id": language_id,
             "parent_id": parent_id
         }
         res = self._req.lemmyRequest("createComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         
         return res["comment_view"]
         
-    def likeComment(self, comment_id:int, score:int=1, instance:str=None, auth_token:str=None):
+    def like(self, comment_id:int, score:int=1, instance:str=None, auth_token:str=None):
         if(score > 1):
             score = 1
         if(score < -1):
             score = -1
         form = {
             "comment_id": comment_id,
             "score": score
         }
         res = self._req.lemmyRequest("likeComment", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["comment_view"]
         
-    def createCommentReport(self, comment_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, comment_id:int, reason:str, instance:str=None, auth_token:str=None):
         form = {
             "comment_id": comment_id,
             "reason": reason
             }
         res = self._req.lemmyRequest("createCommentReport", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def deleteComment(self, comment_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, comment_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "comment_id": comment_id,
             "deleted": deleted
             }
         res = self._req.lemmyRequest("deleteComment", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["comment_view"]
         
-    def removeComment(self, comment_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
+    def remove(self, comment_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
         form = {
             "comment_id": comment_id,
             "mod_person_id": mod_person_id,
             "when_": when_,
             "removed": removed,
             }
         optional={
             "reason":reason,
             }
         res = self._req.lemmyRequest("removeComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["comment_view"]
         
-    def distinguishComment(self, comment_id:int, distinguished:bool=True, instance:str=None, auth_token:str=None):
+    def distinguish(self, comment_id:int, distinguished:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "comment_id": comment_id,
             "distinguished": distinguished,
             }
         res = self._req.lemmyRequest("distinguishComment", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["comment_view"]
         
-    def editComment(self, comment_id:int, content:str=None, language_id:str=None, form_id:str=None, instance:str=None, auth_token:str=None):
+    def edit(self, comment_id:int, content:str=None, language_id:str=None, form_id:str=None, instance:str=None, auth_token:str=None):
         form = {
             "comment_id": comment_id
             }
         optional={
             "content":content,
             "language_id":language_id,
             "form_id":form_id,
             }
         res = self._req.lemmyRequest("editComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["comment_view"]
-    
-    def getComment(self, comment_id:int, instance:str=None, auth:bool=True, auth_token:str=None):
+        
+    def get(self, comment_id:int, instance:str=None, auth:bool=True, auth_token:str=None):    
         form = {
             "comment_id": comment_id
             }
         res = self._req.lemmyRequest("getComment", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
         return res["comment_view"]
-    def getComments(self, 
+        
+    def list(self, 
         comment_type:ListingType=None, 
         sort:CommentSortType=None, 
         max_depth:int=None, 
         page:int=None, 
         limit:int=None, 
         community_id:int=None, 
         post_id:int=None, 
@@ -115,41 +116,41 @@
             "community_name" : community_name  ,
             "parent_id"      : parent_id       ,
             "saved_only"     : saved_only      ,
             }
         res = self._req.lemmyRequest("getComments", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
         return res["comment_view"]
     
-    def listCommentReports(self, page:int=None, limit:int=None, unresolved_only:bool=None, community_id:int=None, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=None, community_id:int=None, instance:str=None, auth_token:str=None):
         form = {}
         optional={
             "page"           : page            ,
             "limit"          : limit           ,
             "community_id"   : community_id    ,
             "unresolved_only": unresolved_only ,
             }
         res = self._req.lemmyRequest("listCommentReports", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
         return
         
-    def markCommentReplyAsRead(self, comment_reply_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markReplyAsRead(self, comment_reply_id:int, read:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "comment_reply_id"  : comment_reply_id  ,
             "read"              : read              ,
             }
         res = self._req.lemmyRequest("markCommentReplyAsRead", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
     
-    def resolveCommentReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
         res = self._req.lemmyRequest("resolveCommentReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
     
-    def saveComment(self, comment_id:int, save:bool=True, instance:str=None, auth_token:str=None):
+    def save(self, comment_id:int, save:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "comment_id"  : comment_id ,
             "save"   : save,
             }
         res = self._req.lemmyRequest("saveComment", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
```

### Comparing `jplaw-0.1.2/jplaw/community.py` & `jplaw-0.1.3/jplaw/community.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,66 @@
-from .requestor import Requestor, HttpType
+from .requestor import Requestor
 from .api_paths import *
 from typing import List
 
 class Community():
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def getCommunity(self, name:str, instance:str=None, auth:bool=True, auth_token:str=None):
+    def get(self, name:str, instance:str=None, auth:bool=True, auth_token:str=None):
         form = {
             "name": name
         }
         res = self._req.lemmyRequest("getCommunity", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res["community_view"]
         
-    def listCommunities(self, instance:str=None, auth:bool=True, auth_token:str=None): 
+    def list(self, instance:str=None, auth:bool=True, auth_token:str=None): 
         form={}
         res = self._req.lemmyRequest("listCommunities", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res["communities"]
         
-    def followCommunity(self, community_id:int, follow:bool=True, instance:str=None, auth_token:str=None):
+    def follow(self, community_id:int, follow:bool=True, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "follow": follow
         }
         res = self._req.lemmyRequest("followCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["community_view"]
-    def addModToCommunity(self, community_id:int, person_id:int, added:bool=True, instance:str=None, auth_token:str=None): 
-        form={
-            "community_id": community_id,
-            "person_id": person_id,
-            "added": added,
-        }
-        res = self._req.lemmyRequest("addModToCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
-        return res
-    def addModToCommunity(self, community_id:int, person_id:int, added:bool=True, instance:str=None, auth_token:str=None):
+    def addMod(self, community_id:int, person_id:int, added:bool=True, instance:str=None, auth_token:str=None): 
         form={
             "community_id": community_id,
             "person_id": person_id,
             "added": added,
         }
         res = self._req.lemmyRequest("addModToCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
     
-    def banFromCommunity(self, community_id:int, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def banPerson(self, community_id:int, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "person_id": person_id,
             "ban": ban,
         }
         optional={
             "remove_data": remove_data,
             "reason": reason,
             "expires": expires,
         }
         res = self._req.lemmyRequest("banFromCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
         
-    def blockCommunity(self, community_id:int, block:bool=True, instance:str=None, auth_token:str=None):
+    def block(self, community_id:int, block:bool=True, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "block": block,
             }
         res = self._req.lemmyRequest("blockCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["community_view"]
         
-    def createCommunity(self, name:str, title:str, description:str=None, icon:str=None, banner:str=None, nsfw:bool=None, posting_restricted_to_mods:bool=None, discussion_languages:List[str]=None, instance:str=None, auth_token:str=None):
+    def create(self, name:str, title:str, description:str=None, icon:str=None, banner:str=None, nsfw:bool=None, posting_restricted_to_mods:bool=None, discussion_languages:List[str]=None, instance:str=None, auth_token:str=None):
         form={
             "name": name,
             "title": title,
             }
         optional={
             "description": description,
             "icon": icon,
@@ -76,23 +68,23 @@
             "nsfw": nsfw,
             "posting_restricted_to_mods": posting_restricted_to_mods,
             "discussion_languages": discussion_languages,
             }
         res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["community_view"]
         
-    def deleteCommunity(self, community_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, community_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "deleted": deleted,
             }
         res = self._req.lemmyRequest("deleteCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["community_view"]
     
-    def editCommunity(self, community_id:int, title:str=None, description:str=None, icon:str=None, banner:str=None, nsfw:bool=None, posting_restricted_to_mods:bool=None, discussion_languages:List[str]=None, instance:str=None, auth_token:str=None):
+    def edit(self, community_id:int, title:str=None, description:str=None, icon:str=None, banner:str=None, nsfw:bool=None, posting_restricted_to_mods:bool=None, discussion_languages:List[str]=None, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             }
         optional={
             "title": title,
             "description": description,
             "icon": icon,
@@ -100,26 +92,26 @@
             "nsfw": nsfw,
             "posting_restricted_to_mods": posting_restricted_to_mods,
             "discussion_languages": discussion_languages,
             }
         res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["community_view"]
         
-    def removeCommunity(self, community_id:int, removed:bool=True, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def remove(self, community_id:int, removed:bool=True, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "removed":removed,
             }
         optional={
             "reason": reason,
             "expires": expires,
             }
         res = self._req.lemmyRequest("removeCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["community_view"]
     
-    def transferCommunity(self, community_id:int, person_id:int, instance:str=None, auth_token:str=None):
+    def transfer(self, community_id:int, person_id:int, instance:str=None, auth_token:str=None):
         form={
             "community_id": community_id,
             "person_id":person_id,
             }
         res = self._req.lemmyRequest("transferCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res["community_view"]
```

### Comparing `jplaw-0.1.2/jplaw/lemmy.py` & `jplaw-0.1.3/jplaw/lemmy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from .requestor import Requestor, HttpType
-from enum import *
+from .requestor import Requestor
 from .comment import Comment
 from .community import Community
 from .post import Post
 from .user import User
 from .site import Site
 from .private_message import PrivateMessage
 
@@ -36,16 +35,16 @@
         self.PrivateMessage = PrivateMessage(self._req)
         # print(self._req.headers.get("Authorization"))
         
     def resolveObject(self, obj, instance=None, auth_token=None):
         form={
             "q": obj
         }
-        res = self._req.lemmyRequest(HttpType.GET, "resolveObject", instance=instance, form=form, auth_token=auth_token)
+        res = self._req.lemmyRequest("resolveObject", instance=instance, form=form, auth_token=auth_token)
         return res
         
     def search(self, term, instance=None, auth_token=None):
         form={
             "q": term
         }
-        res = self._req.request(HttpType.GET, "search", instance=instance, auth_token=auth_token, form=form)
+        res = self._req.request("search", instance=instance, auth_token=auth_token, form=form)
         return res
```

### Comparing `jplaw-0.1.2/jplaw/modlog_action_type.py` & `jplaw-0.1.3/jplaw/types/modlog_action_type.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1 +1 @@
-from enum import Enumclass ModlogActionType(Enum):    All                     = "All"                     ,    ModRemovePost           = "ModRemovePost"           ,    ModLockPost             = "ModLockPost"             ,    ModFeaturePost          = "ModFeaturePost"          ,    ModRemoveComment        = "ModRemoveComment"        ,    ModRemoveCommunity      = "ModRemoveCommunity"      ,    ModBanFromCommunity     = "ModBanFromCommunity"     ,    ModAddCommunity         = "ModAddCommunity"         ,    ModTransferCommunity    = "ModTransferCommunity"    ,    ModAdd                  = "ModAdd"                  ,    ModBan                  = "ModBan"                  ,    ModHideCommunity        = "ModHideCommunity"        ,    AdminPurgePerson        = "AdminPurgePerson"        ,    AdminPurgeCommunity     = "AdminPurgeCommunity"     ,    AdminPurgePost          = "AdminPurgePost"          ,    AdminPurgeComment       = "AdminPurgeComment"       ,
+from enum import Enumclass ModlogActionType(Enum):    All                     = "All"                     ModRemovePost           = "ModRemovePost"           ModLockPost             = "ModLockPost"             ModFeaturePost          = "ModFeaturePost"          ModRemoveComment        = "ModRemoveComment"        ModRemoveCommunity      = "ModRemoveCommunity"      ModBanFromCommunity     = "ModBanFromCommunity"     ModAddCommunity         = "ModAddCommunity"         ModTransferCommunity    = "ModTransferCommunity"    ModAdd                  = "ModAdd"                  ModBan                  = "ModBan"                  ModHideCommunity        = "ModHideCommunity"        AdminPurgePerson        = "AdminPurgePerson"        AdminPurgeCommunity     = "AdminPurgeCommunity"     AdminPurgePost          = "AdminPurgePost"          AdminPurgeComment       = "AdminPurgeComment"
```

### Comparing `jplaw-0.1.2/jplaw/post.py` & `jplaw-0.1.3/jplaw/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,144 +1,144 @@
 from .requestor import Requestor
 from .api_paths import *
-from .post_feature_type import PostFeatureType
+from .types.post_feature_type import PostFeatureType
 
 class Post():
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def getPosts(self, community_id:int, sort:str=None, instance:str=None, auth:bool=True, auth_token:str=None):
+    def list(self, community_id:int, sort:str=None, instance:str=None, auth:bool=True, auth_token:str=None):
         form = { "sort": sort or "New", "community_id": community_id }
         res = self._req.lemmyRequest("getPosts", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res["posts"]
         
-    def getPost(self, community_id, post_id, instance:str=None, auth=True, auth_token:str=None):
+    def get(self, community_id, post_id, instance:str=None, auth=True, auth_token:str=None):
         form = {
             "id": post_id,
         }
         res = self._req.lemmyRequest("getPost", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res["post_view"]
         
-    def createPost(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw=False, language_id=None, instance:str=None, auth_token:str=None):
+    def create(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw=False, language_id=None, instance:str=None, auth_token:str=None):
         #there could be a bug here if instance != logged in instance when trying to create a post
         form = {
             "community_id": community_id,
             "name": title,
             "body": body,
             "language_id": language_id,
             "nsfw": nsfw
             }
         optional={
             "url": remote_url
         }
         res = self._req.lemmyRequest("createPost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["post_view"]
         
-    def editPost(self, post_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw:bool=None, language_id=None, instance:str=None, auth_token:str=None):
+    def edit(self, post_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw:bool=None, language_id=None, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
         }
         optional={
             "url": remote_url,
             "nsfw": nsfw,
             "language_id": language_id,
             "name": name,
             "body": body
         }
         res = self._req.lemmyRequest("editPost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res["post_view"]
         
-    def likePost(self, post_id:int, score:int=1, language_id=None, instance:str=None, auth_token:str=None):
+    def like(self, post_id:int, score:int=1, language_id=None, instance:str=None, auth_token:str=None):
         if(score > 1):
             score = 1
         if(score < -1):
             score = -1
         form = {
             "post_id": post_id,
             "score": score
         }
         res = self._req.lemmyRequest("likePost", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
     
-    def createPostReport(self, post_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, post_id:int, reason:str, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "reason": reason
             }
         res = self._req.lemmyRequest("createPostReport", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def deletePost(self, post_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, post_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "deleted": deleted
             }
         res = self._req.lemmyRequest("deletePost", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def featurePost(self, post_id:int, feature_type: PostFeatureType, featured:bool=True, instance:str=None, auth_token:str=None):
+    def feature(self, post_id:int, feature_type: PostFeatureType, featured:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "feature_type": feature_type.value,
             "featured": featured,
             }
         res = self._req.lemmyRequest("featurePost", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def listPostReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, community_id:int=None, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, community_id:int=None, instance:str=None, auth_token:str=None):
         form = {}
         optional = {
             "page": page,
             "limit": limit,
             "unresolved_only": unresolved_only,
             "community_id": community_id,
             }
         res = self._req.lemmyRequest("listPostReports", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
     
-    def lockPost(self, post_id:int, locked:bool=True, instance:str=None, auth_token:str=None):
+    def lock(self, post_id:int, locked:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "locked": locked,
         }
         res = self._req.lemmyRequest("lockPost", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def markPostAsRead(self, post_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markAsRead(self, post_id:int, read:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "read": read,
         }
         res = self._req.lemmyRequest("markPostAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
     
-    def resolvePostReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
         res = self._req.lemmyRequest("resolvePostReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
         
-    def savePost(self, post_id:int, save:bool=True, instance:str=None, auth_token:str=None):
+    def save(self, post_id:int, save:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "post_id"  : post_id ,
             "save"   : save,
             }
         res = self._req.lemmyRequest("savePost", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
         
     def getSiteMetadata(self, remote_url:str, instance:str=None, auth:bool=True, auth_token:str=None):
         form={
             "url": remote_url,
         }
         res = self._req.lemmyRequest("getSiteMetadata", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res
         
-    def removePost(self, post_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
+    def remove(self, post_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
         form = {
             "post_id": post_id,
             "mod_person_id": mod_person_id,
             "when_": when_,
             "removed": removed,
             }
         optional={
```

### Comparing `jplaw-0.1.2/jplaw/private_message.py` & `jplaw-0.1.3/jplaw/private_message.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,73 +2,73 @@
 from .api_paths import *
 
 
 class PrivateMessage():
     def __init__(self, _req: Requestor):
         self._req = _req
     
-    def getPrivateMessages(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
+    def list(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
         form = {}
         optional={
             "unread_only": unread_only,
             "page": page,
             "limit": limit,
             }
         res = self._req.lemmyRequest("getPrivateMessages", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
-    def createPrivateMessage(self, content:str, recipient_id:int, instance:str=None, auth_token:str=None):
+    def create(self, content:str, recipient_id:int, instance:str=None, auth_token:str=None):
         form = {
             "content": content,
             "recipient_id": recipient_id,
             }
         res = self._req.lemmyRequest("createPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def createPrivateMessageReport(self, private_message_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, private_message_id:int, reason:str, instance:str=None, auth_token:str=None):
         form = {
             "private_message_id": private_message_id,
             "reason": reason,
             }
         res = self._req.lemmyRequest("createPrivateMessageReport", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def editPrivateMessage(self, private_message_id:int, content:str, instance:str=None, auth_token:str=None):
+    def edit(self, private_message_id:int, content:str, instance:str=None, auth_token:str=None):
         form = {
             "private_message_id": private_message_id,
             "content": content,
             }
         res = self._req.lemmyRequest("editPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def deletePrivateMessage(self, private_message_id:int, instance:str=None, auth_token:str=None):
+    def delete(self, private_message_id:int, instance:str=None, auth_token:str=None):
         form = {
             "private_message_id": private_message_id,
             }
         res = self._req.lemmyRequest("deletePrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
         
-    def markPrivateMessageAsRead(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
+    def markAsRead(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
         form={}
         optional = {
             "unread_only": unread_only,
             "page": page,
             "limit": limit,
             }
         res = self._req.lemmyRequest("markPrivateMessageAsRead", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
         
-    def listPrivateMessageReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, instance:str=None, auth_token:str=None):
         form = {}
         optional = {
             "page": page,
             "limit": limit,
             "unresolved_only": unresolved_only,
             }
         res = self._req.lemmyRequest("listPrivateMessageReports", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
-    def resolvePrivateMessageReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
         res = self._req.lemmyRequest("resolvePrivateMessageReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return
```

### Comparing `jplaw-0.1.2/jplaw/requestor.py` & `jplaw-0.1.3/jplaw/requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 import requests
 import json
 from typing import Dict, Any, TypeVar
 from .api_paths import *
-from .http_type import HttpType
+from .types.http_type import HttpType
 
 T = TypeVar("T")
 
 class Requestor:
     def __init__(self, instance:str, username:str, password:str, headers: Dict[str, str]):
         """
         Make an HTTP request
@@ -102,15 +102,15 @@
             Access token
         """
         self.instance = instance or self.instance
         form = { "username_or_email": username, "password": password }
         res_data = self.lemmyRequest("login", form=form, instance=instance)
         return res_data["jwt"]
     
-    def AddIfValue(self, name, value, form):
+    def AddIfValue(self, name:str, value, form: Dict[str, Any]):
         """
         Adds items to form if not None
         Args:
         
         Returns:
             Access token
         """
```

### Comparing `jplaw-0.1.2/jplaw/user.py` & `jplaw-0.1.3/jplaw/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,37 +21,37 @@
             "captcha_uuid"   :captcha_uuid   ,
             "limit"          :limit          ,
             "honeypot"       :honeypot       ,
             "answer"         :answer         ,
             }
         res = self._req.lemmyRequest("register", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
-    def getPersonDetails(self, person_id:str=None, username:str=None, sort:str=None, page:int=0, limit:int=10, community_id:int=None, saved_only:bool=None, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getDetails(self, person_id:str=None, username:str=None, sort:str=None, page:int=0, limit:int=10, community_id:int=None, saved_only:bool=None, instance:str=None, auth:bool=True, auth_token:str=None):
         form={}
         optional={
             "person_id"      :person_id      ,
             "username"       :username       ,
             "sort"           :sort           ,
             "page"           :page           ,
             "limit"          :limit          ,
             "community_id"   :community_id   ,
             "saved_only"     :saved_only     ,
             }
         res = self._req.lemmyRequest("getPersonDetails", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
         return res
     
-    def markPersonMentionAsRead(self, person_mention_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markMentionAsRead(self, person_mention_id:int, read:bool=True, instance:str=None, auth_token:str=None):
         form={
             "person_mention_id": person_mention_id,
             "read": read
             }
         res = self._req.lemmyRequest("markPersonMentionAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
     
-    def getPersonMentions(self, sort:str=None, page:int=0, limit:int=10, unread_only:bool=True, instance:str=None, auth_token:str=None):
+    def getMentions(self, sort:str=None, page:int=0, limit:int=10, unread_only:bool=True, instance:str=None, auth_token:str=None):
         form={}
         optional = {
             "sort"           :sort           ,
             "page"           :page           ,
             "limit"          :limit          ,
             "unread_only"    :unread_only    ,
             }
@@ -65,33 +65,33 @@
             "page"           :page           ,
             "limit"          :limit          ,
             "unread_only"    :unread_only    ,
             }
         res = self._req.lemmyRequest("getReplies", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
     
-    def banPerson(self, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def ban(self, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
         form={
             "person_id"     :person_id,
             "ban"           :ban
             }
         optional = {
             "remove_data"    :remove_data   ,
             "reason"         :reason        ,
             "expires"        :expires
             }
         res = self._req.lemmyRequest("banPerson", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
         return res
     
-    def getBannedPersons(self, instance:str=None, auth_token:str=None):
+    def getBanned(self, instance:str=None, auth_token:str=None):
         form={}
         res = self._req.lemmyRequest(HttpType.GET, "getBannedPersons", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
      
-    def blockPerson(self, person_id:int, block:bool, instance:str=None, auth_token:str=None):
+    def block(self, person_id:int, block:bool, instance:str=None, auth_token:str=None):
         form={
             "person_id": person_id,
             "block": block
             }
         res = self._req.lemmyRequest("blockPerson", instance=instance, form=form, auth=True, auth_token=auth_token)
         return res
```

### Comparing `jplaw-0.1.2/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.3/jplaw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jplaw-0.1.2/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.3/jplaw.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 jplaw/__init__.py
 jplaw/api_paths.py
 jplaw/comment.py
-jplaw/comment_sort_type.py
 jplaw/community.py
-jplaw/http_type.py
 jplaw/language.py
 jplaw/lemmy.py
-jplaw/listing_type.py
-jplaw/modlog_action_type.py
 jplaw/post.py
-jplaw/post_feature_type.py
 jplaw/private_message.py
 jplaw/requestor.py
-jplaw/search_type.py
 jplaw/site.py
-jplaw/sort_type.py
-jplaw/subscribed_type.py
 jplaw/user.py
 jplaw.egg-info/PKG-INFO
 jplaw.egg-info/SOURCES.txt
 jplaw.egg-info/dependency_links.txt
 jplaw.egg-info/requires.txt
-jplaw.egg-info/top_level.txt
+jplaw.egg-info/top_level.txt
+jplaw/types/__init__.py
+jplaw/types/comment_sort_type.py
+jplaw/types/http_type.py
+jplaw/types/listing_type.py
+jplaw/types/modlog_action_type.py
+jplaw/types/post_feature_type.py
+jplaw/types/registration_mode.py
+jplaw/types/search_type.py
+jplaw/types/sort_type.py
+jplaw/types/subscribed_type.py
```

### Comparing `jplaw-0.1.2/pyproject.toml` & `jplaw-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jplaw"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Amar Persaud", email="tehspartaa@gmail.com" },
 ]
 description = "A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jplaw-0.1.2/setup.py` & `jplaw-0.1.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jplaw',
-    version='0.1.2',
-    packages=['jplaw'],
+    version='0.1.3',
+    packages=['jplaw', 'jplaw/types'],
     description='A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)',
     author='Amar Persaud',
     author_email='amar.d.persaud@gmail.com',
     install_requires=["requests >=2.6.0, <3.0"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

