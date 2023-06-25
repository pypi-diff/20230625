# Comparing `tmp/jhu_assembly_linter-0.1.6.tar.gz` & `tmp/jhu_assembly_linter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhu_assembly_linter-0.1.6.tar", max compression
+gzip compressed data, was "jhu_assembly_linter-0.1.7.tar", max compression
```

## Comparing `jhu_assembly_linter-0.1.6.tar` & `jhu_assembly_linter-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1028 2023-06-25 17:37:44.047088 jhu_assembly_linter-0.1.6/README.md
--rw-r--r--   0        0        0     1267 2023-06-25 17:58:39.957257 jhu_assembly_linter-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      883 2023-06-25 02:34:32.637051 jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/cmd.py
--rw-r--r--   0        0        0     1289 2023-06-25 01:35:15.960826 jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/finding.py
--rw-r--r--   0        0        0    11024 2023-06-25 17:58:22.634269 jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/linter.py
--rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 jhu_assembly_linter-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1028 2023-06-25 17:37:44.047088 jhu_assembly_linter-0.1.7/README.md
+-rw-r--r--   0        0        0     1267 2023-06-25 18:02:26.718523 jhu_assembly_linter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-06-25 18:01:14.751383 jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/cmd.py
+-rw-r--r--   0        0        0     1289 2023-06-25 01:35:15.960826 jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/finding.py
+-rw-r--r--   0        0        0    11024 2023-06-25 17:58:22.634269 jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/linter.py
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 jhu_assembly_linter-0.1.7/PKG-INFO
```

### Comparing `jhu_assembly_linter-0.1.6/README.md` & `jhu_assembly_linter-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jhu_assembly_linter-0.1.6/pyproject.toml` & `jhu_assembly_linter-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jhu-assembly-linter"
-version = "0.1.6"
+version = "0.1.7"
 description = "A Linter for JHU's Assembly Classes"
 license = "MIT"
 authors = ["Paul Logston <pbulkle1@jh.edu>"]
 maintainers = ["Paul Logston <pbulkle1@jh.edu>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/jhu-assembly-linter/"
 repository = "https://github.com/LogstonGradSchool/JhuAssemblyStyleLinter"
```

### Comparing `jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/cmd.py` & `jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,18 @@
         nargs='*',
         help='Filenames to lint',
     )
     args = parser.parse_args(argv)
 
     return_code = 0
     for filename in args.files:
-        print(f'--- {filename}')
         linter = Linter(filename)
         linter.lint()
-        for f in linter.findings:
-            print(f)
+
         if linter.findings:
+            print(f'--- {filename}')
+            for f in linter.findings:
+                print(f)
+
             return_code = 1
 
     return return_code
```

### Comparing `jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/finding.py` & `jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/finding.py`

 * *Files identical despite different names*

### Comparing `jhu_assembly_linter-0.1.6/src/jhu_assembly_linter/linter.py` & `jhu_assembly_linter-0.1.7/src/jhu_assembly_linter/linter.py`

 * *Files identical despite different names*

### Comparing `jhu_assembly_linter-0.1.6/PKG-INFO` & `jhu_assembly_linter-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhu-assembly-linter
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Linter for JHU's Assembly Classes
 Home-page: https://pypi.org/project/jhu-assembly-linter/
 License: MIT
 Keywords: jhu,assembly,linter
 Author: Paul Logston
 Author-email: pbulkle1@jh.edu
 Maintainer: Paul Logston
```

