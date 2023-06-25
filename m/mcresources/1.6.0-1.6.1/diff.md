# Comparing `tmp/mcresources-1.6.0.tar.gz` & `tmp/mcresources-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcresources-1.6.0.tar", last modified: Sat Jun 24 20:32:39 2023, max compression
+gzip compressed data, was "mcresources-1.6.1.tar", last modified: Sun Jun 25 17:37:19 2023, max compression
```

## Comparing `mcresources-1.6.0.tar` & `mcresources-1.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-24 20:32:23.000000 mcresources-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-24 20:32:39.845972 mcresources-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-24 20:32:23.000000 mcresources-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/mcresources/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/advancements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/atlases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/block_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/block_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/item_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/loot_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/recipe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/surface_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/mcresources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 20:32:39.845972 mcresources-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-24 20:32:23.000000 mcresources-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:37:19.187076 mcresources-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-25 17:37:04.000000 mcresources-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-25 17:37:19.187076 mcresources-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-25 17:37:04.000000 mcresources-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:37:19.187076 mcresources-1.6.1/mcresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/advancements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/atlases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/block_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/block_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/item_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/loot_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/recipe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/surface_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-06-25 17:37:04.000000 mcresources-1.6.1/mcresources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:37:19.187076 mcresources-1.6.1/mcresources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-25 17:37:19.000000 mcresources-1.6.1/mcresources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-25 17:37:19.000000 mcresources-1.6.1/mcresources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:37:19.000000 mcresources-1.6.1/mcresources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 17:37:19.000000 mcresources-1.6.1/mcresources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 17:37:19.187076 mcresources-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-25 17:37:04.000000 mcresources-1.6.1/setup.py
```

### Comparing `mcresources-1.6.0/LICENSE.txt` & `mcresources-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/PKG-INFO` & `mcresources-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcresources
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python Data Generator for Minecraft Modding
 Home-page: https://github.com/alcatrazEscapee/mcresources
 Author: Alex O'Neill
 Author-email: alex@molleroneill.com
 License: MIT
 Keywords: python,minecraft,resources,modding,forge
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mcresources-1.6.0/README.md` & `mcresources-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/advancements.py` & `mcresources-1.6.1/mcresources/advancements.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/atlases.py` & `mcresources-1.6.1/mcresources/atlases.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/block_context.py` & `mcresources-1.6.1/mcresources/block_context.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/block_states.py` & `mcresources-1.6.1/mcresources/block_states.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/item_context.py` & `mcresources-1.6.1/mcresources/item_context.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/loot_tables.py` & `mcresources-1.6.1/mcresources/loot_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,34 @@
         'conditions': conditions,
         'functions': functions,
         'rolls': rolls,
         'bonus_rolls': bonus_rolls
     }
 
 
+def alternatives(*entries: Json, conditions: Optional[Json] = None, functions: Optional[Json] = None) -> JsonObject:
+    return {
+        'type': 'minecraft:alternatives',
+        'children': entries,
+        'conditions': conditions,
+        'functions': functions
+    }
+
+
 # Loot Conditions
 
 def all_of(*terms: Json) -> Json:
     return {
-        'condition': 'minecraft:any_of',
+        'condition': 'minecraft:all_of',
         'terms': utils.loot_conditions(terms)
     }
 
 def any_of(*terms: Json) -> Json:
     return {
-        'condition': 'minecraft:all_of',
+        'condition': 'minecraft:any_of',
         'terms': utils.loot_conditions(terms)
     }
 
 def inverted(term: Json) -> Json:
     condition = utils.loot_conditions(term)
     assert len(condition) == 1, 'Expected one condition for inverted() term'
     return {
```

### Comparing `mcresources-1.6.0/mcresources/recipe_context.py` & `mcresources-1.6.1/mcresources/recipe_context.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/resource_manager.py` & `mcresources-1.6.1/mcresources/resource_manager.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/surface_rules.py` & `mcresources-1.6.1/mcresources/surface_rules.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/tag.py` & `mcresources-1.6.1/mcresources/tag.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/type_definitions.py` & `mcresources-1.6.1/mcresources/type_definitions.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources/utils.py` & `mcresources-1.6.1/mcresources/utils.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/mcresources.egg-info/PKG-INFO` & `mcresources-1.6.1/mcresources.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcresources
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python Data Generator for Minecraft Modding
 Home-page: https://github.com/alcatrazEscapee/mcresources
 Author: Alex O'Neill
 Author-email: alex@molleroneill.com
 License: MIT
 Keywords: python,minecraft,resources,modding,forge
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mcresources-1.6.0/mcresources.egg-info/SOURCES.txt` & `mcresources-1.6.1/mcresources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcresources-1.6.0/setup.py` & `mcresources-1.6.1/setup.py`

 * *Files identical despite different names*

