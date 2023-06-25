# Comparing `tmp/pqv-0.5.0.tar.gz` & `tmp/pqv-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqv-0.5.0.tar", last modified: Fri May 26 13:50:49 2023, max compression
+gzip compressed data, was "pqv-0.6.0.tar", last modified: Sun Jun 25 21:21:43 2023, max compression
```

## Comparing `pqv-0.5.0.tar` & `pqv-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.435360 pqv-0.5.0/
--rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.5.0/LICENSE
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-05-26 13:50:49.435047 pqv-0.5.0/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.5.0/README.md
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.432750 pqv-0.5.0/pqv/
--rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.5.0/pqv/__init__.py
--rw-r--r--   0 pieter     (501) staff       (20)     4306 2023-05-26 13:42:04.000000 pqv-0.5.0/pqv/__main__.py
--rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.5.0/pqv/style.css
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.434770 pqv-0.5.0/pqv.egg-info/
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      236 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/SOURCES.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/dependency_links.txt
--rw-r--r--   0 pieter     (501) staff       (20)       42 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/entry_points.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.5.0/pqv.egg-info/not-zip-safe
--rw-r--r--   0 pieter     (501) staff       (20)        4 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/top_level.txt
--rw-r--r--   0 pieter     (501) staff       (20)       38 2023-05-26 13:50:49.435454 pqv-0.5.0/setup.cfg
--rw-r--r--   0 pieter     (501) staff       (20)      529 2023-05-26 13:48:47.000000 pqv-0.5.0/setup.py
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.804197 pqv-0.6.0/
+-rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.6.0/LICENSE
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-06-25 21:21:43.803843 pqv-0.6.0/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.6.0/README.md
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.801649 pqv-0.6.0/pqv/
+-rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.6.0/pqv/__init__.py
+-rw-r--r--   0 pieter     (501) staff       (20)     5243 2023-06-25 21:19:56.000000 pqv-0.6.0/pqv/__main__.py
+-rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.6.0/pqv/style.css
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.803562 pqv-0.6.0/pqv.egg-info/
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      236 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/SOURCES.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/dependency_links.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       42 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/entry_points.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.6.0/pqv.egg-info/not-zip-safe
+-rw-r--r--   0 pieter     (501) staff       (20)        4 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/top_level.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       38 2023-06-25 21:21:43.804284 pqv-0.6.0/setup.cfg
+-rw-r--r--   0 pieter     (501) staff       (20)      529 2023-06-25 21:20:39.000000 pqv-0.6.0/setup.py
```

### Comparing `pqv-0.5.0/LICENSE` & `pqv-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqv-0.5.0/pqv/__main__.py` & `pqv-0.6.0/pqv/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 from textual.widgets import Static, Footer
 from textual import events
 import pyperclip
 import json
 from datetime import datetime
 
 
+def parse_if_json(input: str):
+    try:
+        parsed = json.loads(input)
+        return parsed
+    except ValueError:
+        return input
+
+
 class CustomEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime):
             return str(obj)
         if isinstance(obj, bytes):
             return obj.hex()
         return super(CustomEncoder, self).default(obj)
@@ -23,14 +31,15 @@
 
     CSS_PATH = "style.css"
     BINDINGS = [
         ("q", "quit", "Quit"),
         ("←", "previous", "Previous"),
         ("→", "next", "Next"),
         ("s", "schema", "Schema"),
+        ("m", "metadata", "Metadata"),
         ("c", "copy", "Copy"),
     ]
 
     def compose(self) -> ComposeResult:
         yield Static(id="info")
         yield Static(id="json")
         yield Footer()
@@ -43,14 +52,15 @@
             row_dict = dict([(k, v[0]) for k, v in self.group.slice(self.row_index - self.group_offset, 1).to_pydict().items()])
             json_str = json.dumps(row_dict, indent=2, cls=CustomEncoder)
             return json_str
         else:
             return None
 
     def show_row(self):
+        self.state = "row"
         info_view = self.query_one("#info", Static)
         info = f"{self.file_path} - group {self.group_index + 1}/{self.parquet_file.num_row_groups} - row {self.row_index + 1}/{self.parquet_file.metadata.num_rows}"
         info_view.update(info)
 
         json_view = self.query_one("#json", Static)
         row = self.read_line()
         if row is not None:
@@ -58,22 +68,31 @@
             self.content = row
         else:
             syntax = Syntax("", "text", theme="github-dark", line_numbers=True, word_wrap=False, indent_guides=True)
             self.content = ""
         json_view.update(syntax)
 
     def toggle_schema(self):
-        if self.schema is None:
+        if self.state != "schema":
+            self.state = "schema"
             json_view = self.query_one("#json", Static)
-            self.schema = "\n".join(str(self.parquet_file.schema).splitlines(keepends=False)[1:])
             syntax = Syntax(self.schema, "yaml", theme="github-dark", line_numbers=True, word_wrap=False, indent_guides=True)
             self.content = self.schema
             json_view.update(syntax)
         else:
-            self.schema = None
+            self.show_row()
+
+    def toggle_metadata(self):
+        if self.state != "metadata":
+            self.state = "metadata"
+            json_view = self.query_one("#json", Static)
+            syntax = Syntax(self.metadata, "yaml", theme="github-dark", line_numbers=True, word_wrap=False, indent_guides=True)
+            self.content = self.metadata
+            json_view.update(syntax)
+        else:
             self.show_row()
 
     def previous(self):
         self.row_index = self.row_index - 1 if self.row_index > 0 else 0
         if self.row_index < self.group_offset:
             self.group_index = self.group_index - 1
             self.group_offset = self.group_offset - self.group.shape[0]
@@ -95,30 +114,37 @@
     def on_key(self, event: events.Key) -> None:
         if event.key == "left":
             self.previous()
         elif event.key == "right":
             self.next()
         elif event.key == "s":
             self.toggle_schema()
+        elif event.key == "m":
+            self.toggle_metadata()
         elif event.key == "c":
             self.copy()
 
     def on_mount(self) -> None:
         self.group = None
         self.group_index = 0
         self.group_offset = 0
         self.row_index = 0
         self.file_path = sys.argv[1]
+        self.state = "row"
         if not os.path.isfile(self.file_path):
             sys.exit(f"No such file: {self.file_path}")
         try:
             self.parquet_file = ParquetFile(os.path.expanduser(self.file_path))
         except Exception:
             sys.exit(f"Error reading file {self.file_path}")
-        self.schema = None
+        self.schema = "\n".join(str(self.parquet_file.schema).splitlines(keepends=False)[1:])
+        if self.parquet_file.metadata.metadata is not None:
+            self.metadata = json.dumps({k.decode(): parse_if_json(v.decode()) for k, v in self.parquet_file.metadata.metadata.items()}, indent=2)
+        else:
+            self.metadata = ""
         self.update_group()
         self.show_row()
 
 
 def main():
     app = ParquetApp()
     app.run()
```

### Comparing `pqv-0.5.0/setup.py` & `pqv-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="pqv",
-    version="0.5.0",
+    version="0.6.0",
     author="Pieter Provoost",
     author_email="pieterprovoost@gmail.com",
     description="Simple parquet viewer",
     url="https://github.com/pieterprovoost/pqv",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
```

