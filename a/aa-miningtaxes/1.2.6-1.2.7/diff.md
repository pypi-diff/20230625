# Comparing `tmp/aa-miningtaxes-1.2.6.tar.gz` & `tmp/aa-miningtaxes-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-miningtaxes-1.2.6.tar", last modified: Mon Jun 19 16:38:26 2023, max compression
+gzip compressed data, was "aa-miningtaxes-1.2.7.tar", last modified: Sun Jun 25 02:35:13 2023, max compression
```

## Comparing `aa-miningtaxes-1.2.6.tar` & `aa-miningtaxes-1.2.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.355351 aa-miningtaxes-1.2.6/
--rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7451 2023-06-19 16:38:26.356351 aa-miningtaxes-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5740 2023-02-21 19:42:26.000000 aa-miningtaxes-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.347351 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7451 2023-06-19 16:38:26.000000 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2941 2023-06-19 16:38:26.000000 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:38:26.000000 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-19 16:38:26.000000 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-19 16:38:26.000000 aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.349351 aa-miningtaxes-1.2.6/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-19 16:38:21.000000 aa-miningtaxes-1.2.6/miningtaxes/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/miningtaxes/admin.py
--rw-r--r--   0 root         (0) root         (0)     1582 2023-02-21 19:10:53.000000 aa-miningtaxes-1.2.6/miningtaxes/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.2.6/miningtaxes/apps.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.2.6/miningtaxes/auth_hooks.py
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.2.6/miningtaxes/decorators.py
--rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.2.6/miningtaxes/forms.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-06-19 16:38:11.000000 aa-miningtaxes-1.2.6/miningtaxes/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.345351 aa-miningtaxes-1.2.6/miningtaxes/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.350351 aa-miningtaxes-1.2.6/miningtaxes/management/commands/
--rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.2.6/miningtaxes/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-01-08 17:44:15.000000 aa-miningtaxes-1.2.6/miningtaxes/management/commands/miningtaxes_preload_prices.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-04 18:04:31.000000 aa-miningtaxes-1.2.6/miningtaxes/management/commands/miningtaxes_update_manual.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.2.6/miningtaxes/management/commands/miningtaxes_zero_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.351351 aa-miningtaxes-1.2.6/miningtaxes/migrations/
--rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0002_all_models.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0003_alter_general_options.py
--rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0009_stats.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.2.6/miningtaxes/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.352351 aa-miningtaxes-1.2.6/miningtaxes/models/
--rw-r--r--   0 root         (0) root         (0)      438 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7115 2023-06-19 16:18:31.000000 aa-miningtaxes-1.2.6/miningtaxes/models/admin.py
--rw-r--r--   0 root         (0) root         (0)    18238 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/models/character.py
--rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.2.6/miningtaxes/models/general.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-02-21 19:11:09.000000 aa-miningtaxes-1.2.6/miningtaxes/models/orePrices.py
--rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.6/miningtaxes/models/settings.py
--rw-r--r--   0 root         (0) root         (0)    24599 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/models/stats.py
--rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.2.6/miningtaxes/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.345351 aa-miningtaxes-1.2.6/miningtaxes/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.345351 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.352351 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/
--rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/billboards_dark.css
--rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/billboards_light.css
--rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/global.css
--rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/launcher.css
--rw-r--r--   0 root         (0) root         (0)     1555 2023-01-20 16:20:09.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/miningtaxes.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.353351 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/
--rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq1.png
--rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq2.png
--rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq3.png
--rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.2.6/miningtaxes/swagger.json
--rw-r--r--   0 root         (0) root         (0)    13269 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.345351 aa-miningtaxes-1.2.6/miningtaxes/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.354351 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)     6817 2023-04-06 01:58:02.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/admin_launcher.html
--rw-r--r--   0 root         (0) root         (0)    20648 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/admin_tables.html
--rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/base.html
--rw-r--r--   0 root         (0) root         (0)     2755 2023-01-08 18:57:41.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/character_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1740 2022-11-21 01:21:27.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/faq.html
--rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/index.html
--rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/launcher.html
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/ore_prices.html
--rw-r--r--   0 root         (0) root         (0)    11159 2023-02-21 19:12:52.000000 aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/user_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.354351 aa-miningtaxes-1.2.6/miningtaxes/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.354351 aa-miningtaxes-1.2.6/miningtaxes/tests/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_admin_character.py
--rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_character.py
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_orePrice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.355351 aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/
--rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/esi_client_stub.py
--rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/load_entities.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/load_eveuniverse.py
--rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.2.6/miningtaxes/tests/utils.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/urls.py
--rw-r--r--   0 root         (0) root         (0)    20830 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.6/miningtaxes/views.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-19 16:38:26.356351 aa-miningtaxes-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:38:26.355351 aa-miningtaxes-1.2.6/testauth/
--rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/testauth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.2.6/testauth/settingsAA2.py
--rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.2.6/testauth/settingsAA3.py
--rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/testauth/urls.py
--rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.6/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.706298 aa-miningtaxes-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-06-25 02:35:13.706298 aa-miningtaxes-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-24 15:56:29.000000 aa-miningtaxes-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.697298 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-06-25 02:35:13.000000 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-06-25 02:35:13.000000 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 02:35:13.000000 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-25 02:35:13.000000 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-25 02:35:13.000000 aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.699298 aa-miningtaxes-1.2.7/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-25 02:33:08.000000 aa-miningtaxes-1.2.7/miningtaxes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/miningtaxes/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-24 15:56:21.000000 aa-miningtaxes-1.2.7/miningtaxes/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.2.7/miningtaxes/apps.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.2.7/miningtaxes/auth_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.2.7/miningtaxes/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.2.7/miningtaxes/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-06-25 02:35:02.000000 aa-miningtaxes-1.2.7/miningtaxes/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.695298 aa-miningtaxes-1.2.7/miningtaxes/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.700298 aa-miningtaxes-1.2.7/miningtaxes/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.2.7/miningtaxes/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-01-08 17:44:15.000000 aa-miningtaxes-1.2.7/miningtaxes/management/commands/miningtaxes_preload_prices.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-04 18:04:31.000000 aa-miningtaxes-1.2.7/miningtaxes/management/commands/miningtaxes_update_manual.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.2.7/miningtaxes/management/commands/miningtaxes_zero_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.701298 aa-miningtaxes-1.2.7/miningtaxes/migrations/
+-rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0002_all_models.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0003_alter_general_options.py
+-rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
+-rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0009_stats.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.2.7/miningtaxes/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.702298 aa-miningtaxes-1.2.7/miningtaxes/models/
+-rw-r--r--   0 root         (0) root         (0)      438 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2023-06-19 19:07:48.000000 aa-miningtaxes-1.2.7/miningtaxes/models/admin.py
+-rw-r--r--   0 root         (0) root         (0)    18238 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/models/character.py
+-rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.2.7/miningtaxes/models/general.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2023-06-25 02:35:02.000000 aa-miningtaxes-1.2.7/miningtaxes/models/orePrices.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.7/miningtaxes/models/settings.py
+-rw-r--r--   0 root         (0) root         (0)    24599 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/models/stats.py
+-rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.2.7/miningtaxes/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.695298 aa-miningtaxes-1.2.7/miningtaxes/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.695298 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.702298 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/
+-rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/billboards_dark.css
+-rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/billboards_light.css
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/global.css
+-rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/launcher.css
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-01-20 16:20:09.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/miningtaxes.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.703298 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/
+-rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq1.png
+-rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq2.png
+-rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq3.png
+-rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.2.7/miningtaxes/swagger.json
+-rw-r--r--   0 root         (0) root         (0)    13877 2023-06-25 02:35:02.000000 aa-miningtaxes-1.2.7/miningtaxes/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.695298 aa-miningtaxes-1.2.7/miningtaxes/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.704298 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-04-06 01:58:02.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/admin_launcher.html
+-rw-r--r--   0 root         (0) root         (0)    20648 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/admin_tables.html
+-rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/base.html
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-01-08 18:57:41.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/character_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-25 02:32:57.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/faq.html
+-rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/index.html
+-rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/launcher.html
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/ore_prices.html
+-rw-r--r--   0 root         (0) root         (0)    11159 2023-02-21 19:12:52.000000 aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/user_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.704298 aa-miningtaxes-1.2.7/miningtaxes/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.705298 aa-miningtaxes-1.2.7/miningtaxes/tests/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_admin_character.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_orePrice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.705298 aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/esi_client_stub.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/load_entities.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.2.7/miningtaxes/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.7/miningtaxes/urls.py
+-rw-r--r--   0 root         (0) root         (0)    20987 2023-06-25 02:31:46.000000 aa-miningtaxes-1.2.7/miningtaxes/views.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-25 02:35:13.706298 aa-miningtaxes-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 02:35:13.706298 aa-miningtaxes-1.2.7/testauth/
+-rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/testauth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/testauth/celery.py
+-rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.2.7/testauth/settingsAA2.py
+-rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.2.7/testauth/settingsAA3.py
+-rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/testauth/urls.py
+-rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.7/testauth/wsgi.py
```

### Comparing `aa-miningtaxes-1.2.6/LICENSE` & `aa-miningtaxes-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/PKG-INFO` & `aa-miningtaxes-1.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
         
@@ -83,18 +83,18 @@
         
         Name | Description | Default
         -- | -- | --
         MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
         MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
         MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
         MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
+        MININGTAXES_ALWAYS_TAX_REFINED | Always tax the refined rate instead of the raw ore price (if higher) | False
         MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
         MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
         MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
-        MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
         
         
         ## Permissions
         
         Name | Purpose | Example Target Audience
         -- | -- | --
         basic_access | Can access this app and see own tax information, current ore prices, and FAQ. | Member State
```

### Comparing `aa-miningtaxes-1.2.6/README.md` & `aa-miningtaxes-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,18 @@
 
 Name | Description | Default
 -- | -- | --
 MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
 MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
 MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
 MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
+MININGTAXES_ALWAYS_TAX_REFINED | Always tax the refined rate instead of the raw ore price (if higher) | False
 MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
 MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
 MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
-MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
 
 
 ## Permissions
 
 Name | Purpose | Example Target Audience
 -- | -- | --
 basic_access | Can access this app and see own tax information, current ore prices, and FAQ. | Member State
```

### Comparing `aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/PKG-INFO` & `aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
         
@@ -83,18 +83,18 @@
         
         Name | Description | Default
         -- | -- | --
         MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
         MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
         MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
         MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
+        MININGTAXES_ALWAYS_TAX_REFINED | Always tax the refined rate instead of the raw ore price (if higher) | False
         MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
         MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
         MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
-        MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
         
         
         ## Permissions
         
         Name | Purpose | Example Target Audience
         -- | -- | --
         basic_access | Can access this app and see own tax information, current ore prices, and FAQ. | Member State
```

### Comparing `aa-miningtaxes-1.2.6/aa_miningtaxes.egg-info/SOURCES.txt` & `aa-miningtaxes-1.2.7/aa_miningtaxes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/auth_hooks.py` & `aa-miningtaxes-1.2.7/miningtaxes/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/decorators.py` & `aa-miningtaxes-1.2.7/miningtaxes/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/helpers.py` & `aa-miningtaxes-1.2.7/miningtaxes/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0001_initial.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0002_all_models.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0002_all_models.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0003_alter_general_options.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0003_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/migrations/0009_stats.py` & `aa-miningtaxes-1.2.7/miningtaxes/migrations/0009_stats.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/admin.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,17 @@
             structinfo = None
             try:
                 structinfo = esi.client.Universe.get_universe_structures_structure_id(
                     structure_id=entry["observer_id"],
                     token=token.valid_access_token(),
                 ).results()
             except Exception as e:
-                logger.error(f"Unknown struct id. Most likely offlined/old struct, ignoring: {entry['observer_id']}")
+                logger.error(
+                    f"Unknown struct id. Most likely offlined/old struct, ignoring: {entry['observer_id']}"
+                )
                 logger.error(e)
                 pass
             if structinfo is None:
                 continue
             structname = ""
             sys = None
             if type(structinfo) == dict:
```

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/character.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/general.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/general.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/orePrices.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/orePrices.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from django.db import models
 from eveuniverse.models import EveType, EveTypeMaterial
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from .. import __title__
-from ..app_settings import MININGTAXES_REFINED_RATE, MININGTAXES_UNKNOWN_TAX_RATE
+from ..app_settings import (
+    MININGTAXES_ALWAYS_TAX_REFINED,
+    MININGTAXES_REFINED_RATE,
+    MININGTAXES_UNKNOWN_TAX_RATE,
+)
 from ..helpers import PriceGroups
 from .settings import Settings
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def get_tax(eve_type):
@@ -92,10 +96,10 @@
         self.refined_price = 0.0
         for mat in materials:
             q = MININGTAXES_REFINED_RATE * mat.quantity / self.eve_type.portion_size
             self.refined_price += q * get_price(mat.material_eve_type)
         if self.refined_price == 0.0:
             self.refined_price = self.raw_price
         self.taxed_price = self.refined_price
-        if self.raw_price > self.taxed_price:
+        if MININGTAXES_ALWAYS_TAX_REFINED and self.raw_price > self.taxed_price:
             self.taxed_price = self.raw_price
         self.save()
```

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/settings.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/settings.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/models/stats.py` & `aa-miningtaxes-1.2.7/miningtaxes/models/stats.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/billboards_dark.css` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/billboards_light.css` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/billboards_light.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/global.css` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/launcher.css` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/css/miningtaxes.css` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/css/miningtaxes.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq1.png` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq1.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq2.png` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq2.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/static/miningtaxes/images/faq3.png` & `aa-miningtaxes-1.2.7/miningtaxes/static/miningtaxes/images/faq3.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/swagger.json` & `aa-miningtaxes-1.2.7/miningtaxes/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tasks.py` & `aa-miningtaxes-1.2.7/miningtaxes/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,33 @@
 
 
 def calctaxes():
     s = Stats.load()
     return s.calctaxes()
 
 
+def get_user(cid):
+    try:
+        c = EveCharacter.objects.get(character_id=cid)
+        p = c.character_ownership.user.profile
+    except Exception:
+        return None
+    if p is None or p.main_character is None:
+        return None
+    found = None
+    for c in p.user.character_ownerships.all():
+        try:
+            payee = get_object_or_404(Character, eve_character_id=c.character.pk)
+        except Exception:
+            continue
+        found = payee
+        break
+    return found
+
+
 @shared_task(**{**TASK_DEFAULT_KWARGS, **{"bind": True}})
 def notify_taxes_due(self):
     user2taxes = calctaxes()
 
     for u in user2taxes.keys():
         if user2taxes[u][0] > 0.01:
             title = "Taxes are due!"
@@ -327,15 +346,18 @@
                 payee = get_object_or_404(
                     Character,
                     eve_character_id=EveCharacter.objects.get(
                         character_id=entry.taxed_id
                     ).pk,
                 )
             except EveCharacter.DoesNotExist:
-                continue
+                payee = get_user(entry.taxed_id)
+                if payee is None:
+                    continue
+                pass
             except Http404:
                 continue
             payee.tax_credits.update_or_create(
                 date=entry.date, credit=entry.amount, defaults={"credit_type": "paid"}
             )
```

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/admin_launcher.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/admin_launcher.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/admin_tables.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/admin_tables.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/base.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/base.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/character_viewer.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/faq.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/faq.html`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
 		<h3 class="panel-title">Frequently asked questions</h3>
         </div>
         <div class="panel-body">
 		<h4>How do I pay my taxes?</h4>
 		<ol>
-			<li>Open your character window in game and click on your corp.</li>
-			<li>Click on the three dots on the upper right on the information screen about your corp: <br/>
+			<li>Search for any of the following corps: <b> {{ corps }} </b></li>
+			<li>Click on the three dots on the upper right on the information screen about the corp: <br/>
 				<div class='imgcontainer'> <img src="{% static 'miningtaxes/images/faq1.png' %}"/> </div>
 			</li>
 			<li>Select 'Give Money': <br/>
 				<div class='imgcontainer'> <img src="{% static 'miningtaxes/images/faq2.png' %}"/> </div>
 			</li>
 			<li>Enter the appropriate amount and the phrase '{{ phrase }}' without the quotes for the reason: <br/>
 				<div class='imgcontainer'>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends 'miningtaxes/base.html' %} {% load i18n %} {% load static %} {% load
 humanize %} {% load evelinks %} {% block details %}
 **** Frequently asked questions ****
 *** How do I pay my taxes? ***
-   1. Open your character window in game and click on your corp.
+   1. Search for any of the following corps: {{ corps }}
    2. Click on the three dots on the upper right on the information screen
-      about your corp:
+      about the corp:
       [{% static 'miningtaxes/images/faq1.png' %}]
    3. Select 'Give Money':
       [{% static 'miningtaxes/images/faq2.png' %}]
    4. Enter the appropriate amount and the phrase '{{ phrase }}' without the
       quotes for the reason:
       [{% static 'miningtaxes/images/faq3.png' %}]
       {{ phrase }}
```

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/launcher.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/launcher.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/ore_prices.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/ore_prices.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/templates/miningtaxes/user_summary.html` & `aa-miningtaxes-1.2.7/miningtaxes/templates/miningtaxes/user_summary.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_admin_character.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_admin_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_character.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/models/test_orePrice.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/models/test_orePrice.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/esi_client_stub.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/testdata/load_entities.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/tests/utils.py` & `aa-miningtaxes-1.2.7/miningtaxes/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/urls.py` & `aa-miningtaxes-1.2.7/miningtaxes/urls.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/miningtaxes/views.py` & `aa-miningtaxes-1.2.7/miningtaxes/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,20 @@
     s = Stats.load()
     return JsonResponse({"data": s.get_ore_prices_json()})
 
 
 @login_required
 @permission_required("miningtaxes.basic_access")
 def faq(request):
+    corps = []
+    for c in AdminCharacter.objects.all():
+        corps.append(c.eve_character.corporation_name)
+    corps = ",".join(corps)
     settings = Settings.load()
-    context = {"phrase": settings.phrase}
+    context = {"phrase": settings.phrase, "corps": corps}
     return render(request, "miningtaxes/faq.html", context)
 
 
 @login_required
 @permission_required("miningtaxes.basic_access")
 def index(request):
     characters = Character.objects.owned_by_user(request.user)
```

### Comparing `aa-miningtaxes-1.2.6/setup.py` & `aa-miningtaxes-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/testauth/celery.py` & `aa-miningtaxes-1.2.7/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/testauth/settingsAA2.py` & `aa-miningtaxes-1.2.7/testauth/settingsAA2.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.6/testauth/settingsAA3.py` & `aa-miningtaxes-1.2.7/testauth/settingsAA3.py`

 * *Files identical despite different names*

