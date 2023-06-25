# Comparing `tmp/evogfuzz-0.0.2.tar.gz` & `tmp/evogfuzz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evogfuzz-0.0.2.tar", last modified: Mon Jan  9 13:44:54 2023, max compression
+gzip compressed data, was "evogfuzz-0.6.0.tar", last modified: Sun Jun 25 17:10:12 2023, max compression
```

## Comparing `evogfuzz-0.0.2.tar` & `evogfuzz-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,40 @@
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.472977 evogfuzz-0.0.2/
--rw-r--r--   0 martineberlein   (501) staff       (20)       81 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/MANIFEST.in
--rw-r--r--   0 martineberlein   (501) staff       (20)     2352 2023-01-09 13:44:54.473033 evogfuzz-0.0.2/PKG-INFO
--rw-r--r--   0 martineberlein   (501) staff       (20)     1987 2023-01-09 12:31:09.000000 evogfuzz-0.0.2/README.md
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.469813 evogfuzz-0.0.2/notebooks/
--rw-r--r--   0 martineberlein   (501) staff       (20)   266655 2023-01-09 13:10:34.000000 evogfuzz-0.0.2/notebooks/demo.ipynb
--rw-r--r--   0 martineberlein   (501) staff       (20)      671 2023-01-09 13:44:54.473307 evogfuzz-0.0.2/setup.cfg
--rw-r--r--   0 martineberlein   (501) staff       (20)       37 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/setup.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.469158 evogfuzz-0.0.2/src/
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.471737 evogfuzz-0.0.2/src/evogfuzz/
--rw-r--r--   0 martineberlein   (501) staff       (20)       30 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/src/evogfuzz/__init__.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      107 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/src/evogfuzz/cli.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     7182 2023-01-09 13:05:03.000000 evogfuzz-0.0.2/src/evogfuzz/evogfuzz_class.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      467 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/src/evogfuzz/fitness_functions.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      776 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/src/evogfuzz/tournament_selection.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.472556 evogfuzz-0.0.2/src/evogfuzz.egg-info/
--rw-r--r--   0 martineberlein   (501) staff       (20)     2352 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/PKG-INFO
--rw-r--r--   0 martineberlein   (501) staff       (20)      468 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/SOURCES.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)        1 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/dependency_links.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)       47 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/entry_points.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)       44 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/requires.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)        9 2023-01-09 13:44:54.000000 evogfuzz-0.0.2/src/evogfuzz.egg-info/top_level.txt
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-01-09 13:44:54.472820 evogfuzz-0.0.2/tests/
--rw-r--r--   0 martineberlein   (501) staff       (20)      966 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/tests/test_data.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      622 2023-01-09 11:48:35.000000 evogfuzz-0.0.2/tests/test_evogfuzz.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.287570 evogfuzz-0.6.0/
+-rw-r--r--   0 martineberlein   (501) staff       (20)       28 2023-06-25 17:06:39.000000 evogfuzz-0.6.0/MANIFEST.in
+-rw-r--r--   0 martineberlein   (501) staff       (20)     6110 2023-06-25 17:10:12.287688 evogfuzz-0.6.0/PKG-INFO
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5429 2023-06-15 14:56:27.000000 evogfuzz-0.6.0/README.md
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.277860 evogfuzz-0.6.0/notebooks/
+-rw-r--r--   0 martineberlein   (501) staff       (20)    22700 2023-06-15 15:05:11.000000 evogfuzz-0.6.0/notebooks/evogfuzz_demo.ipynb
+-rw-r--r--   0 martineberlein   (501) staff       (20)      960 2023-06-25 17:10:12.288710 evogfuzz-0.6.0/setup.cfg
+-rw-r--r--   0 martineberlein   (501) staff       (20)       37 2023-02-06 12:44:13.000000 evogfuzz-0.6.0/setup.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.276688 evogfuzz-0.6.0/src/
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.281286 evogfuzz-0.6.0/src/evogfuzz/
+-rw-r--r--   0 martineberlein   (501) staff       (20)       75 2023-02-07 09:35:20.000000 evogfuzz-0.6.0/src/evogfuzz/__init__.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      107 2023-05-23 16:31:53.000000 evogfuzz-0.6.0/src/evogfuzz/cli.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)    12951 2023-06-15 13:43:44.000000 evogfuzz-0.6.0/src/evogfuzz/evogfuzz_class.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      304 2023-05-23 07:18:34.000000 evogfuzz-0.6.0/src/evogfuzz/fitness_functions.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1702 2023-05-25 12:43:27.000000 evogfuzz-0.6.0/src/evogfuzz/grammar_transformation.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2109 2023-05-23 07:17:18.000000 evogfuzz-0.6.0/src/evogfuzz/helper.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2212 2023-05-25 12:51:41.000000 evogfuzz-0.6.0/src/evogfuzz/input.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      158 2023-02-10 19:03:43.000000 evogfuzz-0.6.0/src/evogfuzz/oracle.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1194 2023-05-23 07:18:16.000000 evogfuzz-0.6.0/src/evogfuzz/tournament_selection.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)       60 2023-02-07 12:05:17.000000 evogfuzz-0.6.0/src/evogfuzz/type_defs.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      273 2023-05-23 07:17:18.000000 evogfuzz-0.6.0/src/evogfuzz/types.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2234 2023-05-23 07:17:18.000000 evogfuzz-0.6.0/src/evogfuzz/visualization.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.284859 evogfuzz-0.6.0/src/evogfuzz.egg-info/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     6110 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/PKG-INFO
+-rw-r--r--   0 martineberlein   (501) staff       (20)      894 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)        1 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)       47 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/entry_points.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)       64 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/requires.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)       33 2023-06-25 17:10:12.000000 evogfuzz-0.6.0/src/evogfuzz.egg-info/top_level.txt
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.285328 evogfuzz-0.6.0/src/evogfuzz_formalizations/
+-rw-r--r--   0 martineberlein   (501) staff       (20)        0 2023-02-06 12:44:13.000000 evogfuzz-0.6.0/src/evogfuzz_formalizations/__init__.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1630 2023-02-28 17:24:01.000000 evogfuzz-0.6.0/src/evogfuzz_formalizations/calculator.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-25 17:10:12.287176 evogfuzz-0.6.0/tests/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1192 2023-05-23 16:27:28.000000 evogfuzz-0.6.0/tests/test_evogfuzz.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     4704 2023-05-25 12:45:37.000000 evogfuzz-0.6.0/tests/test_evoggen.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2809 2023-05-23 07:18:37.000000 evogfuzz-0.6.0/tests/test_probabilistic_learning.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1247 2023-05-23 07:17:57.000000 evogfuzz-0.6.0/tests/test_selection.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2348 2023-05-23 07:17:18.000000 evogfuzz-0.6.0/tests/test_test_inputs.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1636 2023-05-25 12:44:50.000000 evogfuzz-0.6.0/tests/test_transform_grammar.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2134 2023-05-23 07:17:18.000000 evogfuzz-0.6.0/tests/test_visualization.py
```

### Comparing `evogfuzz-0.0.2/tests/test_data.py` & `evogfuzz-0.6.0/src/evogfuzz_formalizations/calculator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,59 @@
-import string
 import math
+import logging
+
 from fuzzingbook.Grammars import Grammar
-from fuzzingbook.Parser import DerivationTree
 
-from typing import Tuple, Set
+from evogfuzz.oracle import OracleResult
+from evogfuzz.input import Input
+
+
+def arith_eval(inp: Input) -> float:
+    return eval(
+        str(inp), {"sqrt": math.sqrt, "sin": math.sin, "cos": math.cos, "tan": math.tan}
+    )
+
+
+def prop_(inp: Input) -> bool:
+    try:
+        arith_eval(inp)
+        return False
+    except ValueError:
+        return True
+
+
+def prop(inp: Input) -> OracleResult:
+    try:
+        return OracleResult.BUG if prop_(inp) else OracleResult.NO_BUG
+    except SyntaxError:
+        logging.info(
+            f"Input {str(inp)} is not a valid input of the program. You might want to rewrite your grammar!"
+        )
+        return OracleResult.UNDEF
+
+
+grammar: Grammar = {
+    "<start>": ["<function>(<term>)"],
+    "<function>": ["sqrt", "tan", "cos", "sin"],
+    "<term>": ["-<value>", "<value>"],
+    "<value>": ["<integer>.<integer>", "<integer>"],
+    "<integer>": ["<digit><integer>", "<digit>"],
+    "<digit>": ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
+}
 
 
-GRAMMAR: Grammar = {
+grammar_alhazen: Grammar = {
     "<start>": ["<arith_expr>"],
     "<arith_expr>": ["<function>(<number>)"],
     "<function>": ["sqrt", "sin", "cos", "tan"],
     "<number>": ["<maybe_minus><onenine><maybe_digits><maybe_frac>"],
     "<maybe_minus>": ["", "-"],
     "<onenine>": [str(num) for num in range(1, 10)],
-    "<digit>": list(string.digits),
+    "<digit>": [str(num) for num in range(0, 10)],
     "<maybe_digits>": ["", "<digits>"],
     "<digits>": ["<digit>", "<digit><digits>"],
-    "<maybe_frac>": ["", ".<digits>"]
+    "<maybe_frac>": ["", ".<digits>"],
 }
 
-INITIAL_INPUTS = ['cos(10)', 'sqrt(28367)', 'tan(-12)', 'sqrt(3)']
-
-
-def arith_eval(inp: DerivationTree) -> float:
-    return eval(str(inp), {"sqrt": math.sqrt, "sin": math.sin, "cos": math.cos, "tan": math.tan})
+START_SYMBOL = "<start>"
 
-
-def prop(inp: DerivationTree) -> bool:
-    try:
-        arith_eval(inp)
-        return False
-    except ValueError:
-        return True
+initial_inputs = ["cos(12)", "sqrt(-900)"]
```

