# Comparing `tmp/dasy-0.1.8.tar.gz` & `tmp/dasy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasy-0.1.8.tar", max compression
+gzip compressed data, was "dasy-0.1.9.tar", max compression
```

## Comparing `dasy-0.1.8.tar` & `dasy-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      168 2022-08-14 19:00:07.286836 dasy-0.1.8/dasy/__init__.py
--rw-r--r--   0        0        0      249 2022-08-11 17:06:46.704928 dasy-0.1.8/dasy/compiler.py
--rw-r--r--   0        0        0      508 2022-08-11 01:06:16.087962 dasy-0.1.8/dasy/main.py
--rw-r--r--   0        0        0       51 2022-08-14 16:16:52.061001 dasy-0.1.8/dasy/parser/__init__.py
--rw-r--r--   0        0        0    11134 2022-08-14 18:54:56.940061 dasy-0.1.8/dasy/parser/parse.py
--rw-r--r--   0        0        0      374 2022-08-14 16:13:07.984980 dasy-0.1.8/dasy/parser/utils.py
--rw-r--r--   0        0        0      385 2022-08-14 18:59:56.735228 dasy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      719 2022-08-14 19:00:26.929753 dasy-0.1.8/setup.py
--rw-r--r--   0        0        0      342 2022-08-14 19:00:26.929918 dasy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      168 2022-08-14 19:03:40.923615 dasy-0.1.9/dasy/__init__.py
+-rw-r--r--   0        0        0      249 2022-08-11 17:06:46.704928 dasy-0.1.9/dasy/compiler.py
+-rw-r--r--   0        0        0      508 2022-08-11 01:06:16.087962 dasy-0.1.9/dasy/main.py
+-rw-r--r--   0        0        0       51 2022-08-14 16:16:52.061001 dasy-0.1.9/dasy/parser/__init__.py
+-rw-r--r--   0        0        0    11091 2022-08-14 19:02:50.314391 dasy-0.1.9/dasy/parser/parse.py
+-rw-r--r--   0        0        0      374 2022-08-14 16:13:07.984980 dasy-0.1.9/dasy/parser/utils.py
+-rw-r--r--   0        0        0      385 2022-08-14 19:03:34.870808 dasy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      719 2022-08-14 19:03:43.347489 dasy-0.1.9/setup.py
+-rw-r--r--   0        0        0      342 2022-08-14 19:03:43.347625 dasy-0.1.9/PKG-INFO
```

### Comparing `dasy-0.1.8/dasy/parser/parse.py` & `dasy-0.1.9/dasy/parser/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,14 @@
             value_node = vy_nodes.Int(value=int(node), node_id=next_nodeid(), ast_type='Int')
             return value_node
         case models.Symbol(node) if str(node) in BUILTIN_FUNCS:
             return parse_builtin(node)
         case models.Symbol(node) if str(node) in NAME_CONSTS:
             return vy_nodes.NameConstant(value=py_ast.literal_eval(str(node)), id=next_nodeid(), ast_type='NameConstant')
         case models.Symbol(node) if str(node).startswith("self/"):
-            print(f"matched self/ {node}")
             replacement_node = models.Expression((models.Symbol('.'), models.Symbol('self'), models.Symbol(str(node).split('/')[1])))
             return parse_node(replacement_node)
         case models.Symbol(node) | models.Keyword(node):
             name_node = vy_nodes.Name(id=str(node), node_id=next_nodeid(), ast_type='Name')
             return name_node
         case _:
             raise Exception(f"No match for node {node}")
```

### Comparing `dasy-0.1.8/setup.py` & `dasy-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['argparse>=1.4.0,<2.0.0', 'hy>=0.24.0,<0.25.0', 'vyper>=0.3.6,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['dasy = dasy:main']}
 
 setup_kwargs = {
     'name': 'dasy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'z80',
     'author_email': 'z80@ophy.xyz',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

