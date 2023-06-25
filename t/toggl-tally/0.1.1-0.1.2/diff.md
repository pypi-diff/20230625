# Comparing `tmp/toggl-tally-0.1.1.tar.gz` & `tmp/toggl-tally-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggl-tally-0.1.1.tar", last modified: Tue Mar 21 19:34:46 2023, max compression
+gzip compressed data, was "toggl-tally-0.1.2.tar", last modified: Sun Jun 25 18:15:50 2023, max compression
```

## Comparing `toggl-tally-0.1.1.tar` & `toggl-tally-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:34:46.470357 toggl-tally-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45537 2023-03-21 19:34:46.470357 toggl-tally-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-21 19:34:46.470357 toggl-tally-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:34:46.466357 toggl-tally-0.1.1/toggl_tally/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/tally.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-21 19:34:29.000000 toggl-tally-0.1.1/toggl_tally/time_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:34:46.470357 toggl-tally-0.1.1/toggl_tally.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45537 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 19:34:46.000000 toggl-tally-0.1.1/toggl_tally.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:15:50.935190 toggl-tally-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46332 2023-06-25 18:15:50.935190 toggl-tally-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-25 18:15:50.935190 toggl-tally-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:15:50.935190 toggl-tally-0.1.2/toggl_tally/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/tally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-25 18:15:37.000000 toggl-tally-0.1.2/toggl_tally/time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:15:50.935190 toggl-tally-0.1.2/toggl_tally.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46332 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 18:15:50.000000 toggl-tally-0.1.2/toggl_tally.egg-info/top_level.txt
```

### Comparing `toggl-tally-0.1.1/LICENSE` & `toggl-tally-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toggl-tally-0.1.1/PKG-INFO` & `toggl-tally-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggl-tally
-Version: 0.1.1
+Version: 0.1.2
 Summary: A rich CLI to track hours worked towards monthly targets with toggl
 Author-email: Tim Wolff-Piggott <twolffpiggott@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,15 +693,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Toggl Tally
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/toggl-tally/0.1.1)](https://pypi.org/project/toggl-tally/) [![PyPI version](https://badge.fury.io/py/toggl-tally.svg)](https://badge.fury.io/py/toggl-tally)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/toggl-tally/0.1.2)](https://pypi.org/project/toggl-tally/) [![PyPI version](https://badge.fury.io/py/toggl-tally.svg)](https://badge.fury.io/py/toggl-tally)
 
 [![Tests](https://github.com/twolffpiggott/toggl-tally/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/twolffpiggott/toggl-tally/actions/workflows/test.yml)
 
 Toggl tally is a rich Python command line interface for tracking progress against your monthly project targets and calculating the daily hours you need to work to hit your goals. Toggl tally connects to the [Toggl Track API](https://developers.track.toggl.com/), and supports:
 
 - Filtering by workspaces, clients or projects
 - Configurable invoicing day of month
@@ -756,14 +756,44 @@
 exclude_public_holidays: true
 ```
 
 Alternatively, all configuration can be passed with command-line arguments to the `hours` command. See the CLI help for detailed information about each argument and option.
 
 ![Help](https://github.com/twolffpiggott/toggl-tally/raw/main/imgs/hours_help.png)
 
+## Toggl data model and filtering
+
+```mermaid
+erDiagram
+    WORKSPACE ||--o{ CLIENT : has
+    WORKSPACE ||--o{ PROJECT : has
+    WORKSPACE ||--o{ TIME_ENTRY : has
+    CLIENT |o--|{ PROJECT : has
+    PROJECT |o--o{ TIME_ENTRY : has
+```
+
+`toggl_tally` enables filtering by multiple workspace, client or project names. The UNION across all of these entities is taken to determine the final set of time entries. For example, for the filter criteria:
+
+```yaml
+workspaces:
+clients:
+  - MegaCorp
+  - HyperCorp
+projects:
+  - Widget Building
+  - Baz refactoring
+```
+
+A time entry will be included if it:
+
+- Belongs to a project linked to the MegaCorp client OR
+- Belongs to a project linked to the HyperCorp client OR
+- Belongs to the Widget Building project OR
+- Belongs to the Baz refactoring project
+
 ## Hours command
 
 The `hours` command is the core command for Toggl tally. It reports:
 
 - Working days to go before next invoice date
 - Daily hours needed to hit monthly target by next invoice date
 - Hours worked on relevant projects since last invoice
```

### Comparing `toggl-tally-0.1.1/pyproject.toml` & `toggl-tally-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toggl-tally"
-version = "0.1.1"
+version = "0.1.2"
 description = "A rich CLI to track hours worked towards monthly targets with toggl"
 readme = "README.md"
 authors = [{ name = "Tim Wolff-Piggott", email = "twolffpiggott@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: Microsoft :: Windows",
@@ -47,7 +47,11 @@
 Homepage = "https://github.com/twolffpiggott/toggl-tally"
 
 [project.scripts]
 toggl-tally = "toggl_tally.cli:toggl_tally"
 
 [tool.setuptools]
 packages = ["toggl_tally"]
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3
```

### Comparing `toggl-tally-0.1.1/toggl_tally/api.py` & `toggl-tally-0.1.2/toggl_tally/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,19 @@
         headers: Dict[str, str] = {"content-type": "application/json"},
     ):
         self.base_url = base_url
         self.headers = headers
         self.session = requests.Session()
 
     def auth(self):
-        try:
-            api_token = os.environ["TOGGL_API_TOKEN"]
-        except KeyError as exception:
+        api_token = os.getenv("TOGGL_API_TOKEN")
+        if api_token is None:
             raise KeyError(
                 "Please ensure that the 'TOGGL_API_TOKEN' environment variable is set"
-            ) from exception
+            )
         self.session.auth = (api_token, "api_token")
 
     def get_time_entries_between(self, start_date: datetime, end_date: datetime):
         params = dict(start_date=start_date.isoformat(), end_date=end_date.isoformat())
         return self._call_toggl_api(f"{self.base_url}/me/time_entries", params=params)
 
     def get_time_entries_to_date(self):
```

### Comparing `toggl-tally-0.1.1/toggl_tally/cli.py` & `toggl-tally-0.1.2/toggl_tally/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 from pathlib import Path
 from typing import List, Optional
 
 import click
 import yaml
 from rich.console import Console
+from rich.traceback import install
 
 from toggl_tally import RichReport, TogglAPI, TogglFilter, TogglTally
 
 CONTEXT_SETTINGS = dict(
     help_option_names=["-h", "--help"], auto_envvar_prefix="TOGGL_TALLY"
 )
 
@@ -55,14 +56,16 @@
     "--config",
     "-c",
     type=click.Path(exists=True, path_type=Path),
     help="Path to optional yaml config with CLI option values",
 )
 @click.pass_context
 def toggl_tally(ctx: click.Context, config: Optional[Path]):
+    # rich traceback handling
+    install(max_frames=1)
     if config is not None:
         with config.open("r") as f:
             config_dict = yaml.safe_load(f)
         ctx.default_map = dict(hours=config_dict)
 
 
 @toggl_tally.command(
@@ -167,15 +170,15 @@
             api=api,
             projects=projects,
             clients=clients,
             workspaces=workspaces,
         )
     with console.status("[bold dark_cyan]Getting time entries"):
         unfiltered_time_entries = api.get_time_entries_between(
-            start_date=tally.last_invoice_date,
+            start_date=tally.first_billable_date,
             end_date=tally.now,
         )
     filtered_time_entries = filter.filter_time_entries(response=unfiltered_time_entries)
     seconds_worked = sum(entry["duration"] for entry in filtered_time_entries)
     target_seconds = hours_per_month * 60 * 60
     seconds_outstanding = max(target_seconds - seconds_worked, 0)
     reporter = RichReport(console)
```

### Comparing `toggl-tally-0.1.1/toggl_tally/filter.py` & `toggl-tally-0.1.2/toggl_tally/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass, field
-from typing import List, NamedTuple
+from typing import List, NamedTuple, Set
 
 from toggl_tally import TogglAPI
 
 logger = logging.getLogger(__name__)
 
 
 TOGGL_ENTITIES = ["project", "client", "workspace"]
@@ -45,44 +45,64 @@
     ) -> List[dict]:
         """
         Time entries always have a workspace
         Time entries may have a project
         Time entries only have clients by way of projects
         Projects can have no client
 
-        Caller provides incompatible workspaces and clients -> empty result
+        Take the UNION across workspace, client and project filters.
+        i.e. a time entry is included if it belongs to any of the
+        listed workspaces, clients or projects
         """
-        filter_by_workspace = bool(self.filtered_workspaces)
-        if filter_by_workspace:
-            workspace_ids_set = set(self.filtered_workspaces.entity_ids)
-        filter_by_project = bool(self.filtered_projects) or bool(self.filtered_clients)
-        if filter_by_project:
-            project_id_sets = []
-            if self.filtered_projects:
-                project_id_sets.append(set(self.filtered_projects.entity_ids))
-            if self.filtered_clients:
-                project_id_sets.append(set(self.filtered_client_projects.entity_ids))
-            project_ids_intersection = project_id_sets[0]
-            for project_id_set in project_id_sets[1:]:
-                project_ids_intersection = project_ids_intersection & project_id_set
-        filtered_time_entries = []
-        for time_entry in response:
-            if exclude_running_entries:
-                # running entries have duration = -1 * (Unix start time)
-                # https://developers.track.toggl.com/docs/api/time_entries
-                if time_entry["duration"] < 0:
-                    continue
-            if filter_by_workspace:
-                if time_entry["workspace_id"] not in workspace_ids_set:
-                    continue
-            if filter_by_project:
-                if time_entry["project_id"] not in project_ids_intersection:
-                    continue
-            filtered_time_entries.append(time_entry)
-        return filtered_time_entries
+        workspace_ids_set = self._get_entity_ids_set(self.filtered_workspaces)
+        client_project_ids_set = self._get_entity_ids_set(self.filtered_client_projects)
+        project_ids_set = self._get_entity_ids_set(self.filtered_projects)
+
+        return [
+            time_entry
+            for time_entry in response
+            if self._is_valid_time_entry(
+                time_entry,
+                exclude_running_entries=exclude_running_entries,
+                workspace_ids_set=workspace_ids_set,
+                client_project_ids_set=client_project_ids_set,
+                project_ids_set=project_ids_set,
+            )
+        ]
+
+    def _is_valid_time_entry(
+        self,
+        time_entry: dict,
+        exclude_running_entries: bool,
+        workspace_ids_set: Set[int],
+        client_project_ids_set: Set[int],
+        project_ids_set: Set[int],
+    ) -> bool:
+        """
+        Take the UNION across workspace, client and project filters.
+        i.e. a time entry is included if it belongs to any of the
+        listed workspaces, clients or projects
+        """
+        if exclude_running_entries and self._is_running_time_entry(time_entry):
+            return False
+        if time_entry["workspace_id"] in workspace_ids_set:
+            return True
+        if time_entry["project_id"] in client_project_ids_set.union(project_ids_set):
+            return True
+        return False
+
+    def _get_entity_ids_set(self, filtered_entities: TogglEntities) -> Set[int]:
+        if filtered_entities:
+            return set(filtered_entities.entity_ids)
+        return set()
+
+    def _is_running_time_entry(self, time_entry: dict) -> bool:
+        # Running entries have duration = -1 * (Unix start time)
+        # https://developers.track.toggl.com/docs/api/time_entries
+        return time_entry["duration"] < 0
 
     @staticmethod
     def get_toggl_entities(
         response: List[dict],
         toggl_entity: str,
         entity_names: List[str],
     ) -> TogglEntities:
```

### Comparing `toggl-tally-0.1.1/toggl_tally/report.py` & `toggl-tally-0.1.2/toggl_tally/report.py`

 * *Files identical despite different names*

### Comparing `toggl-tally-0.1.1/toggl_tally/tally.py` & `toggl-tally-0.1.2/toggl_tally/tally.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,24 @@
                 self.now.year,
                 tzinfo=self.now.tzinfo,
             )
         else:
             return self.current_month_invoice_date
 
     @property
+    def first_billable_date(self) -> datetime:
+        last_invoice_date = self.last_invoice_date
+        if last_invoice_date.day < self.invoice_day_of_month:
+            # Return the next day
+            return last_invoice_date + timedelta(days=1)
+        else:
+            # Return the last invoice date
+            return last_invoice_date
+
+    @property
     def next_invoice_date(self) -> datetime:
         if self.now < self.current_month_invoice_date:
             return self.current_month_invoice_date
         else:
             return self.calculate_invoice_date(
                 self.invoice_day_of_month,
                 self.now.month + 1,
```

### Comparing `toggl-tally-0.1.1/toggl_tally/time_utils.py` & `toggl-tally-0.1.2/toggl_tally/time_utils.py`

 * *Files identical despite different names*

### Comparing `toggl-tally-0.1.1/toggl_tally.egg-info/PKG-INFO` & `toggl-tally-0.1.2/toggl_tally.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggl-tally
-Version: 0.1.1
+Version: 0.1.2
 Summary: A rich CLI to track hours worked towards monthly targets with toggl
 Author-email: Tim Wolff-Piggott <twolffpiggott@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,15 +693,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Toggl Tally
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/toggl-tally/0.1.1)](https://pypi.org/project/toggl-tally/) [![PyPI version](https://badge.fury.io/py/toggl-tally.svg)](https://badge.fury.io/py/toggl-tally)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/toggl-tally/0.1.2)](https://pypi.org/project/toggl-tally/) [![PyPI version](https://badge.fury.io/py/toggl-tally.svg)](https://badge.fury.io/py/toggl-tally)
 
 [![Tests](https://github.com/twolffpiggott/toggl-tally/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/twolffpiggott/toggl-tally/actions/workflows/test.yml)
 
 Toggl tally is a rich Python command line interface for tracking progress against your monthly project targets and calculating the daily hours you need to work to hit your goals. Toggl tally connects to the [Toggl Track API](https://developers.track.toggl.com/), and supports:
 
 - Filtering by workspaces, clients or projects
 - Configurable invoicing day of month
@@ -756,14 +756,44 @@
 exclude_public_holidays: true
 ```
 
 Alternatively, all configuration can be passed with command-line arguments to the `hours` command. See the CLI help for detailed information about each argument and option.
 
 ![Help](https://github.com/twolffpiggott/toggl-tally/raw/main/imgs/hours_help.png)
 
+## Toggl data model and filtering
+
+```mermaid
+erDiagram
+    WORKSPACE ||--o{ CLIENT : has
+    WORKSPACE ||--o{ PROJECT : has
+    WORKSPACE ||--o{ TIME_ENTRY : has
+    CLIENT |o--|{ PROJECT : has
+    PROJECT |o--o{ TIME_ENTRY : has
+```
+
+`toggl_tally` enables filtering by multiple workspace, client or project names. The UNION across all of these entities is taken to determine the final set of time entries. For example, for the filter criteria:
+
+```yaml
+workspaces:
+clients:
+  - MegaCorp
+  - HyperCorp
+projects:
+  - Widget Building
+  - Baz refactoring
+```
+
+A time entry will be included if it:
+
+- Belongs to a project linked to the MegaCorp client OR
+- Belongs to a project linked to the HyperCorp client OR
+- Belongs to the Widget Building project OR
+- Belongs to the Baz refactoring project
+
 ## Hours command
 
 The `hours` command is the core command for Toggl tally. It reports:
 
 - Working days to go before next invoice date
 - Daily hours needed to hit monthly target by next invoice date
 - Hours worked on relevant projects since last invoice
```

