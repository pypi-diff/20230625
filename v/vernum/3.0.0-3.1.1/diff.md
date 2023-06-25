# Comparing `tmp/vernum-3.0.0.tar.gz` & `tmp/vernum-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernum-3.0.0.tar", last modified: Thu Jun 15 22:27:17 2023, max compression
+gzip compressed data, was "vernum-3.1.1.tar", last modified: Sun Jun 25 02:21:36 2023, max compression
```

## Comparing `vernum-3.0.0.tar` & `vernum-3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.448186 vernum-3.0.0/
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 22:24:30.000000 vernum-3.0.0/.version
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-06-15 03:00:08.000000 vernum-3.0.0/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-15 22:27:17.447683 vernum-3.0.0/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1111 2023-06-15 03:00:08.000000 vernum-3.0.0/README.md
--rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 22:26:45.000000 vernum-3.0.0/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 22:27:17.448308 vernum-3.0.0/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.436440 vernum-3.0.0/vernum/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 03:00:08.000000 vernum-3.0.0/vernum/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-06-15 21:44:28.000000 vernum-3.0.0/vernum/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2203 2023-06-15 22:16:32.000000 vernum-3.0.0/vernum/handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.447025 vernum-3.0.0/vernum.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      250 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       47 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/top_level.txt
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.374286 vernum-3.1.1/
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-25 02:21:13.000000 vernum-3.1.1/.version
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-06-15 03:00:08.000000 vernum-3.1.1/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-25 02:21:36.373787 vernum-3.1.1/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1111 2023-06-15 03:00:08.000000 vernum-3.1.1/README.md
+-rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-25 02:11:54.000000 vernum-3.1.1/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-25 02:21:36.374419 vernum-3.1.1/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.368782 vernum-3.1.1/vernum/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 03:00:08.000000 vernum-3.1.1/vernum/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-06-25 02:07:23.000000 vernum-3.1.1/vernum/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2349 2023-06-25 02:07:23.000000 vernum-3.1.1/vernum/handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-25 02:21:36.373206 vernum-3.1.1/vernum.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      250 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       47 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-06-25 02:21:36.000000 vernum-3.1.1/vernum.egg-info/top_level.txt
```

### Comparing `vernum-3.0.0/LICENSE` & `vernum-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vernum-3.0.0/PKG-INFO` & `vernum-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 3.0.0
+Version: 3.1.1
 Summary: Easy semantic versioning for projects in Git
 Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vernum-3.0.0/README.md` & `vernum-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vernum-3.0.0/pyproject.toml` & `vernum-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vernum-3.0.0/vernum/handler.py` & `vernum-3.1.1/vernum/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 LEVELS = ['major','minor','patch']
 
 @dataclass
 class Handler:
 
     dry_run:bool = False
+    push_tag:bool = False
 
     def git(self, command, dry_ok=False):
         print('git ' + command)
         if dry_ok or not self.dry_run:
             result = run(['git'] + command.split(),
                                     capture_output=True, text=True)
             if result.returncode != 0:
@@ -50,19 +51,21 @@
 
     def do(self, level=None):
         status = self.git('status -s')
         if status:
             raise SystemExit('Git working tree must be clean to update version')
         version = self.update_version(level)
         print('Version updated to ' + version)
-        print(self.git(f"tag -a v{version} -m v{version}"))
-        print(self.git('push --tags'))
+        if self.push_tag:
+            print(self.git(f"tag -a v{version} -m v{version}"))
+            print(self.git('push --tags'))
         print('Release complete')
 
 def main():
     parser = ArgumentParser()
     parser.add_argument('level', choices=LEVELS, default='patch', nargs='?')
-    parser.add_argument('--dry-run','-n', action='store_true')
+    parser.add_argument('--dry-run', '-n', action='store_true')
+    parser.add_argument('--push-tag', '-t', action='store_true')
     namespace = parser.parse_args()
-    handler = Handler(namespace.dry_run)
+    handler = Handler(namespace.dry_run, namespace.push_tag)
     handler.do(namespace.level)
```

### Comparing `vernum-3.0.0/vernum.egg-info/PKG-INFO` & `vernum-3.1.1/vernum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 3.0.0
+Version: 3.1.1
 Summary: Easy semantic versioning for projects in Git
 Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

