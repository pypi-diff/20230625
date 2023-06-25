# Comparing `tmp/liitos-2023.6.22.tar.gz` & `tmp/liitos-2023.6.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liitos-2023.6.22.tar", last modified: Thu Jun 22 18:40:35 2023, max compression
+gzip compressed data, was "liitos-2023.6.25.tar", last modified: Sun Jun 25 18:43:23 2023, max compression
```

## Comparing `liitos-2023.6.22.tar` & `liitos-2023.6.25.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.450073 liitos-2023.6.22/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.6.22/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.6.22/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-22 18:40:35.449924 liitos-2023.6.22/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.6.22/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.433150 liitos-2023.6.22/liitos/
--rw-r--r--   0 ruth       (501) staff       (20)     5016 2023-06-22 18:39:03.000000 liitos-2023.6.22/liitos/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.6.22/liitos/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     5052 2023-06-22 18:04:59.000000 liitos-2023.6.22/liitos/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1856 2023-06-22 17:55:57.000000 liitos-2023.6.22/liitos/captions.py
--rw-r--r--   0 ruth       (501) staff       (20)     6830 2023-06-22 18:04:41.000000 liitos-2023.6.22/liitos/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)    10347 2023-06-22 17:56:51.000000 liitos-2023.6.22/liitos/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    31870 2023-06-22 18:05:37.000000 liitos-2023.6.22/liitos/concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.6.22/liitos/configure.py
--rw-r--r--   0 ruth       (501) staff       (20)     1849 2023-06-22 17:57:21.000000 liitos-2023.6.22/liitos/description_lists.py
--rw-r--r--   0 ruth       (501) staff       (20)     2018 2023-06-17 18:14:28.000000 liitos-2023.6.22/liitos/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     1725 2023-06-22 17:58:10.000000 liitos-2023.6.22/liitos/figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    12919 2023-06-22 18:04:28.000000 liitos-2023.6.22/liitos/gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     4406 2023-06-22 17:58:35.000000 liitos-2023.6.22/liitos/labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.6.22/liitos/liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    41823 2023-06-22 17:54:03.000000 liitos-2023.6.22/liitos/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.6.22/liitos/patch.py
--rw-r--r--   0 ruth       (501) staff       (20)    19019 2023-06-22 18:05:07.000000 liitos-2023.6.22/liitos/render.py
--rw-r--r--   0 ruth       (501) staff       (20)    25142 2023-06-22 17:59:43.000000 liitos-2023.6.22/liitos/tables.py
--rw-r--r--   0 ruth       (501) staff       (20)     1548 2023-06-22 18:00:40.000000 liitos-2023.6.22/liitos/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.440016 liitos-2023.6.22/liitos/templates/
--rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.6.22/liitos/templates/approvals.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1283 2023-06-17 17:00:35.000000 liitos-2023.6.22/liitos/templates/bookmatter.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.6.22/liitos/templates/changes.yml
--rw-r--r--   0 ruth       (501) staff       (20)      889 2023-05-10 17:17:37.000000 liitos-2023.6.22/liitos/templates/driver.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)       90 2023-06-17 17:58:54.000000 liitos-2023.6.22/liitos/templates/layout.yml
--rw-r--r--   0 ruth       (501) staff       (20)       97 2023-06-17 17:49:55.000000 liitos-2023.6.22/liitos/templates/meta-patch.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1516 2023-06-17 17:52:06.000000 liitos-2023.6.22/liitos/templates/meta.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.6.22/liitos/templates/metadata.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.6.22/liitos/templates/mkdocs.yml.in
--rw-r--r--   0 ruth       (501) staff       (20)     1347 2023-06-17 17:32:59.000000 liitos-2023.6.22/liitos/templates/publisher.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     9727 2023-06-17 17:26:10.000000 liitos-2023.6.22/liitos/templates/setup.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.6.22/liitos/templates/vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)     7522 2023-06-22 18:01:41.000000 liitos-2023.6.22/liitos/tools.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.435203 liitos-2023.6.22/liitos.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1292 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      179 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       15 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2753 2023-06-22 17:39:51.000000 liitos-2023.6.22/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-22 18:40:35.450112 liitos-2023.6.22/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.449597 liitos-2023.6.22/test/
--rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.6.22/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.6.22/test/test_captions.py
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.6.22/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     3728 2023-06-17 18:29:21.000000 liitos-2023.6.22/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.6.22/test/test_concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.6.22/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.6.22/test/test_figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    10514 2023-06-17 18:30:26.000000 liitos-2023.6.22/test/test_gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.6.22/test/test_labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.6.22/test/test_liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.6.22/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.6.22/test/test_patch.py
--rw-r--r--   0 ruth       (501) staff       (20)      575 2023-06-22 17:30:47.000000 liitos-2023.6.22/test/test_render.py
--rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.6.22/test/test_tables.py
--rw-r--r--   0 ruth       (501) staff       (20)      431 2023-06-17 18:28:31.000000 liitos-2023.6.22/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.6.22/test/test_tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-25 18:43:23.373557 liitos-2023.6.25/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.6.25/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.6.25/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-25 18:43:23.373289 liitos-2023.6.25/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.6.25/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-25 18:43:23.256543 liitos-2023.6.25/liitos/
+-rw-r--r--   0 ruth       (501) staff       (20)     5002 2023-06-25 18:40:12.000000 liitos-2023.6.25/liitos/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.6.25/liitos/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5052 2023-06-22 18:04:59.000000 liitos-2023.6.25/liitos/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1856 2023-06-22 17:55:57.000000 liitos-2023.6.25/liitos/captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6830 2023-06-22 18:04:41.000000 liitos-2023.6.25/liitos/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10347 2023-06-22 17:56:51.000000 liitos-2023.6.25/liitos/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    31870 2023-06-22 18:05:37.000000 liitos-2023.6.25/liitos/concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.6.25/liitos/configure.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1849 2023-06-22 17:57:21.000000 liitos-2023.6.25/liitos/description_lists.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2018 2023-06-17 18:14:28.000000 liitos-2023.6.25/liitos/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1725 2023-06-22 17:58:10.000000 liitos-2023.6.25/liitos/figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12919 2023-06-22 18:04:28.000000 liitos-2023.6.25/liitos/gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4406 2023-06-22 17:58:35.000000 liitos-2023.6.25/liitos/labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.6.25/liitos/liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    42884 2023-06-25 18:21:13.000000 liitos-2023.6.25/liitos/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.6.25/liitos/patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)    19019 2023-06-22 18:05:07.000000 liitos-2023.6.25/liitos/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)    25142 2023-06-22 17:59:43.000000 liitos-2023.6.25/liitos/tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1548 2023-06-22 18:00:40.000000 liitos-2023.6.25/liitos/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-25 18:43:23.349077 liitos-2023.6.25/liitos/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.6.25/liitos/templates/approvals.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1283 2023-06-17 17:00:35.000000 liitos-2023.6.25/liitos/templates/bookmatter.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.6.25/liitos/templates/changes.yml
+-rw-r--r--   0 ruth       (501) staff       (20)      889 2023-05-10 17:17:37.000000 liitos-2023.6.25/liitos/templates/driver.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)       90 2023-06-17 17:58:54.000000 liitos-2023.6.25/liitos/templates/layout.yml
+-rw-r--r--   0 ruth       (501) staff       (20)       97 2023-06-17 17:49:55.000000 liitos-2023.6.25/liitos/templates/meta-patch.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1613 2023-06-25 18:12:28.000000 liitos-2023.6.25/liitos/templates/meta.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.6.25/liitos/templates/metadata.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.6.25/liitos/templates/mkdocs.yml.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1347 2023-06-17 17:32:59.000000 liitos-2023.6.25/liitos/templates/publisher.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)    10134 2023-06-25 18:08:47.000000 liitos-2023.6.25/liitos/templates/setup.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.6.25/liitos/templates/vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     7522 2023-06-22 18:01:41.000000 liitos-2023.6.25/liitos/tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-25 18:43:23.268954 liitos-2023.6.25/liitos.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1292 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      179 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       15 2023-06-25 18:43:23.000000 liitos-2023.6.25/liitos.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2752 2023-06-25 18:39:20.000000 liitos-2023.6.25/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-25 18:43:23.373719 liitos-2023.6.25/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-25 18:43:23.372762 liitos-2023.6.25/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.6.25/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.6.25/test/test_captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.6.25/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3728 2023-06-17 18:29:21.000000 liitos-2023.6.25/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.6.25/test/test_concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.6.25/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.6.25/test/test_figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10514 2023-06-17 18:30:26.000000 liitos-2023.6.25/test/test_gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.6.25/test/test_labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.6.25/test/test_liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.6.25/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.6.25/test/test_patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)      575 2023-06-22 17:30:47.000000 liitos-2023.6.25/test/test_render.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.6.25/test/test_tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)      431 2023-06-17 18:28:31.000000 liitos-2023.6.25/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.6.25/test/test_tools.py
```

### Comparing `liitos-2023.6.22/LICENSE` & `liitos-2023.6.25/LICENSE`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/PKG-INFO` & `liitos-2023.6.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.6.22
+Version: 2023.6.25
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.6.22/README.md` & `liitos-2023.6.25/README.md`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/__init__.py` & `liitos-2023.6.25/liitos/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 import pathlib
 import shellingham  # type: ignore
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.6.22+parent.v2023.6.17-25-ga525df55'
-# [[[end]]] (checksum: e713b82096b77b208181225e7aa7082a)
+__version__ = '2023.6.25+parent.ga2a8921e'
+# [[[end]]] (checksum: afe822f28ae8e3e33a4052e9cff5789a)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Splice (Finnish liitos) contributions.'
 APP_ALIAS = 'liitos'
 APP_ENV = 'LIITOS'
```

### Comparing `liitos-2023.6.22/liitos/approvals.py` & `liitos-2023.6.25/liitos/approvals.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/captions.py` & `liitos-2023.6.25/liitos/captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/changes.py` & `liitos-2023.6.25/liitos/changes.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/cli.py` & `liitos-2023.6.25/liitos/cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/concat.py` & `liitos-2023.6.25/liitos/concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/configure.py` & `liitos-2023.6.25/liitos/configure.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/description_lists.py` & `liitos-2023.6.25/liitos/description_lists.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/eject.py` & `liitos-2023.6.25/liitos/eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/figures.py` & `liitos-2023.6.25/liitos/figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/gather.py` & `liitos-2023.6.25/liitos/gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/labels.py` & `liitos-2023.6.25/liitos/labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/meta.py` & `liitos-2023.6.25/liitos/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     'bold_font': 'ITCFranklinGothicStd-Demi',
     'italic_font': 'ITCFranklinGothicStd-BookIt',
     'bold_italic_font': 'ITCFranklinGothicStd-DemiIt',
     'main_font': 'ITCFranklinGothicStd-Book',
     'fixed_font_package': 'sourcecodepro',
     'code_fontsize': r'\scriptsize',
     'chosen_logo': '/opt/logo/liitos-logo.png',
+    'footer_outer_field_normal_pages': r'\theMetaPageNumPrefix { } \thepage { }',
     'adjustable_vertical_space': '2.5em',
 }
 ACROSS = {
     'eff_font_folder': '',
     'eff_font_suffix': '',
 }
 
@@ -328,14 +329,35 @@
         return text.replace(VALUE_SLOT, chosen_logo)
     else:
         log.warning(f'chosen_logo value missing ... setting default ({defaults["chosen_logo"]})')
         return text.replace(VALUE_SLOT, defaults['chosen_logo'])
 
 
 @no_type_check
+def weave_setup_footer_outer_field_normal_pages(
+    mapper: dict[str, Union[str, int, bool, None]],
+    text: str,
+) -> str:
+    """Weave in the footer_outer_field_normal_pages from mapper or default for driver.
+
+    Trigger is text.rstrip().endswith('%%_PATCH_%_NORMAL_%_PAGES_%_OUTER_%_FOOT_%_CONTENT_%_VALUE_%%')
+    """
+    defaults = {**WEAVE_DEFAULTS}
+    if mapper.get('footer_outer_field_normal_pages'):
+        footer_outer_field_normal_pages = mapper.get('footer_outer_field_normal_pages')
+        return text.replace(VALUE_SLOT, footer_outer_field_normal_pages)
+    else:
+        log.warning(
+            'footer_outer_field_normal_pages value missing ...'
+            f' setting default ({defaults["footer_outer_field_normal_pages"]})'
+        )
+        return text.replace(VALUE_SLOT, defaults['footer_outer_field_normal_pages'])
+
+
+@no_type_check
 def dispatch_setup_weaver(
     mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Dispatch the driver weaver by mapping to handled groups per source marker."""
     dispatch = {
         '%%_PATCH_%_FONT_%_PATH_%%': weave_setup_font_path,
@@ -343,14 +365,15 @@
         '%%_PATCH_%_BOLD_%_FONT_%%': weave_setup_bold_font,
         '%%_PATCH_%_ITALIC_%_FONT_%%': weave_setup_italic_font,
         '%%_PATCH_%_BOLDITALIC_%_FONT_%%': weave_setup_bold_italic_font,
         '%%_PATCH_%_MAIN_%_FONT_%%': weave_setup_main_font,
         '%%_PATCH_%_FIXED_%_FONT_%_PACKAGE_%%': weave_setup_fixed_font_package,
         '%%_PATCH_%_CODE_%_FONTSIZE_%%': weave_setup_code_fontsize,
         '%%_PATCH_%_CHOSEN_%_LOGO_%%': weave_setup_chosen_logo,
+        '%%_PATCH_%_NORMAL_%_PAGES_%_OUTER_%_FOOT_%_CONTENT_%_VALUE_%%': weave_setup_footer_outer_field_normal_pages,
     }
     for trigger, weaver in dispatch.items():
         if text.rstrip().endswith(trigger):
             return weaver(mapper, text)
     return text
```

### Comparing `liitos-2023.6.22/liitos/patch.py` & `liitos-2023.6.25/liitos/patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/render.py` & `liitos-2023.6.25/liitos/render.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/tables.py` & `liitos-2023.6.25/liitos/tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/template_loader.py` & `liitos-2023.6.25/liitos/template_loader.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/bookmatter.tex.in` & `liitos-2023.6.25/liitos/templates/bookmatter.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/driver.tex.in` & `liitos-2023.6.25/liitos/templates/driver.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/meta.yml` & `liitos-2023.6.25/liitos/templates/meta.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     change_log_revision_label: Rev.
     chosen_logo: /opt/logo/liitos-logo.png
     code_fontsize: \scriptsize
     fixed_font_package: sourcecodepro
     font_path: /opt/fonts/
     font_suffix: .otf
     footer_frame_note: null
+    footer_outer_field_normal_pages: \theMetaPageNumPrefix { } \thepage { } / \pageref{LastPage}
     footer_page_number_prefix: Page
     has_approvals: true
     has_changes: true
     has_notices: true
     header_date: null
     header_date_enable_auto: true
     header_date_label: 'Date:'
```

### Comparing `liitos-2023.6.22/liitos/templates/metadata.tex.in` & `liitos-2023.6.25/liitos/templates/metadata.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/mkdocs.yml.in` & `liitos-2023.6.25/liitos/templates/mkdocs.yml.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/publisher.tex.in` & `liitos-2023.6.25/liitos/templates/publisher.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/templates/setup.tex.in` & `liitos-2023.6.25/liitos/templates/setup.tex.in`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,37 @@
   openlevel=2,
   numbered,
 }
 \usepackage{microtype}
 \usepackage{ragged2e}
 \RaggedRight
 
+\usepackage{lastpage}
 \usepackage{amsmath,amssymb}
 \usepackage{setspace}
 \setstretch{1.2}
 \usepackage{iftex}
 \usepackage{unicode-math}
 \usepackage{fontspec}
 \setmainfont[
     Path = VALUE.SLOT,%%_PATCH_%_FONT_%_PATH_%%
     Extension = VALUE.SLOT,%%_PATCH_%_FONT_%_SUFFIX_%%
     Ligatures = TeX,
     BoldFont={VALUE.SLOT},%%_PATCH_%_BOLD_%_FONT_%%
     ItalicFont={VALUE.SLOT},%%_PATCH_%_ITALIC_%_FONT_%%
     BoldItalicFont={VALUE.SLOT}%%_PATCH_%_BOLDITALIC_%_FONT_%%
 ]{VALUE.SLOT}%%_PATCH_%_MAIN_%_FONT_%%
+\setsansfont[
+    Path = VALUE.SLOT,%%_PATCH_%_FONT_%_PATH_%%
+    Extension = VALUE.SLOT,%%_PATCH_%_FONT_%_SUFFIX_%%
+    Ligatures = TeX,
+    BoldFont={VALUE.SLOT},%%_PATCH_%_BOLD_%_FONT_%%
+    ItalicFont={VALUE.SLOT},%%_PATCH_%_ITALIC_%_FONT_%%
+    BoldItalicFont={VALUE.SLOT}%%_PATCH_%_BOLDITALIC_%_FONT_%%
+]{VALUE.SLOT}%%_PATCH_%_MAIN_%_FONT_%%
 \usepackage{VALUE.SLOT}%%_PATCH_%_FIXED_%_FONT_%_PACKAGE_%%
 
 % use upquote if available, for straight quotes in verbatim environments
 \IfFileExists{upquote.sty}{\usepackage{upquote}}{}
 \IfFileExists{microtype.sty}{% use microtype if available
   \usepackage[]{microtype}
   \UseMicrotypeSet[protrusion]{basicmath} % disable protrusion for tt fonts
@@ -197,15 +206,15 @@
   \ohead*{%%
     \vskip -10mm\begin{tabular*}{64mm}[t]{@{}p{15mm}p{55mm}@{}}%% ... tuned ... effective 70mm
       \hfill & \hbox{\hspace{-5mm}\includegraphics[width=55mm]{\theChosenLogo}} \\
     \end{tabular*}
   }
   \ifoot*{\upshape{\footnotesize \theMetaPropInfo}}
   \cfoot*{}
-  \ofoot*{\upshape{\footnotesize \theMetaPageNumPrefix { } \thepage}}
+  \ofoot*{\upshape{\footnotesize VALUE.SLOT}}%%_PATCH_%_NORMAL_%_PAGES_%_OUTER_%_FOOT_%_CONTENT_%_VALUE_%%
   \setlength{\headheight}{29.6mm}%% ... tuned
   \setlength{\footheight}{18mm}%% ... tuned
 }
 
 % The liitos title page header and footer style:
 \newpairofpagestyles{liitos-title-header-footer}{%%
   \clearpairofpagestyles
```

### Comparing `liitos-2023.6.22/liitos/templates/vocabulary.yml` & `liitos-2023.6.25/liitos/templates/vocabulary.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos/tools.py` & `liitos-2023.6.25/liitos/tools.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/liitos.egg-info/PKG-INFO` & `liitos-2023.6.25/liitos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.6.22
+Version: 2023.6.25
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.6.22/liitos.egg-info/SOURCES.txt` & `liitos-2023.6.25/liitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/pyproject.toml` & `liitos-2023.6.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liitos"
-version = "2023.6.22"
+version = "2023.6.25"
 description = "Splice (Finnish liitos) contributions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -115,8 +115,7 @@
 [tool.mypy]
 strict = true
 implicit_reexport = true
 
 [tool.pytest]
 testpaths = "test"
 filterwarnings = "error"
-
```

### Comparing `liitos-2023.6.22/test/test_captions.py` & `liitos-2023.6.25/test/test_captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_cli.py` & `liitos-2023.6.25/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_concat.py` & `liitos-2023.6.25/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_eject.py` & `liitos-2023.6.25/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_figures.py` & `liitos-2023.6.25/test/test_figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_gather.py` & `liitos-2023.6.25/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_labels.py` & `liitos-2023.6.25/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_meta.py` & `liitos-2023.6.25/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_patch.py` & `liitos-2023.6.25/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_render.py` & `liitos-2023.6.25/test/test_render.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_tables.py` & `liitos-2023.6.25/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.22/test/test_tools.py` & `liitos-2023.6.25/test/test_tools.py`

 * *Files identical despite different names*

