# Comparing `tmp/automation-utilities-1.2.0.tar.gz` & `tmp/automation-utilities-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.2.0.tar", last modified: Sun Jun 25 18:09:46 2023, max compression
+gzip compressed data, was "automation-utilities-1.2.1.tar", last modified: Sun Jun 25 18:37:41 2023, max compression
```

## Comparing `automation-utilities-1.2.0.tar` & `automation-utilities-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.017130 automation-utilities-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.014120 automation-utilities-1.2.0/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-25 18:09:46.016133 automation-utilities-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.015131 automation-utilities-1.2.0/automation_utilities/
--rw-rw-rw-   0        0        0     1053 2023-06-25 18:09:28.000000 automation-utilities-1.2.0/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-25 18:09:46.017130 automation-utilities-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-25 18:09:29.000000 automation-utilities-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:41.876850 automation-utilities-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:41.874851 automation-utilities-1.2.1/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-25 18:37:41.000000 automation-utilities-1.2.1/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-06-25 18:37:41.000000 automation-utilities-1.2.1/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:37:41.000000 automation-utilities-1.2.1/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 18:37:41.000000 automation-utilities-1.2.1/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-25 18:37:41.876850 automation-utilities-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 18:37:41.874851 automation-utilities-1.2.1/automation_utilities/
+-rw-rw-rw-   0        0        0     1054 2023-06-25 18:32:18.000000 automation-utilities-1.2.1/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:37:41.876850 automation-utilities-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-25 18:32:19.000000 automation-utilities-1.2.1/setup.py
```

### Comparing `automation-utilities-1.2.0/automation_utilities/__init__.py` & `automation-utilities-1.2.1/automation_utilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     @staticmethod
     def add(text: str, to: str) -> None:
         Files.lock.acquire()
         open(to, 'a').write(text)
         Files.lock.release()
 
 
-class Input:
+class Inputs:
     @staticmethod
     def int_input(prompt: str, default: int) -> int:
         try:
             return int(input(prompt))
         except IndexError:
             return default
```

