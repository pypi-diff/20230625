# Comparing `tmp/pyrefact-86.tar.gz` & `tmp/pyrefact-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-86.tar", last modified: Sun Jun 25 15:17:49 2023, max compression
+gzip compressed data, was "pyrefact-9.tar", last modified: Wed Nov  2 20:30:27 2022, max compression
```

## Comparing `pyrefact-86.tar` & `pyrefact-9.tar`

### file list

```diff
@@ -1,33 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:17:49.692288 pyrefact-86/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-25 15:17:34.000000 pyrefact-86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-25 15:17:49.692288 pyrefact-86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-25 15:17:34.000000 pyrefact-86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-25 15:17:34.000000 pyrefact-86/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:17:49.688289 pyrefact-86/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26568 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   126558 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13113 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    33697 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/symbolic_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-06-25 15:17:34.000000 pyrefact-86/pyrefact/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:17:49.688289 pyrefact-86/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 15:17:49.000000 pyrefact-86/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:17:49.692288 pyrefact-86/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:17:49.688289 pyrefact-86/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-25 15:17:34.000000 pyrefact-86/tests/testing_infra.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405663 pyrefact-9/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-9/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.405542 pyrefact-9/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-9/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.404795 pyrefact-9/pyrefact/
+-rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-9/pyrefact/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-9/pyrefact/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/completion.py
+-rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-9/pyrefact/constants.py
+-rw-r--r--   0 olle       (501) staff       (20)    31081 2022-11-02 20:24:19.000000 pyrefact-9/pyrefact/fixes.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-9/pyrefact/main.py
+-rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/parsing.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405383 pyrefact-9/pyrefact.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 20:30:27.405698 pyrefact-9/setup.cfg
+-rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 20:30:04.000000 pyrefact-9/setup.py
```

### Comparing `pyrefact-86/LICENSE` & `pyrefact-9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefact-86/pyrefact/symbolic_math.py` & `pyrefact-9/pyrefact/fixes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,846 +1,875 @@
-"""Features related to symbolic mathematics."""
-from __future__ import annotations
-
-
 import ast
+import builtins
 import collections
+import heapq
+import io
 import itertools
-import math
-from typing import Callable, Mapping, Sequence, Tuple
+import queue
+import re
+import sys
+import tempfile
+from pathlib import Path
+from typing import Collection, Iterable, List, Mapping, Tuple, Union
+
+import black
+import isort
+import rmspace
+from pylint.lint import Run
+
+from pyrefact import parsing
+from pyrefact.constants import ASSUMED_PACKAGES, ASSUMED_SOURCES, PACKAGE_ALIASES
+
+_REDUNDANT_UNDERSCORED_ASSIGN_RE_PATTERN = r"(?<![^\n]) *(\*?_ *,? *)+[\*\+\/\-\|\&:]?= *(?![=])"
+
+
+def _deconstruct_pylint_warning(error_line: str) -> Tuple[Path, int, int, str, str]:
+    filename, lineno, charno, error_code, error_msg = error_line.split(":")
+
+    return filename, lineno, charno, error_code.strip(), error_msg.strip()
+
+
+def _find_pylint_errors(content: str, error_code: str) -> Iterable[str]:
+    original_sys_stdout = sys.stdout
+    with tempfile.NamedTemporaryFile(suffix=".py") as temp:
+        temp.write(content.encode("utf-8"))
+        temp.seek(0)
+        stdout = io.StringIO()
+        args = [
+            "--disable",
+            "all",
+            "--enable",
+            f"{error_code}",
+            temp.name,
+        ]
+        try:
+            sys.stdout = stdout
+            Run(args, exit=False)
+        finally:
+            sys.stdout = original_sys_stdout
+
+    re_pattern = re.compile(r".*\.py:\d+:\d+: \w\d+: .* \(" + error_code + r"\)")
+    output = stdout.getvalue()
+    for line in output.splitlines():
+        if re_pattern.match(line):
+            yield line
 
-import sympy
-import sympy.parsing
 
-from pyrefact import constants, parsing, processing
+def _get_undefined_variables(content: str) -> Collection[str]:
+    variables = set()
+    for line in _find_pylint_errors(content, "undefined-variable"):
+        try:
+            _, *_, error_msg = _deconstruct_pylint_warning(line)
+            _, variable_name, _ = error_msg.split("'")
+            variables.add(variable_name)
+        except ValueError:
+            pass
 
+    return variables
 
-def _get_range_start_end(rng: ast.Call) -> Tuple[ast.AST, ast.AST]:
-    if not (isinstance(rng.func, ast.Name) and rng.func.id == "range"):
-        raise ValueError(f"Expected range call, not {rng}")
 
-    if len(rng.args) == 1:
-        return ast.Constant(value=0, kind=None), rng.args[0], ast.Constant(value=1, kind=None)
+def _is_private(variable: str) -> bool:
+    return variable.startswith("_")
 
-    if len(rng.args) == 2:
-        return *rng.args, ast.Constant(value=1, kind=None)
 
-    if len(rng.args) == 3:
-        return tuple(rng.args)
+def _rename_variable(variable: str, *, static: bool, private: bool) -> str:
+    if variable == "_":
+        return variable
 
-    raise NotImplementedError(f"Cannot parse range with arg count of {len(rng.args)}")
+    renamed_variable = variable.upper() if static else variable.lower()
+    renamed_variable = re.sub("_{1,}", "_", renamed_variable)
 
+    if renamed_variable.endswith("_"):
+        renamed_variable = renamed_variable[:-1]
 
-def _parse_sympy_expr(expression):
-    return sympy.parsing.sympy_parser.parse_expr(expression)
+    if private and not _is_private(renamed_variable):
+        renamed_variable = f"_{renamed_variable}"
+    if not private and _is_private(renamed_variable):
+        renamed_variable = renamed_variable.lstrip("_")
 
+    if renamed_variable:
+        return renamed_variable
 
-def _ast_to_symmath_expr_conversion(node, conversion):
-    if isinstance(node, ast.BoolOp):
-        values = []
-        for value in node.values:
-            expression, node_conversion = _ast_to_symmath_expr_conversion(value, conversion)
-            conversion.update(node_conversion)
-            values.append(expression)
-        if isinstance(node.op, ast.And):
-            return sympy.And(*values), conversion
-        if isinstance(node.op, ast.Or):
-            return sympy.Or(*values), conversion
+    raise RuntimeError(f"Unable to find a replacement name for {variable}")
 
-    if isinstance(node, ast.UnaryOp) and isinstance(node.op, ast.Not):
-        operand, conversion = _ast_to_symmath_expr_conversion(node.operand, conversion)
-        return sympy.Not(operand), conversion
 
+def _rename_class(name: str, *, private: bool) -> str:
+    name = re.sub("_{1,}", "_", name)
+    if len(name) == 0:
+        raise ValueError("Cannot rename empty name")
+    if len(name) == 1:
+        name = name.upper()
+    else:
+        accum = (last := name[0].upper())
+        for char in name[1:]:
+            if last == "_":
+                accum += (last := char.upper())
+            else:
+                accum += char
+            last = char
+
+        name = accum
+
+    if private and not _is_private(name):
+        return f"_{name}"
+    if not private and _is_private(name):
+        return name[1:]
+
+    return name
+
+
+def _get_uses_of(node: ast.AST, scope: ast.AST, content: str) -> Iterable[ast.Name]:
+    name = node.id if isinstance(node, ast.Name) else node.name
+    reference_nodes = {
+        refnode
+        for refnode in ast.walk(scope)
+        if isinstance(refnode, ast.Name)
+        and isinstance(refnode.ctx, ast.Load)
+        and refnode.id == name
+    }
     if isinstance(node, ast.Name):
-        return sympy.Symbol(node.id), conversion
+        start = (node.lineno, node.col_offset)
+        end = (node.end_lineno, node.end_col_offset)
+    elif isinstance(node, (ast.ClassDef, ast.AsyncFunctionDef, ast.FunctionDef)):
+        start_charno, end_charno = _get_func_name_start_end(node, content)
+        start = (node.lineno, start_charno)
+        end = (node.lineno, end_charno)
+    else:
+        raise NotImplementedError(f"Unknown type: {type(node)}")
+    for refnode in reference_nodes:
+        n_start = (refnode.lineno, refnode.col_offset)
+        n_end = (refnode.end_lineno, refnode.end_col_offset)
+        if end < n_start:
+            yield refnode
+        elif isinstance(node, (ast.Module, ast.ClassDef)) and n_end < start:
+            yield refnode
+
+
+def _get_variable_name_substitutions(ast_tree: ast.AST, content: str) -> Mapping[ast.AST, str]:
+    renamings = collections.defaultdict(set)
+    classdefs: List[parsing.Statement] = []
+    funcdefs: List[parsing.Statement] = []
+    for node in parsing.iter_classdefs(ast_tree):
+        name = node.name
+        substitute = _rename_class(name, private=_is_private(name))
+        classdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    for node in parsing.iter_funcdefs(ast_tree):
+        name = node.name
+        substitute = _rename_variable(name, private=_is_private(name), static=False)
+        funcdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    for node in parsing.iter_assignments(ast_tree):
+        substitute = _rename_variable(node.id, private=_is_private(node.id), static=True)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    while funcdefs or classdefs:
+        for partial_tree in classdefs.copy():
+            classdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = _rename_class(name, private=_is_private(name))
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                if name.startswith("__") and name.endswith("__"):
+                    continue
+                funcdefs.append(node)
+                substitute = _rename_variable(name, private=_is_private(name), static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                substitute = _rename_variable(name, private=_is_private(name), static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+        for partial_tree in funcdefs.copy():
+            funcdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = _rename_class(name, private=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                funcdefs.append(node)
+                substitute = _rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                substitute = _rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+
+    return renamings
+
+
+def _get_variable_re_pattern(variable) -> str:
+    return r"(?<![A-Za-z_\.])" + variable + r"(?![A-Za-z_])"
+
+
+def _get_func_name_start_end(
+    node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef], content: str
+) -> Tuple[int, int]:
+    start, end = parsing.get_charnos(node, content)
+    codeblock = content[start:end]
+    for match in re.finditer(_get_variable_re_pattern(node.name), codeblock):
+        if match.group() == node.name:
+            end = start + match.end()
+            start += match.start()
+            return start, end
+
+    raise RuntimeError(f"Cannot find {node.name} in code block:\n{codeblock}")
+
+
+def _fix_variable_names(
+    content: str,
+    renamings: Mapping[ast.AST, str],
+    preserve: Collection[str] = frozenset(),
+) -> str:
+    replacements = []
+    for node, substitutes in renamings.items():
+        if len(substitutes) != 1:
+            raise RuntimeError(
+                f"Expected 1 substitute, got {len(substitutes)}: {substitutes}\nCode:\n{ast.dump(node, indent=2)}"
+            )
+        substitute = substitutes.pop()
+        if isinstance(node, ast.Name):
+            if node.id != substitute and node.id not in preserve:
+                start, end = parsing.get_charnos(node, content)
+                replacements.append((start, end, substitute))
+            continue
 
-    unparse = parsing.unparse(node)
-    if unparse in conversion:
-        expression, _ = conversion[unparse]
-        return expression, conversion
-
-    variable_name = f"__unparse_var_{len(conversion)}__"
-    if conversion:
-        _, variable_names = zip(*conversion.values())
-        assert variable_name not in variable_names
-
-    expression = sympy.Symbol(variable_name)
-    conversion[unparse] = expression, node
-    return expression, conversion
-
-
-def _ast_to_symmath_expr(node):
-    expression, conversion = _ast_to_symmath_expr_conversion(node, {})
-    conversion = dict(conversion.values())
-    return expression, conversion
-
-
-def _symmath_expr_to_ast(expression, conversion: Mapping[str, ast.AST]):
-    if isinstance(expression, sympy.Symbol):
-        if expression in conversion:
-            return conversion[expression]
-        return ast.Name(id=expression.name)
-    if isinstance(expression, sympy.And):
-        return ast.BoolOp(
-            op=ast.And(), values=[_symmath_expr_to_ast(v, conversion) for v in expression.args]
-        )
-    if isinstance(expression, sympy.Or):
-        return ast.BoolOp(
-            op=ast.Or(), values=[_symmath_expr_to_ast(v, conversion) for v in expression.args]
-        )
-    if isinstance(expression, sympy.Not):
-        return ast.UnaryOp(
-            op=ast.Not(), operand=_symmath_expr_to_ast(expression.args[0], conversion)
-        )
-    if isinstance(expression, sympy.logic.boolalg.BooleanTrue):
-        return ast.Constant(value=True, kind=None)
-    if isinstance(expression, sympy.logic.boolalg.BooleanFalse):
-        return ast.Constant(value=False, kind=None)
+        if node.name == substitute or node.name in preserve:
+            continue
 
-    raise ValueError(f"Unsupported expression: {expression} of type {type(expression)}")
+        if not isinstance(node, (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef)):
+            raise TypeError(f"Unknown type: {type(node)}")
 
+        start, end = _get_func_name_start_end(node, content)
 
-def simplify_ast_boolop(node: ast.BoolOp | ast.UnaryOp) -> ast.BoolOp | ast.UnaryOp:
-    """Simplify boolean AST expression.
+        replacements.append((start, end, substitute))
 
-    Args:
-        node (ast.BoolOp | ast.UnaryOp): Boolean AST expression
+    for start, end, substitute in sorted(set(replacements), reverse=True):
+        print(f"Replacing {content[start:end]} with {substitute}")
+        content = content[:start] + substitute + content[end:]
 
-    Returns:
-        ast.BoolOp | ast.UnaryOp: Simplified boolean AST expression
+    return content
 
-    """
-    expression, conversion = _ast_to_symmath_expr(node)
-    expression = expression.simplify()
 
-    return _symmath_expr_to_ast(expression, conversion)
+def _fix_undefined_variables(content: str, variables: Collection[str]) -> str:
+    variables = set(variables)
 
+    lines = content.splitlines()
+    change_count = -len(lines)
+    lineno = next(
+        i
+        for i, line in enumerate(lines)
+        if not line.startswith("#")
+        and not line.startswith("'''")
+        and not line.startswith('"""')
+        and not line.startswith("from __future__ import")
+    )
+    for package, package_variables in ASSUMED_SOURCES.items():
+        overlap = variables.intersection(package_variables)
+        if overlap:
+            fix = f"from {package} import " + ", ".join(sorted(overlap))
+            print(f"Inserting '{fix}' at line {lineno}")
+            lines.insert(lineno, fix)
 
-def _simplify_math(f: Callable) -> ast.AST:
-    def wrapper(*args, **kwargs):
-        expression = f(*args, **kwargs)
-        source = parsing.unparse(expression).strip()
+    for package in ASSUMED_PACKAGES & variables:
+        fix = f"import {package}"
+        print(f"Inserting '{fix}' at line {lineno}")
+        lines.insert(lineno, fix)
 
-        # TODO substitute constant calls, attributes and other stuff with variables
+    for alias in PACKAGE_ALIASES.keys() & variables:
+        package = PACKAGE_ALIASES[alias]
+        fix = f"import {package} as {alias}"
+        print(f"Inserting '{fix}' at line {lineno}")
+        lines.insert(lineno, fix)
 
-        source = str(sympy.simplify(source))
-        return parsing.parse(source)
+    change_count += len(lines)
 
-    return wrapper
+    assert change_count >= 0
 
+    if change_count == 0:
+        return content
 
-@_simplify_math
-def _sum_int_squares_to(value: ast.AST) -> ast.AST:
-    return ast.BinOp(
-        left=ast.BinOp(
-            left=ast.BinOp(left=value, op=ast.Sub(), right=ast.Constant(value=1, kind=None)),
-            op=ast.Mult(),
-            right=value,
-        ),
-        op=ast.Div(),
-        right=ast.Constant(value=2, kind=None),
-    )
+    return "\n".join(lines) + "\n"
 
 
-@_simplify_math
-def _sum_range(rng: ast.Call) -> ast.AST:
-    start, end, step = _get_range_start_end(rng)
-
-    if not parsing.match_template(step, ast.Constant(value=1)):
-        return rng
-
-    if parsing.match_template(end, ast.Constant(value=0)):
-        return _sum_int_squares_to(end)
-
-    return ast.BinOp(left=_sum_int_squares_to(end), op=ast.Sub(), right=_sum_int_squares_to(start))
-
-
-@_simplify_math
-def _sum_constants(values: Sequence[ast.AST]) -> ast.AST:
-    expr = " + ".join(parsing.unparse(node).strip() for node in values)
-    return parsing.parse(expr)
-
-
-def _integrate_over(expr: ast.AST, generators: Sequence[ast.comprehension]) -> ast.AST:
-    source = parsing.unparse(expr).strip()
-    sym_expr = _parse_sympy_expr(source)
-    for comprehension in generators:
-        integrand = _parse_sympy_expr(parsing.unparse(comprehension.target).strip())
-        if isinstance(comprehension.iter, ast.Call):
-            start, end, step = _get_range_start_end(comprehension.iter)
-            lower = _parse_sympy_expr(parsing.unparse(start).strip())
-            upper = _parse_sympy_expr(parsing.unparse(end).strip())
-            step = _parse_sympy_expr(parsing.unparse(step).strip())
+def define_undefined_variables(content: str) -> str:
+    """Attempt to find imports matching all undefined variables.
 
-            if step == 1:
-                upper -= 1
-            else:
-                n_steps = math.floor((upper - lower) / step)
-                lower = lower / step
-                upper = lower + n_steps
-                sym_expr = sym_expr.subs(integrand, step * integrand)
-
-            sym_expr = sympy.Sum(sym_expr, (integrand, lower, upper))
-
-        elif isinstance(comprehension.iter, (ast.Tuple, ast.List, ast.Set)):
-            values = [
-                _parse_sympy_expr(parsing.unparse(value).strip())
-                for value in comprehension.iter.elts
-            ]
-            if isinstance(comprehension.iter, ast.Set):
-                values = set(values)
+    Args:
+        content (str): Python source code
 
-            sym_expr = sum(sym_expr.subs(integrand, value) for value in values)
+    Returns:
+        str: Source code with added imports
+    """
+    undefined_variables = _get_undefined_variables(content)
+    if undefined_variables:
+        return _fix_undefined_variables(content, undefined_variables)
 
-        else:
-            raise NotImplementedError(f"Cannot parse iterator: {comprehension.iter}")
+    return content
 
-    sym_expr = sym_expr.doit()
-    sym_expr = sympy.simplify(sym_expr)
 
-    return parsing.parse(str(sym_expr))
+def _recursive_attribute_name(attribute: ast.Attribute) -> str:
+    if isinstance(attribute.value, ast.Attribute):
+        return f"{_recursive_attribute_name(attribute.value)}.{attribute.attr}"
+    return f"{attribute.value.id}.{attribute.attr}"
 
 
-@processing.fix
-def simplify_math_iterators(source: str) -> str:
-    root = parsing.parse(source)
+def _get_unused_imports(ast_tree: ast.Module) -> str:
 
-    template = ast.Call(
-        func=ast.Name(id=tuple(constants.MATH_FUNCTIONS)), keywords=[], args=[object]
-    )
-    basic_types_template = {ast.Name, ast.Constant, ast.UnaryOp, ast.BinOp}
-    basic_iter_template = (
-        ast.Call(func=ast.Name(id="range"), args=basic_types_template),
-        ast.Set(elts=basic_types_template),
-        ast.List(elts=basic_types_template),
-        ast.Tuple(elts=basic_types_template),
-    )
-    basic_generator_template = ast.comprehension(iter=basic_iter_template, ifs=[], target=ast.Name)
-    basic_comprehension_template = (
-        ast.GeneratorExp(generators={basic_generator_template}),
-        ast.ListComp(generators={basic_generator_template}),
+    names = set()
+    attributes = set()
+    imports = set()
+    for node in ast.walk(ast_tree):
+        if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load):
+            names.add(node)
+        elif isinstance(node, ast.Attribute):
+            attributes.add(node)
+        elif isinstance(node, (ast.Import, ast.ImportFrom)):
+            if isinstance(node, ast.ImportFrom) and node.module == "__future__":
+                continue
+            for alias in node.names:
+                imports.add(alias.name if alias.asname is None else alias.asname)
+
+    used_names = {name.id for name in names}
+    for attribute in attributes:
+        try:
+            full_name = _recursive_attribute_name(attribute)
+        except AttributeError:
+            continue
+
+        used_names.add(full_name)
+        while "." in full_name:
+            full_name = re.sub(r"\.[^\.]*$", "", full_name)
+            used_names.add(full_name)
+
+    return imports - used_names
+
+
+def _get_unused_imports_split(
+    ast_tree: ast.Module, unused_imports: Collection[str]
+) -> Tuple[
+    Collection[Union[ast.Import, ast.ImportFrom]],
+    Collection[Union[ast.Import, ast.ImportFrom]],
+]:
+    import_unused_aliases = collections.defaultdict(set)
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            for alias in node.names:
+                used_name = alias.name if alias.asname is None else alias.asname
+                if used_name in unused_imports:
+                    import_unused_aliases[node].add(alias)
+
+    partially_unused_imports = set()
+    completely_unused_imports = set()
+
+    for node, unused_aliases in import_unused_aliases.items():
+        if set(node.names) - unused_aliases:
+            partially_unused_imports.add(node)
+        else:
+            completely_unused_imports.add(node)
+
+    return completely_unused_imports, partially_unused_imports
+
+
+def _construct_import_statement(
+    node: Union[ast.Import, ast.ImportFrom], unused_imports: Collection[str]
+) -> str:
+    statement = "import " + ", ".join(
+        sorted(
+            alias.name if alias.asname is None else f"{alias.name} as {alias.asname}"
+            for alias in node.names
+            if (alias.name if alias.asname is None else alias.asname) not in unused_imports
+        )
     )
-    basic_collection_template = (
-        ast.Tuple(elts={ast.Constant, ast.UnaryOp, ast.BinOp}),
-        ast.List(elts={ast.Constant, ast.UnaryOp, ast.BinOp}),
+    if isinstance(node, ast.Import):
+        return statement
+
+    return f"from {node.module} {statement}"
+
+
+def _remove_unused_imports(
+    ast_tree: ast.Module, content: str, unused_imports: Collection[str]
+) -> str:
+    completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
+        ast_tree, unused_imports
     )
+    if completely_unused_imports:
+        content = remove_nodes(content, completely_unused_imports, ast_tree)
+        if not partially_unused_imports:
+            return content
+        ast_tree = ast.parse(content)
+        completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
+            ast_tree, unused_imports
+        )
 
-    for node in parsing.walk(root, template):
-        arg = node.args[0]
-        if parsing.match_template(arg, ast.Call(func=ast.Name(id="range"))):
-            if any((node is not arg for node in parsing.walk(arg, (ast.Attribute, ast.Call)))):
-                continue
-            if node.func.id != "sum":
-                continue
-            yield node, _sum_range(arg)
+    if completely_unused_imports:
+        raise RuntimeError("Failed to remove unused imports")
 
-        elif parsing.match_template(arg, basic_collection_template):
-            if any(parsing.walk(arg, ast.Attribute)):
-                continue
-            if not all(
-                parsing.match_template(node.func, ast.Name(id="range"))
-                for node in parsing.walk(arg, ast.Call)
-            ):
-                continue
-            yield node, _sum_constants(arg.elts)
+    # For every import, construct what we would like it to look like with redundant stuff removed, find the old
+    # version of it, and replace it.
 
-        elif parsing.match_template(arg, basic_comprehension_template):
-            if any(parsing.walk(arg, ast.Attribute)):
-                continue
-            if not all(
-                parsing.match_template(node.func, ast.Name(id="range"))
-                for node in parsing.walk(arg, ast.Call)
-            ):
-                continue
-            yield node, _integrate_over(arg.elt, arg.generators)
+    # Iterate from bottom to top of file, so we don't have to re-calculate the linenos etc.
+    for node in sorted(
+        partially_unused_imports,
+        key=lambda n: (n.lineno, n.col_offset, n.end_lineno, n.end_col_offset),
+        reverse=True,
+    ):
+        start, end = parsing.get_charnos(node, content)
+        code = content[start:end]
+        replacement = _construct_import_statement(node, unused_imports)
+        print(f"Replacing:\n{code}\nWith:\n{replacement}")
+        content = content[:start] + replacement + content[end:]
 
+    return content
 
-@processing.fix
-def simplify_boolean_expressions(source: str) -> str:
-    root = parsing.parse(source)
 
-    regular_compare_template = ast.Compare(
-        left=object,
-        ops=[(ast.Eq, ast.NotEq, ast.Gt, ast.Lt, ast.GtE, ast.LtE)],
-        comparators=[object],
-    )
+def remove_unused_imports(content: str) -> str:
+    """Remove unused imports from source code.
 
-    for node in parsing.walk(root, ast.BoolOp):
-        if isinstance(node.op, (ast.And, ast.Or)):
-            # Find opposite expressions
-            expression_conditions = collections.defaultdict(set)
-            for value in node.values:
-                if isinstance(value, ast.UnaryOp) and isinstance(value.op, ast.Not):
-                    expression_conditions[parsing.unparse(value.operand)].add(False)
-                else:
-                    expression_conditions[parsing.unparse(value)].add(True)
+    Args:
+        content (str): Python source code
 
-            if {True, False} in expression_conditions.values():
-                # Something can (in the or case) or must (in the and case) be both True and False
-                if isinstance(node.op, ast.Or):
-                    yield node, ast.Constant(value=True, kind=None)
-                else:
-                    yield node, ast.Constant(value=False, kind=None)
+    Returns:
+        str: Source code, with added imports removed
+    """
+    ast_tree = ast.parse(content)
+    unused_imports = _get_unused_imports(ast_tree)
+    if unused_imports:
+        content = _remove_unused_imports(ast_tree, content, unused_imports)
 
-                continue
+    return content
 
-            # Find redundant combinations of >, >=, <, >=, ==, !=
-            constant_bounds = collections.defaultdict(lambda: collections.defaultdict(set))
-            # Should contain for example:
-            # {"f(x)": {ast.Gt: {(4, <ast>)}, ast.Lt: {(6, <ast>)}, ast.Eq: {(5, <ast>)}}}
-            # Which would mean that f(x) is between 4 and 6, and is equal to 5, so this
-            # could be simplified to f(x) == 5. Since the asts that provided the Gt, Lt
-            # and Eq constraints are also known, we know that we can remove the ones that
-            # gave the gt and lt constraints.
-            constraint_values = list(node.values)
-            for value in constraint_values:
-                if parsing.match_template(value, ast.BoolOp(op=type(node.op))):
-                    constraint_values.extend(value.values)
-                    continue
 
-            for value in parsing.filter_nodes(constraint_values, regular_compare_template):
-                left_is_unparsed = False
-                right_is_unparsed = False
-                try:
-                    left = parsing.literal_value(value.left)
-                except ValueError:
-                    left = parsing.unparse(value.left)
-                    left_is_unparsed = True
-
-                try:
-                    right = parsing.literal_value(value.comparators[0])
-                except ValueError:
-                    right = parsing.unparse(value.comparators[0])
-                    right_is_unparsed = True
+def fix_rmspace(content: str) -> str:
+    """Remove trailing whitespace from source code.
 
-                if left_is_unparsed and right_is_unparsed:
-                    continue
+    Args:
+        content (str): Python source code
 
-                if not left_is_unparsed and not right_is_unparsed:
-                    # Pure literal comparison is handled in the next step
-                    continue
+    Returns:
+        str: Source code, without trailing whitespace
+    """
+    return rmspace.format_str(content)
 
-                op_type = type(value.ops[0])
-                opposite_op_mapping = {
-                    ast.Eq: ast.Eq,
-                    ast.NotEq: ast.NotEq,
-                    ast.Gt: ast.Lt,
-                    ast.Lt: ast.Gt,
-                    ast.GtE: ast.LtE,
-                    ast.LtE: ast.GtE,
-                }
-                if right_is_unparsed:
-                    op_type = opposite_op_mapping[op_type]
-                    left, right = right, left
 
-                if not isinstance(right, (int, float, bool)):
-                    continue
+def fix_black(content: str) -> str:
+    """Format source code with black.
 
-                try:
-                    constant_bounds[left][op_type].add((right, value))
-                except TypeError:
-                    pass
-
-            redundant_and_values = set()
-            redundant_or_values = set()
-            always_true = False
-            always_false = False
-            for left, bounds in constant_bounds.items():
-                bounds_ordered = {
-                    operator_type: sorted(
-                        values, key=lambda tup: (tup[1].lineno, tup[1].col_offset)
-                    )
-                    for operator_type, values in bounds.items()
-                }
-                bounds.clear()
-                bounds.update(bounds_ordered)
-                # Check for identical constraints
-                for (thr1, thr1_value), (thr2, thr2_value) in itertools.chain.from_iterable(
-                    itertools.combinations(subset, 2) for subset in bounds.values()
-                ):
-                    if thr1 == thr2:
-                        redundant_value = thr2_value if thr2_value in node.values else thr1_value
-                        redundant_and_values.add(redundant_value)
-                        redundant_or_values.add(redundant_value)
-
-                # Check for redundant constraints, where one is stronger than the other.
-                # These checks purposefully do not cover the case where the two constraints
-                # are equal, since that is already covered by the previous check.
-                if len(bounds[ast.Eq]) >= 2:
-                    for (eq1, _), (eq2, _) in itertools.combinations(bounds[ast.Eq], 2):
-                        if eq1 != eq2:
-                            always_false |= isinstance(node.op, ast.And)
-
-                if len(bounds[ast.Gt]) >= 2:
-                    for (gt1, gt1_value), (gt2, gt2_value) in itertools.combinations(
-                        bounds[ast.Gt], 2
-                    ):
-                        if gt1 > gt2:
-                            redundant_and_values.add(gt2_value)
-                            redundant_or_values.add(gt1_value)
-                        if gt1 < gt2:
-                            redundant_and_values.add(gt1_value)
-                            redundant_or_values.add(gt2_value)
-
-                if len(bounds[ast.Lt]) >= 2:
-                    for (lt1, lt1_value), (lt2, lt2_value) in itertools.combinations(
-                        bounds[ast.Lt], 2
-                    ):
-                        if lt1 < lt2:
-                            redundant_and_values.add(lt2_value)
-                            redundant_or_values.add(lt1_value)
-                        if lt1 > lt2:
-                            redundant_and_values.add(lt1_value)
-                            redundant_or_values.add(lt2_value)
-
-                if len(bounds[ast.GtE]) >= 2:
-                    for (gte1, gte1_value), (gte2, gte2_value) in itertools.combinations(
-                        bounds[ast.GtE], 2
-                    ):
-                        if gte1 > gte2:
-                            redundant_and_values.add(gte2_value)
-                            redundant_or_values.add(gte1_value)
-                        if gte1 < gte2:
-                            redundant_and_values.add(gte1_value)
-                            redundant_or_values.add(gte2_value)
-
-                if len(bounds[ast.LtE]) >= 2:
-                    for (lte1, lte1_value), (lte2, lte2_value) in itertools.combinations(
-                        bounds[ast.LtE], 2
-                    ):
-                        if lte1 < lte2:
-                            redundant_and_values.add(lte2_value)
-                            redundant_or_values.add(lte1_value)
-                        if lte1 > lte2:
-                            redundant_and_values.add(lte1_value)
-                            redundant_or_values.add(lte2_value)
-
-                # eq vs everything else
-                for eq, eq_value in bounds[ast.Eq]:
-                    for neq, neq_value in bounds[ast.NotEq]:
-                        if eq == neq:
-                            always_true |= isinstance(node.op, ast.Or)
-                            always_false |= isinstance(node.op, ast.And)
-                        if eq != neq:
-                            redundant_or_values.add(eq_value)
-                            redundant_and_values.add(neq_value)
-
-                    for gt, gt_value in bounds[ast.Gt]:
-                        if eq <= gt:
-                            always_false |= isinstance(node.op, ast.And)
-                        if eq > gt:
-                            redundant_or_values.add(eq_value)
-                            redundant_and_values.add(gt_value)
-
-                    for lt, lt_value in bounds[ast.Lt]:
-                        if eq >= lt:
-                            always_false |= isinstance(node.op, ast.And)
-                        if eq < lt:
-                            redundant_or_values.add(eq_value)
-                            redundant_and_values.add(lt_value)
-
-                    for gte, gte_value in bounds[ast.GtE]:
-                        if eq < gte:
-                            always_false |= isinstance(node.op, ast.And)
-                        if eq >= gte:
-                            redundant_or_values.add(eq_value)
-                            redundant_and_values.add(gte_value)
-
-                    for lte, lte_value in bounds[ast.LtE]:
-                        if eq > lte:
-                            always_false |= isinstance(node.op, ast.And)
-                        if eq <= lte:
-                            redundant_or_values.add(eq_value)
-                            redundant_and_values.add(lte_value)
-
-                # neq vs everything else, except eq
-                for neq, neq_value in bounds[ast.NotEq]:
-                    for gt, gt_value in bounds[ast.Gt]:
-                        if neq <= gt:
-                            redundant_and_values.add(neq_value)
-                            redundant_or_values.add(gt_value)
-                        if neq > gt:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                    for lt, lt_value in bounds[ast.Lt]:
-                        if neq >= lt:
-                            redundant_and_values.add(neq_value)
-                            redundant_or_values.add(lt_value)
-                        if neq < lt:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                    for gte, gte_value in bounds[ast.GtE]:
-                        if neq < gte:
-                            redundant_and_values.add(neq_value)
-                            redundant_or_values.add(gte_value)
-                        if neq >= gte:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                    for lte, lte_value in bounds[ast.LtE]:
-                        if neq > lte:
-                            redundant_and_values.add(neq_value)
-                            redundant_or_values.add(lte_value)
-                        if neq <= lte:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                # gt vs everything else, except eq and neq
-                for gt, gt_value in bounds[ast.Gt]:
-                    for lt, lt_value in bounds[ast.Lt]:
-                        if gt >= lt:
-                            always_false |= isinstance(node.op, ast.And)
-                        if gt < lt:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                        if gt == lt:
-                            for eq, eq_value in bounds[ast.Eq]:
-                                if gt == eq:
-                                    always_true |= isinstance(node.op, ast.Or)
-                                    always_false |= isinstance(node.op, ast.And)
-
-                    for lte, lte_value in bounds[ast.LtE]:
-                        if gt >= lte:
-                            always_false |= isinstance(node.op, ast.And)
-                        if gt < lte:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                    for gte, gte_value in bounds[ast.GtE]:
-                        if gt > gte:
-                            redundant_and_values.add(gte_value)
-                            redundant_or_values.add(gt_value)
-                        if gt <= gte:
-                            redundant_and_values.add(gt_value)
-                            redundant_or_values.add(gte_value)
-
-                # gte vs everything else, except eq, neq and gt
-                for gte, gte_value in bounds[ast.GtE]:
-                    for lt, lt_value in bounds[ast.Lt]:
-                        if gte >= lt:
-                            always_false |= isinstance(node.op, ast.And)
-                        if gte < lt:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                    for lte, lte_value in bounds[ast.LtE]:
-                        if gte > lte:
-                            always_false |= isinstance(node.op, ast.And)
-                        if gte <= lte:
-                            always_true |= isinstance(node.op, ast.Or)
-
-                # lt vs everything else, except eq, neq, gt and gte (i.e. only lte)
-                for lt, lt_value in bounds[ast.Lt]:
-                    for lte, lte_value in bounds[ast.LtE]:
-                        if lt <= lte:
-                            redundant_and_values.add(lte_value)
-                            redundant_or_values.add(lt_value)
-                        if lt > lte:
-                            redundant_and_values.add(lt_value)
-                            redundant_or_values.add(lte_value)
+    Args:
+        content (str): Python source code
 
-            if always_false:
-                yield node, ast.Constant(value=False, kind=None)
-                continue
+    Returns:
+        str: Source code, formatted with black
+    """
+    return black.format_str(content, mode=black.Mode(line_length=100))
 
-            if always_true:
-                yield node, ast.Constant(value=True, kind=None)
-                continue
 
-            if redundant_and_values and isinstance(node.op, ast.And):
-                values = [value for value in node.values if value not in redundant_and_values]
-                if len(values) == 1:
-                    yield node, values[0]
-                    continue
-                if values != node.values:
-                    yield node, ast.BoolOp(op=node.op, values=values)
-                    continue
+def fix_isort(content: str, *, line_length: int = 100) -> str:
+    """Format source code with isort
 
-            if redundant_or_values and isinstance(node.op, ast.Or):
-                values = [value for value in node.values if value not in redundant_or_values]
-                if len(values) == 1:
-                    yield node, values[0]
-                    continue
-                if values != node.values:
-                    yield node, ast.BoolOp(op=node.op, values=values)
-                    continue
+    Args:
+        content (str): Python source code
+        line_length (int, optional): Line length. Defaults to 100.
 
-        if isinstance(node.op, ast.And):
-            # One of node.values is always False => Expression is always False
-            if any(isinstance(value, ast.Constant) and not value.value for value in node.values):
-                yield node, ast.Constant(value=False, kind=None)
-                continue
+    Returns:
+        str: Source code, formatted with isort
+    """
+    return isort.code(content, config=isort.Config(profile="black", line_length=line_length))
 
-            # Remove all True values
-            values = [
-                value
-                for value in node.values
-                if not parsing.match_template(value, ast.Constant(value=True))
-            ]
-            if not values:
-                yield node, ast.Constant(value=True, kind=None)
-                continue
 
-            if len({parsing.unparse(value) for value in values}) == 1:
-                yield node, values[0]
-                continue
+def align_variable_names_with_convention(
+    content: str, preserve: Collection[str] = frozenset()
+) -> str:
+    """Align variable names with normal convention
 
-            if len(values) < len(node.values):
-                yield node, ast.BoolOp(op=ast.And(), values=values)
-                continue
+    Class names should have CamelCase names
+    Non-static variables and functions should have snake_case names
+    Static variables should have UPPERCASE_UNDERSCORED names
 
-        elif isinstance(node.op, ast.Or):
-            # One of node.values is always True => Expression is always True
-            if any(isinstance(value, ast.Constant) and value.value for value in node.values):
-                yield node, ast.Constant(value=True, kind=None)
-                continue
+    All names defined in global scope may be private and start with a single underscore
+    Names outside global scope are never allowed to be private
+    __magic__ names may only be defined in global scope
 
-            # Remove all False values
-            values = [
-                value
-                for value in node.values
-                if not parsing.match_template(value, ast.Constant(value=False))
-            ]
-            if not values:
-                yield node, ast.Constant(value=False, kind=None)
-                continue
+    Args:
+        content (str): Python source code
 
-            if len({parsing.unparse(value) for value in values}) == 1:
-                yield node, values[0]
-                continue
+    Returns:
+        str: Source code, where all variable names comply with normal convention
+    """
+    ast_tree = ast.parse(content)
+    renamings = _get_variable_name_substitutions(ast_tree, content)
 
-            if len(values) < len(node.values):
-                yield node, ast.BoolOp(op=ast.Or(), values=values)
-                continue
+    if renamings:
+        content = _fix_variable_names(content, renamings, preserve)
 
-    for node in parsing.walk(root, ast.UnaryOp):
-        if isinstance(node.op, ast.Not) and isinstance(node.operand, ast.Constant):
-            yield node, ast.Constant(value=not node.operand.value, kind=None)
-
-    for node in parsing.walk(root, regular_compare_template):
-        operator = node.ops[0]
-        comparator = node.comparators[0]
-        try:
-            left = parsing.literal_value(node.left)
-            right = parsing.literal_value(comparator)
-        except ValueError:
-            if isinstance(operator, ast.Eq) and parsing.unparse(node.left) == parsing.unparse(
-                comparator
+    return content
+
+
+def _iter_bodies_recursive(
+    ast_root: ast.Module,
+) -> Iterable[Union[ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef]]:
+    left = list(ast_root.body)
+    while left:
+        for node in left.copy():
+            left.remove(node)
+            if isinstance(
+                node,
+                (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef, ast.For, ast.While, ast.With),
             ):
-                yield node, ast.Constant(value=True, kind=None)
+                left.extend(node.body)
+                yield node
+            if isinstance(node, ast.If):
+                left.extend(node.body)
+                left.extend(node.orelse)
+                yield node
+
+
+def _unique_assignment_targets(
+    node: Union[ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For]
+) -> Collection[ast.Name]:
+    targets = set()
+    if isinstance(node, (ast.AugAssign, ast.AnnAssign, ast.For)):
+        for subtarget in ast.walk(node.target):
+            if isinstance(subtarget, ast.Name) and isinstance(subtarget.ctx, ast.Store):
+                targets.add(subtarget)
+        return targets
+    if isinstance(node, ast.Assign):
+        for target in node.targets:
+            for subtarget in ast.walk(target):
+                if isinstance(subtarget, ast.Name) and isinstance(subtarget.ctx, ast.Store):
+                    targets.add(subtarget)
+        return targets
+    raise TypeError(f"Expected Assignment type, got {type(node)}")
 
-            continue
 
-        if isinstance(operator, ast.Eq):
-            yield node, ast.Constant(value=left == right, kind=None)
+def undefine_unused_variables(content: str, preserve: Collection[str] = frozenset()) -> str:
+    """Remove definitions of unused variables
 
-        elif isinstance(operator, ast.NotEq):
-            yield node, ast.Constant(value=left != right, kind=None)
+    Args:
+        content (str): Python source code
+        preserve (Collection[str], optional): Variable names to preserve
 
-        elif isinstance(operator, ast.Gt):
-            yield node, ast.Constant(value=left > right, kind=None)
+    Returns:
+        str: Python source code, with no definitions of unused variables
+    """
+    ast_tree = ast.parse(content)
+    renamings = collections.defaultdict(set)
+    imports = set()
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            imports.update(alias.name for alias in node.names)
+
+    for def_node in itertools.chain(
+        [ast_tree],
+        parsing.iter_funcdefs(ast_tree),
+    ):
+        reference_nodes = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load)
+        }
+        body = queue.PriorityQueue()
+        for node in def_node.body:
+            body.put((node.lineno, node, None))
+        while not body.empty():
+            _, node, containing_loop_node = body.get()
+            if isinstance(node, (ast.For, ast.While)):
+                for subnode in reversed(node.body):
+                    body.put((subnode.lineno, subnode, containing_loop_node or node))
+            elif isinstance(node, ast.If):
+                for subnode in node.body:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
+                for subnode in node.orelse:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
+            if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For)):
+                target_nodes = _unique_assignment_targets(node)
+                if not target_nodes:
+                    continue
+                target_names = {x.id for x in target_nodes}
+                referenced_names = set()
+                starts = []
+                ends = []
+                if containing_loop_node is not None:
+                    loop_start, loop_end = parsing.get_charnos(containing_loop_node, content)
+                else:
+                    loop_start = loop_end = -1
+                for target_node in target_nodes:
+                    s, e = parsing.get_charnos(target_node, content)
+                    starts.append(s)
+                    ends.append(e)
+                start = min(starts)
+                end = max(ends)
+                for refnode in reference_nodes:
+                    n_start, n_end = parsing.get_charnos(refnode, content)
+                    if (
+                        end < n_start
+                        or (isinstance(def_node, (ast.ClassDef, ast.Module)) and n_end < start)
+                        or isinstance(def_node, ast.For)
+                        or loop_start <= n_start <= n_end <= loop_end
+                    ):
+                        referenced_names.add(refnode.id)
+                redundant_targets = target_names - referenced_names - imports
+                if def_node is ast_tree:
+                    redundant_targets = redundant_targets - preserve
+                for target_node in target_nodes:
+                    if isinstance(target_node, ast.Attribute):
+                        target_node = target_node.value
+                    if target_node.id in redundant_targets:
+                        renamings[target_node].add("_")
+
+    if renamings:
+        content = _fix_variable_names(content, renamings, preserve)
+        ast_tree = ast.parse(content)
+
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign)):
+            target_nodes = _unique_assignment_targets(node)
+            target_names = {x.id for x in target_nodes}
+            if target_names == {"_"}:
+                code = parsing.get_code(node, content)
+                changed_code = re.sub(_REDUNDANT_UNDERSCORED_ASSIGN_RE_PATTERN, "", code)
+                if code != changed_code:
+                    print(f"Removing redundant assignments in {code}")
+                    content = content.replace(code, changed_code)
 
-        elif isinstance(operator, ast.Lt):
-            yield node, ast.Constant(value=left < right, kind=None)
+    return content
 
-        elif isinstance(operator, ast.GtE):
-            yield node, ast.Constant(value=left >= right, kind=None)
 
-        elif isinstance(operator, ast.LtE):
-            yield node, ast.Constant(value=left <= right, kind=None)
+def remove_nodes(content: str, nodes: Iterable[ast.AST], root: ast.Module) -> str:
+    """Remove ast nodes from code
 
+    Args:
+        content (str): Python source code
+        nodes (Iterable[ast.AST]): Nodes to delete from code
+        root (ast.Module): Complete corresponding module
 
-@processing.fix(restart_on_replace=True)
-def simplify_boolean_expressions_symmath(source: str) -> str:
-    root = parsing.parse(source)
-    for node in parsing.walk(root, (ast.BoolOp, ast.UnaryOp)):
-        try:
-            simplified = simplify_ast_boolop(node)
-        except ValueError:
+    Returns:
+        str: Code after deleting nodes
+    """
+    keep_mask = [True] * len(content)
+    nodes = list(nodes)
+    for node in nodes:
+        start, end = parsing.get_charnos(node, content)
+        print(f"Removing:\n{content[start:end]}")
+        keep_mask[start:end] = [False] * (end - start)
+        for decorator_node in getattr(node, "decorator_list", []):
+            start, end = parsing.get_charnos(decorator_node, content)
+            start -= 1  # The @ is missed otherwise
+            print(f"Removing:\n{content[start:end]}")
+            keep_mask[start:end] = [False] * (end - start)
+
+    passes = [len(content) + 1]
+
+    for node in ast.walk(root):
+        for bodytype in "body", "finalbody", "orelse":
+            if body := getattr(node, bodytype, []):
+                if isinstance(body, list) and all(child in nodes for child in body):
+                    print(f"Found empty {bodytype}")
+                    start_charno, _ = parsing.get_charnos(body[0], content)
+                    passes.append(start_charno)
+
+    heapq.heapify(passes)
+
+    next_pass = heapq.heappop(passes)
+    chars = []
+    for i, char, keep in zip(range(len(content)), content, keep_mask):
+        if i == next_pass:
+            chars.extend("pass")
+        elif next_pass < i < next_pass + 3:
             continue
+        else:
+            if i > next_pass:
+                next_pass = heapq.heappop(passes)
+            if keep:
+                chars.append(char)
 
-        node_complexity = sum(len(x.values) for x in parsing.walk(node, ast.BoolOp))
-        simplified_complexity = sum(len(x.values) for x in parsing.walk(simplified, ast.BoolOp))
-
-        if simplified_complexity < node_complexity:
-            yield node, simplified
+    return "".join(chars)
 
 
-@processing.fix
-def simplify_constrained_range(source: str) -> str:
-    root = parsing.parse(source)
+def _compute_safe_funcdef_calls(root: ast.Module) -> Collection[str]:
+    """Compute what functions can safely be called without having a side effect.
 
-    # i.e.:
-    # (x for x in range(10) if x > 5) => (x for x in range(6, 10))
-    # {y for y in range(18, 99) if y % 2 == 0} => {y for y in range(18, 99, 2)}
+    This is also to compute the inverse, i.e. what function calls may be removed
+    without breaking something.
 
-    comprehension_template = ast.comprehension(
-        iter=ast.Call(func=ast.Name(id="range"), keywords=[]), target=ast.Name(id=str)
-    )
-    template = (
-        ast.GeneratorExp(generators=[comprehension_template]),
-        ast.ListComp(generators=[comprehension_template]),
-        ast.SetComp(generators=[comprehension_template]),
-    )
-    for node in parsing.walk(root, template):
-        comp = node.generators[0]
-        if not comp.ifs:
-            continue
+    Args:
+        root (ast.Module): Module to find function definitions in
 
-        if len(comp.iter.args) == 1:
-            args = [ast.Constant(value=0), comp.iter.args[0], ast.Constant(value=1)]
-        elif len(comp.iter.args) == 2:
-            args = [comp.iter.args[0], comp.iter.args[1], ast.Constant(value=1)]
-        elif len(comp.iter.args) == 3:
-            args = comp.iter.args.copy()
-        else:
-            continue
+    Returns:
+        Collection[str]: Names of all functions that have no side effect when called.
+    """
+    defined_names = {
+        node.id
+        for node in ast.walk(root)
+        if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Store)
+    }
+    function_defs = {
+        node for node in ast.walk(root) if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef))
+    }
+    builtin_names = set(dir(builtins))
+    safe_callables = builtin_names - {"print", "exit"}
+    safe_callable_nodes = set()
+    changes = True
+    while changes:
+        changes = False
+        for node in function_defs:
+            if node.name in defined_names:
+                continue
+            nonreturn_children = [
+                child
+                for child in node.body
+                if not isinstance(
+                    child,
+                    (ast.Return, ast.Yield, ast.YieldFrom, ast.Continue, ast.Break),
+                )
+            ]
+            if not any(
+                parsing.has_side_effect(child, safe_callables) for child in nonreturn_children
+            ):
+                safe_callable_nodes.add(node)
+                safe_callables.add(node.name)
+                changes = True
+        function_defs = {node for node in function_defs if node.name not in safe_callables}
+
+    for node in ast.walk(root):
+        if isinstance(node, ast.ClassDef):
+            constructors = {
+                child
+                for child in node.body
+                if isinstance(child, ast.FunctionDef)
+                and child.name in ("__init__", "__post_init__", "__new__")
+            }
+            if not constructors - safe_callable_nodes:
+                safe_callables.add(node.name)
 
-        if parsing.match_template(args[0], ast.Constant(value=int)):
-            start = args[0].value
-        else:
-            start = None
+    return safe_callables
 
-        if parsing.match_template(args[1], ast.Constant(value=int)):
-            stop = args[1].value
-        else:
-            stop = None
 
-        if parsing.match_template(args[2], ast.Constant(value=int)):
-            step = args[2].value
-        else:
-            step = None
+def delete_pointless_statements(content: str) -> str:
+    """Delete pointless statements with no side effects from code
 
-        target_name = comp.target.id
+    Args:
+        content (str): Python source code.
 
-        conditions = set()
-        ifs = comp.ifs.copy()
-        while ifs:
-            condition = ifs.pop()
-            if parsing.match_template(condition, ast.BoolOp(op=ast.And())):
-                ifs.extend(condition.values)
-                continue
+    Returns:
+        str: Modified code
+    """
+    ast_tree = ast.parse(content)
+    delete = []
+    safe_callables = _compute_safe_funcdef_calls(ast_tree)
+    for node in itertools.chain([ast_tree], _iter_bodies_recursive(ast_tree)):
+        for i, child in enumerate(node.body):
+            if not parsing.has_side_effect(child, safe_callables):
+                if i > 0 or not (
+                    isinstance(child, ast.Expr)
+                    and isinstance(child.value, ast.Constant)
+                    and isinstance(child.value.value, str)
+                ):
+                    delete.append(child)
 
-            conditions.add(condition)
+    content = remove_nodes(content, delete, ast_tree)
 
-        gt_template = (
-            ast.Compare(
-                left=ast.Name(id=target_name), ops=[ast.Gt()], comparators=[ast.Constant()]
-            ),
-            ast.Compare(
-                left=ast.Constant(), ops=[ast.Lt()], comparators=[ast.Name(id=target_name)]
-        ),)
-        lt_template = (
-            ast.Compare(
-                left=ast.Name(id=target_name), ops=[ast.Lt()], comparators=[ast.Constant()]
-            ),
-            ast.Compare(
-                left=ast.Constant(), ops=[ast.Gt()], comparators=[ast.Name(id=target_name)]
-        ),)
-        gte_template = (
-            ast.Compare(
-                left=ast.Name(id=target_name), ops=[ast.GtE()], comparators=[ast.Constant()]
-            ),
-            ast.Compare(
-                left=ast.Constant(), ops=[ast.LtE()], comparators=[ast.Name(id=target_name)]
-        ),)
-        lte_template = (
-            ast.Compare(
-                left=ast.Name(id=target_name), ops=[ast.LtE()], comparators=[ast.Constant()]
-            ),
-            ast.Compare(
-                left=ast.Constant(), ops=[ast.GtE()], comparators=[ast.Name(id=target_name)]
-        ),)
-        eq_template = (
-            ast.Compare(
-                left=ast.Name(id=target_name), ops=[ast.Eq()], comparators=[ast.Constant()]
-            ),
-            ast.Compare(
-                left=ast.Constant(), ops=[ast.Eq()], comparators=[ast.Name(id=target_name)]
-        ),)
-        templates = (gt_template, lt_template, gte_template, lte_template, eq_template)
+    return content
 
-        if parsing.match_template(step, ast.Constant(value=int)) and step.value < 0:
-            continue
 
-        redundant_conditions = set()
-        for condition in parsing.filter_nodes(conditions, templates):
-            if isinstance(condition.left, ast.Constant):
-                comparator = condition.left
-            else:
-                comparator = condition.comparators[0]
+def _get_unused_functions_classes(root: ast.AST, preserve: Collection[str]) -> Iterable[ast.AST]:
+    funcdefs = []
+    classdefs = []
+    names = []
+
+    for node in ast.walk(root):
+        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+            funcdefs.append(node)
+        elif isinstance(node, ast.ClassDef):
+            classdefs.append(node)
+        elif isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load):
+            names.append(node)
+
+    class_magics = collections.defaultdict(set)
+    for node in classdefs:
+        for child in node.body:
+            if (
+                isinstance(child, ast.FunctionDef)
+                and child.name.startswith("__")
+                and child.name.endswith("__")
+            ):
+                class_magics[node].add(child)
 
-            if parsing.match_template(condition, gt_template):
-                if start is None or comparator.value > start:
-                    start = comparator.value + 1
-                    redundant_conditions.add(condition)
-
-            elif parsing.match_template(condition, lt_template):
-                if stop is None or comparator.value <= stop:
-                    stop = comparator.value
-                    redundant_conditions.add(condition)
-
-            elif parsing.match_template(condition, gte_template):
-                if start is None or comparator.value >= start:
-                    start = comparator.value
-                    redundant_conditions.add(condition)
-
-            elif parsing.match_template(condition, lte_template):
-                if stop is None or comparator.value <= stop:
-                    stop = comparator.value + 1
-                    redundant_conditions.add(condition)
-
-            elif parsing.match_template(condition, eq_template):
-                changes = False
-                if start is None or comparator.value >= start:
-                    start = comparator.value
-                    changes = True
-                elif comparator.value < start:  # Infeasible
-                    start = stop = 0
-
-                if stop is None or comparator.value < stop:
-                    stop = comparator.value + 1
-                    changes = True
-                elif comparator.value >= stop:  # Infeasible
-                    start = stop = 0
-
-                if changes:
-                    redundant_conditions.add(condition)
-
-        if stop is not None and start >= stop:
-            new_comp = ast.comprehension(
-                target=comp.target, iter=ast.Tuple(elts=[]), ifs=[], is_async=comp.is_async
-            )
-            yield node, type(node)(generators=[new_comp], elt=node.elt)
+    magic_source_classes = {}
+    for classdef, magics in class_magics.items():
+        for magic in magics:
+            magic_source_classes[magic] = classdef
 
-        if not redundant_conditions:
+    for def_node in funcdefs:
+        if def_node.name in preserve:
             continue
+        usages = {node for node in names if node.id == def_node.name}
+        if parent_class := magic_source_classes.get(def_node):
+            usages.update(node for node in names if node.id == parent_class.name)
+        recursive_usages = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name) and node.id == def_node.name
+        }
+        if not usages - recursive_usages:
+            print(f"{def_node.name} is never used")
+            yield def_node
 
-        if start == 0:
-            start = None
-
-        if step == 1:
-            step = None
+    for def_node in classdefs:
+        if def_node.name in preserve:
+            continue
+        usages = {node for node in names if node.id == def_node.name}
+        internal_usages = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name)
+            and isinstance(node.ctx, ast.Load)
+            and node.id in (def_node.name, "self", "cls")
+        }
+        if not usages - internal_usages:
+            print(f"{def_node.name} is never used")
+            yield def_node
+
+
+def delete_unused_functions_and_classes(
+    content: str, preserve: Collection[str] = frozenset()
+) -> str:
+    """Delete unused functions and classes from code.
 
-        for condition in redundant_conditions:
-            yield condition, ast.Constant(value=True, kind=None)
+    Args:
+        content (str): Python source code
+        preserve (Collection[str], optional): Names to preserve
 
-        if start is not None and step is not None:
-            yield comp.iter, ast.Call(
-                func=ast.Name(id="range"),
-                args=[
-                    ast.Constant(value=start, kind=None),
-                    ast.Constant(value=stop, kind=None),
-                    ast.Constant(value=step, kind=None),
-                ],
-                keywords=[],
-            )
+    Returns:
+        str: Python source code, where unused functions and classes have been deleted.
+    """
+    root = ast.parse(content)
 
-        elif start is not None:
-            yield comp.iter, ast.Call(
-                func=ast.Name(id="range"),
-                args=[ast.Constant(value=start, kind=None), ast.Constant(value=stop, kind=None)],
-                keywords=[],
-            )
+    delete = set(_get_unused_functions_classes(root, preserve))
 
-        else:
-            yield comp.iter, ast.Call(
-                func=ast.Name(id="range"), args=[ast.Constant(value=stop, kind=None)], keywords=[]
-            )
+    content = remove_nodes(content, delete, root)
 
-        return
+    return content
```

