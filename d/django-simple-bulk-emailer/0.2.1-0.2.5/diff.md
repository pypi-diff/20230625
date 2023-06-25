# Comparing `tmp/django_simple_bulk_emailer-0.2.1.tar.gz` & `tmp/django_simple_bulk_emailer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_bulk_emailer-0.2.1.tar", last modified: Wed Nov  9 18:01:04 2022, max compression
+gzip compressed data, was "django_simple_bulk_emailer-0.2.5.tar", last modified: Sun Jun 25 19:20:05 2023, max compression
```

## Comparing `django_simple_bulk_emailer-0.2.1.tar` & `django_simple_bulk_emailer-0.2.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.542880 django_simple_bulk_emailer-0.2.1/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2021-12-23 20:38:21.000000 django_simple_bulk_emailer-0.2.1/LICENSE
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      146 2019-02-05 21:19:31.000000 django_simple_bulk_emailer-0.2.1/MANIFEST.in
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    23256 2022-11-09 18:01:04.543016 django_simple_bulk_emailer-0.2.1/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    22324 2021-08-25 17:13:53.000000 django_simple_bulk_emailer-0.2.1/README.rst
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.524393 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:05:58.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    11544 2021-08-25 16:22:17.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/admin.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      284 2021-05-13 20:01:20.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/apps.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2134 2019-12-10 18:56:05.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/forms.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.525788 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/__init__.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.528284 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      401 2020-03-07 20:24:25.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/delete_expired_emails.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      835 2021-08-03 14:29:15.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/delete_expired_stats.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      527 2020-03-07 20:24:54.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      621 2019-12-09 19:45:53.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/import_sites.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4696 2022-04-07 19:58:41.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/send_bulk_email.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4866 2022-04-07 20:26:28.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/sync_mailchimp.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6788 2022-04-07 20:04:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/update_email_stats.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.530034 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     9299 2021-07-02 21:15:25.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0001_initial.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4870 2021-08-12 20:36:15.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1027 2021-08-24 19:06:30.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      428 2022-11-09 17:34:43.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0004_bulkemail_update_datetime.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-03-07 21:10:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    13663 2022-11-09 17:49:03.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/runtests.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.530293 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/signals/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/signals/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2780 2020-03-03 19:58:58.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/signals/handlers.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.530542 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-02-07 19:17:46.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.520367 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/admin/
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.530760 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/admin/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      534 2021-08-12 16:53:21.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.531032 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:27:20.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.532007 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2607 2022-01-07 11:59:32.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      122 2021-08-11 21:19:35.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer_preview.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.532640 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:58.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2166 2021-05-26 21:55:30.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.533443 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-04-24 18:58:47.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      582 2021-05-28 19:55:32.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.533945 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2021-05-28 18:19:58.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.534243 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-06-06 22:04:10.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.534430 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:24.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.535081 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5347 2022-11-09 17:30:24.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      843 2022-11-09 17:30:08.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.535950 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-03-29 13:50:42.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2658 2021-08-24 16:38:59.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4100 2022-11-09 17:29:10.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.536336 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-08-09 18:56:49.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.536921 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2019-03-28 18:47:23.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/bulk_email_send.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      681 2019-03-27 19:36:44.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      329 2019-08-22 20:13:23.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_text.txt
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.539187 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-08-25 17:58:15.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1831 2021-08-13 19:05:49.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2314 2021-08-13 19:07:02.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      587 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      488 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_success.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      688 2021-08-13 19:10:54.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1882 2021-08-13 19:11:26.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      522 2021-08-13 19:03:43.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.542595 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    27378 2022-04-07 19:30:56.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/functions.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1888 2020-03-04 20:25:13.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/settings.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    43095 2022-04-07 20:51:24.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_commands.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4320 2022-04-07 19:10:54.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_forms.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    12277 2021-08-24 15:43:34.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    50205 2022-04-07 19:30:56.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_views.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      280 2020-01-09 17:21:22.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1374 2021-07-13 14:59:06.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    19904 2022-04-07 20:13:05.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/views.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-11-09 18:01:04.525539 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    23256 2022-11-09 18:01:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4660 2022-11-09 18:01:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2022-11-09 18:01:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      141 2022-11-09 18:01:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/requires.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2022-11-09 18:01:04.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/top_level.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-08-25 18:06:31.000000 django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/zip-safe
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1088 2022-11-09 18:01:04.543356 django_simple_bulk_emailer-0.2.1/setup.cfg
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:33:59.000000 django_simple_bulk_emailer-0.2.1/setup.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.520069 django_simple_bulk_emailer-0.2.5/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2023-06-25 19:01:42.000000 django_simple_bulk_emailer-0.2.5/LICENSE
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      146 2019-02-05 21:19:31.000000 django_simple_bulk_emailer-0.2.5/MANIFEST.in
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    23297 2023-06-25 19:20:05.520183 django_simple_bulk_emailer-0.2.5/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    22324 2021-08-25 17:13:53.000000 django_simple_bulk_emailer-0.2.5/README.rst
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.505353 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:05:58.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    11586 2023-06-19 17:53:40.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/admin.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      284 2021-05-13 20:01:20.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/apps.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2134 2019-12-10 18:56:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/forms.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.506801 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/__init__.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.508807 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      401 2020-03-07 20:24:25.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/delete_expired_emails.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      835 2021-08-03 14:29:15.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/delete_expired_stats.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      527 2020-03-07 20:24:54.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      621 2019-12-09 19:45:53.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/import_sites.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4696 2022-04-07 19:58:41.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/send_bulk_email.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4866 2022-04-07 20:26:28.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/sync_mailchimp.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6788 2022-04-07 20:04:04.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/update_email_stats.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.510084 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     9299 2021-07-02 21:15:25.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0001_initial.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4870 2021-08-12 20:36:15.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1027 2021-08-24 19:06:30.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      378 2023-06-18 21:52:50.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0004_bulkemail_update_datetime.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-03-07 21:10:04.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    13663 2022-11-09 17:49:03.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/runtests.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.510300 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/signals/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/signals/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2780 2020-03-03 19:58:58.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/signals/handlers.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.510492 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-02-07 19:17:46.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.500904 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/admin/
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.510671 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/admin/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      534 2021-08-12 16:53:21.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.510950 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:27:20.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.511595 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2607 2022-01-07 11:59:32.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      122 2021-08-11 21:19:35.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer_preview.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.512051 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:58.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2166 2021-05-26 21:55:30.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.512775 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-04-24 18:58:47.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      582 2021-05-28 19:55:32.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.513059 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2021-05-28 18:19:58.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.513297 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-06-06 22:04:10.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.513436 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-05-28 19:18:24.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.513912 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5347 2022-11-09 17:30:24.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      843 2022-11-09 17:30:08.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.514514 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-03-29 13:50:42.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2658 2021-08-24 16:38:59.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4100 2022-11-09 17:29:10.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.514762 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2019-08-09 18:56:49.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.515208 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2019-03-28 18:47:23.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/bulk_email_send.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      681 2019-03-27 19:36:44.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      329 2019-08-22 20:13:23.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_text.txt
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.517207 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-08-25 17:58:15.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1831 2021-08-13 19:05:49.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2314 2021-08-13 19:07:02.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      587 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      488 2021-08-13 19:10:22.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_success.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      688 2021-08-13 19:10:54.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1882 2021-08-13 19:11:26.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      522 2021-08-13 19:03:43.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.519924 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    27447 2023-06-18 21:48:41.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/functions.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1888 2020-03-04 20:25:13.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/settings.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    43095 2022-04-07 20:51:24.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_commands.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4320 2022-04-07 19:10:54.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_forms.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    12277 2021-08-24 15:43:34.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    50205 2022-04-07 19:30:56.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_views.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      280 2020-01-09 17:21:22.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1374 2021-07-13 14:59:06.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    19904 2022-04-07 20:13:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/views.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:20:05.506536 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    23297 2023-06-25 19:20:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4660 2023-06-25 19:20:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-25 19:20:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      145 2023-06-25 19:20:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/requires.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2023-06-25 19:20:05.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-08-25 18:06:31.000000 django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/zip-safe
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1122 2023-06-25 19:20:05.520488 django_simple_bulk_emailer-0.2.5/setup.cfg
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:33:59.000000 django_simple_bulk_emailer-0.2.5/setup.py
```

### Comparing `django_simple_bulk_emailer-0.2.1/LICENSE` & `django_simple_bulk_emailer-0.2.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2015-22 Jonathan Rickard
+Copyright (c) 2015-23 Jonathan Rickard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django_simple_bulk_emailer-0.2.1/PKG-INFO` & `django_simple_bulk_emailer-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: django_simple_bulk_emailer
-Version: 0.2.1
+Version: 0.2.5
 Summary: A Django app for sending bulk email
 Home-page: https://github.com/jonathanrickard/django-simple-bulk-emailer
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,email
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ==========================
 django-simple-bulk-emailer
```

### Comparing `django_simple_bulk_emailer-0.2.1/README.rst` & `django_simple_bulk_emailer-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/admin.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 )
 from django.db import (
     models,
 )
 
 
 from adminsortable2.admin import (
+    SortableAdminBase,
     SortableAdminMixin,
     SortableInlineAdminMixin,
 )
 from django_simple_file_handler.file_types import (
     CHECK_DOC,
     CHECK_WEB_IMAGE,
 )
@@ -365,15 +366,15 @@
                 },
             ),
             'publication_date': admin.widgets.AdminDateWidget,
             'deletion_date': admin.widgets.AdminDateWidget,
         }
 
 
-class BulkEmailAdmin(BaseAdmin):
+class BulkEmailAdmin(SortableAdminBase, BaseAdmin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.readonly_fields = [
             'subscription_name',
             'short_headline',
             'page_preview',
             'email_preview',
```

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/forms.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/delete_expired_stats.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/delete_expired_stats.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/delete_unsubscribed_users.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/import_sites.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/import_sites.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/send_bulk_email.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/send_bulk_email.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/sync_mailchimp.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/sync_mailchimp.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/management/commands/update_email_stats.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/management/commands/update_email_stats.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0001_initial.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0002_auto_20210812_1535.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/migrations/0003_auto_20210824_1148.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/models.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/signals/handlers.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/admin/css/django_simple_bulk_emailer.css`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/css/django_simple_bulk_emailer.css`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/images/file_icon_64x64.png`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/static/django_simple_bulk_emailer/js/django_simple_bulk_emailer.js`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_html.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/emails/email_template_text.txt`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/list_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/subscription/pages/page_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/emails/subscribe_email_html.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/bulk_email_preview.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/manage_subscriptions_error.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/quick_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/templates/django_simple_bulk_emailer/universal/pages/subscribe_success.html`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/functions.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,18 @@
             added_permission = Permission.objects.get(
                 codename=permission,
             )
             user.user_permissions.add(added_permission)
     return user
 
 
+def dummy_get_response(request):
+    return None
+
+
 def create_request_response(self, get_post, page='1', key='empty', time_dict=None):
     reverse_name = f'django_simple_bulk_emailer:{self.view_name}'
     with self.settings(
         SITE_ID=self.profile_instance.site_ptr.id,
     ):
         reverse_string = reverse(
             reverse_name,
@@ -246,15 +250,15 @@
             self.request = RequestFactory().get(
                 reverse_string,
             )
         try:
             self.request.user = self.user
         except AttributeError:
             pass
-        SessionMiddleware().process_request(self.request)
+        SessionMiddleware(dummy_get_response).process_request(self.request)
         if time_dict:
             load_time = timezone.now() - timedelta(**time_dict)
             self.request.session['form_load_time'] = load_time.timestamp()
             self.request.session.save()
         args = []
         for key, value in self.kwargs.items():
             args.append(value)
```

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/settings.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_commands.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_forms.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_models.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/tests/test_views.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/urls.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/urls.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer/views.py` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer/views.py`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/PKG-INFO` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: django-simple-bulk-emailer
-Version: 0.2.1
+Version: 0.2.5
 Summary: A Django app for sending bulk email
 Home-page: https://github.com/jonathanrickard/django-simple-bulk-emailer
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,email
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ==========================
 django-simple-bulk-emailer
```

### Comparing `django_simple_bulk_emailer-0.2.1/django_simple_bulk_emailer.egg-info/SOURCES.txt` & `django_simple_bulk_emailer-0.2.5/django_simple_bulk_emailer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_bulk_emailer-0.2.1/setup.cfg` & `django_simple_bulk_emailer-0.2.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [metadata]
 name = django_simple_bulk_emailer
-version = 0.2.1
+version = 0.2.5
 author = Jonathan Rickard
 author_email = jonathan@jonathanrickard.com
 license = MIT License
 description = A Django app for sending bulk email
 keywords = django, email
 url = https://github.com/jonathanrickard/django-simple-bulk-emailer
 long_description = file: README.rst
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: Developers
 	Topic :: Internet :: WWW/HTTP
 	License :: OSI Approved :: MIT License
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = True
 install_requires = 
-	Django >= 3.2, < 4.0
-	django-admin-sortable2 >= 1.0
+	Django >= 4.1, < 5.0
+	django-admin-sortable2 >= 2.1.8
 	django-ckeditor >= 6.2
-	django-simple-file-handler >= 0.3
+	django-simple-file-handler >= 0.3.3
 	mailchimp3 >= 3.0
 	Pillow >= 9.0
 	requests >= 2.27
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

