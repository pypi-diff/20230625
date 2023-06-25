# Comparing `tmp/django_simple_forms-0.1.2.tar.gz` & `tmp/django_simple_forms-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_forms-0.1.2.tar", last modified: Mon Dec  5 21:42:50 2022, max compression
+gzip compressed data, was "django_simple_forms-0.1.7.tar", last modified: Sun Jun 25 19:21:00 2023, max compression
```

## Comparing `django_simple_forms-0.1.2.tar` & `django_simple_forms-0.1.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.673383 django_simple_forms-0.1.2/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2021-12-23 20:38:59.000000 django_simple_forms-0.1.2/LICENSE
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      132 2020-11-25 20:09:02.000000 django_simple_forms-0.1.2/MANIFEST.in
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6020 2022-12-05 21:42:50.673489 django_simple_forms-0.1.2/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5075 2022-12-03 11:56:53.000000 django_simple_forms-0.1.2/README.rst
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.662810 django_simple_forms-0.1.2/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       55 2020-03-13 19:52:39.000000 django_simple_forms-0.1.2/django_simple_forms/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    28509 2022-10-25 00:07:24.000000 django_simple_forms-0.1.2/django_simple_forms/admin.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      187 2021-05-13 20:01:43.000000 django_simple_forms-0.1.2/django_simple_forms/apps.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     3688 2022-12-03 11:34:51.000000 django_simple_forms-0.1.2/django_simple_forms/forms.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.664090 django_simple_forms-0.1.2/django_simple_forms/management/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.2/django_simple_forms/management/__init__.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.665049 django_simple_forms-0.1.2/django_simple_forms/management/commands/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.2/django_simple_forms/management/commands/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      879 2022-09-13 13:39:05.000000 django_simple_forms-0.1.2/django_simple_forms/management/commands/delete_expired_responses.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      340 2022-09-08 16:57:08.000000 django_simple_forms-0.1.2/django_simple_forms/management/commands/delete_unused_addresses.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      636 2021-01-27 18:01:44.000000 django_simple_forms-0.1.2/django_simple_forms/management/commands/forms_import_sites.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.665824 django_simple_forms-0.1.2/django_simple_forms/migrations/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    15282 2022-12-03 11:20:36.000000 django_simple_forms-0.1.2/django_simple_forms/migrations/0001_initial.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-11-16 20:10:59.000000 django_simple_forms-0.1.2/django_simple_forms/migrations/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    26775 2022-12-03 11:33:21.000000 django_simple_forms-0.1.2/django_simple_forms/models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_forms-0.1.2/django_simple_forms/runtests.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.665979 django_simple_forms-0.1.2/django_simple_forms/static/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-08-11 18:16:52.000000 django_simple_forms-0.1.2/django_simple_forms/static/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.666260 django_simple_forms-0.1.2/django_simple_forms/static/admin/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-20 21:01:11.000000 django_simple_forms-0.1.2/django_simple_forms/static/admin/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.666803 django_simple_forms-0.1.2/django_simple_forms/static/admin/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      113 2022-08-26 11:26:25.000000 django_simple_forms-0.1.2/django_simple_forms/static/admin/css/delete_button.css
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      684 2022-08-26 11:11:09.000000 django_simple_forms-0.1.2/django_simple_forms/static/admin/css/django_simple_forms.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.667031 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2020-11-25 15:13:25.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.667311 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:21.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.667744 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:30.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/css/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2507 2022-08-19 10:18:57.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/css/form_style.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.667998 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:15:02.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.668536 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/css/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 18:16:52.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1742 2022-08-11 20:10:24.000000 django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/css/post_html.css
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.668820 django_simple_forms-0.1.2/django_simple_forms/templates/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-10-13 19:03:38.000000 django_simple_forms-0.1.2/django_simple_forms/templates/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.669123 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-11-25 15:18:01.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.669364 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:18:06.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.669935 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1471 2022-10-11 20:33:41.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      393 2021-04-21 22:11:13.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/pages/form_submitted.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.670423 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:13:43.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.670929 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/emails/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2028 2022-10-16 18:37:40.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      319 2022-10-16 18:49:33.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      477 2022-10-13 18:59:37.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/internal_base.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.671747 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-01-19 16:10:11.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      815 2022-10-13 19:20:58.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2082 2022-10-16 18:38:52.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.671991 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pdfs/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1021 2022-10-16 19:13:03.000000 django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.672963 django_simple_forms-0.1.2/django_simple_forms/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_forms-0.1.2/django_simple_forms/tests/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1811 2022-12-03 11:21:14.000000 django_simple_forms-0.1.2/django_simple_forms/tests/settings.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      274 2022-12-03 11:22:49.000000 django_simple_forms-0.1.2/django_simple_forms/tests/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1699 2022-08-12 21:41:33.000000 django_simple_forms-0.1.2/django_simple_forms/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    21187 2022-12-04 19:19:33.000000 django_simple_forms-0.1.2/django_simple_forms/views.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-12-05 21:42:50.663853 django_simple_forms-0.1.2/django_simple_forms.egg-info/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6020 2022-12-05 21:42:50.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2664 2022-12-05 21:42:50.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2022-12-05 21:42:50.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      129 2022-12-05 21:42:50.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/requires.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       20 2022-12-05 21:42:50.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/top_level.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:42:55.000000 django_simple_forms-0.1.2/django_simple_forms.egg-info/zip-safe
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1075 2022-12-05 21:42:50.673903 django_simple_forms-0.1.2/setup.cfg
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:48:14.000000 django_simple_forms-0.1.2/setup.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.937937 django_simple_forms-0.1.7/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2023-06-25 19:14:54.000000 django_simple_forms-0.1.7/LICENSE
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      132 2020-11-25 20:09:02.000000 django_simple_forms-0.1.7/MANIFEST.in
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6010 2023-06-25 19:21:00.938072 django_simple_forms-0.1.7/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5075 2022-12-03 11:56:53.000000 django_simple_forms-0.1.7/README.rst
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.928530 django_simple_forms-0.1.7/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       55 2020-03-13 19:52:39.000000 django_simple_forms-0.1.7/django_simple_forms/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    28570 2023-06-19 18:11:48.000000 django_simple_forms-0.1.7/django_simple_forms/admin.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      187 2021-05-13 20:01:43.000000 django_simple_forms-0.1.7/django_simple_forms/apps.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     3688 2022-12-03 11:34:51.000000 django_simple_forms-0.1.7/django_simple_forms/forms.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.930045 django_simple_forms-0.1.7/django_simple_forms/management/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.7/django_simple_forms/management/__init__.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.930747 django_simple_forms-0.1.7/django_simple_forms/management/commands/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2017-08-21 13:49:56.000000 django_simple_forms-0.1.7/django_simple_forms/management/commands/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      879 2022-09-13 13:39:05.000000 django_simple_forms-0.1.7/django_simple_forms/management/commands/delete_expired_responses.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      340 2022-09-08 16:57:08.000000 django_simple_forms-0.1.7/django_simple_forms/management/commands/delete_unused_addresses.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      636 2021-01-27 18:01:44.000000 django_simple_forms-0.1.7/django_simple_forms/management/commands/forms_import_sites.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.931232 django_simple_forms-0.1.7/django_simple_forms/migrations/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    15282 2022-12-03 11:20:36.000000 django_simple_forms-0.1.7/django_simple_forms/migrations/0001_initial.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2020-11-16 20:10:59.000000 django_simple_forms-0.1.7/django_simple_forms/migrations/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    26775 2022-12-03 11:33:21.000000 django_simple_forms-0.1.7/django_simple_forms/models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      381 2020-03-07 20:39:02.000000 django_simple_forms-0.1.7/django_simple_forms/runtests.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.931346 django_simple_forms-0.1.7/django_simple_forms/static/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-08-11 18:16:52.000000 django_simple_forms-0.1.7/django_simple_forms/static/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.931599 django_simple_forms-0.1.7/django_simple_forms/static/admin/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-20 21:01:11.000000 django_simple_forms-0.1.7/django_simple_forms/static/admin/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.932159 django_simple_forms-0.1.7/django_simple_forms/static/admin/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      113 2022-08-26 11:26:25.000000 django_simple_forms-0.1.7/django_simple_forms/static/admin/css/delete_button.css
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      574 2023-06-19 18:15:07.000000 django_simple_forms-0.1.7/django_simple_forms/static/admin/css/django_simple_forms.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.932502 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2020-11-25 15:13:25.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.932696 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:21.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.933125 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:13:30.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/css/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2507 2022-08-19 10:18:57.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/css/form_style.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.933377 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:15:02.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.933965 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/css/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 18:16:52.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1742 2022-08-11 20:10:24.000000 django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/css/post_html.css
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.934187 django_simple_forms-0.1.7/django_simple_forms/templates/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2022-10-13 19:03:38.000000 django_simple_forms-0.1.7/django_simple_forms/templates/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.934441 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-11-25 15:18:01.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.934598 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2020-11-25 15:18:06.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.935126 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1471 2022-10-11 20:33:41.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      393 2021-04-21 22:11:13.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/pages/form_submitted.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.935705 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2022-08-11 17:13:43.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.936156 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/emails/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2028 2022-10-16 18:37:40.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      319 2022-10-16 18:49:33.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      477 2022-10-13 18:59:37.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/internal_base.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.936878 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6148 2021-01-19 16:10:11.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      815 2022-10-13 19:20:58.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2082 2022-10-16 18:38:52.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.937068 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pdfs/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1021 2022-10-16 19:13:03.000000 django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.937708 django_simple_forms-0.1.7/django_simple_forms/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_forms-0.1.7/django_simple_forms/tests/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1811 2022-12-03 11:21:14.000000 django_simple_forms-0.1.7/django_simple_forms/tests/settings.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      274 2022-12-03 11:22:49.000000 django_simple_forms-0.1.7/django_simple_forms/tests/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1699 2022-08-12 21:41:33.000000 django_simple_forms-0.1.7/django_simple_forms/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    21187 2022-12-04 19:19:33.000000 django_simple_forms-0.1.7/django_simple_forms/views.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-25 19:21:00.929710 django_simple_forms-0.1.7/django_simple_forms.egg-info/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6010 2023-06-25 19:21:00.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2664 2023-06-25 19:21:00.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-25 19:21:00.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      133 2023-06-25 19:21:00.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/requires.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       20 2023-06-25 19:21:00.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/top_level.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:42:55.000000 django_simple_forms-0.1.7/django_simple_forms.egg-info/zip-safe
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1069 2023-06-25 19:21:00.938497 django_simple_forms-0.1.7/setup.cfg
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:48:14.000000 django_simple_forms-0.1.7/setup.py
```

### Comparing `django_simple_forms-0.1.2/LICENSE` & `django_simple_forms-0.1.7/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2015-22 Jonathan Rickard
+Copyright (c) 2015-23 Jonathan Rickard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django_simple_forms-0.1.2/PKG-INFO` & `django_simple_forms-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django_simple_forms
-Version: 0.1.2
+Version: 0.1.7
 Summary: A Django app for creating forms
 Home-page: https://github.com/jonathanrickard
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,forms
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
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ===================
 django-simple-forms
```

### Comparing `django_simple_forms-0.1.2/README.rst` & `django_simple_forms-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/admin.py` & `django_simple_forms-0.1.7/django_simple_forms/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 )
 from django.utils.safestring import (
     mark_safe,
 )
 
 
 from adminsortable2.admin import (
+    SortableAdminBase,
     SortableInlineAdminMixin,
 )
 
 
 from .models import (
     ChoiceDefinition,
     EmailAddress,
@@ -228,15 +229,15 @@
 class ChoiceDefinitionInline(SortableInlineAdminMixin, admin.TabularInline):
     model = ChoiceDefinition
     exclude = [
     ]
     extra = 0
 
 
-class InputDefinitionAdmin(CloneableAdmin):
+class InputDefinitionAdmin(SortableAdminBase, CloneableAdmin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.readonly_fields = [
             'def_links',
             'inst_count',
         ] + self.readonly_fields
         self.top_fieldsets = [
@@ -380,15 +381,15 @@
             formfield.queryset = form_definition.input_instances
         return formfield
 
     model = TableField
     extra = 0
 
 
-class FormDefinitionAdmin(CloneableAdmin):
+class FormDefinitionAdmin(SortableAdminBase, CloneableAdmin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.obj = None
         self.readonly_fields = [
             'inst_links',
             'inst_count',
         ] + self.readonly_fields
```

### Comparing `django_simple_forms-0.1.2/django_simple_forms/forms.py` & `django_simple_forms-0.1.7/django_simple_forms/forms.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/management/commands/delete_expired_responses.py` & `django_simple_forms-0.1.7/django_simple_forms/management/commands/delete_expired_responses.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/management/commands/forms_import_sites.py` & `django_simple_forms-0.1.7/django_simple_forms/management/commands/forms_import_sites.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/migrations/0001_initial.py` & `django_simple_forms-0.1.7/django_simple_forms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/models.py` & `django_simple_forms-0.1.7/django_simple_forms/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/admin/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/admin/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/css/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/external/css/form_style.css` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/external/css/form_style.css`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/static/django_simple_forms/internal/css/post_html.css` & `django_simple_forms-0.1.7/django_simple_forms/static/django_simple_forms/internal/css/post_html.css`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/external/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/emails/form_email.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/post_form.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pages/post_view.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html` & `django_simple_forms-0.1.7/django_simple_forms/templates/django_simple_forms/internal/pdfs/default_pdf.html`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/tests/settings.py` & `django_simple_forms-0.1.7/django_simple_forms/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/urls.py` & `django_simple_forms-0.1.7/django_simple_forms/urls.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms/views.py` & `django_simple_forms-0.1.7/django_simple_forms/views.py`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/django_simple_forms.egg-info/PKG-INFO` & `django_simple_forms-0.1.7/django_simple_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-simple-forms
-Version: 0.1.2
+Version: 0.1.7
 Summary: A Django app for creating forms
 Home-page: https://github.com/jonathanrickard
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,forms
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
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ===================
 django-simple-forms
```

### Comparing `django_simple_forms-0.1.2/django_simple_forms.egg-info/SOURCES.txt` & `django_simple_forms-0.1.7/django_simple_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_forms-0.1.2/setup.cfg` & `django_simple_forms-0.1.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [metadata]
 name = django_simple_forms
-version = 0.1.2
+version = 0.1.7
 author = Jonathan Rickard
 author_email = jonathan@jonathanrickard.com
 license = MIT License
 description = A Django app for creating forms
 keywords = django, forms
 url = https://github.com/jonathanrickard
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
 	Programming Language :: Python :: 3.10
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
 	django-ckeditor >= 6.1
-	django-simple-file-handler >= 0.3
+	django-simple-file-handler >= 0.3.3
 	requests >= 2.28
 	xlsxwriter >= 3.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

