# Comparing `tmp/nonebot-plugin-alconna-0.8.1.tar.gz` & `tmp/nonebot-plugin-alconna-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.8.1.tar", last modified: Thu Jun 22 16:21:51 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.8.2.tar", last modified: Sun Jun 25 15:31:35 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.8.1.tar` & `nonebot-plugin-alconna-0.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.1/LICENSE
--rw-r--r--   0        0        0     1524 2023-06-22 16:21:04.954312 nonebot-plugin-alconna-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.1/README.md
--rw-r--r--   0        0        0     1789 2023-06-22 16:21:04.935845 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0     5109 2023-06-22 16:21:04.974805 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2295 2023-06-22 14:54:15.807613 nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1524 2023-06-25 11:31:51.131389 nonebot-plugin-alconna-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.2/README.md
+-rw-r--r--   0        0        0     1912 2023-06-25 11:34:36.599625 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0     6259 2023-06-25 15:29:08.347891 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2295 2023-06-22 14:54:15.807613 nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.2/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.8.1/LICENSE` & `nonebot-plugin-alconna-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/pyproject.toml` & `nonebot-plugin-alconna-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.8.1"
+version = "0.8.2"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "arclet-alconna<2.0.0, >=1.7.7",
```

### Comparing `nonebot-plugin-alconna-0.8.1/README.md` & `nonebot-plugin-alconna-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,31 +18,33 @@
 from .params import assign as assign
 from .params import match_path as match_path
 from .params import match_value as match_value
 from .rule import alconna as alconna
 from .rule import set_output_converter as set_output_converter
 from .config import Config
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 _meta_source = {
     "name": "Alconna 插件",
     "description": "提供 [Alconna](https://github.com/ArcletProject/Alconna) 的 Nonebot2 适配版本与工具",
     "usage": "matcher = on_alconna(...)",
     "homepage": "https://github.com/ArcletProject/Alconna",
     "type": "library",
+    "supported_adapters": None,
     "config": Config,
     "extra": {
         "author": "RF-Tar-Railt",
         "priority": 1,
         "version": __version__,
     }
 }
 
 
 if not nonebot_version.split(".")[-1].isdigit():
     _meta_source["extra"]["homepage"] = _meta_source.pop("homepage")
     _meta_source["extra"]["type"] = _meta_source.pop("type")
     _meta_source["extra"]["config"] = _meta_source.pop("config")
+    _meta_source["extra"]["supported_adapters"] = _meta_source.pop("supported_adapters")
 
 
 __plugin_meta__ = PluginMetadata(**_meta_source)
```

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/__init__.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """通用标注, 无法用于创建 MS对象"""
-from nonebot_plugin_alconna.typings import gen_unit
-from nonebot.internal.adapter.message import MessageSegment
-from nepattern import create_local_patterns
 from dataclasses import dataclass, field
+import re
 from typing import Optional
 
+from nepattern import create_local_patterns
+from nonebot.internal.adapter.message import MessageSegment
+from nonebot_plugin_alconna.typings import gen_unit
 
 Text = str
 
 @dataclass
 class Segment:
     """基类标注"""
     origin: MessageSegment
@@ -16,14 +17,21 @@
 
 @dataclass
 class At(Segment):
     """At对象, 表示一类提醒某用户的元素"""
     target: str
 
 @dataclass
+class Emoji(Segment):
+    """Emoji对象, 表示一类表情元素"""
+    id: str
+    name: Optional[str] = field(default=None)
+
+
+@dataclass
 class Media(Segment):
     url: Optional[str] = field(default=None)
     id: Optional[str] = field(default=None)
 
 @dataclass
 class Image(Media):
     """Image对象, 表示一类图片元素"""
@@ -43,35 +51,61 @@
 @dataclass
 class File(Segment):
     """File对象, 表示一类文件元素"""
     id: str
     name: Optional[str] = field(default=None)
 
 
+def _handle_kmarkdown_met(seg: MessageSegment):
+    content = seg.data["content"]
+    if not content.startswith("(met)"):
+        return None
+    if (end := content.find("(met)", 5)) == -1:
+        return None
+    return content[5: end] not in ("here", "all") and At(seg, content[5: end])
+
 _At = gen_unit(
     At,
     {
         "at": lambda seg: At(seg, str(seg.data.get("qq", seg.data.get("user_id")))),
         "mention": lambda seg: At(seg, seg.data.get("user_id", seg.data.get("text"))),
         "mention_user": lambda seg: At(seg, str(seg.data["user_id"])),
         "At": lambda seg: At(seg, str(seg, seg.data["target"])),
-        "kmarkdown": lambda seg: (
-            seg.startswith("(met)") and
-            ((end := seg.find("(met)", 5)) != -1 and seg[5: end] not in ("here", "all") and At(seg, seg[5: end]))
-        ),
+        "kmarkdown": _handle_kmarkdown_met
     }
 )
 """
 at: ob11, feishu
 mention: ob12, tg
 mention_user: qqguild
 At: mirai
 kmarkdown: kook
 """
 
+def _handle_kmarkdown_emj(seg: MessageSegment):
+    content = seg.data["content"]
+    if content.startswith("(emj)"):
+        mat = re.search(r"\(emj\)(?P<name>[^()\[\]]+)\(emj\)\[(?P<id>[^\[\]]+)\]", content)
+        return mat and Emoji(seg, mat["id"], mat["name"])
+    if content.startswith(":"):
+        mat = re.search(r":(?P<name>[^:]+):", content)
+        return mat and Emoji(seg, mat["name"], mat["name"])
+
+_Emoji = gen_unit(
+    Emoji,
+    {
+        "emoji": lambda seg: Emoji(seg, str(seg.data.get("id", seg.data.get("name")))),
+        "Face": lambda seg: Emoji(seg, str(seg.data["faceId"]), seg.data["name"]),
+        "face": lambda seg: str(Emoji(seg, seg.data["id"])),
+        "custom_emoji": lambda seg: Emoji(seg, seg.data["custom_emoji_id"], seg.data["text"]),
+        "kmarkdown": _handle_kmarkdown_emj
+    }
+)
+
+
 
 def _handle_image(seg: MessageSegment):
     if "file_id" in seg.data:  # ob12
         return Image(seg, id=seg.data["file_id"])
     if "image_key" in seg.data:  # feishu
         return Image(seg, url=seg.data["image_key"])
     if "file_key" in seg.data:  # kook
```

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.8.2/src/nonebot_plugin_alconna/typings.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.1/PKG-INFO` & `nonebot-plugin-alconna-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.8.1
+Version: 0.8.2
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
```

