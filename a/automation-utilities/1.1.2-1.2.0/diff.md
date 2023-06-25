# Comparing `tmp/automation-utilities-1.1.2.tar.gz` & `tmp/automation-utilities-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.1.2.tar", last modified: Sun Jun 25 09:39:36 2023, max compression
+gzip compressed data, was "automation-utilities-1.2.0.tar", last modified: Sun Jun 25 18:09:46 2023, max compression
```

## Comparing `automation-utilities-1.1.2.tar` & `automation-utilities-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.901282 automation-utilities-1.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.898282 automation-utilities-1.1.2/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-25 09:39:36.900282 automation-utilities-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.899283 automation-utilities-1.1.2/automation_utilities/
--rw-rw-rw-   0        0        0      818 2023-06-25 09:38:36.000000 automation-utilities-1.1.2/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-25 09:39:36.901282 automation-utilities-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-25 09:39:30.000000 automation-utilities-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.017130 automation-utilities-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.014120 automation-utilities-1.2.0/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 18:09:45.000000 automation-utilities-1.2.0/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-25 18:09:46.016133 automation-utilities-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 18:09:46.015131 automation-utilities-1.2.0/automation_utilities/
+-rw-rw-rw-   0        0        0     1053 2023-06-25 18:09:28.000000 automation-utilities-1.2.0/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:09:46.017130 automation-utilities-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-25 18:09:29.000000 automation-utilities-1.2.0/setup.py
```

### Comparing `automation-utilities-1.1.2/automation_utilities/__init__.py` & `automation-utilities-1.2.0/automation_utilities/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     """This class was made to deal with data used in automation projects"""
 
     lock = threading.Lock()
 
     def __init__(self, file_name: str):
         self.file_name = file_name
         self.data = json.load(open(file_name, 'r'))
+        self._privte = 15
 
     def get(self, key):
         if isinstance(self.data[key], int):
             Data.lock.acquire()
             self.data[key] += 1
             json.dump(self.data, open(self.file_name, 'w'), indent=2)
             Data.lock.release()
@@ -23,11 +24,20 @@
 
 
 class Files:
 
     lock = threading.Lock()
 
     @staticmethod
-    def add(text: str, to: str):
+    def add(text: str, to: str) -> None:
         Files.lock.acquire()
         open(to, 'a').write(text)
         Files.lock.release()
+
+
+class Input:
+    @staticmethod
+    def int_input(prompt: str, default: int) -> int:
+        try:
+            return int(input(prompt))
+        except IndexError:
+            return default
```

