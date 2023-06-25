# Comparing `tmp/vernum-3.1.1.tar.gz` & `tmp/vernum-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernum-3.1.1.tar", last modified: Sun Jun 25 02:21:36 2023, max compression
+gzip compressed data, was "vernum-3.1.5.tar", last modified: Sun Jun 25 03:19:57 2023, max compression
```

## Comparing `vernum-3.1.1.tar` & `vernum-3.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.374286 vernum-3.1.1/
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-25 02:21:13.000000 vernum-3.1.1/.version
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-06-15 03:00:08.000000 vernum-3.1.1/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-25 02:21:36.373787 vernum-3.1.1/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1111 2023-06-15 03:00:08.000000 vernum-3.1.1/README.md
--rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-25 02:11:54.000000 vernum-3.1.1/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-25 02:21:36.374419 vernum-3.1.1/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.368782 vernum-3.1.1/vernum/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 03:00:08.000000 vernum-3.1.1/vernum/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-06-25 02:07:23.000000 vernum-3.1.1/vernum/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2349 2023-06-25 02:07:23.000000 vernum-3.1.1/vernum/handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.373206 vernum-3.1.1/vernum.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      250 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       47 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.283413 vernum-3.1.5/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-25 03:19:25.000000 vernum-3.1.5/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-25 03:19:47.000000 vernum-3.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-06-25 03:19:57.283413 vernum-3.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-06-25 03:19:47.000000 vernum-3.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-25 03:19:47.000000 vernum-3.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 03:19:57.283413 vernum-3.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.282413 vernum-3.1.5/vernum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.283413 vernum-3.1.5/vernum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/top_level.txt
```

### Comparing `vernum-3.1.1/LICENSE` & `vernum-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vernum-3.1.1/PKG-INFO` & `vernum-3.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-Metadata-Version: 2.1
-Name: vernum
-Version: 3.1.1
-Summary: Easy semantic versioning for projects in Git
-Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# VERNUM
+# VerNum
 
 Version numbering and git tagging for project releases
 
 ## Installation
 
 Requires Python 3 to run the command; your project can be anything.
 
 ```
-sudo pip3 install vernum
+pip3 install vernum
 ```
 
 ## What it does
 
 - Maintain a file at the root of a project called simply "version" with the version number, e.g. "5.6.2"
 - Update the release file for major, minor, or patch releases - patch is the default
-- Always create and push a git tag with the version number in it
+- Optionally create and push a git tag with the version number in it
 
 ## Usage
 
 Requirements:
 
 - CD to the root of the project before running it
 - Be on the branch that you use for releases (i.e. `master`)
@@ -38,8 +28,15 @@
 
 - `vernum major` to update the major version level, i.e. 5.6.2 -> 6.0.0
 - `vernum minor` to update the minor version level, i.e. 5.6.2 -> 5.7.0
 - `vernum patch` to update the patch version level, i.e. 5.6.2 -> 5.6.3
 
 Note that `patch` is the default so you can just say `vernum` for a patch release
 
-Reference the `version` file within your code when it needs to know the version. For example, see `setup.py` in this project.
+Reference the `.version` file within your code when it needs to know the version. For example, see `pyproject.toml` in this project.
+
+VerNum looks at the most recent git tag that fits the format, then increments it appropriately. It also generates the `.version` file.
+
+Options:
+
+- `--push-tag` create a git tag for the version and push it
+- `--dry-run` just output the information; don't do anything
```

### Comparing `vernum-3.1.1/pyproject.toml` & `vernum-3.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vernum-3.1.1/vernum/handler.py` & `vernum-3.1.5/vernum/handler.py`

 * *Files identical despite different names*

