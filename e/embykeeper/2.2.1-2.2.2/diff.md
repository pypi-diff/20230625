# Comparing `tmp/embykeeper-2.2.1.tar.gz` & `tmp/embykeeper-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.1.tar", last modified: Thu Jun 15 16:44:48 2023, max compression
+gzip compressed data, was "embykeeper-2.2.2.tar", last modified: Sun Jun 25 17:04:45 2023, max compression
```

## Comparing `embykeeper-2.2.1.tar` & `embykeeper-2.2.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.196441 embykeeper-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 16:44:35.000000 embykeeper-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 16:44:35.000000 embykeeper-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-15 16:44:48.196441 embykeeper-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-06-15 16:44:35.000000 embykeeper-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.180441 embykeeper-2.2.1/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.188441 embykeeper-2.2.1/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:47.000000 embykeeper-2.2.1/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/cascadia-code.css
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 16:44:35.000000 embykeeper-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:44:48.196441 embykeeper-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-15 16:44:35.000000 embykeeper-2.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 17:04:33.000000 embykeeper-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 17:04:33.000000 embykeeper-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21662 2023-06-25 17:04:45.197747 embykeeper-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-06-25 17:04:33.000000 embykeeper-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.189747 embykeeper-2.2.2/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.189747 embykeeper-2.2.2/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21662 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:04:44.000000 embykeeper-2.2.2/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/cascadia-code.css
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-25 17:04:33.000000 embykeeper-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:04:45.197747 embykeeper-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-25 17:04:33.000000 embykeeper-2.2.2/tests/test_cli.py
```

### Comparing `embykeeper-2.2.1/LICENSE` & `embykeeper-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/PKG-INFO` & `embykeeper-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.1
+Version: 2.2.2
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -82,15 +83,15 @@
 
 ## 安装与使用
 
 ### Railway 在线部署
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.1 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.2 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
-:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
-status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
-embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
-v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
-//img.shields.io/pypi/dm/
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Console Classifier: Environment :: Web Environment Classifier: Intended
+Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
+(Simplified) Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE [![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -88,15 +89,17 @@
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
 å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
-WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
+embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
+embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
```

### Comparing `embykeeper-2.2.1/README.md` & `embykeeper-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## 安装与使用
 
 ### Railway 在线部署
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
```

#### html2text {}

```diff
@@ -77,15 +77,17 @@
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
 å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
-WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
+embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
+embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
```

### Comparing `embykeeper-2.2.1/embykeeper/cli.py` & `embykeeper-2.2.2/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/data.py` & `embykeeper-2.2.2/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.2/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/embywatcher/main.py` & `embykeeper-2.2.2/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/log.py` & `embykeeper-2.2.2/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/settings.py` & `embykeeper-2.2.2/embykeeper/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         if len(embies) > 0:
             logger.info(f"您当前填写了 {len(embies)} 个 Emby 账号信息.")
             more = Confirm.ask(pad + "是否继续添加?", default=False)
         else:
             more = Confirm.ask(pad + "是否添加 Emby 账号?", default=True)
         if not more:
             break
-        url = Prompt.ask(pad + "请输入您的 Emby 站点 URL <协议://域名:端口> [dark_green](https://abc.com:443)[/]")
+        url = Prompt.ask(pad + "请输入您的 Emby 站点 URL [dark_green](https://abc.com:443)[/]")
         username = Prompt.ask(pad + "请输入您在该 Emby 站点的用户名")
         password = Prompt.ask(pad + "请输入您在该 Emby 站点的密码 (不显示, 按回车确认)", password=True)
         time = IntPrompt.ask(pad + "设置模拟观看时长 (秒)", default=10, show_default=True)
         progress = IntPrompt.ask(pad + "设置模拟观看后进度条位置 (秒)", default=1000, show_default=True)
         embies.append(
             {"url": url, "username": username, "password": password, "progress": progress, "time": time}
         )
```

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.2/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/link.py` & `embykeeper-2.2.2/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/log.py` & `embykeeper-2.2.2/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/main.py` & `embykeeper-2.2.2/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.2/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.2/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.2/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/telechecker/tele.py` & `embykeeper-2.2.2/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper/utils.py` & `embykeeper-2.2.2/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.2/embykeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.1
+Version: 2.2.2
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -82,15 +83,15 @@
 
 ## 安装与使用
 
 ### Railway 在线部署
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.1 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.2 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
-:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
-status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
-embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
-v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
-//img.shields.io/pypi/dm/
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Console Classifier: Environment :: Web Environment Classifier: Intended
+Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
+(Simplified) Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE [![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -88,15 +89,17 @@
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
 å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
-WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
+embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
+embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
```

### Comparing `embykeeper-2.2.1/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.2/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/app.py` & `embykeeper-2.2.2/embykeeperweb/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import pty
 import select
 import fcntl
 import struct
 import subprocess
 import termios
 import time
+import signal
 
 import typer
 from loguru import logger
 from flask import Flask, render_template, request, redirect, url_for
 from flask_socketio import SocketIO
 from flask_login import LoginManager, login_user, login_required
 
-from embykeeper import settings
-
 cli = typer.Typer()
 app = Flask(__name__, static_folder="templates/assets")
 app.config["SECRET_KEY"] = os.urandom(24)
 socketio = SocketIO(app)
 login_manager = LoginManager()
 login_manager.init_app(app)
 login_manager.login_view = "login"
@@ -114,15 +113,15 @@
             (data, _, _) = select.select([app.config["fd"]], [], [], 0)
             if data:
                 output = os.read(app.config["fd"], max_read_bytes).decode(errors="ignore")
                 app.config["hist"] += output
                 socketio.emit("pty-output", {"output": output}, namespace="/pty")
 
 
-@socketio.on("embykeeper", namespace="/pty")
+@socketio.on("embykeeper_start", namespace="/pty")
 def start(data):
     if app.config["fd"]:
         set_size(app.config["fd"], data["rows"], data["cols"])
         socketio.emit("pty-output", {"output": app.config["hist"]}, namespace="/pty")
     else:
         (pid, fd) = pty.fork()
         if pid == 0:
@@ -131,14 +130,33 @@
             app.config["fd"] = fd
             app.config["pid"] = pid
             logger.debug(f"Embykeeper started at: {pid}.")
             set_size(app.config["fd"], data["rows"], data["cols"])
             socketio.start_background_task(target=read_and_forward_pty_output)
 
 
+@socketio.on("embykeeper_kill", namespace="/pty")
+def stop():
+    if app.config["pid"] is not None:
+        os.kill(app.config["pid"], signal.SIGINT)
+        for _ in range(50):
+            try:
+                os.kill(app.config["pid"], 0)
+            except OSError:
+                break
+            else:
+                time.sleep(0.1)
+        else:
+            os.kill(app.config["pid"], signal.SIGKILL)
+        app.config["fd"] = None
+        app.config["pid"] = None
+        app.config["hist"] = ""
+        logger.debug(f"Embykeeper stopped.")
+
+
 @cli.command(context_settings={"ignore_unknown_options": True, "allow_extra_args": True})
 def run(ctx: typer.Context, port: int = 1818, host: str = "0.0.0.0", debug: bool = False):
     app.config["args"] = ctx.args
     logger.info(f"Embykeeper webserver started at {host}:{port}.")
     socketio.run(app, port=port, host=host, debug=debug)
```

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/404.html` & `embykeeper-2.2.2/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.2/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.2/embykeeperweb/templates/assets/js/console.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -25,35 +25,54 @@
     term.loadAddon(fit);
     term.loadAddon(new SearchAddon.SearchAddon());
 
     term.open(document.getElementById("terminal"));
     fit.fit();
     console.debug("Web console init: ", term.cols, term.rows);
 
-    const socket = io.connect("/pty");
+    const socket = io.connect("/pty", {
+        'reconnection': true,
+        'reconnectionDelay': 1000
+    });
     socket.on("connect", () => {
         var statusIcon = document.getElementById("status-icon");
         statusIcon.style.backgroundColor = "green";
         var statusMsg = document.getElementById("status-msg");
-        statusMsg.textContent = "Program Connected"
+        statusMsg.textContent = "Program Connected";
+        var restartIcon = document.getElementById("restart-icon");
+        restartIcon.style.animationPlayState = "paused";
         console.info("Web console connected: ", term.cols, term.rows);
-        term.focus()
-        term.clear()
+        term.focus();
+        term.clear();
+        term.reset();
         const dims = {
             cols: term.cols,
             rows: term.rows
         };
-        socket.emit("embykeeper", dims);
+        socket.emit("embykeeper_start", dims);
     });
 
     socket.on("disconnect", () => {
         var statusIcon = document.getElementById("status-icon");
         statusIcon.style.backgroundColor = "red";
         var statusMsg = document.getElementById("status-msg");
-        statusMsg.textContent = "Program Disconnected"
+        statusMsg.textContent = "Program Disconnected";
+        var restartIcon = document.getElementById("restart-icon");
+        restartIcon.style.animationPlayState = "running";
+        console.info("Web console disconnected.");
+    });
+
+    var restartBtn = document.getElementById("restart-btn");
+    restartBtn.addEventListener('click', () => {
+        socket.emit("embykeeper_kill");
+        socket.disconnect();
+        var statusMsg = document.getElementById("status-msg");
+        statusMsg.textContent = "Program Restarting"
+        console.info("Web console restarting.");
+        socket.open();
     });
 
     function resize() {
         fit.fit();
         console.debug("Web console resize: ", term.cols, term.rows);
         const dims = {
             cols: term.cols,
```

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.2/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/console.html` & `embykeeper-2.2.2/embykeeperweb/templates/login.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,95 +3,93 @@
 
 <head>
     <meta charset="utf-8">
 <meta name="robots" content="noindex, nofollow">
 <meta name="googlebot" content="noindex, nofollow">
 <meta name="baiduspider" content="noindex, nofollow">
     <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
-    <title>Embykeeper</title>
+    <title>Log in - Embykeeper</title>
     <meta name="description" content="Embykeeper: 中文社群规则下用于 Emby 影视服务器签到和保号的自动执行工具">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="stylesheet" href="assets/bootstrap/css/bootstrap.min.css">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800&amp;display=swap">
     <link rel="stylesheet" href="assets/css/cascadia-code.css">
     <link rel="stylesheet" href="assets/css/icons.css">
     <link rel="stylesheet" href="assets/css/styles.css">
-    <link rel="stylesheet" href="https://unpkg.com/xterm@5.2.1/css/xterm.css">
 </head>
 
 <body>
     <nav class="navbar navbar-light navbar-expand-md fixed-top navbar-shrink py-3" id="mainNav">
         <div class="container"><a class="navbar-brand d-flex align-items-center" href="/"><span>Embykeeper</span></a><button data-bs-toggle="collapse" class="navbar-toggler" data-bs-target="#navcol-1"><span class="visually-hidden">Toggle navigation</span><span class="navbar-toggler-icon"></span></button>
             <div class="collapse navbar-collapse" id="navcol-1">
                 <ul class="navbar-nav mx-auto"></ul>
                 <a class="btn btn-primary shadow" role="button" href="/console">Web Console</a>
             </div>
         </div>
     </nav>
-    <section class="py-5 mt-5">
-        <div class="container">
+    <section class="py-4 py-md-5 my-5">
+        <div class="container py-md-5">
             <div class="row">
-                <div class="col-12 mx-auto">
-                    <div class="d-inline-flex reccircle bg-light my-2 px-3 align-items-center">
-                        <div id="status-icon" class="small-dot" style="border-radius: 50%;"></div>
-                        <div class="text-center">
-                            <p class="fw-semibold my-0 ms-2" id="status-msg">Console Connecting</p>
-                        </div>
-                    </div>
-                    <div></div>
-                    <div class="card" style="border-radius: 5px;height: 65vh;">
-                        <div class="card-body">
-                            <div id="terminal" class="h-100"></div>
+                <div class="col-md-6 text-center"><img class="img-fluid w-100" src="assets/img/illustrations/login.svg"></div>
+                <div class="col-md-5 text-center text-md-start">
+                    <h2 class="display-6 fw-bold mb-5 mt-md-4 mt-lg-5"><span class="underline pb-1"><strong>Login</strong><br></span></h2>
+                    {% if emsg %}
+                        <div class="card mb-3 shadow">
+                            <div class="card-body d-flex align-items-center py-2"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-exclamation-triangle-fill text-danger">
+                                    <path d="M8.982 1.566a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566zM8 5c.535 0 .954.462.9.995l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995A.905.905 0 0 1 8 5zm.002 6a1 1 0 1 1 0 2 1 1 0 0 1 0-2z"></path>
+                                </svg>
+                                <p class="d-inline-block ms-3 my-0">{{ emsg }}</p>
+                            </div>
                         </div>
-                    </div>
+                    {% endif %}
+                    <form method="post">
+                        <div class="mb-3"><input class="shadow form-control" type="password" name="password" placeholder="Password"></div>
+                        <div class="mb-5"><button class="btn btn-primary shadow" type="submit">Log in</button></div>
+                        <p class="text-muted"><a href="https://github.com/embykeeper/embykeeper#%E5%9C%A8%E7%BA%BF%E9%83%A8%E7%BD%B2">What is web console password?</a></p>
+                    </form>
                 </div>
             </div>
         </div>
     </section>
     <footer class="text-center py-4">
         <div class="container">
             <div class="row row-cols-1 row-cols-lg-3">
                 <div class="col">
                     <p class="text-muted my-2">Copyright&nbsp;© 2023 Embykeeper</p>
                 </div>
                 <div class="col">
                     <ul class="list-inline my-2">
-                        <li class="list-inline-item me-4"><a href="https://github.com/embykeeper/embykeeper" target="_blank" rel="noopener noreferrer">
-                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-github">
-                                        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
-                                    </svg></div>
-                            </a></li>
-                        <li class="list-inline-item me-4"><a href="https://t.me/embykeeper_bot" target="_blank" rel="noopener noreferrer">
-                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-telegram">
-                                        <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.287 5.906c-.778.324-2.334.994-4.666 2.01-.378.15-.577.298-.595.442-.03.243.275.339.69.47l.175.055c.408.133.958.288 1.243.294.26.006.549-.1.868-.32 2.179-1.471 3.304-2.214 3.374-2.23.05-.012.12-.026.166.016.047.041.042.12.037.141-.03.129-1.227 1.241-1.846 1.817-.193.18-.33.307-.358.336a8.154 8.154 0 0 1-.188.186c-.38.366-.664.64.015 1.088.327.216.589.393.85.571.284.194.568.387.936.629.093.06.183.125.27.187.331.236.63.448.997.414.214-.02.435-.22.547-.82.265-1.417.786-4.486.906-5.751a1.426 1.426 0 0 0-.013-.315.337.337 0 0 0-.114-.217.526.526 0 0 0-.31-.093c-.3.005-.763.166-2.984 1.09z"></path>
-                                    </svg></div>
-                            </a></li>
-                        <li class="list-inline-item"><a href="https://afdian.net/a/jackzzs" target="_blank" rel="noopener noreferrer">
-                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-heart-fill">
-                                        <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z"></path>
-                                    </svg></div>
-                            </a></li>
+                        <li class="list-inline-item me-4">
+                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-github">
+                                    <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
+                                </svg></div>
+                        </li>
+                        <li class="list-inline-item me-4">
+                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-telegram">
+                                    <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.287 5.906c-.778.324-2.334.994-4.666 2.01-.378.15-.577.298-.595.442-.03.243.275.339.69.47l.175.055c.408.133.958.288 1.243.294.26.006.549-.1.868-.32 2.179-1.471 3.304-2.214 3.374-2.23.05-.012.12-.026.166.016.047.041.042.12.037.141-.03.129-1.227 1.241-1.846 1.817-.193.18-.33.307-.358.336a8.154 8.154 0 0 1-.188.186c-.38.366-.664.64.015 1.088.327.216.589.393.85.571.284.194.568.387.936.629.093.06.183.125.27.187.331.236.63.448.997.414.214-.02.435-.22.547-.82.265-1.417.786-4.486.906-5.751a1.426 1.426 0 0 0-.013-.315.337.337 0 0 0-.114-.217.526.526 0 0 0-.31-.093c-.3.005-.763.166-2.984 1.09z"></path>
+                                </svg></div>
+                        </li>
+                        <li class="list-inline-item">
+                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-heart-fill">
+                                    <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z"></path>
+                                </svg></div>
+                        </li>
                     </ul>
                 </div>
                 <div class="col">
                     <ul class="list-inline my-2">
-                        <li class="list-inline-item"><a class="link-primary" href="https://github.com/embykeeper/embykeeper/blob/main/LICENSE">License</a></li>
-                        <li class="list-inline-item"><a class="link-primary" href="https://github.com/embykeeper/embykeeper#%E5%A3%B0%E6%98%8E">Terms of Use</a></li>
+                        <li class="list-inline-item"><a class="link-primary" href="#">License</a></li>
+                        <li class="list-inline-item"><a class="link-primary" href="#">Terms of Use</a></li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
     <script src="assets/bootstrap/js/bootstrap.min.js"></script>
     <script src="assets/js/script.js"></script>
-    <script src="https://unpkg.com/xterm@5.2.1/lib/xterm.js"></script>
-    <script src="https://unpkg.com/xterm-addon-fit@0.7.0/lib/xterm-addon-fit.js"></script>
-    <script src="https://unpkg.com/xterm-addon-search@0.12.0/lib/xterm-addon-search.js"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.6.2/socket.io.min.js"></script>
-    <script src="assets/js/console.js"></script>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -8,16 +8,24 @@
 
 
 
 
 
 
 
-
 EmbykeeperToggle navigation
 Web_Console
 
-Console Connecting
+[assets/img/illustrations/login.svg]
+***** Login
+ *****
+{% if emsg %}
+
+{{ emsg }}
+{% endif %}
+[********************]
+Log in
+What_is_web_console_password?
 
 Copyright Â© 2023 Embykeeper
     * License
     * Terms_of_Use
```

### Comparing `embykeeper-2.2.1/embykeeperweb/templates/login.html` & `embykeeper-2.2.2/embykeeperweb/templates/console.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,93 +3,104 @@
 
 <head>
     <meta charset="utf-8">
 <meta name="robots" content="noindex, nofollow">
 <meta name="googlebot" content="noindex, nofollow">
 <meta name="baiduspider" content="noindex, nofollow">
     <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
-    <title>Log in - Embykeeper</title>
+    <title>Embykeeper</title>
     <meta name="description" content="Embykeeper: 中文社群规则下用于 Emby 影视服务器签到和保号的自动执行工具">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="stylesheet" href="assets/bootstrap/css/bootstrap.min.css">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800&amp;display=swap">
     <link rel="stylesheet" href="assets/css/cascadia-code.css">
     <link rel="stylesheet" href="assets/css/icons.css">
     <link rel="stylesheet" href="assets/css/styles.css">
+    <link rel="stylesheet" href="https://unpkg.com/xterm@5.2.1/css/xterm.css">
 </head>
 
 <body>
     <nav class="navbar navbar-light navbar-expand-md fixed-top navbar-shrink py-3" id="mainNav">
         <div class="container"><a class="navbar-brand d-flex align-items-center" href="/"><span>Embykeeper</span></a><button data-bs-toggle="collapse" class="navbar-toggler" data-bs-target="#navcol-1"><span class="visually-hidden">Toggle navigation</span><span class="navbar-toggler-icon"></span></button>
             <div class="collapse navbar-collapse" id="navcol-1">
                 <ul class="navbar-nav mx-auto"></ul>
                 <a class="btn btn-primary shadow" role="button" href="/console">Web Console</a>
             </div>
         </div>
     </nav>
-    <section class="py-4 py-md-5 my-5">
-        <div class="container py-md-5">
+    <section class="py-5 mt-5">
+        <div class="container">
             <div class="row">
-                <div class="col-md-6 text-center"><img class="img-fluid w-100" src="assets/img/illustrations/login.svg"></div>
-                <div class="col-md-5 text-center text-md-start">
-                    <h2 class="display-6 fw-bold mb-5 mt-md-4 mt-lg-5"><span class="underline pb-1"><strong>Login</strong><br></span></h2>
-                    {% if emsg %}
-                        <div class="card mb-3 shadow">
-                            <div class="card-body d-flex align-items-center py-2"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-exclamation-triangle-fill text-danger">
-                                    <path d="M8.982 1.566a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566zM8 5c.535 0 .954.462.9.995l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995A.905.905 0 0 1 8 5zm.002 6a1 1 0 1 1 0 2 1 1 0 0 1 0-2z"></path>
-                                </svg>
-                                <p class="d-inline-block ms-3 my-0">{{ emsg }}</p>
-                            </div>
+                <div class="col-10 mx-auto">
+                    <div class="d-inline-flex reccircle bg-light my-2 px-3 align-items-center">
+                        <div id="status-icon" class="small-dot" style="border-radius: 50%;"></div>
+                        <div class="text-center">
+                            <p class="fw-semibold my-0 ms-2" id="status-msg">Program Connecting</p>
+                        </div>
+                    </div>
+                </div>
+                <div class="col d-flex d-lg-flex justify-content-end" id="restart-btn">
+                    <div class="bs-icon-circle bs-icon my-2 bg-light"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-arrow-repeat" id="restart-icon">
+                            <path d="M11.534 7h3.932a.25.25 0 0 1 .192.41l-1.966 2.36a.25.25 0 0 1-.384 0l-1.966-2.36a.25.25 0 0 1 .192-.41zm-11 2h3.932a.25.25 0 0 0 .192-.41L2.692 6.23a.25.25 0 0 0-.384 0L.342 8.59A.25.25 0 0 0 .534 9z"></path>
+                            <path fill-rule="evenodd" d="M8 3c-1.552 0-2.94.707-3.857 1.818a.5.5 0 1 1-.771-.636A6.002 6.002 0 0 1 13.917 7H12.9A5.002 5.002 0 0 0 8 3zM3.1 9a5.002 5.002 0 0 0 8.757 2.182.5.5 0 1 1 .771.636A6.002 6.002 0 0 1 2.083 9H3.1z"></path>
+                        </svg></div>
+                </div>
+            </div>
+            <div class="row">
+                <div class="col">
+                    <div class="card" style="border-radius: 5px;height: 65vh;">
+                        <div class="card-body">
+                            <div id="terminal" class="h-100"></div>
                         </div>
-                    {% endif %}
-                    <form method="post">
-                        <div class="mb-3"><input class="shadow form-control" type="password" name="password" placeholder="Password"></div>
-                        <div class="mb-5"><button class="btn btn-primary shadow" type="submit">Log in</button></div>
-                        <p class="text-muted"><a href="https://github.com/embykeeper/embykeeper#%E5%9C%A8%E7%BA%BF%E9%83%A8%E7%BD%B2">What is web console password?</a></p>
-                    </form>
+                    </div>
                 </div>
             </div>
         </div>
     </section>
     <footer class="text-center py-4">
         <div class="container">
             <div class="row row-cols-1 row-cols-lg-3">
                 <div class="col">
                     <p class="text-muted my-2">Copyright&nbsp;© 2023 Embykeeper</p>
                 </div>
                 <div class="col">
                     <ul class="list-inline my-2">
-                        <li class="list-inline-item me-4">
-                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-github">
-                                    <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
-                                </svg></div>
-                        </li>
-                        <li class="list-inline-item me-4">
-                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-telegram">
-                                    <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.287 5.906c-.778.324-2.334.994-4.666 2.01-.378.15-.577.298-.595.442-.03.243.275.339.69.47l.175.055c.408.133.958.288 1.243.294.26.006.549-.1.868-.32 2.179-1.471 3.304-2.214 3.374-2.23.05-.012.12-.026.166.016.047.041.042.12.037.141-.03.129-1.227 1.241-1.846 1.817-.193.18-.33.307-.358.336a8.154 8.154 0 0 1-.188.186c-.38.366-.664.64.015 1.088.327.216.589.393.85.571.284.194.568.387.936.629.093.06.183.125.27.187.331.236.63.448.997.414.214-.02.435-.22.547-.82.265-1.417.786-4.486.906-5.751a1.426 1.426 0 0 0-.013-.315.337.337 0 0 0-.114-.217.526.526 0 0 0-.31-.093c-.3.005-.763.166-2.984 1.09z"></path>
-                                </svg></div>
-                        </li>
-                        <li class="list-inline-item">
-                            <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-heart-fill">
-                                    <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z"></path>
-                                </svg></div>
-                        </li>
+                        <li class="list-inline-item me-4"><a href="https://github.com/embykeeper/embykeeper" target="_blank" rel="noopener noreferrer">
+                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-github">
+                                        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
+                                    </svg></div>
+                            </a></li>
+                        <li class="list-inline-item me-4"><a href="https://t.me/embykeeper_bot" target="_blank" rel="noopener noreferrer">
+                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-telegram">
+                                        <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.287 5.906c-.778.324-2.334.994-4.666 2.01-.378.15-.577.298-.595.442-.03.243.275.339.69.47l.175.055c.408.133.958.288 1.243.294.26.006.549-.1.868-.32 2.179-1.471 3.304-2.214 3.374-2.23.05-.012.12-.026.166.016.047.041.042.12.037.141-.03.129-1.227 1.241-1.846 1.817-.193.18-.33.307-.358.336a8.154 8.154 0 0 1-.188.186c-.38.366-.664.64.015 1.088.327.216.589.393.85.571.284.194.568.387.936.629.093.06.183.125.27.187.331.236.63.448.997.414.214-.02.435-.22.547-.82.265-1.417.786-4.486.906-5.751a1.426 1.426 0 0 0-.013-.315.337.337 0 0 0-.114-.217.526.526 0 0 0-.31-.093c-.3.005-.763.166-2.984 1.09z"></path>
+                                    </svg></div>
+                            </a></li>
+                        <li class="list-inline-item"><a href="https://afdian.net/a/jackzzs" target="_blank" rel="noopener noreferrer">
+                                <div class="bs-icon-circle bs-icon-primary bs-icon"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="currentColor" viewBox="0 0 16 16" class="bi bi-heart-fill">
+                                        <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z"></path>
+                                    </svg></div>
+                            </a></li>
                     </ul>
                 </div>
                 <div class="col">
                     <ul class="list-inline my-2">
-                        <li class="list-inline-item"><a class="link-primary" href="#">License</a></li>
-                        <li class="list-inline-item"><a class="link-primary" href="#">Terms of Use</a></li>
+                        <li class="list-inline-item"><a class="link-primary" href="https://github.com/embykeeper/embykeeper/blob/main/LICENSE">License</a></li>
+                        <li class="list-inline-item"><a class="link-primary" href="https://github.com/embykeeper/embykeeper#%E5%A3%B0%E6%98%8E">Terms of Use</a></li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
     <script src="assets/bootstrap/js/bootstrap.min.js"></script>
     <script src="assets/js/script.js"></script>
+    <script src="https://unpkg.com/xterm@5.2.1/lib/xterm.js"></script>
+    <script src="https://unpkg.com/xterm-addon-fit@0.7.0/lib/xterm-addon-fit.js"></script>
+    <script src="https://unpkg.com/xterm-addon-search@0.12.0/lib/xterm-addon-search.js"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.6.2/socket.io.min.js"></script>
+    <script src="assets/js/console.js"></script>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -8,24 +8,17 @@
 
 
 
 
 
 
 
+
 EmbykeeperToggle navigation
 Web_Console
 
-[assets/img/illustrations/login.svg]
-***** Login
- *****
-{% if emsg %}
-
-{{ emsg }}
-{% endif %}
-[********************]
-Log in
-What_is_web_console_password?
+Program Connecting
+
 
 Copyright Â© 2023 Embykeeper
     * License
     * Terms_of_Use
```

### Comparing `embykeeper-2.2.1/pyproject.toml` & `embykeeper-2.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
     "checkin",
     "automator",
     "bot",
     "telegram bot",
     "keep active",
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
+    "Environment :: Web Environment",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: Chinese (Simplified)",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `embykeeper-2.2.1/tests/test_cli.py` & `embykeeper-2.2.2/tests/test_cli.py`

 * *Files identical despite different names*

