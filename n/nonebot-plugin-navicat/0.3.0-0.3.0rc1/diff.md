# Comparing `tmp/nonebot-plugin-navicat-0.3.0.tar.gz` & `tmp/nonebot-plugin-navicat-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-navicat-0.3.0.tar", last modified: Sun Jun 25 08:54:51 2023, max compression
+gzip compressed data, was "nonebot-plugin-navicat-0.3.0rc1.tar", last modified: Thu Oct 20 06:47:08 2022, max compression
```

## Comparing `nonebot-plugin-navicat-0.3.0.tar` & `nonebot-plugin-navicat-0.3.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:54:51.965833 nonebot-plugin-navicat-0.3.0/
--rw-rw-rw-   0        0        0    35821 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5516 2023-06-25 08:54:51.966336 nonebot-plugin-navicat-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 08:54:51.959801 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/
--rw-rw-rw-   0        0        0     1004 2023-06-25 08:49:46.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/command.py
--rw-rw-rw-   0        0        0     1198 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/elasticsearch.py
--rw-rw-rw-   0        0        0     1311 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/mongodb.py
--rw-rw-rw-   0        0        0      984 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/mysql.py
--rw-rw-rw-   0        0        0     1004 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/postgre.py
--rw-rw-rw-   0        0        0     3442 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/redis.py
--rw-rw-rw-   0        0        0      905 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:54:51.964325 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/
--rw-rw-rw-   0        0        0     5516 2023-06-25 08:54:51.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-06-25 08:54:51.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:54:51.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-06-25 08:54:51.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-25 08:54:51.000000 nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1039 2023-06-25 08:54:51.966839 nonebot-plugin-navicat-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2050 2023-06-25 08:52:05.000000 nonebot-plugin-navicat-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:54:51.964828 nonebot-plugin-navicat-0.3.0/test/
--rw-rw-rw-   0        0        0      420 2023-04-25 14:37:58.000000 nonebot-plugin-navicat-0.3.0/test/test_sential.py
+drwxrwxrwx   0        0        0        0 2022-10-20 06:47:08.293540 nonebot-plugin-navicat-0.3.0rc1/
+-rw-rw-rw-   0        0        0    35821 2022-10-20 06:09:59.000000 nonebot-plugin-navicat-0.3.0rc1/LICENSE
+-rw-rw-rw-   0        0        0     5540 2022-10-20 06:47:08.297538 nonebot-plugin-navicat-0.3.0rc1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-20 06:47:07.824762 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/
+-rw-rw-rw-   0        0        0      725 2022-10-20 06:24:58.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/__init__.py
+-rw-rw-rw-   0        0        0     1222 2022-10-20 06:33:18.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/command.py
+-rw-rw-rw-   0        0        0     1198 2022-10-20 06:18:33.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/elasticsearch.py
+-rw-rw-rw-   0        0        0     1311 2022-10-20 06:24:34.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/mongodb.py
+-rw-rw-rw-   0        0        0      984 2022-10-20 06:24:34.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/mysql.py
+-rw-rw-rw-   0        0        0     1004 2022-10-20 06:24:35.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/postgre.py
+-rw-rw-rw-   0        0        0     3442 2022-10-20 06:33:18.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/redis.py
+-rw-rw-rw-   0        0        0      905 2022-10-20 06:24:26.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/sqlite.py
+drwxrwxrwx   0        0        0        0 2022-10-20 06:47:08.204581 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/
+-rw-rw-rw-   0        0        0     5540 2022-10-20 06:46:59.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2022-10-20 06:47:06.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-20 06:47:00.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2022-10-20 06:47:05.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2022-10-20 06:47:05.000000 nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2022-10-20 06:09:59.000000 nonebot-plugin-navicat-0.3.0rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1042 2022-10-20 06:47:08.328526 nonebot-plugin-navicat-0.3.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2053 2022-10-20 06:41:56.000000 nonebot-plugin-navicat-0.3.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-20 06:47:08.274550 nonebot-plugin-navicat-0.3.0rc1/test/
+-rw-rw-rw-   0        0        0      403 2022-10-20 06:33:37.000000 nonebot-plugin-navicat-0.3.0rc1/test/test_sential.py
```

### Comparing `nonebot-plugin-navicat-0.3.0/LICENSE` & `nonebot-plugin-navicat-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/PKG-INFO` & `nonebot-plugin-navicat-0.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-navicat
-Version: 0.3.0
+Version: 0.3.0rc1
 Summary: A batabase manager plugin for nonebot2,provide capability of connection to all kinds of databases
 Home-page: https://github.com/synodriver/nonebot_plugin_navicat
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/synodriver/nonebot_plugin_navicat/issues
 Keywords: nonebot
+Platform: UNKNOWN
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -183,7 +184,8 @@
 - [nonebot / nonebot2](https://github.com/nonebot/nonebot2)
 
 ## 优化建议
 
 - bug report
 - more databases support
 ![](https://i.pixiv.cat/img-original/img/2018/08/29/00/16/10/70434240_p0.png "bug哪里跑 看姐姐给你们全抓起来~")
+
```

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/__init__.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from nonebot.plugin import PluginMetadata
-from nonebot.config import Config
-
 from . import elasticsearch, mongodb, mysql, postgre, redis, sqlite
 
 if hasattr(elasticsearch, "elasticsearch"):
     elasticsearch = elasticsearch.elasticsearch
 if hasattr(mongodb, "mongodb_client"):
     mongodb_client = mongodb.mongodb_client
 if hasattr(mysql, "mysql_pool"):
@@ -16,16 +13,7 @@
     redis_client = redis.redis_client
 if hasattr(redis, "redis_sentinel"):
     redis_sentinel = redis.redis_sentinel
 if hasattr(redis, "redis_cluster"):
     redis_cluster = redis.redis_cluster
 if hasattr(sqlite, "sqlite_pool"):
     sqlite_pool = sqlite.sqlite_pool
-
-
-__plugin_meta__ = PluginMetadata(
-    name="nonebot_plugin_navicat",
-    description="Nonebot数据库支持",
-    usage="被别的插件require使用",
-    config=Config,
-    extra={},
-)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/command.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/elasticsearch.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/mongodb.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/mongodb.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/mysql.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/mysql.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/postgre.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/postgre.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/redis.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/redis.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat/sqlite.py` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat/sqlite.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/PKG-INFO` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-navicat
-Version: 0.3.0
+Version: 0.3.0rc1
 Summary: A batabase manager plugin for nonebot2,provide capability of connection to all kinds of databases
 Home-page: https://github.com/synodriver/nonebot_plugin_navicat
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/synodriver/nonebot_plugin_navicat/issues
 Keywords: nonebot
+Platform: UNKNOWN
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -183,7 +184,8 @@
 - [nonebot / nonebot2](https://github.com/nonebot/nonebot2)
 
 ## 优化建议
 
 - bug report
 - more databases support
 ![](https://i.pixiv.cat/img-original/img/2018/08/29/00/16/10/70434240_p0.png "bug哪里跑 看姐姐给你们全抓起来~")
+
```

### Comparing `nonebot-plugin-navicat-0.3.0/nonebot_plugin_navicat.egg-info/SOURCES.txt` & `nonebot-plugin-navicat-0.3.0rc1/nonebot_plugin_navicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-navicat-0.3.0/setup.cfg` & `nonebot-plugin-navicat-0.3.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f6e 6562 6f74 2d70 6c75 6769   = nonebot-plugi
 00000020: 6e2d 6e61 7669 6361 740d 0a76 6572 7369  n-navicat..versi
-00000030: 6f6e 203d 2030 2e33 2e30 0d0a 6b65 7977  on = 0.3.0..keyw
-00000040: 6f72 6473 203d 200d 0a09 6e6f 6e65 626f  ords = ...nonebo
-00000050: 740d 0a61 7574 686f 7220 3d20 7379 6e6f  t..author = syno
-00000060: 6472 6976 6572 0d0a 6175 7468 6f72 5f65  driver..author_e
-00000070: 6d61 696c 203d 2064 6967 756f 6875 616e  mail = diguohuan
-00000080: 676a 6961 6a69 6e77 6569 6a75 6e40 676d  gjiajinweijun@gm
-00000090: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-000000a0: 7469 6f6e 203d 2041 2062 6174 6162 6173  tion = A batabas
-000000b0: 6520 6d61 6e61 6765 7220 706c 7567 696e  e manager plugin
-000000c0: 2066 6f72 206e 6f6e 6562 6f74 322c 7072   for nonebot2,pr
-000000d0: 6f76 6964 6520 6361 7061 6269 6c69 7479  ovide capability
-000000e0: 206f 6620 636f 6e6e 6563 7469 6f6e 2074   of connection t
-000000f0: 6f20 616c 6c20 6b69 6e64 7320 6f66 2064  o all kinds of d
-00000100: 6174 6162 6173 6573 0d0a 6c6f 6e67 5f64  atabases..long_d
-00000110: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000120: 653a 2052 4541 444d 452e 6d61 726b 646f  e: README.markdo
-00000130: 776e 0d0a 6c6f 6e67 5f64 6573 6372 6970  wn..long_descrip
-00000140: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000150: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000160: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 7379 6e6f  /github.com/syno
-00000180: 6472 6976 6572 2f6e 6f6e 6562 6f74 5f70  driver/nonebot_p
-00000190: 6c75 6769 6e5f 6e61 7669 6361 740d 0a70  lugin_navicat..p
-000001a0: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-000001b0: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001d0: 6d2f 7379 6e6f 6472 6976 6572 2f6e 6f6e  m/synodriver/non
-000001e0: 6562 6f74 5f70 6c75 6769 6e5f 6e61 7669  ebot_plugin_navi
-000001f0: 6361 742f 6973 7375 6573 0d0a 636c 6173  cat/issues..clas
-00000200: 7369 6669 6572 7320 3d20 0d0a 0946 7261  sifiers = ...Fra
-00000210: 6d65 776f 726b 203a 3a20 4173 796e 6349  mework :: AsyncI
-00000220: 4f0d 0a09 4f70 6572 6174 696e 6720 5379  O...Operating Sy
-00000230: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000240: 656e 6465 6e74 0d0a 094c 6963 656e 7365  endent...License
-00000250: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000260: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
-00000270: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
-00000280: 3320 2847 504c 7633 290d 0a09 5072 6f67  3 (GPLv3)...Prog
-00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002a0: 203a 3a20 5079 7468 6f6e 0d0a 0950 726f   :: Python...Pro
-000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002d0: 2e37 0d0a 0950 726f 6772 616d 6d69 6e67  .7...Programming
-000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002f0: 686f 6e20 3a3a 2033 2e38 0d0a 0950 726f  hon :: 3.8...Pro
-00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000320: 2e39 0d0a 0950 726f 6772 616d 6d69 6e67  .9...Programming
-00000330: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000340: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-00000350: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-00000360: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000370: 6573 203d 200d 0a09 6e6f 6e65 626f 7432  es = ...nonebot2
-00000380: 0d0a 0964 6174 6162 6173 6573 0d0a 0d0a  ...databases....
-00000390: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
-000003a0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-000003b0: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
-000003c0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-000003d0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-000003e0: 370d 0a0d 0a5b 6567 675f 696e 666f 5d0d  7....[egg_info].
-000003f0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000400: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000030: 6f6e 203d 2030 2e33 2e30 7263 310d 0a6b  on = 0.3.0rc1..k
+00000040: 6579 776f 7264 7320 3d20 0d0a 096e 6f6e  eywords = ...non
+00000050: 6562 6f74 0d0a 6175 7468 6f72 203d 2073  ebot..author = s
+00000060: 796e 6f64 7269 7665 720d 0a61 7574 686f  ynodriver..autho
+00000070: 725f 656d 6169 6c20 3d20 6469 6775 6f68  r_email = diguoh
+00000080: 7561 6e67 6a69 616a 696e 7765 696a 756e  uangjiajinweijun
+00000090: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
+000000a0: 7269 7074 696f 6e20 3d20 4120 6261 7461  ription = A bata
+000000b0: 6261 7365 206d 616e 6167 6572 2070 6c75  base manager plu
+000000c0: 6769 6e20 666f 7220 6e6f 6e65 626f 7432  gin for nonebot2
+000000d0: 2c70 726f 7669 6465 2063 6170 6162 696c  ,provide capabil
+000000e0: 6974 7920 6f66 2063 6f6e 6e65 6374 696f  ity of connectio
+000000f0: 6e20 746f 2061 6c6c 206b 696e 6473 206f  n to all kinds o
+00000100: 6620 6461 7461 6261 7365 730d 0a6c 6f6e  f databases..lon
+00000110: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00000120: 6669 6c65 3a20 5245 4144 4d45 2e6d 6172  file: README.mar
+00000130: 6b64 6f77 6e0d 0a6c 6f6e 675f 6465 7363  kdown..long_desc
+00000140: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000150: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000160: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000180: 796e 6f64 7269 7665 722f 6e6f 6e65 626f  ynodriver/nonebo
+00000190: 745f 706c 7567 696e 5f6e 6176 6963 6174  t_plugin_navicat
+000001a0: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+000001b0: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+000001c0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001d0: 2e63 6f6d 2f73 796e 6f64 7269 7665 722f  .com/synodriver/
+000001e0: 6e6f 6e65 626f 745f 706c 7567 696e 5f6e  nonebot_plugin_n
+000001f0: 6176 6963 6174 2f69 7373 7565 730d 0a63  avicat/issues..c
+00000200: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000210: 4672 616d 6577 6f72 6b20 3a3a 2041 7379  Framework :: Asy
+00000220: 6e63 494f 0d0a 094f 7065 7261 7469 6e67  ncIO...Operating
+00000230: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000240: 6465 7065 6e64 656e 740d 0a09 4c69 6365  dependent...Lice
+00000250: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000260: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
+00000270: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+00000280: 6520 7633 2028 4750 4c76 3329 0d0a 0950  e v3 (GPLv3)...P
+00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002a0: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
+000002b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002d0: 3a20 332e 370d 0a09 5072 6f67 7261 6d6d  : 3.7...Programm
+000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002f0: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
+00000300: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000310: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000320: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+00000330: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000340: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
+00000350: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
+00000360: 686f 6e0d 0a69 6e73 7461 6c6c 5f72 6571  hon..install_req
+00000370: 7569 7265 7320 3d20 0d0a 096e 6f6e 6562  uires = ...noneb
+00000380: 6f74 320d 0a09 6461 7461 6261 7365 730d  ot2...databases.
+00000390: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 696e  ...[options]..in
+000003a0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+000003b0: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
+000003c0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000003d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000003e0: 3d33 2e37 0d0a 0d0a 5b65 6767 5f69 6e66  =3.7....[egg_inf
+000003f0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000400: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000410: 0d0a                                     ..
```

### Comparing `nonebot-plugin-navicat-0.3.0/setup.py` & `nonebot-plugin-navicat-0.3.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         return f.read()
 
 
 def main():
     dis = get_dis()
     setup(
         name="nonebot-plugin-navicat",
-        version="0.3.0",
+        version="0.3.0rc1",
         url="https://github.com/synodriver/nonebot_plugin_navicat",
         packages=packages,
         keywords=["nonebot"],
         description="A batabase manager plugin for nonebot2,provide capability of connection to all kinds of databases",
         long_description_content_type="text/markdown",
         long_description=dis,
         author="synodriver",
```

