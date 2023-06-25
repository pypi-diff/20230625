# Comparing `tmp/tuck-0.2.2.tar.gz` & `tmp/tuck-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuck-0.2.2.tar", last modified: Sun Jun 25 12:08:51 2023, max compression
+gzip compressed data, was "tuck-0.2.3.tar", last modified: Sun Jun 25 13:08:05 2023, max compression
```

## Comparing `tuck-0.2.2.tar` & `tuck-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-06-25 12:08:42.000000 tuck-0.2.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 12:08:51.601364 tuck-0.2.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-06-25 12:08:42.000000 tuck-0.2.2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      981 2023-06-25 12:08:51.601364 tuck-0.2.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-06-25 12:08:42.000000 tuck-0.2.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/tuck/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9059 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/ast.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3554 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/editing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5645 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14951 2023-06-25 12:08:42.000000 tuck-0.2.2/tuck/wrappers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:08:51.597364 tuck-0.2.2/tuck.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-25 12:08:51.000000 tuck-0.2.2/tuck.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-06-25 13:07:56.000000 tuck-0.2.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 13:08:05.082511 tuck-0.2.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-06-25 13:07:56.000000 tuck-0.2.3/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      981 2023-06-25 13:08:05.086511 tuck-0.2.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-06-25 13:07:56.000000 tuck-0.2.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/tuck/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9057 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/ast.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3584 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/editing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5655 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14949 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/wrappers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/tuck.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/top_level.txt
```

### Comparing `tuck-0.2.2/LICENSE` & `tuck-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tuck-0.2.2/PKG-INFO` & `tuck-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.2
+Version: 0.2.3
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
```

### Comparing `tuck-0.2.2/README.md` & `tuck-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tuck-0.2.2/setup.cfg` & `tuck-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tuck-0.2.2/setup.py` & `tuck-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages  # type: ignore[import]
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='tuck',
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/PeterJCLaw/tuck',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/tuck/issues',
     },
     description="Semi-automated Python formatting.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tuck-0.2.2/tuck/ast.py` & `tuck-0.2.3/tuck/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import ast
 import token
 import functools
-from typing import List, Type, Tuple, TypeVar, Optional
+from typing import TypeVar
 
 import asttokens.util
 from asttokens import ASTTokens
 
 from .exceptions import TuckError
 
 TAst = TypeVar('TAst', bound=ast.AST)
@@ -30,32 +32,32 @@
     """
     A position within a document, compatible with Python AST positions.
 
     Line numbers are one-based, columns are zero-based.
     """
 
     @classmethod
-    def from_node_start(cls, node: ast.AST) -> 'Position':
+    def from_node_start(cls, node: ast.AST) -> Position:
         return cls(*_first_token(node).start)
 
     @classmethod
-    def from_node_end(cls, node: ast.AST) -> 'Position':
+    def from_node_end(cls, node: ast.AST) -> Position:
         return cls(*_last_token(node).start)
 
     def __init__(self, line: int, col: int) -> None:
         self.line = line
         self.col = col
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Position):
             return NotImplemented
 
         return self.line == other.line and self.col == other.col
 
-    def __lt__(self, other: 'Position') -> bool:
+    def __lt__(self, other: Position) -> bool:
         if not isinstance(other, Position):
             return NotImplemented  # type: ignore[unreachable]
 
         if self.line < other.line:
             return True
 
         if self.line > other.line:
@@ -73,49 +75,49 @@
 
 class NoNodeFoundError(NodeSearchError):
     def __init__(self) -> None:
         super().__init__('no_node_found', "No AST nodes were found!")
 
 
 class NoSuitableNodeFoundError(NodeSearchError):
-    def __init__(self, node_stack: List[ast.AST]) -> None:
+    def __init__(self, node_stack: list[ast.AST]) -> None:
         self.node_stack = node_stack
         super().__init__(
             'no_suitable_node_found',
             "No suitable node found (stack: {})".format(
                 " > ".join(type(x).__name__ for x in node_stack),
             ),
         )
 
 
 class NoSupportedNodeFoundError(NodeSearchError):
-    def __init__(self, node_stack: List[ast.AST]) -> None:
+    def __init__(self, node_stack: list[ast.AST]) -> None:
         self.node_stack = node_stack
         super().__init__(
             'no_supported_node_found',
             "No supported nodes found (stack: {})".format(
                 " > ".join(type(x).__name__ for x in node_stack),
             ),
         )
 
 
 class NodeFinder(ast.NodeVisitor):
     """
     Visitor which finds the AST node that should be wrapped for a given position.
     """
 
-    def __init__(self, position: Position, node_types: Tuple[Type[ast.AST], ...]) -> None:
+    def __init__(self, position: Position, node_types: tuple[type[ast.AST], ...]) -> None:
         self.target_position = position
         self.target_node_types = node_types
 
-        self.node_stack: List[ast.AST] = []
+        self.node_stack: list[ast.AST] = []
 
         self.found = False
 
-    def get_filtered_stack(self) -> List[ast.AST]:
+    def get_filtered_stack(self) -> list[ast.AST]:
         """
         In some cases we want to skip over the actual place in the AST and
         onwards to a parent node. This filtering achieves that.
 
         For convenience we also return the stack in reversed order, so that the
         nodes closest to the target position are at the front of the list.
         """
@@ -243,15 +245,15 @@
     Nodes which are all on the same line will never be considered matches.
     """
 
     def __init__(self, position: Position) -> None:
         self.target_position = position
 
         self._found: bool = False
-        self.found_node: Optional[ast.AST] = None
+        self.found_node: ast.AST | None = None
 
     def generic_visit(self, node: ast.AST) -> None:
         if self._found:
             return
 
         if not hasattr(node, 'lineno'):
             super().generic_visit(node)
```

### Comparing `tuck-0.2.2/tuck/cli.py` & `tuck-0.2.3/tuck/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import sys
 import json
 import difflib
 import argparse
-from typing import Dict, List, Union
+from typing import Dict, Union
 
 from .ast import Position
 from .main import process
 from .editing import Insertion, apply_insertions
 from .exceptions import TuckError
 
 FAIL = '\033[91m'
@@ -28,25 +30,25 @@
     pos = {'line': position.line - 1, 'character': position.col}
     return {
         'range': {'start': pos, 'end': pos},
         'newText': new_text,
     }
 
 
-def print_edits(insertions: List[Insertion]) -> None:
+def print_edits(insertions: list[Insertion]) -> None:
     edits = [insertion_as_lsp_data(*x) for x in insertions]
     print(json.dumps({'edits': edits}))
 
 
 def parse_position(position: str) -> Position:
     line, col = (int(x) for x in position.split(':'))
     return Position(line, col)
 
 
-def parse_args(argv: List[str]) -> argparse.Namespace:
+def parse_args(argv: list[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Wrap the python statement at a given position within a text document.",
     )
     parser.add_argument(
         'file',
         type=argparse.FileType(mode='r'),
         help="The file to read from. Use '-' to read from STDIN.",
@@ -112,9 +114,9 @@
     elif args.edits:
         print_edits(insertions)
     else:
         new_content = apply_insertions(content, insertions)
         print(new_content, end='')
 
 
-def main(argv: List[str] = sys.argv[1:]) -> None:
+def main(argv: list[str] = sys.argv[1:]) -> None:
     return run(parse_args(argv))
```

### Comparing `tuck-0.2.2/tuck/editing.py` & `tuck-0.2.3/tuck/editing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import ast
 import enum
 import itertools
-from typing import Set, List, Tuple, Iterable, Sequence
+from typing import List, Tuple, Iterable, Sequence
 
 from asttokens import ASTTokens
 
 from .ast import Position, AffectedNodeFinder
 from .exceptions import TuckError
 
 INDENT_SIZE = 4
@@ -51,15 +53,15 @@
 
     # Add indentations for things which were already wrapped somewhat. We're
     # only interested in lines which appear inside nodes that are themselves
     # going to be impacted by the wrapping and assume that outside of those
     # cases things are already in the right place. This assumption may turn out
     # to be invalid, in which case a new approach may be needed here.
 
-    lines_to_indent: Set[int] = set()
+    lines_to_indent: set[int] = set()
 
     for position, mutation_type in wrapping_summary:
         if mutation_type not in (
             MutationType.INDENT,
             MutationType.WRAP_INDENT,
         ):
             continue
@@ -92,36 +94,36 @@
         )
 
     wrapping_summary.sort(key=lambda x: x[0])
 
     return wrapping_summary
 
 
-def coalesce(summary: WrappingSummary) -> Iterable[Tuple[Position, List[MutationType]]]:
+def coalesce(summary: WrappingSummary) -> Iterable[tuple[Position, list[MutationType]]]:
     for pos, grouped in itertools.groupby(summary, lambda x: x[0]):
         yield pos, [x for _, x in grouped]
 
 
-def all_are_disjoint(grouped: Iterable[List[Position]]) -> bool:
+def all_are_disjoint(grouped: Iterable[list[Position]]) -> bool:
     ranges = sorted(
         (min(positions), max(positions))
         for positions in grouped
         if positions
     )
 
     for (_, lower_end), (upper_start, _) in zip(ranges, ranges[1:]):
         if upper_start < lower_end:
             return False
 
     return True
 
 
-def merge_insertions(grouped_insertions: Iterable[List[Insertion]]) -> List[Insertion]:
+def merge_insertions(grouped_insertions: Iterable[list[Insertion]]) -> list[Insertion]:
     flat_insertions = []
-    positions: List[List[Position]] = []
+    positions: list[list[Position]] = []
 
     for insertions in grouped_insertions:
         flat_insertions.extend(insertions)
         positions.append([x for x, _ in insertions])
 
     if not all_are_disjoint(positions):
         raise EditsOverlapError()
```

### Comparing `tuck-0.2.2/tuck/main.py` & `tuck-0.2.3/tuck/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import ast
-from typing import List, Tuple, TypeVar, Optional
+from typing import TypeVar
 
 from asttokens import ASTTokens
 
 from .ast import Position, NodeFinder, get_current_indent
 from .editing import (
     coalesce,
     Insertion,
@@ -53,15 +55,15 @@
 
     if not wrapping_summary:
         return wrapping_summary
 
     def should_keep(
         position: Position,
         mutation: MutationType,
-        previous: Optional[Tuple[Position, MutationType]],
+        previous: tuple[Position, MutationType] | None,
     ) -> bool:
         if mutation == MutationType.TRAILING_COMMA:
             tok = asttokens.get_token(position.line, position.col)
             if tok.string == ',':
                 return False
 
             prev_token = asttokens.prev_token(tok)
@@ -117,15 +119,15 @@
         for prev, current in zip([None, *wrapping_summary], wrapping_summary)
         if should_keep(*current, prev)
     ]
 
     return wrapping_summary
 
 
-def determine_insertions(asttokens: ASTTokens, position: Position) -> List[Insertion]:
+def determine_insertions(asttokens: ASTTokens, position: Position) -> list[Insertion]:
     finder = NodeFinder(position, WRAPPABLE_NODE_TYPES)
     assert asttokens.tree is not None
     finder.visit(asttokens.tree)
 
     node = finder.get_found_node(asttokens)
 
     # Note: insertions are actually applied in reverse, though we'll generate
@@ -161,18 +163,18 @@
         for pos, mutation_types in coalesce(wrapping_summary)
     ]
 
     return insertions
 
 
 def process(
-    positions: List[Position],
+    positions: list[Position],
     content: str,
     filename: str,
-) -> List[Insertion]:
+) -> list[Insertion]:
     try:
         asttokens = ASTTokens(content, parse=True, filename=filename)
     except SyntaxError as e:
         # Catch syntax errors within the file we were asked to parse. We trust
         # that the error is not within asttokens itself.
         raise TargetSyntaxError(e) from e
```

### Comparing `tuck-0.2.2/tuck/wrappers.py` & `tuck-0.2.3/tuck/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+from __future__ import annotations
+
 import ast
 import token
 import keyword
-from typing import List, Type, Tuple, Union, TypeVar, Callable, Iterable
+from typing import TypeVar, Callable, Iterable
 
 from asttokens import ASTTokens
 from asttokens.util import Token
 
 from .ast import Position, _last_token, _first_token
 from .editing import MutationType, WrappingSummary
 
 TAst = TypeVar('TAst', bound=ast.AST)
 
 
 WRAPPING_FUNCTIONS = []
 
 
-def node_wrapper(ast_type: Type[TAst]) -> Callable[
+def node_wrapper(ast_type: type[TAst]) -> Callable[
     [Callable[[ASTTokens, TAst], WrappingSummary]],
     Callable[[ASTTokens, TAst], WrappingSummary],
 ]:
     def wrapper(
         func: Callable[[ASTTokens, TAst], WrappingSummary],
     ) -> Callable[[ASTTokens, TAst], WrappingSummary]:
         WRAPPING_FUNCTIONS.append((ast_type, func))
         return func
     return wrapper
 
 
-def get_node_bounds(asttokens: ASTTokens, node: ast.expr) -> Tuple[Token, Token]:
+def get_node_bounds(asttokens: ASTTokens, node: ast.expr) -> tuple[Token, Token]:
     """
     Determine the outer bounds of the node, consuming any surrounding parentheses.
     """
 
     first_token = _first_token(node)
     last_token = _last_token(node)
 
@@ -68,15 +70,15 @@
         return True
 
     return False
 
 
 def expression_is_parenthesised(
     asttokens: ASTTokens,
-    node: Union[ast.BoolOp, ast.IfExp],
+    node: ast.BoolOp | ast.IfExp,
 ) -> bool:
     prev_token = asttokens.prev_token(_first_token(node))
     next_token = asttokens.next_token(_last_token(node))
     if prev_token.string == '(' and next_token.string == ')':
         return True
 
     return False
@@ -90,15 +92,15 @@
 
     return Position(*first_token.start)
 
 
 def node_start_positions(
     asttokens: ASTTokens,
     nodes: Iterable[ast.AST],
-) -> List[Position]:
+) -> list[Position]:
     return [node_start_position(asttokens, x) for x in nodes]
 
 
 def wrap_node_start_positions(
     asttokens: ASTTokens,
     nodes: Iterable[ast.AST],
 ) -> WrappingSummary:
@@ -107,15 +109,15 @@
         for pos in node_start_positions(asttokens, nodes)
     ]
 
 
 def wrap_generator_body(
     asttokens: ASTTokens,
     elt: ast.expr,
-    generators: List[ast.comprehension],
+    generators: list[ast.comprehension],
 ) -> WrappingSummary:
     start_positions = [Position.from_node_start(elt)]
 
     for generator in generators:
         start_positions.append(Position.from_node_start(generator))
         for compare in generator.ifs:
             if_token = asttokens.find_token(
@@ -280,15 +282,15 @@
     summary = wrap_generator_body(asttokens, node.key, node.generators)
     append_wrap_end(summary, node)
     return summary
 
 
 def wrap_function_def(
     asttokens: ASTTokens,
-    node: Union[ast.AsyncFunctionDef, ast.FunctionDef],
+    node: ast.AsyncFunctionDef | ast.FunctionDef,
 ) -> WrappingSummary:
     positions = node_start_positions(asttokens, node.args.args)
 
     if node.args.vararg:
         # Account for the * before the name
         args_star = asttokens.prev_token(_first_token(node.args.vararg))
         positions.append(Position(*args_star.start))
```

### Comparing `tuck-0.2.2/tuck.egg-info/PKG-INFO` & `tuck-0.2.3/tuck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.2
+Version: 0.2.3
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
```

