# Comparing `tmp/Bigsansar-1.7.3.tar.gz` & `tmp/Bigsansar-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.7.3.tar", last modified: Sun Jun 18 11:17:44 2023, max compression
+gzip compressed data, was "Bigsansar-1.7.4.tar", last modified: Sun Jun 25 11:49:04 2023, max compression
```

## Comparing `Bigsansar-1.7.3.tar` & `Bigsansar-1.7.4.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.808899 Bigsansar-1.7.3/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.678899 Bigsansar-1.7.3/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4927 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5001 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-18 11:17:44.000000 Bigsansar-1.7.3/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.7.3/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4927 2023-06-18 11:17:44.808899 Bigsansar-1.7.3/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4367 2023-06-18 11:17:26.000000 Bigsansar-1.7.3/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.688899 Bigsansar-1.7.3/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.688899 Bigsansar-1.7.3/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.688899 Bigsansar-1.7.3/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.688899 Bigsansar-1.7.3/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.688899 Bigsansar-1.7.3/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.698899 Bigsansar-1.7.3/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      208 2023-06-18 11:06:16.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.708899 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      296 2023-06-18 11:06:29.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      634 2023-06-18 11:03:03.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.7.3/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.708899 Bigsansar-1.7.3/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2302 2023-06-16 11:18:51.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.718899 Bigsansar-1.7.3/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.718899 Bigsansar-1.7.3/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2123 2023-06-18 11:14:37.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.7.3/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.7.3/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.728899 Bigsansar-1.7.3/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.738899 Bigsansar-1.7.3/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.668899 Bigsansar-1.7.3/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.668899 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.668899 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.738899 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.738899 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.788899 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 11:17:44.808899 Bigsansar-1.7.3/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.7.3/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.7.3/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.7.3/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-18 11:01:43.000000 Bigsansar-1.7.3/bigsansar/templates/styles.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.3/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.7.3/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4968 2023-06-18 11:03:42.000000 Bigsansar-1.7.3/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-18 11:17:44.808899 Bigsansar-1.7.3/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-18 11:16:22.000000 Bigsansar-1.7.3/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.978314 Bigsansar-1.7.4/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4940 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5033 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-25 11:49:04.000000 Bigsansar-1.7.4/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.7.4/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4940 2023-06-25 11:49:04.978314 Bigsansar-1.7.4/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4380 2023-06-25 11:48:41.000000 Bigsansar-1.7.4/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      208 2023-06-18 11:06:16.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      296 2023-06-18 11:06:29.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      634 2023-06-18 11:03:03.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.7.4/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2302 2023-06-16 11:18:51.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2050 2023-06-25 11:46:51.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.918315 Bigsansar-1.7.4/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2225 2023-06-25 11:45:49.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.7.4/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.7.4/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.908315 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.928315 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.938315 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.968315 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-25 11:49:04.978314 Bigsansar-1.7.4/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.7.4/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.7.4/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-25 11:39:45.000000 Bigsansar-1.7.4/bigsansar/templates/script.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.7.4/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      101 2023-06-18 11:01:43.000000 Bigsansar-1.7.4/bigsansar/templates/styles.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.4/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1080 2023-06-25 11:47:13.000000 Bigsansar-1.7.4/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4791 2023-06-25 11:44:31.000000 Bigsansar-1.7.4/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-25 11:49:04.978314 Bigsansar-1.7.4/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-25 11:48:10.000000 Bigsansar-1.7.4/setup.py
```

### Comparing `Bigsansar-1.7.3/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.7.4/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.7.3
+Version: 1.7.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## New update
-* sitemap and styles.css system can edit manually from pages
+* sitemap , javascript and styles.css system can edit manually from pages
 * now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 
  
 # How to get Bigsansar
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE ## New update * sitemap and styles.css system
-can edit manually from pages * now sitemap system can add or edit manually *
-fixed control system for superuser and normal user in to custom domain and blog
-post modols. * fixed visitor system in to blog post. * added thumbnails model
-field in blog system # How to get Bigsansar Bigsansar is available open-source
-under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
-recommend using the latest version of Python 3. Bigsansar is Fully based on
-django. You can use [bigsansar](https://bigsansar.com) for install packaged.
-view our tutorials in [youtube](https://youtube.com/bigsansar) for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-
-LC6i7YQAaqB57FaCfWEZkth) # Get the latest development version The latest and
-greatest Bigsasnar version is the one thatâs in our Git repository (our
-revision-control system). This is only for experienced users who want to try
-incoming changes and help identify bugs before an official release. Get it
-using this shell command, which requires [Git](https://git-scm.com/): `git
-clone https://github.com/pokhrelb9/bigsansar.git` You can also download a
-[gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development
-version. This archive is updated every time we commit code. # After you install
-bigsansar Type `bigsansar init` command for **automatically** setup server . #
-How to access admin pannel in local env Go to [localhost:8000](http://
-localhost:8000) # some usefull link [sitemap.xml](http://localhost:8000/
-sitemap.xml) [script.js](http://localhost:8000/script.js) [styles.css](http://
-localhost:8000/styles.css) # how to edit sitemap , js and css from pages create
-a page **slug** name with sitemap,script , styles # How to change admin URL in
-server side with domain go to **VirtualHost.py** file and change **localhost:
-8000** with your subdomain ## Some usefull commands: `python3 manage.py
-createuser` - get unlimited users. ## templatetags for extends and include {%
-extends '/.html' %} {% include '/.html' %} ## load blog list in templates `{%
-load blogs %} {% get_blog as bloglist %} {% for list in bloglist %}
+markdown License-File: LICENSE ## New update * sitemap , javascript and
+styles.css system can edit manually from pages * now sitemap system can add or
+edit manually * fixed control system for superuser and normal user in to custom
+domain and blog post modols. * fixed visitor system in to blog post. * added
+thumbnails model field in blog system # How to get Bigsansar Bigsansar is
+available open-source under the [MIT](https://en.wikipedia.org/wiki/
+MIT_License) license. We recommend using the latest version of Python 3.
+Bigsansar is Fully based on django. You can use [bigsansar](https://
+bigsansar.com) for install packaged. view our tutorials in [youtube](https://
+youtube.com/bigsansar) for playlist: [bigsansar for django](https://
+www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) # Get the
+latest development version The latest and greatest Bigsasnar version is the one
+thatâs in our Git repository (our revision-control system). This is only for
+experienced users who want to try incoming changes and help identify bugs
+before an official release. Get it using this shell command, which requires
+[Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
+bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
+project/Bigsansar/#files) of the development version. This archive is updated
+every time we commit code. # After you install bigsansar Type `bigsansar init`
+command for **automatically** setup server . # How to access admin pannel in
+local env Go to [localhost:8000](http://localhost:8000) # some usefull link
+[sitemap.xml](http://localhost:8000/sitemap.xml) [script.js](http://localhost:
+8000/script.js) [styles.css](http://localhost:8000/styles.css) # how to edit
+sitemap , js and css from pages create a page **slug** name with sitemap,script
+, styles # How to change admin URL in server side with domain go to
+**VirtualHost.py** file and change **localhost:8000** with your subdomain ##
+Some usefull commands: `python3 manage.py createuser` - get unlimited users. ##
+templatetags for extends and include {% extends '/.html' %} {% include '/.html'
+%} ## load blog list in templates `{% load blogs %} {% get_blog as bloglist %}
+{% for list in bloglist %}
 ** {{list.title}} - {{ list.domain }} **
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 Read_More
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
 { get_blog.publish_date }} {{ get_blog.domain }} {{ get_blog.id }} {
 { get_blog.slug }} {{ get_blog.body | safe }} {{ get_blog.visitor }} ` ## Count
```

### Comparing `Bigsansar-1.7.3/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.7.4/Bigsansar.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -109,9 +109,10 @@
 bigsansar/templates/__init__.py
 bigsansar/templates/acc_active_email.html
 bigsansar/templates/base.html
 bigsansar/templates/blog_preview.html
 bigsansar/templates/default.html
 bigsansar/templates/defaultpage.html
 bigsansar/templates/parking.html
+bigsansar/templates/script.html
 bigsansar/templates/sitemap.html
 bigsansar/templates/styles.html
```

### Comparing `Bigsansar-1.7.3/LICENSE` & `Bigsansar-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/PKG-INFO` & `Bigsansar-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.7.3
+Version: 1.7.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## New update
-* sitemap and styles.css system can edit manually from pages
+* sitemap , javascript and styles.css system can edit manually from pages
 * now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 
  
 # How to get Bigsansar
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE ## New update * sitemap and styles.css system
-can edit manually from pages * now sitemap system can add or edit manually *
-fixed control system for superuser and normal user in to custom domain and blog
-post modols. * fixed visitor system in to blog post. * added thumbnails model
-field in blog system # How to get Bigsansar Bigsansar is available open-source
-under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
-recommend using the latest version of Python 3. Bigsansar is Fully based on
-django. You can use [bigsansar](https://bigsansar.com) for install packaged.
-view our tutorials in [youtube](https://youtube.com/bigsansar) for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-
-LC6i7YQAaqB57FaCfWEZkth) # Get the latest development version The latest and
-greatest Bigsasnar version is the one thatâs in our Git repository (our
-revision-control system). This is only for experienced users who want to try
-incoming changes and help identify bugs before an official release. Get it
-using this shell command, which requires [Git](https://git-scm.com/): `git
-clone https://github.com/pokhrelb9/bigsansar.git` You can also download a
-[gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development
-version. This archive is updated every time we commit code. # After you install
-bigsansar Type `bigsansar init` command for **automatically** setup server . #
-How to access admin pannel in local env Go to [localhost:8000](http://
-localhost:8000) # some usefull link [sitemap.xml](http://localhost:8000/
-sitemap.xml) [script.js](http://localhost:8000/script.js) [styles.css](http://
-localhost:8000/styles.css) # how to edit sitemap , js and css from pages create
-a page **slug** name with sitemap,script , styles # How to change admin URL in
-server side with domain go to **VirtualHost.py** file and change **localhost:
-8000** with your subdomain ## Some usefull commands: `python3 manage.py
-createuser` - get unlimited users. ## templatetags for extends and include {%
-extends '/.html' %} {% include '/.html' %} ## load blog list in templates `{%
-load blogs %} {% get_blog as bloglist %} {% for list in bloglist %}
+markdown License-File: LICENSE ## New update * sitemap , javascript and
+styles.css system can edit manually from pages * now sitemap system can add or
+edit manually * fixed control system for superuser and normal user in to custom
+domain and blog post modols. * fixed visitor system in to blog post. * added
+thumbnails model field in blog system # How to get Bigsansar Bigsansar is
+available open-source under the [MIT](https://en.wikipedia.org/wiki/
+MIT_License) license. We recommend using the latest version of Python 3.
+Bigsansar is Fully based on django. You can use [bigsansar](https://
+bigsansar.com) for install packaged. view our tutorials in [youtube](https://
+youtube.com/bigsansar) for playlist: [bigsansar for django](https://
+www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) # Get the
+latest development version The latest and greatest Bigsasnar version is the one
+thatâs in our Git repository (our revision-control system). This is only for
+experienced users who want to try incoming changes and help identify bugs
+before an official release. Get it using this shell command, which requires
+[Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
+bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
+project/Bigsansar/#files) of the development version. This archive is updated
+every time we commit code. # After you install bigsansar Type `bigsansar init`
+command for **automatically** setup server . # How to access admin pannel in
+local env Go to [localhost:8000](http://localhost:8000) # some usefull link
+[sitemap.xml](http://localhost:8000/sitemap.xml) [script.js](http://localhost:
+8000/script.js) [styles.css](http://localhost:8000/styles.css) # how to edit
+sitemap , js and css from pages create a page **slug** name with sitemap,script
+, styles # How to change admin URL in server side with domain go to
+**VirtualHost.py** file and change **localhost:8000** with your subdomain ##
+Some usefull commands: `python3 manage.py createuser` - get unlimited users. ##
+templatetags for extends and include {% extends '/.html' %} {% include '/.html'
+%} ## load blog list in templates `{% load blogs %} {% get_blog as bloglist %}
+{% for list in bloglist %}
 ** {{list.title}} - {{ list.domain }} **
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 Read_More
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
 { get_blog.publish_date }} {{ get_blog.domain }} {{ get_blog.id }} {
 { get_blog.slug }} {{ get_blog.body | safe }} {{ get_blog.visitor }} ` ## Count
```

### Comparing `Bigsansar-1.7.3/README.md` & `Bigsansar-1.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## New update
-* sitemap and styles.css system can edit manually from pages
+* sitemap , javascript and styles.css system can edit manually from pages
 * now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 
  
 # How to get Bigsansar
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-## New update * sitemap and styles.css system can edit manually from pages *
-now sitemap system can add or edit manually * fixed control system for
-superuser and normal user in to custom domain and blog post modols. * fixed
+## New update * sitemap , javascript and styles.css system can edit manually
+from pages * now sitemap system can add or edit manually * fixed control system
+for superuser and normal user in to custom domain and blog post modols. * fixed
 visitor system in to blog post. * added thumbnails model field in blog system #
 How to get Bigsansar Bigsansar is available open-source under the [MIT](https:/
 /en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
 version of Python 3. Bigsansar is Fully based on django. You can use
 [bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
 [youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
 (https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) #
```

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/account/forms.py` & `Bigsansar-1.7.4/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.7.4/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/account/models.py` & `Bigsansar-1.7.4/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.7.4/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/advance/models.py` & `Bigsansar-1.7.4/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.7.4/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.7.4/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.7.4/bigsansar/contrib/blogs/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,14 @@
             pass
         
         super().delete()
 
     def __str__(self):
         return self.title
     
-    def get_absolute_url(self):
-        return "http://%s/blog/preview/%s" % (self.domain, self.id)
 
     class Meta:
         verbose_name = 'Posts'
         verbose_name_plural = 'Posts'
 
     # def get_absolute_url(self):
     #     return reverse("blog", kwargs={"slug": self.slug})
```

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.7.4/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.7.4/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.7.4/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.7.4/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/contrib/sites/models.py` & `Bigsansar-1.7.4/bigsansar/contrib/sites/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         return self.domain.domain
 
     def get_absolute_url(self):
         if self.slug == 'styles':
             return "http://%s/%s.css" % (self.domain, self.slug)
         elif self.slug == 'sitemap':
             return "http://%s/%s.xml" % (self.domain, self.slug)
+        elif self.slug == 'script':
+            return "http://%s/%s.js" % (self.domain, self.slug)
         else:
             return "http://%s/%s" % (self.domain, self.slug)
 
     def delete(self, using=None, keep_parents=False):
         filename = 'templates' + '/' + str(self.domain.domain) + '/' + self.slug + '.html'
         full_url = os.path.join(BASE_DIR, filename)
         if os.path.exists(full_url):
```

### Comparing `Bigsansar-1.7.3/bigsansar/core/__init__.py` & `Bigsansar-1.7.4/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/core/init.py` & `Bigsansar-1.7.4/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/management/commands/createuser.py` & `Bigsansar-1.7.4/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.7.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/logo.png` & `Bigsansar-1.7.4/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/static/style.css` & `Bigsansar-1.7.4/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/404.html` & `Bigsansar-1.7.4/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/base.html` & `Bigsansar-1.7.4/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/blog_preview.html` & `Bigsansar-1.7.4/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/default.html` & `Bigsansar-1.7.4/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/defaultpage.html` & `Bigsansar-1.7.4/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/templates/parking.html` & `Bigsansar-1.7.4/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.3/bigsansar/urls.py` & `Bigsansar-1.7.4/bigsansar/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from django.urls import path
 
 from bigsansar import views
 
 
 urlpatterns = [
-    path('blog/preview/<id>', views.blog_preview, name = 'blog preview'),
     path('sitemap.xml', views.sitemap, name= 'sitemap'),
     path('script.js', views.getjavascript, name = 'javascripts'),
     path('styles.css', views.getcss, name = 'custom css'),
     path('', views.index, name='index'),
     path('<url>', views.pathviews, name='path'),
     path('<path>/<slug>', views.get_path_url, name = 'get_path_args'),
```

### Comparing `Bigsansar-1.7.3/bigsansar/views.py` & `Bigsansar-1.7.4/bigsansar/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,24 +96,28 @@
         template = loader.select_template((full_url, default_page))
         gethttp =  HttpResponse(template.render({}, request))
         gethttp['Content-Type'] = 'text/css'
         return gethttp
     
 
 def getjavascript(request):
+    default_page = 'script.html'
     try:
         current_site = get_current_site(request)
         db = domains.objects.get(domain=current_site)
-        get_javascript = javascript.objects.get(domain = db)
+        page = pages.objects.get(domain=db, slug='script')
+
     except:
         return render(request, '404.html')
     
     else:
-
-        getjavahttp = HttpResponse(get_javascript.javascript)
+        asp = 'templates/' + str(db.domain) + '/' + page.slug + '.html'
+        full_url = os.path.join(BASE_DIR, asp)
+        template = loader.select_template((full_url, default_page))
+        getjavahttp =  HttpResponse(template.render({}, request))
         getjavahttp['Content-Type'] = 'text/javascript'
         return getjavahttp
     
 
 def sitemap(request):
     default_page = 'sitemap.html'
 
@@ -128,18 +132,9 @@
     else:
         asp = 'templates/' + str(db.domain) + '/' + page.slug + '.html'
         full_url = os.path.join(BASE_DIR, asp)
         template = loader.select_template((full_url, default_page))
         getsitemaphttp =  HttpResponse(template.render({}, request))
         getsitemaphttp['Content-Type'] = 'application/xml'
         return getsitemaphttp
+    
 
-
-def blog_preview(request,id):
-    try:
-        current_site = get_current_site(request)
-        db = domains.objects.get(domain=current_site)
-        get_post = post.objects.get(pk=id, domain=db)
-    except:
-        return render(request, '404.html')
-    else:
-        return render(request, 'blog_preview.html', {'title': get_post.title,'thumbnails': get_post.thumbnails, 'content': get_post.body})
```

### Comparing `Bigsansar-1.7.3/setup.py` & `Bigsansar-1.7.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.7.3",
+    version="1.7.4",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

