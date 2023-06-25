# Comparing `tmp/nonebot_plugin_helltide-0.1.6.tar.gz` & `tmp/nonebot_plugin_helltide-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helltide-0.1.6.tar", last modified: Sat Jun 24 17:56:28 2023, max compression
+gzip compressed data, was "nonebot_plugin_helltide-0.1.7.tar", last modified: Sun Jun 25 13:19:47 2023, max compression
```

## Comparing `nonebot_plugin_helltide-0.1.6.tar` & `nonebot_plugin_helltide-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-24 17:56:20.616546 nonebot_plugin_helltide-0.1.6/LICENSE
--rw-r--r--   0        0        0     2598 2023-06-24 17:56:20.616546 nonebot_plugin_helltide-0.1.6/README.md
--rw-r--r--   0        0        0     3093 2023-06-24 17:56:20.616546 nonebot_plugin_helltide-0.1.6/nonebot_plugin_helltide/.gitignore
--rw-r--r--   0        0        0    11680 2023-06-24 17:56:20.616546 nonebot_plugin_helltide-0.1.6/nonebot_plugin_helltide/__init__.py
--rw-r--r--   0        0        0      219 2023-06-24 17:56:20.616546 nonebot_plugin_helltide-0.1.6/nonebot_plugin_helltide/config.py
--rw-r--r--   0        0        0     1045 2023-06-24 17:56:28.072628 nonebot_plugin_helltide-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-25 13:19:39.846669 nonebot_plugin_helltide-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2598 2023-06-25 13:19:39.846669 nonebot_plugin_helltide-0.1.7/README.md
+-rw-r--r--   0        0        0     3093 2023-06-25 13:19:39.846669 nonebot_plugin_helltide-0.1.7/nonebot_plugin_helltide/.gitignore
+-rw-r--r--   0        0        0    11691 2023-06-25 13:19:39.846669 nonebot_plugin_helltide-0.1.7/nonebot_plugin_helltide/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-25 13:19:39.846669 nonebot_plugin_helltide-0.1.7/nonebot_plugin_helltide/config.py
+-rw-r--r--   0        0        0     1045 2023-06-25 13:19:47.898756 nonebot_plugin_helltide-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_helltide-0.1.6/LICENSE` & `nonebot_plugin_helltide-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.6/README.md` & `nonebot_plugin_helltide-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.6/nonebot_plugin_helltide/.gitignore` & `nonebot_plugin_helltide-0.1.7/nonebot_plugin_helltide/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.6/nonebot_plugin_helltide/__init__.py` & `nonebot_plugin_helltide-0.1.7/nonebot_plugin_helltide/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from nonebot.adapters.onebot.v11 import (
     GroupMessageEvent,
     MessageEvent,
 )
 import datetime
 
 __plugin_meta__ = PluginMetadata(
-    name="helltide",
-    description="一个Diablo4的helltide和世界boss的提醒小助手",
+    name="Diablo4地狱狂潮boss提醒小助手",
+    description="支持订阅，在D4继续上班",
     # BEGIN: 7d7f3c7b5d4a
     usage="这是一个diablo4插件，可以订阅游戏中的事件，如boss刷新、地狱潮汐等，\n当事件即将发生时会自动提醒订阅用户。使用方法：\n1. 订阅事件：d4订阅 boss/helltide\n2. 取消订阅事件：d4取消订阅 boss/helltide\n3. 查询订阅列表：d4查询订阅",
     # END: 7d7f3c7b5d4a
     homepage="https://github.com/QBkira/nonebot-plugin-helltide",
-    type="library",
+    type="application",
     config=Config,
     supported_adapters={"~onebot.v11"},
     extra={"author": "qbkira"},
 )
 
 my_config = Config.parse_obj(get_driver().config)
```

### Comparing `nonebot_plugin_helltide-0.1.6/pyproject.toml` & `nonebot_plugin_helltide-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-plugin-helltide"
-version = "0.1.6"
+version = "0.1.7"
 description = "Diablo 4 Helltide Event Tracker work with nonebot2"
 authors = [
     { name = "qbkira", email = "qbuouo@gmail.com" },
 ]
 dependencies = [
     "nonebot2",
     "nonebot2[fastapi]",
```

### Comparing `nonebot_plugin_helltide-0.1.6/PKG-INFO` & `nonebot_plugin_helltide-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helltide
-Version: 0.1.6
+Version: 0.1.7
 Summary: Diablo 4 Helltide Event Tracker work with nonebot2
 Home-page: https://github.com/QBkira/nonebot-plugin-helltide
 Author-Email: qbkira <qbuouo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/QBkira/nonebot-plugin-helltide
 Project-URL: Repository, https://github.com/QBkira/nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide
 Project-URL: Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.7 Summary:
 Diablo 4 Helltide Event Tracker work with nonebot2 Home-page: https://
 github.com/QBkira/nonebot-plugin-helltide Author-Email: qbkira
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/QBkira/
 nonebot-plugin-helltide Project-URL: Repository, https://github.com/QBkira/
 nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide Project-URL:
 Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
 Requires-Python: >=3.8 Requires-Dist: nonebot2 Requires-Dist: nonebot2[fastapi]
```

