# Comparing `tmp/tui_rsync-0.8.13.tar.gz` & `tmp/tui_rsync-0.8.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_rsync-0.8.13.tar", max compression
+gzip compressed data, was "tui_rsync-0.8.14.tar", max compression
```

## Comparing `tui_rsync-0.8.13.tar` & `tui_rsync-0.8.14.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      389 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/README.rst
--rw-r--r--   0        0        0      725 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/__init__.py
--rw-r--r--   0        0        0      163 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/__init__.py
--rw-r--r--   0        0        0     1889 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/cli.py
--rw-r--r--   0        0        0       47 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/__init__.py
--rw-r--r--   0        0        0     1814 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_prompt.py
--rw-r--r--   0        0        0     2432 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_remove.py
--rw-r--r--   0        0        0     3600 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_update.py
--rw-r--r--   0        0        0     2644 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/groups.py
--rw-r--r--   0        0        0     3018 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/label_prompt.py
--rw-r--r--   0        0        0     2110 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/path_prompt.py
--rw-r--r--   0        0        0     2000 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/rsync.py
--rw-r--r--   0        0        0       47 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/__init__.py
--rw-r--r--   0        0        0     3349 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source.py
--rw-r--r--   0        0        0     2414 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_remove.py
--rw-r--r--   0        0        0     2363 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_show.py
--rw-r--r--   0        0        0     4146 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_update.py
--rw-r--r--   0        0        0     4311 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/sync.py
--rw-r--r--   0        0        0       38 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/config/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/config/app.py
--rw-r--r--   0        0        0      156 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/main.py
--rw-r--r--   0        0        0      230 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/models/__init__.py
--rw-r--r--   0        0        0     7126 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/models/models.py
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.13/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.13/PKG-INFO
+-rw-r--r--   0        0        0      389 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/README.rst
+-rw-r--r--   0        0        0      725 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/__init__.py
+-rw-r--r--   0        0        0     1889 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/cli.py
+-rw-r--r--   0        0        0       47 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/__init__.py
+-rw-r--r--   0        0        0     1814 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/group_prompt.py
+-rw-r--r--   0        0        0     2432 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/group_remove.py
+-rw-r--r--   0        0        0     2374 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/group_show.py
+-rw-r--r--   0        0        0     3600 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/group_update.py
+-rw-r--r--   0        0        0     2761 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/groups/groups.py
+-rw-r--r--   0        0        0     3018 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/label_prompt.py
+-rw-r--r--   0        0        0     2110 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/path_prompt.py
+-rw-r--r--   0        0        0     2000 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/rsync.py
+-rw-r--r--   0        0        0       47 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/source/__init__.py
+-rw-r--r--   0        0        0     3349 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/source/source.py
+-rw-r--r--   0        0        0     2414 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/source/source_remove.py
+-rw-r--r--   0        0        0     2363 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/source/source_show.py
+-rw-r--r--   0        0        0     4146 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/source/source_update.py
+-rw-r--r--   0        0        0     4311 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/cli/sync.py
+-rw-r--r--   0        0        0       38 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/config/__init__.py
+-rw-r--r--   0        0        0     2211 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/config/app.py
+-rw-r--r--   0        0        0      156 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/main.py
+-rw-r--r--   0        0        0      230 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/models/__init__.py
+-rw-r--r--   0        0        0     7537 2023-06-25 15:09:19.693185 tui_rsync-0.8.14/tui_rsync/models/models.py
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.14/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.14/PKG-INFO
```

### Comparing `tui_rsync-0.8.13/pyproject.toml` & `tui_rsync-0.8.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tui-rsync"
-version = "0.8.13"
+version = "0.8.14"
 description = "tui-rsync will help you to manage yours backups."
 authors = ["Kostiantyn Klochko <kostya_klochko@ukr.net>"]
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 packages = [{include = "tui_rsync"}]
 repository = "https://gitlab.com/KKlochko/tui-rsync"
 keywords = ["tui", "cli", "rsync", "backup"]
```

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/cli.py` & `tui_rsync-0.8.14/tui_rsync/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/groups/group_prompt.py` & `tui_rsync-0.8.14/tui_rsync/cli/groups/group_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/groups/group_remove.py` & `tui_rsync-0.8.14/tui_rsync/cli/groups/group_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/groups/group_update.py` & `tui_rsync-0.8.14/tui_rsync/cli/groups/group_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/groups/groups.py` & `tui_rsync-0.8.14/tui_rsync/cli/groups/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 from rich.prompt import Confirm, Prompt
 from typing import List, Optional
 import typer
 
 from tui_rsync.cli.label_prompt import LabelPrompt
 from tui_rsync.cli.rsync import Rsync
 from tui_rsync.models.models import Group, count_all_labels_except
+from tui_rsync.cli.groups.group_show import group_show
 from tui_rsync.cli.groups.group_update import group_update
 from tui_rsync.cli.groups.group_remove import group_remove
 
 console = Console()
 groups = typer.Typer()
+groups.add_typer(group_show, name="show", help="Show groups")
 groups.add_typer(group_update, name="update", help="Update groups")
 groups.add_typer(group_remove, name="remove", help="Remove groups")
 
 @groups.command()
 def add(
     group_label: str = typer.Option(
         None, "--group-label", "-g",
```

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/label_prompt.py` & `tui_rsync-0.8.14/tui_rsync/cli/label_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/path_prompt.py` & `tui_rsync-0.8.14/tui_rsync/cli/path_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/rsync.py` & `tui_rsync-0.8.14/tui_rsync/cli/rsync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/source/source.py` & `tui_rsync-0.8.14/tui_rsync/cli/source/source.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/source/source_remove.py` & `tui_rsync-0.8.14/tui_rsync/cli/source/source_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/source/source_show.py` & `tui_rsync-0.8.14/tui_rsync/cli/source/source_show.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/source/source_update.py` & `tui_rsync-0.8.14/tui_rsync/cli/source/source_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/cli/sync.py` & `tui_rsync-0.8.14/tui_rsync/cli/sync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/config/app.py` & `tui_rsync-0.8.14/tui_rsync/config/app.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.13/tui_rsync/models/models.py` & `tui_rsync-0.8.14/tui_rsync/models/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,23 +106,27 @@
 
     def __str__(self) -> str:
         return f"{self.label}"
 
     def __repr__(self) -> str:
         return f"{self.label}"
 
-    def show_format(self) -> str:
+    def show_format(self, prefix='') -> str:
         output = f"[b]label:[/] {self.label}\n" \
                  f"[b]source:[/] {self.source.path}\n" \
                  f"[b]args:[/] {self.args}\n" \
                  f"[b]destionations:[/] \n"
 
         for destination in self.destinations:
             output+=f"\t{destination.path}\n"
 
+        if prefix != '':
+            keepends = True
+            output = prefix + f'{prefix}'.join(output.splitlines(keepends))
+
         return output
 
 class Destination(BaseModel):
     source = ForeignKeyField(Source, backref='destinations')
     path = ForeignKeyField(Path)
 
     def __str__(self) -> str:
@@ -180,14 +184,24 @@
 
     def __str__(self) -> str:
         return f"{self.label}"
 
     def __repl__(self) -> str:
         return f"{self.label}"
 
+    def show_format(self) -> str:
+        output = f"[b]label:[/] {self.label}\n" \
+                 f"[b]sources:[/] \n"
+
+        for source in self.sources:
+            prefix = '\t'
+            output+=f"{source.source.show_format(prefix)}\n"
+
+        return output
+
 class GroupSource(BaseModel):
     group = ForeignKeyField(Group, backref='sources')
     source = ForeignKeyField(Source)
 
     @staticmethod
     def create_group_source(group:Group, source_label:str) -> bool:
         """
```

### Comparing `tui_rsync-0.8.13/setup.py` & `tui_rsync-0.8.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['tui-rsync = tui_rsync.main:main']}
 
 setup_kwargs = {
     'name': 'tui-rsync',
-    'version': '0.8.13',
+    'version': '0.8.14',
     'description': 'tui-rsync will help you to manage yours backups.',
     'long_description': 'tui-rsync\n=========\n\n|PyPI version|\n\ntui-rsync is the application that will help you to manage yours backups.\nIt uses rsync for syncing backups.\n\nDependencies\n============\n\n-  rsync\n-  fzf\n\nAuthor\n======\n\nKostiantyn Klochko (c) 2023\n\nLicense\n=======\n\nUnder GNU GPL v3 license\n\n.. |PyPI version| image:: https://badge.fury.io/py/tui-rsync.svg\n   :target: https://badge.fury.io/py/tui-rsync\n',
     'author': 'Kostiantyn Klochko',
     'author_email': 'kostya_klochko@ukr.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/KKlochko/tui-rsync',
```

### Comparing `tui_rsync-0.8.13/PKG-INFO` & `tui_rsync-0.8.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui-rsync
-Version: 0.8.13
+Version: 0.8.14
 Summary: tui-rsync will help you to manage yours backups.
 Home-page: https://gitlab.com/KKlochko/tui-rsync
 License: GPL-3.0-or-later
 Keywords: tui,cli,rsync,backup
 Author: Kostiantyn Klochko
 Author-email: kostya_klochko@ukr.net
 Requires-Python: >=3.10,<4.0
```

