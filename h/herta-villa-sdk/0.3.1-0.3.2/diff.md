# Comparing `tmp/herta_villa_sdk-0.3.1.tar.gz` & `tmp/herta_villa_sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.3.1.tar", last modified: Sat Jun 24 10:17:43 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.3.2.tar", last modified: Sun Jun 25 10:54:13 2023, max compression
```

## Comparing `herta_villa_sdk-0.3.1.tar` & `herta_villa_sdk-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/LICENSE
--rw-r--r--   0        0        0     2039 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/README.md
--rw-r--r--   0        0        0      555 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/__init__.py
--rw-r--r--   0        0        0    11250 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/bot.py
--rw-r--r--   0        0        0     4864 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1617 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/image.py
--rw-r--r--   0        0        0      981 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/post.py
--rw-r--r--   0        0        0     6461 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/text.py
--rw-r--r--   0        0        0      369 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/types.py
--rw-r--r--   0        0        0     2396 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/model.py
--rw-r--r--   0        0        0     2932 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/server.py
--rw-r--r--   0        0        0      565 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/version.py
--rw-r--r--   0        0        0     2128 2023-06-24 10:17:43.581042 herta_villa_sdk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      572 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2039 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/README.md
+-rw-r--r--   0        0        0      555 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/__init__.py
+-rw-r--r--   0        0        0    11250 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/bot.py
+-rw-r--r--   0        0        0     4842 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3799 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1414 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/types.py
+-rw-r--r--   0        0        0     2396 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/model.py
+-rw-r--r--   0        0        0     2932 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/server.py
+-rw-r--r--   0        0        0      564 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/version.py
+-rw-r--r--   0        0        0     2128 2023-06-25 10:54:13.204465 herta_villa_sdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.2/PKG-INFO
```

### Comparing `herta_villa_sdk-0.3.1/LICENSE` & `herta_villa_sdk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/README.md` & `herta_villa_sdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/__init__.py` & `herta_villa_sdk-0.3.2/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/bot.py` & `herta_villa_sdk-0.3.2/hertavilla/bot.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/event.py` & `herta_villa_sdk-0.3.2/hertavilla/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,15 @@
             body = entity["entity"]
             type_ = body.pop("type")
             if offset != end_offset:
                 # 两个 Entity 偏移相差为文字
                 chain.append(
                     Text(text[_rc(end_offset) : _rc(offset)].decode("utf-16")),
                 )
-            else:
-                chain.append(entity_types[type_](**body))
+            chain.append(entity_types[type_](**body))
             last_offset = offset
             last_length = entity["length"]
             end_offset = last_offset + last_length
         if _rc(end_offset) != len(text):
             # 最后一个 Entity 之后是文字
             chain.append(
                 Text(text[_rc(end_offset) :].decode("utf-16")),
```

### Comparing `herta_villa_sdk-0.3.1/hertavilla/exception.py` & `herta_villa_sdk-0.3.2/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/match.py` & `herta_villa_sdk-0.3.2/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/message/image.py` & `herta_villa_sdk-0.3.2/hertavilla/message/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, TypedDict, cast
+from typing import TYPE_CHECKING, Optional, cast
 
-from hertavilla.message.types import (
-    MsgContent,
-    MsgContentInfo,
-    _Segment,
-)
+from hertavilla.message.types import MsgContent, MsgContentInfo, _Segment
+from hertavilla.typing import TypedDict
 
 if TYPE_CHECKING:
     from hertavilla.bot import VillaBot
 
 
 # MsgContentInfo for image
 class ImageMsgContentInfo(MsgContentInfo):
@@ -44,28 +41,18 @@
 
     async def get_text(self, _: VillaBot) -> str:
         return "[图片]"
 
 
 # MsgContent for image
 class ImageMsgContent(MsgContent):
-    def __init__(
-        self,
-        url: str,
-        size: Size | None = None,
-        file_size: int | None = None,
-    ) -> None:
-        self.url = url
-        if size:
-            self.size = size
-        if file_size:
-            self.file_size = file_size
+    url: str
+    size: Optional[Size] = None
+    file_size: Optional[int] = None
 
 
-def image_to_content(image: Image) -> ImageMsgContentInfo:
-    return {
-        "content": ImageMsgContent(
-            image.url,
-            cast(Optional[Size], image.size),
-            image.file_size,
-        ),
-    }
+def image_to_content(image: Image) -> ImageMsgContent:
+    return ImageMsgContent(
+        url=image.url,
+        size=cast(Optional[Size], image.size),
+        file_size=image.file_size,
+    )
```

### Comparing `herta_villa_sdk-0.3.1/hertavilla/message/post.py` & `herta_villa_sdk-0.3.2/hertavilla/message/post.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 
 if TYPE_CHECKING:
     from hertavilla.bot import VillaBot
 
 
 # MsgContentInfo for post
-class ImageMsgContentInfo(MsgContentInfo):
+class PostMsgContentInfo(MsgContentInfo):
     content: PostMsgContent
 
 
 # Segment for post
 
 
 class Post(_Segment):
@@ -31,13 +31,12 @@
         #
         # https://bbs-api.miyoushe.com/post/wapi/semPosts?gids=6&post_id={}
         return "[帖子]"
 
 
 # MsgContent for post
 class PostMsgContent(MsgContent):
-    def __init__(self, post_id: str) -> None:
-        self.post_id = post_id
+    post_id: str
 
 
-def post_to_content(post: Post) -> ImageMsgContentInfo:
-    return {"content": PostMsgContent(post.post_id)}
+def post_to_content(post: Post) -> PostMsgContentInfo:
+    return {"content": PostMsgContent(post_id=post.post_id)}
```

### Comparing `herta_villa_sdk-0.3.1/hertavilla/message/text.py` & `herta_villa_sdk-0.3.2/hertavilla/message/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 from __future__ import annotations
 
-import sys
 from typing import TYPE_CHECKING, Any, List, Literal, Optional, cast
 
-# Pydantic:
-#   TypeError: You should use `typing_extensions.TypedDict`
-#   instead of `typing.TypedDict` with Python < 3.9.2.
-#   Without it, there is no way to differentiate
-#   required and optional fields when subclassed.
-if sys.version_info >= (3, 9, 2):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
-
+from hertavilla.message.image import ImageMsgContent
 from hertavilla.message.types import MsgContent, MsgContentInfo, _Segment
+from hertavilla.typing import TypedDict
 from hertavilla.utils import _c
 
 if TYPE_CHECKING:
     from hertavilla.bot import VillaBot
 
 entity_types: dict[str, type["_TextEntity"]] = {}
 
@@ -163,22 +154,23 @@
         raise NotImplementedError
 
 
 # MsgContent for text
 
 
 class TextMsgContent(MsgContent):
-    def __init__(self, text: str, entities: list[EntityDict]) -> None:
-        self.text = text
-        self.entities = entities
+    text: str
+    entities: List[EntityDict]
+    images: Optional[List[ImageMsgContent]] = None
 
 
 async def text_to_content(
     text_entities: list[_TextEntity],
     bot: VillaBot,
+    image: list[ImageMsgContent] | None = None,
 ) -> TextMsgContentInfo:
     texts: list[str] = []
     entities: list[EntityDict] = []
     mentioned_info: MentionedInfo | None = None
     quote: QuoteInfo | None = None
     offset = 0
     for i, entity in enumerate(text_entities):
@@ -224,11 +216,15 @@
                         mentioned_info["type"] = type_
                     user_id_list = mentioned_info["userIdList"]
                 if type_ != 1:
                     user_id_list.append(id_)
         offset += len(text)
         texts.append(text)
     return {
-        "content": TextMsgContent("".join(texts), entities),
+        "content": TextMsgContent(
+            text="".join(texts),
+            entities=entities,
+            images=image,
+        ),
         "quote": quote,
         "mentionedInfo": mentioned_info,
     }
```

### Comparing `herta_villa_sdk-0.3.1/hertavilla/model.py` & `herta_villa_sdk-0.3.2/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/server.py` & `herta_villa_sdk-0.3.2/hertavilla/server.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.1/hertavilla/utils.py` & `herta_villa_sdk-0.3.2/hertavilla/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class MsgEncoder(json.JSONEncoder):
     def default(self, obj):
         from hertavilla.message.types import MsgContent
 
         if isinstance(obj, MsgContent):
-            data = obj.__dict__
+            data = obj.dict()
             for k in data.copy().keys():
                 if k.startswith("_"):
                     data.pop(k)
             return data
         return json.JSONEncoder.default(self, obj)
```

### Comparing `herta_villa_sdk-0.3.1/pyproject.toml` & `herta_villa_sdk-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.3.1"
+version = "0.3.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/MingxuanGame/Herta-villa-SDK"
 Documentation = "https://github.com/MingxuanGame/Herta-villa-SDK"
```

### Comparing `herta_villa_sdk-0.3.1/tests/test_utils.py` & `herta_villa_sdk-0.3.2/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 def test_msg_encoder():
     import json
 
     from hertavilla.message.types import MsgContent
     from hertavilla.utils import MsgEncoder
 
     class TestMsgContent(MsgContent):
-        def __init__(self) -> None:
-            self.test = 1
-            self._private = 0
+        test: int = 1
+        _private: int = 0
 
     assert json.loads(json.dumps(TestMsgContent(), cls=MsgEncoder)) == {
         "test": 1,
     }
```

### Comparing `herta_villa_sdk-0.3.1/PKG-INFO` & `herta_villa_sdk-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/MingxuanGame/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/MingxuanGame/Herta-villa-SDK
 Project-URL: Repository, https://github.com/MingxuanGame/Herta-villa-SDK
```

