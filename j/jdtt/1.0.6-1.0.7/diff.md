# Comparing `tmp/jdtt-1.0.6.tar.gz` & `tmp/jdtt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtt-1.0.6.tar", last modified: Sat Jun 24 21:15:09 2023, max compression
+gzip compressed data, was "jdtt-1.0.7.tar", last modified: Sun Jun 25 06:36:03 2023, max compression
```

## Comparing `jdtt-1.0.6.tar` & `jdtt-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:09.642703 jdtt-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-24 21:15:09.642703 jdtt-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 21:14:58.000000 jdtt-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-24 21:14:58.000000 jdtt-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-24 21:15:09.646703 jdtt-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:09.642703 jdtt-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:09.642703 jdtt-1.0.6/src/jdtt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 21:14:58.000000 jdtt-1.0.6/src/jdtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-24 21:14:58.000000 jdtt-1.0.6/src/jdtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-24 21:14:58.000000 jdtt-1.0.6/src/jdtt/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:15:09.642703 jdtt-1.0.6/src/jdtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 21:15:09.000000 jdtt-1.0.6/src/jdtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 06:36:03.317344 jdtt-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 06:35:50.000000 jdtt-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 06:35:50.000000 jdtt-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 06:36:03.321344 jdtt-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/jdtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/jdtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/top_level.txt
```

### Comparing `jdtt-1.0.6/PKG-INFO` & `jdtt-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdtt
-Version: 1.0.6
+Version: 1.0.7
 Summary: JSON to programming language schema converter
 Author: Joey Shi
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
```

### Comparing `jdtt-1.0.6/setup.cfg` & `jdtt-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.6/src/jdtt/__main__.py` & `jdtt-1.0.7/src/jdtt/__main__.py`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.6/src/jdtt/conversion.py` & `jdtt-1.0.7/src/jdtt/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     members: Dict[str, str]
 
 class TargetLanguage(Enum):
     PYTHON = 1
     SCALA = 2
 
 def schema_to_python_str(schema: Schema) -> str:
-    formatter = "@dataclass\nclass {class_name}:\n{members}"
+    formatter = "@dataclass\r\nclass {class_name}:\r\n{members}"
     member_str_list = []
     for member, mtype in schema.members.items():
         member_str_list.append(f"    {member}: {mtype}")
-    members_str = "\n".join(member_str_list)
+    members_str = "\r\n".join(member_str_list)
     return formatter.format(class_name=schema.name, members=members_str)
 
 def schema_to_scala_str(schema: Schema) -> str:
-    formatter = "case class {class_name}(\n{members}\n)"
+    formatter = "case class {class_name}(\r\n{members}\r\n)"
     member_str_list = []
     for member, mtype in schema.members.items():
         member_str_list.append(f"    {member}: {mtype}")
-    members_str = ",\n".join(member_str_list)
+    members_str = ",\r\n".join(member_str_list)
     return formatter.format(class_name=schema.name, members=members_str)
 
 converters = {
     TargetLanguage.PYTHON: schema_to_python_str,
     TargetLanguage.SCALA: schema_to_scala_str
 }
 
@@ -47,15 +47,15 @@
         "str": "String",
         "list": "IndexedSeq",
         "date": "DateTime"
     }
 }
 
 import_statements = {
-    TargetLanguage.PYTHON: "import datetime\nfrom dataclasses import dataclass",
+    TargetLanguage.PYTHON: "import datetime\r\nfrom dataclasses import dataclass",
     TargetLanguage.SCALA: "import org.joda.time.DateTime"
 }
 
 file_extensions = {
     TargetLanguage.PYTHON: ".py",
     TargetLanguage.SCALA: ".scala"
 }
@@ -105,8 +105,8 @@
     schema_strs = []
     to_language_str = converters[target_language]
     for _, schema in infos.items():
         schema_strs.append(to_language_str(schema))
 
     schema_str = "\n\n".join(schema_strs)
     target_import_statements = import_statements[target_language]
-    return target_import_statements + "\n\n" + schema_str
+    return target_import_statements + "\r\n\r\n" + schema_str
```

### Comparing `jdtt-1.0.6/src/jdtt.egg-info/PKG-INFO` & `jdtt-1.0.7/src/jdtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdtt
-Version: 1.0.6
+Version: 1.0.7
 Summary: JSON to programming language schema converter
 Author: Joey Shi
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
```

