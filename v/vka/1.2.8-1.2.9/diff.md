# Comparing `tmp/vka-1.2.8.tar.gz` & `tmp/vka-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vka-1.2.8.tar", last modified: Wed Mar  8 14:04:40 2023, max compression
+gzip compressed data, was "vka-1.2.9.tar", last modified: Sun Mar 12 11:44:36 2023, max compression
```

## Comparing `vka-1.2.8.tar` & `vka-1.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.208702 vka-1.2.8/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2699 2023-03-08 14:04:40.208912 vka-1.2.8/PKG-INFO
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2251 2022-11-20 17:55:44.000000 vka-1.2.8/README.md
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       38 2023-03-08 14:04:40.209773 vka-1.2.8/setup.cfg
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      778 2023-03-08 14:04:08.000000 vka-1.2.8/setup.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.190954 vka-1.2.8/vka/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      279 2023-03-08 13:57:49.000000 vka-1.2.8/vka/__init__.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5441 2023-03-08 13:58:05.000000 vka-1.2.8/vka/api.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.198576 vka-1.2.8/vka/base/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       70 2022-11-20 17:53:11.000000 vka-1.2.8/vka/base/__init__.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     8944 2022-11-20 17:53:11.000000 vka-1.2.8/vka/base/attrdict.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.199874 vka-1.2.8/vka/base/buiders/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5461 2022-11-20 17:53:11.000000 vka-1.2.8/vka/base/buiders/button.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2646 2021-07-12 17:07:51.000000 vka-1.2.8/vka/base/buiders/keyboard.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      719 2022-11-25 17:37:28.000000 vka-1.2.8/vka/base/exception.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3373 2022-12-18 14:58:23.000000 vka-1.2.8/vka/base/longpoll.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5137 2023-03-08 07:11:42.000000 vka-1.2.8/vka/base/wrapper.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     7154 2022-12-18 15:17:40.000000 vka-1.2.8/vka/bot.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.206637 vka-1.2.8/vka/chatbot/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       78 2022-12-18 11:51:35.000000 vka-1.2.8/vka/chatbot/__init__.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     8745 2023-03-07 19:15:03.000000 vka-1.2.8/vka/chatbot/checking.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)    12344 2023-03-08 10:14:35.000000 vka-1.2.8/vka/chatbot/context.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       24 2022-11-20 17:53:11.000000 vka-1.2.8/vka/chatbot/filter.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3635 2023-01-02 09:45:54.000000 vka-1.2.8/vka/chatbot/menu.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     1812 2022-12-17 16:32:21.000000 vka-1.2.8/vka/chatbot/push_button_menu.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2227 2023-03-08 14:04:08.000000 vka-1.2.8/vka/chatbot/registration.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      751 2022-12-17 19:12:09.000000 vka-1.2.8/vka/chatbot/storage.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.207907 vka-1.2.8/vka/chatbot/wrappers/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3873 2023-03-07 16:25:42.000000 vka-1.2.8/vka/chatbot/wrappers/messege.py
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      771 2023-01-04 10:13:44.000000 vka-1.2.8/vka/chatbot/wrappers/user.py
-drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-08 14:04:40.194237 vka-1.2.8/vka.egg-info/
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2699 2023-03-08 14:04:40.000000 vka-1.2.8/vka.egg-info/PKG-INFO
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      618 2023-03-08 14:04:40.000000 vka-1.2.8/vka.egg-info/SOURCES.txt
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)        1 2023-03-08 14:04:40.000000 vka-1.2.8/vka.egg-info/dependency_links.txt
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       25 2023-03-08 14:04:40.000000 vka-1.2.8/vka.egg-info/requires.txt
--rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       63 2023-03-08 14:04:40.000000 vka-1.2.8/vka.egg-info/top_level.txt
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.506598 vka-1.2.9/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2699 2023-03-12 11:44:36.507146 vka-1.2.9/PKG-INFO
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2251 2022-11-20 17:55:44.000000 vka-1.2.9/README.md
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       38 2023-03-12 11:44:36.507979 vka-1.2.9/setup.cfg
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      778 2023-03-12 11:43:26.000000 vka-1.2.9/setup.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.483667 vka-1.2.9/vka/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      279 2023-03-08 13:57:49.000000 vka-1.2.9/vka/__init__.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5441 2023-03-08 13:58:05.000000 vka-1.2.9/vka/api.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.492225 vka-1.2.9/vka/base/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       70 2022-11-20 17:53:11.000000 vka-1.2.9/vka/base/__init__.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     8944 2022-11-20 17:53:11.000000 vka-1.2.9/vka/base/attrdict.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.493940 vka-1.2.9/vka/base/buiders/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5461 2022-11-20 17:53:11.000000 vka-1.2.9/vka/base/buiders/button.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2646 2021-07-12 17:07:51.000000 vka-1.2.9/vka/base/buiders/keyboard.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      719 2022-11-25 17:37:28.000000 vka-1.2.9/vka/base/exception.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3373 2022-12-18 14:58:23.000000 vka-1.2.9/vka/base/longpoll.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     5137 2023-03-08 07:11:42.000000 vka-1.2.9/vka/base/wrapper.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     7154 2022-12-18 15:17:40.000000 vka-1.2.9/vka/bot.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.502100 vka-1.2.9/vka/chatbot/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       78 2022-12-18 11:51:35.000000 vka-1.2.9/vka/chatbot/__init__.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     8746 2023-03-12 08:20:40.000000 vka-1.2.9/vka/chatbot/checking.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)    12605 2023-03-12 08:17:26.000000 vka-1.2.9/vka/chatbot/context.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       24 2022-11-20 17:53:11.000000 vka-1.2.9/vka/chatbot/filter.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3635 2023-01-02 09:45:54.000000 vka-1.2.9/vka/chatbot/menu.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     1812 2022-12-17 16:32:21.000000 vka-1.2.9/vka/chatbot/push_button_menu.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2351 2023-03-12 11:43:00.000000 vka-1.2.9/vka/chatbot/registration.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      751 2023-03-12 08:11:33.000000 vka-1.2.9/vka/chatbot/storage.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.505117 vka-1.2.9/vka/chatbot/wrappers/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     3873 2023-03-07 16:25:42.000000 vka-1.2.9/vka/chatbot/wrappers/messege.py
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      771 2023-01-04 10:13:44.000000 vka-1.2.9/vka/chatbot/wrappers/user.py
+drwxr-xr-x   0 aleksejzuravlev   (501) staff       (20)        0 2023-03-12 11:44:36.486672 vka-1.2.9/vka.egg-info/
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)     2699 2023-03-12 11:44:36.000000 vka-1.2.9/vka.egg-info/PKG-INFO
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)      618 2023-03-12 11:44:36.000000 vka-1.2.9/vka.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)        1 2023-03-12 11:44:36.000000 vka-1.2.9/vka.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       25 2023-03-12 11:44:36.000000 vka-1.2.9/vka.egg-info/requires.txt
+-rw-r--r--   0 aleksejzuravlev   (501) staff       (20)       63 2023-03-12 11:44:36.000000 vka-1.2.9/vka.egg-info/top_level.txt
```

### Comparing `vka-1.2.8/PKG-INFO` & `vka-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vka
-Version: 1.2.8
+Version: 1.2.9
 Summary: module for the vk api wrapper
 Home-page: https://github.com/MrCreEper002/vka
 Author: Major4ik
 Author-email: 2772771882@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vka-1.2.8/README.md` & `vka-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/setup.py` & `vka-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='vka',
-	version='1.2.8',
+	version='1.2.9',
 	author='Major4ik',
 	author_email='2772771882@mail.ru',
 	description='module for the vk api wrapper',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/MrCreEper002/vka',
 	include_package_data=True,
```

### Comparing `vka-1.2.8/vka/api.py` & `vka-1.2.9/vka/api.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/attrdict.py` & `vka-1.2.9/vka/base/attrdict.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/buiders/button.py` & `vka-1.2.9/vka/base/buiders/button.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/buiders/keyboard.py` & `vka-1.2.9/vka/base/buiders/keyboard.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/exception.py` & `vka-1.2.9/vka/base/exception.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/longpoll.py` & `vka-1.2.9/vka/base/longpoll.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/base/wrapper.py` & `vka-1.2.9/vka/base/wrapper.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/bot.py` & `vka-1.2.9/vka/bot.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/chatbot/checking.py` & `vka-1.2.9/vka/chatbot/checking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import asyncio
 import json
 
 from loguru import logger
+
 from vka.base import AttrDict
 from vka.chatbot.context import Context
 
 
 class CheckingEventForCommand:
 
     def __init__(
```

### Comparing `vka-1.2.8/vka/chatbot/context.py` & `vka-1.2.9/vka/chatbot/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import json
 from typing import Optional, List, Union, Dict, AsyncIterable
 from loguru import logger
-from vka import API, random_
+from vka import API, random_, VkApiError
 from vka.base.wrapper import Event, Message
 from vka.chatbot.wrappers.user import User
 
 
 class Context:
 
     def __init__(self, event, api: API, bot):
         self._bot = bot
         self._api = api
         self._event = event
-        self.command = None
+        self.command = ''
 
     @property
     def api(self) -> API:
         return self._api
 
     @property
     def event(self) -> Event:
@@ -158,15 +158,26 @@
             message: str,
             **kwargs,
     ):
         # TODO Переписать или удалить!
         """
         данная функция означает что будет изменено последнее сообщение бота
         """
-        await self.edit(message, self.msg.conversation_message_id, **kwargs)
+        try:
+            await self.edit(
+                message,
+                self.msg.conversation_message_id,
+                **kwargs
+            )
+        except VkApiError as error:
+            if f"[{error.error_code}] {error.error_msg}" \
+                    == "[909] Can't edit this message, because it's too old":
+                await self.answer(
+                    message, **kwargs
+                )
 
     async def fetch_sender(
             self,
             fields: List[str] = None,
             name_case: str = None,
             **kwargs
     ) -> list[User] | None | User:
@@ -292,35 +303,23 @@
                     if self.msg.from_id in any_user:
                         return True
                 elif any_user is Ellipsis:
                     return True
             return False
         return False
 
-    async def _messages_send(self, locals_: locals, params: Dict) -> int:
-        for name, value in locals_.items():
-            if name == "kwargs":
-                params.update(value)
-            elif name != "self" and value is not None:
-                params.update({name: value})
+    async def _messages_send(self, locals_: locals, params: Dict) -> dict:
+        params = check_params(locals_=locals_, params=params)
 
-        del params["params"]
         params['random_id'] = random_()
         messages_id = await self.api.method("messages.send", params)
         return messages_id
 
-    async def _messages_edit(self, locals_: locals, params: Dict):
-
-        for name, value in locals_.items():
-            if name == "kwargs":
-                params.update(value)
-            elif name != "self" and value is not None:
-                params.update({name: value})
-
-        del params["params"]
+    async def _messages_edit(self, locals_: locals, params: Dict) -> dict:
+        params = check_params(locals_=locals_, params=params)
 
         messages_id = await self.api.method("messages.edit", params)
         return messages_id
 
     async def receiving(self):
         while True:
             try:
@@ -331,17 +330,27 @@
                 logger.error(vka_error)
                 continue
 
     async def for_receiving(self, new_event, any_user):
         for event in new_event:
             logger.warning(event)
             event = Event(event)
-            logger.success(event)
             ctx = Context(event=event, api=self.api, bot=self)
 
             match event.type:
                 case ['message_new', 'message_event']:
                     if any_user:
                         yield ctx
                     else:
                         if self.msg.from_id in ctx.msg.from_id:
                             yield ctx
+
+
+def check_params(locals_: locals, params: dict) -> dict:
+    for name, value in locals_.items():
+        if name == "kwargs":
+            params.update(value)
+        elif name != "self" and value is not None:
+            params.update({name: value})
+
+    del params["params"]
+    return params
```

### Comparing `vka-1.2.8/vka/chatbot/menu.py` & `vka-1.2.9/vka/chatbot/menu.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/chatbot/push_button_menu.py` & `vka-1.2.9/vka/chatbot/push_button_menu.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/chatbot/registration.py` & `vka-1.2.9/vka/chatbot/registration.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,28 +33,31 @@
         s = await self.soup()
 
         last_logged_in = datetime.strptime(
             s.find('ya:lastloggedin').attrs.get('dc:date'),
             "%Y-%m-%dT%H:%M:%S+03:00"
         ) if s.find('ya:lastloggedin') is not None \
             else s.find('ya:lastloggedin')
+        location = s.find('ya:location').attrs.get('ya:city') \
+            if s.find('ya:lastloggedin') is not None \
+            else s.find('ya:location')
 
         return {
             "public_access": s.find('ya:publicaccess').text,
             "profile_state": s.find('ya:profilestate').text,
             "id": s.find('ya:uri').attrs.get('rdf:resource'),
             "first_name": s.find('ya:firstname').text,
             "second_name": s.find('ya:secondname').text,
             "name": s.find('foaf:name').text,
             "gender": s.find('foaf:gender').text,
             "subscribers_count": s.find('ya:subscriberscount').text,
             "friends_count": s.find('ya:friendscount').text,
             "subscribed_to_count": s.find('ya:subscribedtocount').text,
             "birthday": s.find('foaf:birthday').text,
-            "location": s.find('ya:location').attrs.get('ya:city'),
+            "location": location,
             "created": datetime.strptime(
                 s.find('ya:created').attrs.get('dc:date'),
                 "%Y-%m-%dT%H:%M:%S+03:00"
             ),
             "modified": datetime.strptime(
                 s.find('ya:modified').attrs.get('dc:date'),
                 "%Y-%m-%dT%H:%M:%S+03:00"
```

### Comparing `vka-1.2.8/vka/chatbot/storage.py` & `vka-1.2.9/vka/chatbot/storage.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/chatbot/wrappers/messege.py` & `vka-1.2.9/vka/chatbot/wrappers/messege.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka/chatbot/wrappers/user.py` & `vka-1.2.9/vka/chatbot/wrappers/user.py`

 * *Files identical despite different names*

### Comparing `vka-1.2.8/vka.egg-info/PKG-INFO` & `vka-1.2.9/vka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vka
-Version: 1.2.8
+Version: 1.2.9
 Summary: module for the vk api wrapper
 Home-page: https://github.com/MrCreEper002/vka
 Author: Major4ik
 Author-email: 2772771882@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vka-1.2.8/vka.egg-info/SOURCES.txt` & `vka-1.2.9/vka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

