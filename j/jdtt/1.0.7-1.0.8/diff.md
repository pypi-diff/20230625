# Comparing `tmp/jdtt-1.0.7.tar.gz` & `tmp/jdtt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtt-1.0.7.tar", last modified: Sun Jun 25 06:36:03 2023, max compression
+gzip compressed data, was "jdtt-1.0.8.tar", last modified: Sun Jun 25 20:18:48 2023, max compression
```

## Comparing `jdtt-1.0.7.tar` & `jdtt-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 06:36:03.317344 jdtt-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 06:35:50.000000 jdtt-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 06:35:50.000000 jdtt-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 06:36:03.321344 jdtt-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/jdtt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-25 06:35:50.000000 jdtt-1.0.7/src/jdtt/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:36:03.317344 jdtt-1.0.7/src/jdtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 06:36:03.000000 jdtt-1.0.7/src/jdtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 20:18:48.919533 jdtt-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 20:18:35.000000 jdtt-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 20:18:35.000000 jdtt-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 20:18:48.919533 jdtt-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.915533 jdtt-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/src/jdtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/src/jdtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/top_level.txt
```

### Comparing `jdtt-1.0.7/PKG-INFO` & `jdtt-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: JSON to programming language schema converter
 Author: Joey Shi
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
```

### Comparing `jdtt-1.0.7/setup.cfg` & `jdtt-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.7/src/jdtt/__main__.py` & `jdtt-1.0.8/src/jdtt/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import argparse
 from jdtt.conversion import json_to_language_str, TargetLanguage, file_extensions
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--target_language", type=str, choices=["python", "scala"], default="python", help="target language")
+    parser.add_argument("--target_language", type=str, choices=["python", "scala", "typescript"], default="python", help="target language")
     parser.add_argument("--root_schema", type=str, default="Root", help="name of root schema")
     parser.add_argument("--detect_date", action="store_true", help="detect datetime fields and convert to date type")
     parser.add_argument("schema_path", type=str, help="filepath to schema json")
     args = parser.parse_args()
 
     schema_path = args.schema_path
     target_language = TargetLanguage[args.target_language.upper()]
```

### Comparing `jdtt-1.0.7/src/jdtt/conversion.py` & `jdtt-1.0.8/src/jdtt/conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,117 @@
 import re
 from enum import Enum
 from typing import Dict
 from dataclasses import dataclass
 
-@dataclass
-class Schema:
-    name: str
-    members: Dict[str, str]
+Schema = Dict[str, Dict[str, str]]
 
 class TargetLanguage(Enum):
     PYTHON = 1
     SCALA = 2
+    TYPESCRIPT = 3
+
+@dataclass
+class TargetLanguageTypes:
+    bool_type: str
+    int_type: str
+    str_type: str
+    list_type: str
+    date_type: str
 
-def schema_to_python_str(schema: Schema) -> str:
-    formatter = "@dataclass\r\nclass {class_name}:\r\n{members}"
+def schema_to_python_str(name: str, members: Dict[str, str]) -> str:
+    formatter = "@dataclass\nclass {class_name}:\n{members}"
     member_str_list = []
-    for member, mtype in schema.members.items():
+    for member, mtype in members.items():
         member_str_list.append(f"    {member}: {mtype}")
-    members_str = "\r\n".join(member_str_list)
-    return formatter.format(class_name=schema.name, members=members_str)
+    members_str = "\n".join(member_str_list)
+    return formatter.format(class_name=name, members=members_str)
 
-def schema_to_scala_str(schema: Schema) -> str:
-    formatter = "case class {class_name}(\r\n{members}\r\n)"
+def schema_to_scala_str(name: str, members: Dict[str, str]) -> str:
+    formatter = "case class {class_name}(\n{members}\n)"
     member_str_list = []
-    for member, mtype in schema.members.items():
+    for member, mtype in members.items():
         member_str_list.append(f"    {member}: {mtype}")
-    members_str = ",\r\n".join(member_str_list)
-    return formatter.format(class_name=schema.name, members=members_str)
+    members_str = ",\n".join(member_str_list)
+    return formatter.format(class_name=name, members=members_str)
+
+def schema_to_typescript_str(name: str, members: Dict[str, str]) -> str:
+    formatter = "export interface {class_name} {{\n{members}\n}}"
+    member_str_list = []
+    for member, mtype in members.items():
+        member_str_list.append(f"    {member}: {mtype};")
+    members_str = "\n".join(member_str_list)
+    return formatter.format(class_name=name, members=members_str)
 
 converters = {
     TargetLanguage.PYTHON: schema_to_python_str,
-    TargetLanguage.SCALA: schema_to_scala_str
+    TargetLanguage.SCALA: schema_to_scala_str,
+    TargetLanguage.TYPESCRIPT: schema_to_typescript_str
 }
 
 language_dtypes = {
-    TargetLanguage.PYTHON: {
-        "bool": "bool",
-        "int": "int",
-        "str": "str",
-        "list": "list",
-        "date": "datetime.datetime"
-    },
-    TargetLanguage.SCALA: {
-        "bool": "Boolean",
-        "int": "Int",
-        "str": "String",
-        "list": "IndexedSeq",
-        "date": "DateTime"
-    }
+    TargetLanguage.PYTHON: TargetLanguageTypes("bool", "int", "str", "list[{item_name}]", "datetime.datetime"),
+    TargetLanguage.SCALA: TargetLanguageTypes("Boolean", "Int", "String", "IndexedSeq[{item_name}]", "DateTime"),
+    TargetLanguage.TYPESCRIPT: TargetLanguageTypes("boolean", "number", "string", "{item_name}[]", "Date")
 }
 
 import_statements = {
-    TargetLanguage.PYTHON: "import datetime\r\nfrom dataclasses import dataclass",
-    TargetLanguage.SCALA: "import org.joda.time.DateTime"
+    TargetLanguage.PYTHON: "import datetime\nfrom dataclasses import dataclass",
+    TargetLanguage.SCALA: "import org.joda.time.DateTime",
+    TargetLanguage.TYPESCRIPT: ""
 }
 
 file_extensions = {
     TargetLanguage.PYTHON: ".py",
-    TargetLanguage.SCALA: ".scala"
+    TargetLanguage.SCALA: ".scala",
+    TargetLanguage.TYPESCRIPT: ".ts"
 }
 
 date_regex = r"\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2})?(\.\d{3})?Z"
 
-def json_to_schemas(schema, target_language: TargetLanguage, root_name="Root", detect_date=True) -> Dict[str, Schema]:
+def json_to_schemas(schema_json, target_language: TargetLanguage, root_name="Root", detect_date=True) -> Schema:
     """Converts a json schema to a dictionary of Schema objects."""
-    return _json_to_schemas(root_name, schema, language_dtypes[target_language], {}, detect_date)
+    return _json_to_schemas(root_name, schema_json, language_dtypes[target_language], {}, detect_date)
 
-def _json_to_schemas(name, schema, dtypes: Dict[str, str], infos: Dict[str, Schema], detect_date: bool) -> Dict[str, Schema]:
-    if not isinstance(schema, dict) or name in infos:
-        return infos
-    info = Schema(name, {})
-    infos[name] = info
-    for member, mvalue in schema.items():
-        _get_or_create_member_type(member, mvalue, dtypes, info, infos, detect_date)
-    return infos
+def _json_to_schemas(name: str, schema_json, dtypes: TargetLanguageTypes, schema: Schema, detect_date: bool) -> Schema:
+    if not isinstance(schema_json, dict) or name in schema:
+        return schema
+    members = {}
+    schema[name] = members
+    for member, mvalue in schema_json.items():
+        members[member] = _get_or_create_member_type(member, mvalue, dtypes, schema, detect_date)
+    return schema
 
-def _get_or_create_member_type(member: str, mvalue, dtypes: Dict[str, str], info: Schema, infos: Dict[str, Schema], detect_date: bool):
+def _get_or_create_member_type(member: str, mvalue, dtypes: TargetLanguageTypes, schema: Schema, detect_date: bool):
     """Returns the type of a member, creating a new schema if necessary."""
     schema_type = type(mvalue)
-    if detect_date and isinstance(mvalue, str) and re.match(date_regex, mvalue):
-        info.members[member] = dtypes["date"]
-    elif schema_type == bool:
-        info.members[member] = dtypes["bool"]
-    elif schema_type == int:
-        info.members[member] = dtypes["int"]
-    elif schema_type == str:
-        info.members[member] = dtypes["str"]
-    elif schema_type == list:
+    if detect_date and schema_type == str and re.match(date_regex, mvalue):
+        return dtypes.date_type
+    if schema_type == bool:
+        return dtypes.bool_type
+    if schema_type == int:
+        return dtypes.int_type
+    if schema_type == str:
+        return dtypes.str_type
+    if schema_type == list:
         item_name = member + "Item"
         count = 1
-        while item_name in infos:
+        while item_name in schema:
             item_name = member + "Item" + str(count)
             count += 1
         schema_item = mvalue[0]
-        info.members[member] = f"{dtypes['list']}[{item_name}]"
-        _json_to_schemas(item_name, schema_item, dtypes, infos, detect_date)
-    else:
-        info.members[member] = member
-        _json_to_schemas(member, mvalue, dtypes, infos, detect_date)
+        item_type = _get_or_create_member_type(item_name, schema_item, dtypes, schema, detect_date)
+        return dtypes.list_type.format(item_name=item_type)
+    _json_to_schemas(member, mvalue, dtypes, schema, detect_date)
+    return member
 
-def json_to_language_str(schema_json, target_language: TargetLanguage, root_name: str, detect_date=True) -> str:
+def json_to_language_str(schema_json, target_language: TargetLanguage, root_name="Root", detect_date=True) -> str:
     """Converts a json schema to a string of the target language."""
     infos = json_to_schemas(schema_json, target_language, root_name, detect_date)
     schema_strs = []
     to_language_str = converters[target_language]
-    for _, schema in infos.items():
-        schema_strs.append(to_language_str(schema))
+    for name, schema in infos.items():
+        schema_strs.append(to_language_str(name, schema))
 
     schema_str = "\n\n".join(schema_strs)
     target_import_statements = import_statements[target_language]
-    return target_import_statements + "\r\n\r\n" + schema_str
+    return target_import_statements + "\n\n" + schema_str
```

### Comparing `jdtt-1.0.7/src/jdtt.egg-info/PKG-INFO` & `jdtt-1.0.8/src/jdtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: JSON to programming language schema converter
 Author: Joey Shi
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
```

