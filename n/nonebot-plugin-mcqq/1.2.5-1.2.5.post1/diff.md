# Comparing `tmp/nonebot-plugin-mcqq-1.2.5.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.5.tar", last modified: Sat Jun 24 12:41:29 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.5.post1.tar", last modified: Sun Jun 25 05:26:49 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.5.tar` & `nonebot-plugin-mcqq-1.2.5.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:29.519236 nonebot-plugin-mcqq-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-24 12:41:29.519236 nonebot-plugin-mcqq-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:29.519236 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:29.519236 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-24 12:41:29.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-24 12:41:29.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:41:29.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 12:41:29.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-24 12:41:29.000000 nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:41:29.519236 nonebot-plugin-mcqq-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-24 12:41:23.000000 nonebot-plugin-mcqq-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.5/LICENSE` & `nonebot-plugin-mcqq-1.2.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.5/PKG-INFO` & `nonebot-plugin-mcqq-1.2.5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.5
+Version: 1.2.5.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.5/README.md` & `nonebot-plugin-mcqq-1.2.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Union
 
-from mcqq_tool.config import Config
-from mcqq_tool.common import GUILD_ADMIN
-from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 from nonebot import on_message, on_command, get_driver, require
+
+require("nonebot_plugin_guild_patch")
+
 from nonebot.params import CommandArg
 from nonebot.adapters import Message
 from nonebot.plugin import PluginMetadata
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
-
-require("nonebot_plugin_guild_patch")
+from mcqq_tool.config import Config
+from mcqq_tool.common import GUILD_ADMIN
+from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
 from .data_source import start_ws_server, stop_ws_server
 from .utils import msg_rule
 
 __plugin_meta__ = PluginMetadata(
```

### Comparing `nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.5/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.5
+Version: 1.2.5.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.5/setup.py` & `nonebot-plugin-mcqq-1.2.5.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.5",
+    version="1.2.5-post1",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
     packages=["nonebot_plugin_mcqq"],
```

