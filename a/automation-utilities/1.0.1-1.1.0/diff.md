# Comparing `tmp/automation-utilities-1.0.1.tar.gz` & `tmp/automation-utilities-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.0.1.tar", last modified: Sat Jun 24 16:37:08 2023, max compression
+gzip compressed data, was "automation-utilities-1.1.0.tar", last modified: Sun Jun 25 09:31:08 2023, max compression
```

## Comparing `automation-utilities-1.0.1.tar` & `automation-utilities-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:37:08.373666 automation-utilities-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-24 16:37:08.369665 automation-utilities-1.0.1/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      145 2023-06-24 16:37:08.000000 automation-utilities-1.0.1/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-24 16:37:08.000000 automation-utilities-1.0.1/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:37:08.000000 automation-utilities-1.0.1/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-24 16:37:08.000000 automation-utilities-1.0.1/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      145 2023-06-24 16:37:08.372667 automation-utilities-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 16:37:08.371671 automation-utilities-1.0.1/automation_utilities/
--rw-rw-rw-   0        0        0      619 2023-06-24 16:08:22.000000 automation-utilities-1.0.1/automation_utilities/Data.py
--rw-rw-rw-   0        0        0        0 2023-06-24 16:08:22.000000 automation-utilities-1.0.1/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-24 16:37:08.373666 automation-utilities-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      259 2023-06-24 16:35:38.000000 automation-utilities-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:31:08.487383 automation-utilities-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:31:08.484385 automation-utilities-1.1.0/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      142 2023-06-25 09:31:08.000000 automation-utilities-1.1.0/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-25 09:31:08.000000 automation-utilities-1.1.0/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:31:08.000000 automation-utilities-1.1.0/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 09:31:08.000000 automation-utilities-1.1.0/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-06-25 09:31:08.487383 automation-utilities-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 09:31:08.486384 automation-utilities-1.1.0/automation_utilities/
+-rw-rw-rw-   0        0        0      619 2023-06-24 16:08:22.000000 automation-utilities-1.1.0/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 16:08:22.000000 automation-utilities-1.1.0/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:31:08.487383 automation-utilities-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      256 2023-06-25 09:30:32.000000 automation-utilities-1.1.0/setup.py
```

### Comparing `automation-utilities-1.0.1/automation_utilities/Data.py` & `automation-utilities-1.1.0/automation_utilities/Data.py`

 * *Files identical despite different names*

