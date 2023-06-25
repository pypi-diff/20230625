# Comparing `tmp/tuck-0.2.1.tar.gz` & `tmp/tuck-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuck-0.2.1.tar", last modified: Sat Feb 18 19:22:34 2023, max compression
+gzip compressed data, was "tuck-0.2.2.tar", last modified: Sun Jun 25 12:08:51 2023, max compression
```

## Comparing `tuck-0.2.1.tar` & `tuck-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 19:22:34.589453 tuck-0.2.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-02-18 19:22:24.000000 tuck-0.2.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2041 2023-02-18 19:22:34.589453 tuck-0.2.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-02-18 19:22:24.000000 tuck-0.2.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-02-18 19:22:34.589453 tuck-0.2.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1316 2023-02-18 19:22:24.000000 tuck-0.2.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 19:22:34.589453 tuck-0.2.1/tuck/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9153 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/ast.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3554 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4607 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/editing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5661 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14959 2023-02-18 19:22:24.000000 tuck-0.2.1/tuck/wrappers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 19:22:34.589453 tuck-0.2.1/tuck.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2041 2023-02-18 19:22:34.000000 tuck-0.2.1/tuck.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-02-18 19:22:34.000000 tuck-0.2.1/tuck.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-18 19:22:34.000000 tuck-0.2.1/tuck.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-02-18 19:22:34.000000 tuck-0.2.1/tuck.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-02-18 19:22:34.000000 tuck-0.2.1/tuck.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-06-25 12:08:42.000000 tuck-0.2.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 12:08:51.601364 tuck-0.2.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-06-25 12:08:42.000000 tuck-0.2.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      981 2023-06-25 12:08:51.601364 tuck-0.2.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-06-25 12:08:42.000000 tuck-0.2.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/tuck/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9059 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/ast.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3554 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/editing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5645 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14951 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/wrappers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/tuck.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/top_level.txt
```

### Comparing `tuck-0.2.1/LICENSE` & `tuck-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuck-0.2.1/PKG-INFO` & `tuck-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.1
+Version: 0.2.2
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tuck
 
 [![CircleCI](https://circleci.com/gh/PeterJCLaw/tuck/tree/main.svg?style=svg)](https://circleci.com/gh/PeterJCLaw/tuck/tree/main)
```

### Comparing `tuck-0.2.1/README.md` & `tuck-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tuck-0.2.1/setup.cfg` & `tuck-0.2.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	__pycache__,
 	build,
 	debian,
 	script
 ignore = 
 	W503
 max_line_length = 95
+noqa-require-code = true
 
 [isort]
 atomic = True
 balanced_wrapping = True
 combine_as_imports = True
 include_trailing_comma = True
 length_sort = True
```

### Comparing `tuck-0.2.1/setup.py` & `tuck-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages  # type: ignore[import]
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='tuck',
-    version='0.2.1',
+    version='0.2.2',
     url='https://github.com/PeterJCLaw/tuck',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/tuck/issues',
     },
     description="Semi-automated Python formatting.",
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -37,8 +37,9 @@
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
     ],
 
     install_requires=(
         'asttokens >=2, <3',
     ),
+    python_requires='>=3.7',
 )
```

### Comparing `tuck-0.2.1/tuck/ast.py` & `tuck-0.2.2/tuck/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         if self.line > other.line:
             return False
 
         return self.col < other.col
 
     def __repr__(self) -> str:
-        return 'Position(line={}, col={})'.format(self.line, self.col)
+        return f'Position(line={self.line}, col={self.col})'
 
 
 class NodeSearchError(TuckError, ValueError):
     """Base type for all node search errors."""
 
 
 class NoNodeFoundError(NodeSearchError):
@@ -103,15 +103,15 @@
     Visitor which finds the AST node that should be wrapped for a given position.
     """
 
     def __init__(self, position: Position, node_types: Tuple[Type[ast.AST], ...]) -> None:
         self.target_position = position
         self.target_node_types = node_types
 
-        self.node_stack = []  # type: List[ast.AST]
+        self.node_stack: List[ast.AST] = []
 
         self.found = False
 
     def get_filtered_stack(self) -> List[ast.AST]:
         """
         In some cases we want to skip over the actual place in the AST and
         onwards to a parent node. This filtering achieves that.
@@ -160,18 +160,15 @@
 
     def get_found_node(self, asttokens: ASTTokens) -> ast.AST:
         if not self.found:
             raise NoNodeFoundError()
 
         reversed_stack = self.get_filtered_stack()
 
-        for node, prev_node in zip(
-            reversed_stack,
-            [None, *reversed_stack],
-        ):
+        for node in reversed_stack:
             if isinstance(node, self.target_node_types):
                 self._check_not_in_body(node, asttokens)
                 return node
 
         raise NoSupportedNodeFoundError(self.node_stack)
 
     def _get_end_of_node(self, node: ast.AST) -> Position:
```

### Comparing `tuck-0.2.1/tuck/cli.py` & `tuck-0.2.2/tuck/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def print_edits(insertions: List[Insertion]) -> None:
     edits = [insertion_as_lsp_data(*x) for x in insertions]
     print(json.dumps({'edits': edits}))
 
 
 def parse_position(position: str) -> Position:
-    line, col = [int(x) for x in position.split(':')]
+    line, col = (int(x) for x in position.split(':'))
     return Position(line, col)
 
 
 def parse_args(argv: List[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Wrap the python statement at a given position within a text document.",
     )
```

### Comparing `tuck-0.2.1/tuck/editing.py` & `tuck-0.2.2/tuck/editing.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             return False
 
     return True
 
 
 def merge_insertions(grouped_insertions: Iterable[List[Insertion]]) -> List[Insertion]:
     flat_insertions = []
-    positions = []  # type: List[List[Position]]
+    positions: List[List[Position]] = []
 
     for insertions in grouped_insertions:
         flat_insertions.extend(insertions)
         positions.append([x for x, _ in insertions])
 
     if not all_are_disjoint(positions):
         raise EditsOverlapError()
@@ -137,14 +137,14 @@
         col = position.col
 
         text = new_content[line]
         left, right = text[:col], text[col:]
 
         if insertion.startswith('\n'):
             # TODO: ideally we'd have full edit support, rather than just
-            # insertions, which would mean we could handle this at an earler
+            # insertions, which would mean we could handle this at an earlier
             # stage and thus in a way that also works for editors.
             left = left.rstrip()
 
         new_content[line] = left + insertion + right
 
     return "".join(new_content)
```

### Comparing `tuck-0.2.1/tuck/main.py` & `tuck-0.2.2/tuck/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 def get_wrapping_summary(asttokens: ASTTokens, node: ast.AST) -> WrappingSummary:
     for ast_type, func in WRAPPING_FUNCTIONS:
         if isinstance(node, ast_type):
             return func(asttokens, node)
 
     if not isinstance(node, WRAPPABLE_NODE_TYPES):
-        raise AssertionError("Unable to get wrapping positions for {}".format(node))
+        raise AssertionError(f"Unable to get wrapping positions for {node}")
 
-    raise AssertionError("Unsupported node type {}".format(node))
+    raise AssertionError(f"Unsupported node type {node}")
 
 
 def remove_redundant_wrapping_operations(
     asttokens: ASTTokens,
     wrapping_summary: WrappingSummary,
     node_start: Position,
 ) -> WrappingSummary:
```

### Comparing `tuck-0.2.1/tuck/wrappers.py` & `tuck-0.2.2/tuck/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     if (
         len(node.args) == 1
         and not named_args
         and isinstance(node.args[0], ast.GeneratorExp)
         and not generator_is_parenthesised(asttokens, node.args[0])
     ):
-        generator_node = node.args[0]  # type: ast.GeneratorExp
+        generator_node: ast.GeneratorExp = node.args[0]
         # The generator needs parentheses adding, as well as wrapping
         summary = [(
             Position.from_node_start(generator_node),
             MutationType.WRAP_INDENT,
         ), (
             Position.from_node_start(generator_node),
             MutationType.OPEN_PAREN,
```

### Comparing `tuck-0.2.1/tuck.egg-info/PKG-INFO` & `tuck-0.2.2/tuck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.1
+Version: 0.2.2
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tuck
 
 [![CircleCI](https://circleci.com/gh/PeterJCLaw/tuck/tree/main.svg?style=svg)](https://circleci.com/gh/PeterJCLaw/tuck/tree/main)
```

