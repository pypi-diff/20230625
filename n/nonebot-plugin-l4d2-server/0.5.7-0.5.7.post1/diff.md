# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.7.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.7.post1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.7.tar` & `nonebot_plugin_l4d2_server-0.5.7.post1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-25 10:10:57.169930 nonebot_plugin_l4d2_server-0.5.7/LICENSE
--rw-r--r--   0        0        0     5683 2023-06-25 10:10:57.169930 nonebot_plugin_l4d2_server-0.5.7/README.md
--rw-r--r--   0        0        0    19815 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1879 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3691 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10990 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8989 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5960 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9672 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    15320 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1604 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 13:39:28.959299 nonebot_plugin_l4d2_server-0.5.7.post1/LICENSE
+-rw-r--r--   0        0        0     5683 2023-06-25 13:39:28.959299 nonebot_plugin_l4d2_server-0.5.7.post1/README.md
+-rw-r--r--   0        0        0    19815 2023-06-25 13:39:28.963299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-25 13:39:28.963299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-25 13:39:28.967299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1714 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1879 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3736 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10990 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8989 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5960 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9672 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    15320 2023-06-25 13:39:28.971299 nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1610 2023-06-25 13:39:28.975299 nonebot_plugin_l4d2_server-0.5.7.post1/pyproject.toml
+-rw-r--r--   0        0        0     7553 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.7.post1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7/LICENSE` & `nonebot_plugin_l4d2_server-0.5.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/README.md` & `nonebot_plugin_l4d2_server-0.5.7.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import a2s
 from typing import List
 
 async def queries(ip:str,port:int):
     port = int(port)
     msg_dict = await queries_dict(ip,port)
-    message += '名称：' + msg_dict['name'] + '\n'
+    print(msg_dict['name'],type(msg_dict['name']))
+    message = f"名称：{msg_dict['name']}\n"
     message += f"地图：{msg_dict['map_']}\n"
     message += f"延迟：{msg_dict['ping']}\n"
     message += f"玩家：{msg_dict['players']} / {msg_dict['max_players']}\n"
     return message
 
 async def queries_dict(ip:str,port:int) -> dict:
     port = int(port)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.7.post1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.7/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.7.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.7"
+version = "0.5.7.post1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.7/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.7.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.7
+Version: 0.5.7.post1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.7 Summary:
-L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.7.post1
+Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

