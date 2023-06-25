# Comparing `tmp/automation-utilities-1.1.1.tar.gz` & `tmp/automation-utilities-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.1.1.tar", last modified: Sun Jun 25 09:35:16 2023, max compression
+gzip compressed data, was "automation-utilities-1.1.2.tar", last modified: Sun Jun 25 09:39:36 2023, max compression
```

## Comparing `automation-utilities-1.1.1.tar` & `automation-utilities-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:35:16.271671 automation-utilities-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-25 09:35:16.267673 automation-utilities-1.1.1/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      142 2023-06-25 09:35:16.000000 automation-utilities-1.1.1/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-06-25 09:35:16.000000 automation-utilities-1.1.1/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 09:35:16.000000 automation-utilities-1.1.1/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 09:35:16.000000 automation-utilities-1.1.1/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-06-25 09:35:16.271671 automation-utilities-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 09:35:16.269673 automation-utilities-1.1.1/automation_utilities/
--rw-rw-rw-   0        0        0      619 2023-06-25 09:34:22.000000 automation-utilities-1.1.1/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      217 2023-06-25 09:28:55.000000 automation-utilities-1.1.1/automation_utilities/Files.py
--rw-rw-rw-   0        0        0        0 2023-06-24 16:08:22.000000 automation-utilities-1.1.1/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-25 09:35:16.271671 automation-utilities-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      256 2023-06-25 09:34:01.000000 automation-utilities-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.901282 automation-utilities-1.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.898282 automation-utilities-1.1.2/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 09:39:36.000000 automation-utilities-1.1.2/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-25 09:39:36.900282 automation-utilities-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 09:39:36.899283 automation-utilities-1.1.2/automation_utilities/
+-rw-rw-rw-   0        0        0      818 2023-06-25 09:38:36.000000 automation-utilities-1.1.2/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:39:36.901282 automation-utilities-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-25 09:39:30.000000 automation-utilities-1.1.2/setup.py
```

### Comparing `automation-utilities-1.1.1/automation_utilities/Data.py` & `automation-utilities-1.1.2/automation_utilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,7 +16,18 @@
             Data.lock.acquire()
             self.data[key] += 1
             json.dump(self.data, open(self.file_name, 'w'), indent=2)
             Data.lock.release()
             return self.data[key] - 1
         else:
             return self.data[key]
+
+
+class Files:
+
+    lock = threading.Lock()
+
+    @staticmethod
+    def add(text: str, to: str):
+        Files.lock.acquire()
+        open(to, 'a').write(text)
+        Files.lock.release()
```

