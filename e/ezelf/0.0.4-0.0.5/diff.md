# Comparing `tmp/ezelf-0.0.4.tar.gz` & `tmp/ezelf-0.0.5.tar.gz`

## Comparing `ezelf-0.0.4.tar` & `ezelf-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.4/tox.ini
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/fake.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/ezelf/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/ezelf/__main__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/ezelf/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/ezelf/sync/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ezelf-0.0.4/src/ezelf/sync/ezpie.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ezelf-0.0.4/tests/test_simple.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.4/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.4/README.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 ezelf-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 ezelf-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.0.5/tox.ini
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/fake.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/ezelf/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/ezelf/__main__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/ezelf/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/ezelf/sync/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ezelf-0.0.5/src/ezelf/sync/ezpie.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ezelf-0.0.5/tests/test_simple.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ezelf-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.0.5/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.0.5/README.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 ezelf-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 ezelf-0.0.5/PKG-INFO
```

### Comparing `ezelf-0.0.4/tox.ini` & `ezelf-0.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.4/.github/workflows/release.yml` & `ezelf-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.4/.github/workflows/test.yml` & `ezelf-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.4/.gitignore` & `ezelf-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.4/LICENSE` & `ezelf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezelf-0.0.4/PKG-INFO` & `ezelf-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezelf
-Version: 0.0.4
+Version: 0.0.5
 Summary: A elf for ezpie
 License: MIT License
         
         Copyright (c) 2023 ez-pie
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

