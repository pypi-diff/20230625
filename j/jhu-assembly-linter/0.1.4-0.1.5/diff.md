# Comparing `tmp/jhu_assembly_linter-0.1.4.tar.gz` & `tmp/jhu_assembly_linter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhu_assembly_linter-0.1.4.tar", max compression
+gzip compressed data, was "jhu_assembly_linter-0.1.5.tar", max compression
```

## Comparing `jhu_assembly_linter-0.1.4.tar` & `jhu_assembly_linter-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1030 2023-06-25 01:48:17.976931 jhu_assembly_linter-0.1.4/README.md
--rw-r--r--   0        0        0     1267 2023-06-25 02:37:42.696521 jhu_assembly_linter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      883 2023-06-25 02:34:32.637051 jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/cmd.py
--rw-r--r--   0        0        0     1289 2023-06-25 01:35:15.960826 jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/finding.py
--rw-r--r--   0        0        0    10955 2023-06-25 01:40:31.271171 jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/linter.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 jhu_assembly_linter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1028 2023-06-25 17:37:44.047088 jhu_assembly_linter-0.1.5/README.md
+-rw-r--r--   0        0        0     1267 2023-06-25 17:48:23.776176 jhu_assembly_linter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      883 2023-06-25 02:34:32.637051 jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/cmd.py
+-rw-r--r--   0        0        0     1289 2023-06-25 01:35:15.960826 jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/finding.py
+-rw-r--r--   0        0        0    11023 2023-06-25 17:47:41.409971 jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/linter.py
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 jhu_assembly_linter-0.1.5/PKG-INFO
```

### Comparing `jhu_assembly_linter-0.1.4/README.md` & `jhu_assembly_linter-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -31,20 +31,19 @@
 
 To lint a whole directory:
 
 ```
 find . -name "*.s" | xargs -I{} jhu-assembly-linter  {}
 ```
 
-SOON TO BE IMPLEMENTED:
-To add a pre-commit hook:
+To add a pre-commit hook to you repo:
 ```
 repos:
 -   repo: https://github.com/LogstonGradSchool/JhuAssemblyStyleLinter
-    rev: v0.1.0
+    rev: <latest version>
     hooks:
     -   id: jhu-assembly-linter
 ```
 
 ### Tests
 
 ```
```

### Comparing `jhu_assembly_linter-0.1.4/pyproject.toml` & `jhu_assembly_linter-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jhu-assembly-linter"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Linter for JHU's Assembly Classes"
 license = "MIT"
 authors = ["Paul Logston <pbulkle1@jh.edu>"]
 maintainers = ["Paul Logston <pbulkle1@jh.edu>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/jhu-assembly-linter/"
 repository = "https://github.com/LogstonGradSchool/JhuAssemblyStyleLinter"
```

### Comparing `jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/cmd.py` & `jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/cmd.py`

 * *Files identical despite different names*

### Comparing `jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/finding.py` & `jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/finding.py`

 * *Files identical despite different names*

### Comparing `jhu_assembly_linter-0.1.4/src/jhu_assembly_linter/linter.py` & `jhu_assembly_linter-0.1.5/src/jhu_assembly_linter/linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,16 @@
                     chunk = line[pos:]
 
     def _check_line_empty_with_nonzero_space(self):
         """
         Check check that empty lines have no trailing whitespace.
         """
         for i, line in enumerate(self._lines, start=1):
-            if len(line) > 0 and len(line.strip()) == 0:
+            tmp_line = line.replace('\r', '').replace('\n', '')
+            if len(tmp_line) > 0 and len(line.strip()) == 0:
                 self._findings.append(Finding(
                     'Non-functional whitespace found.',
                     line_number=i,
                     columns=(0, len(line)),
                     source=line,
                 ))
```

### Comparing `jhu_assembly_linter-0.1.4/PKG-INFO` & `jhu_assembly_linter-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhu-assembly-linter
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Linter for JHU's Assembly Classes
 Home-page: https://pypi.org/project/jhu-assembly-linter/
 License: MIT
 Keywords: jhu,assembly,linter
 Author: Paul Logston
 Author-email: pbulkle1@jh.edu
 Maintainer: Paul Logston
@@ -54,20 +54,19 @@
 
 To lint a whole directory:
 
 ```
 find . -name "*.s" | xargs -I{} jhu-assembly-linter  {}
 ```
 
-SOON TO BE IMPLEMENTED:
-To add a pre-commit hook:
+To add a pre-commit hook to you repo:
 ```
 repos:
 -   repo: https://github.com/LogstonGradSchool/JhuAssemblyStyleLinter
-    rev: v0.1.0
+    rev: <latest version>
     hooks:
     -   id: jhu-assembly-linter
 ```
 
 ### Tests
 
 ```
```

