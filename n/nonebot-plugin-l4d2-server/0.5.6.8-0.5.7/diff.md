# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.6.8.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.7.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.6.8.tar` & `nonebot_plugin_l4d2_server-0.5.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-23 05:19:02.821281 nonebot_plugin_l4d2_server-0.5.6.8/LICENSE
--rw-r--r--   0        0        0     5683 2023-06-23 05:19:02.821281 nonebot_plugin_l4d2_server-0.5.6.8/README.md
--rw-r--r--   0        0        0    19808 2023-06-23 05:19:02.825281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-23 05:19:02.825281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-23 05:19:02.825281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-23 05:19:02.829280 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1879 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10990 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9345 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5875 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    15044 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1606 2023-06-23 05:19:02.833281 nonebot_plugin_l4d2_server-0.5.6.8/pyproject.toml
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 10:10:57.169930 nonebot_plugin_l4d2_server-0.5.7/LICENSE
+-rw-r--r--   0        0        0     5683 2023-06-25 10:10:57.169930 nonebot_plugin_l4d2_server-0.5.7/README.md
+-rw-r--r--   0        0        0    19815 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-25 10:10:57.173930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-25 10:10:57.177930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1714 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1879 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-25 10:10:57.181930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3691 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10990 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8989 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5960 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9672 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    15320 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1604 2023-06-25 10:10:57.185930 nonebot_plugin_l4d2_server-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.7/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/LICENSE` & `nonebot_plugin_l4d2_server-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/README.md` & `nonebot_plugin_l4d2_server-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
 
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
     supported_adapters={"~onebot.v11"},
@@ -292,15 +292,15 @@
     for one_msg in ip:
         if one_msg and one_msg[-1].isdigit():
             break
     if not one_msg:
         await matcher.finish()
     ip_list = split_maohao(one_msg)
     msg = await queries_server(ip_list)
-    await matcher.finish(msg)
+    await str_to_picstr(msg,matcher)
     
 
 @add_queries.handle()
 async def _(matcher:Matcher,event:GroupMessageEvent,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg)==0:
         await matcher.finish('请在该指令后加入参数，例如【114.51.49.19:1810】')
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import a2s
 from typing import List
 
 async def queries(ip:str,port:int):
     port = int(port)
     msg_dict = await queries_dict(ip,port)
-    message = 'ip:' + msg_dict['ip'] + '\n'
     message += '名称：' + msg_dict['name'] + '\n'
     message += f"地图：{msg_dict['map_']}\n"
     message += f"延迟：{msg_dict['ping']}\n"
     message += f"玩家：{msg_dict['players']} / {msg_dict['max_players']}\n"
     return message
 
 async def queries_dict(ip:str,port:int) -> dict:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -135,69 +135,59 @@
             logger.info(f'已加载：{key} | {count}个')
             if key == '云':
                 ANNE_IP = {key:value}
         sleep(1)
     count_ips(ALL_HOST)
     ip_anne_list=[] 
     try:
-        ips = ALL_HOST['云']
-        ip_anne_list = []
-        for one_ip in ips:
-            host,port = split_maohao(one_ip['ip'])
-            ip_anne_list.append((one_ip['id'],host,port))
+        for one_tag in l4_config.l4_zl_tag:
+            ips = ALL_HOST[one_tag]
+            ip_anne_list = []
+            for one_ip in ips:
+                host,port = split_maohao(one_ip['ip'])
+                ip_anne_list.append((one_ip['id'],host,port))
     except KeyError:
         pass
     await get_read_ip(ip_anne_list)
 
         
     @tan_jian.handle()
     async def _(matcher:Matcher,event:MessageEvent):
         msg = await get_tan_jian(ip_anne_list,1)
-        await matcher.finish(msg)  
+        await str_to_picstr(push_msg=msg,matcher=matcher) 
         
     @prison.handle()
     async def _(matcher:Matcher,event:MessageEvent):
         msg = await get_tan_jian(ip_anne_list,2)
-        await matcher.finish(msg)
+        await str_to_picstr(push_msg=msg,matcher=matcher)
 
     @open_prison.handle()
     async def _(matcher:Matcher,event:MessageEvent):
 
         msg = await get_tan_jian(ip_anne_list,3)
-        await matcher.finish(msg)
+        await str_to_picstr(push_msg=msg,matcher=matcher)
         
     
     
 async def get_read_ip(ip_anne_list):    
     get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
     @get_ip.handle()
     async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
-        # global matchers
-        # if get_ip.plugin_name not in matchers:
-        #     matchers[get_ip.plugin_name] = []
-        # matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
         if isinstance(push_msg ,bytes):
             await matcher.finish(MessageSegment.image(push_msg))
         elif msg and isinstance(push_msg ,list):
             await matcher.finish(MessageSegment.image(push_msg[0]) + Message(push_msg[-1]))
         elif msg and isinstance(push_msg ,str):
-            if l4_config.l4_image:
-                lines = push_msg.splitlines()
-                first_str = lines[0]
-                last_str = lines[-1]
-                push_msg = '\n'.join(lines[1:-1])
-                await matcher.finish(mode_txt_to_img(first_str,push_msg)+Message(last_str))
-            else:
-                await matcher.finish(push_msg)
+            await str_to_picstr(push_msg,matcher)
 
 async def get_ip_to_mes(msg:str ,command: str = ''):   
     if not msg:
         # 以图片输出全部当前
         igr = False
         if command in gamemode_list:
             this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
@@ -250,10 +240,10 @@
     global matchers
     # print('启动辣')
     from ..l4d2_update import l4d_restart,l4d_update,get_update_log,driver
     await get_des_ip()
     
    
     
-@driver.on_bot_connect
+@driver.on_startup
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
 class L4d2Config(BaseModel):
     total_enable: bool = Field(True, alias='是否全局启用求生功能')
+    l4_image: bool = Field(False , alias='是否启用图片')
     web_username: str = Field('l4d2', alias='后台管理用户名')
     web_password: str = Field('admin', alias='后台管理密码')
     l4_style: str = Field("standard", alias='图片风格')
-    l4_image: bool = Field(False , alias='是否启用图片')
     l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
         [{
         'id_rank':'1',
         'place': False,
         'location':'C:\\l4d2',
         'host':'127.0.0.1',
         'port':'20715',
@@ -85,14 +85,15 @@
                                 alias='后台管理token密钥')
     l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
     l4_push_interval: int = Field(3, alias='定时任务间隔')
     l4_push_times: int = Field(10, alias='定时任务次数')
+    l4_connect: bool = Field(True, alias="是否在查服命令后加入connect ip")
     group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 
 from nonebot.adapters.onebot.v11 import Bot,MessageEvent,GroupMessageEvent
 from nonebot.log import logger
+from nonebot.matcher import Matcher
 import struct
 import httpx
 import os
 from pathlib import Path
 
 from typing import List,Dict,Union,Optional
 from .txt_to_img import txt_to_img
 from .config import *
 from ..l4d2_anne import write_player,del_player,anne_messgae
 from ..l4d2_server.rcon import read_server_cfg_rcon,rcon_server
 from ..l4d2_queries import queries,player_queries
 from ..l4d2_queries.qqgroup import *
 from ..l4d2_server.workshop import workshop_to_dict
 from ..l4d2_image.steam import url_to_byte
+from .txt_to_img import mode_txt_to_img
 import tempfile
 import random
 
 
 
 async def get_file(url: str, down_file: Path):
     '''
@@ -136,14 +138,15 @@
     """查询ip返回信息"""
     ip = msg[0]
     port = msg[1]
     msgs = ''
     try:
         msgs = await  queries(ip,port)
         msgs += await player_queries(ip,port)
+        msgs += f"connect {ip}:{port}"
     except (struct.error,TimeoutError):
         pass
     # except Exception:
         # msgs = '有无法识别的用户名'
         # return msgs
     return msgs
 
@@ -300,8 +303,25 @@
 async def extract_last_digit(msg: str) -> tuple[str, str]:
     "分离str和数字"
     for i in range(len(msg) - 1, -1, -1):
         if msg[i].isdigit():
             last_digit = msg[i]
             new_msg = msg[:i]
             return new_msg, last_digit
-    return msg, ''
+    return msg, ''
+
+async def str_to_picstr(push_msg:str,matcher:Matcher):
+    """判断图片输出还是正常输出"""
+    if l4_config.l4_image:
+        lines = push_msg.splitlines()
+        first_str = lines[0]
+        last_str = lines[-1]
+        push_msg = '\n'.join(lines[1:-1])
+        if l4_config.l4_connect:
+            await matcher.send(mode_txt_to_img(first_str,push_msg)+last_str)
+        else:
+            await matcher.send(mode_txt_to_img(first_str,push_msg))
+    else:
+        if l4_config.l4_connect:
+            await matcher.send(push_msg)
+        else:
+            await matcher.send('\n'.join(push_msg.splitlines()[1:-1]))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,17 @@
                                      content='机器人返回图片中文字的字体。')),
         Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
                   labelRemark=Remark(shape='circle',
                                      content='仅仅是批量查询的风格')),
         Switch(label='是否优先上传地图', name='l4_only', value='${l4_only}', onText='开启', offText='关闭',
                labelRemark=Remark(shape='circle',
                                   content='开启时，上传地图会保证优先级，从而阻碍其他指令')),
+        Switch(label='是否显示connect', name='l4_connect', value='${l4_connect}', onText='开启', offText='关闭',
+               labelRemark=Remark(shape='circle',
+                                  content='关闭后，查询服务器将不再显示connect和ip地址')),
         InputNumber(label='定时推送间隔（min）', name='l4_push_interval', value='${l4_push_interval}',
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次')),
         InputNumber(label='定时推次数', name='l4_push_times', value='${l4_push_times}',
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，将按照推送间隔时间推送x此')),        
         InputNumber(label='当前路径序号', name='l4_number', value='${l4_number}',
@@ -79,19 +82,19 @@
                                      content='如果选定了路径，则上传地图优先传这个路径')),     
         InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),           
 
-        InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
+        InputTag(label='坐牢三指令tag', name='l4_zl_tag', value='${l4_zl_tag}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
-                                    content='在这里加入的用户，才能上传地图')),
+                                    content='在这里的指令，可以响应坐牢三指令')),
 
     ],
     actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
              Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
 upload_map_form = Form(
```

#### html2text {}

```diff
@@ -37,32 +37,35 @@
 (shape='circle', content='æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã')), Select
 (label='å¾çé£æ ¼', name='l4_style', value='${l4_style}',source='$
 {l4_styles}', labelRemark=Remark(shape='circle',
 content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), Switch
 (label='æ¯å¦ä¼åä¸ä¼ å°å¾', name='l4_only', value='${l4_only}',
 onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
 content='å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤')),
+Switch(label='æ¯å¦æ¾ç¤ºconnect', name='l4_connect', value='${l4_connect}',
+onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
+content='å³é­åï¼æ¥è¯¢æå¡å¨å°ä¸åæ¾ç¤ºconnectåipå°å')),
 InputNumber(label='å®æ¶æ¨éé´éï¼minï¼', name='l4_push_interval',
 value='${l4_push_interval}', labelRemark=Remark(shape='circle',
 content='è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡')),
 InputNumber(label='å®æ¶æ¨æ¬¡æ°', name='l4_push_times', value='$
 {l4_push_times}', labelRemark=Remark(shape='circle',
 content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputNumber
 (label='å½åè·¯å¾åºå·', name='l4_number', value='${l4_number}',
 labelRemark=Remark(shape='circle',
 content='å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾')),
 InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
 {l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
 {total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
 (shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')),
-InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
-{l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
-{total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
-(shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ],
-actions=[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
+InputTag(label='åç¢ä¸æä»¤tag', name='l4_zl_tag', value='${l4_zl_tag}',
+enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
+joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
+content='å¨è¿éçæä»¤ï¼å¯ä»¥ååºåç¢ä¸æä»¤')), ], actions=
+[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
 Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
 l4d2_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
 value='${web_username}', labelRemark=Remark(shape='circle',
 content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
 value='${web_password}', labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.6.8"
+version = "0.5.7"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.8/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.6.8
+Version: 0.5.7
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
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.6.8
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.7 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

