# Comparing `tmp/sbmlmath-0.0.1.tar.gz` & `tmp/sbmlmath-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlmath-0.0.1.tar", last modified: Tue Jun 20 06:19:09 2023, max compression
+gzip compressed data, was "sbmlmath-0.0.2.tar", last modified: Sun Jun 25 05:08:51 2023, max compression
```

## Comparing `sbmlmath-0.0.1.tar` & `sbmlmath-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.github/workflows/deploy_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/sbmlmath/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/cfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/csymbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/mathml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/mathml_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/species_symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/sbmlmath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_csymbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_mathml_parser_sbml_semantic_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.460614 sbmlmath-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.460614 sbmlmath-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.github/workflows/deploy_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/sbmlmath/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/cfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/mathml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/mathml_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/sbmlmath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_mathml_parser_sbml_semantic_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_species_symbol.py
```

### Comparing `sbmlmath-0.0.1/.github/workflows/ci.yaml` & `sbmlmath-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/.github/workflows/deploy_release.yaml` & `sbmlmath-0.0.2/.github/workflows/deploy_release.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/.pre-commit-config.yaml` & `sbmlmath-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/LICENSE` & `sbmlmath-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/PKG-INFO` & `sbmlmath-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.1
+Version: 0.0.2
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sbmlmath-0.0.1/README.md` & `sbmlmath-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/pyproject.toml` & `sbmlmath-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sbmlmath"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Daniel Weindl", email = "sci@danielweindl.de"},
 ]
 description = "SBML Math <-> SymPy"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "BSD-3-Clause"}
```

### Comparing `sbmlmath-0.0.1/sbmlmath/__init__.py` & `sbmlmath-0.0.2/sbmlmath/__init__.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/sbmlmath/cfunction.py` & `sbmlmath-0.0.2/sbmlmath/cfunction.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/sbmlmath/csymbol.py` & `sbmlmath-0.0.2/sbmlmath/csymbol.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/sbmlmath/mathml_parser.py` & `sbmlmath-0.0.2/sbmlmath/mathml_parser.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/sbmlmath/mathml_printer.py` & `sbmlmath-0.0.2/sbmlmath/mathml_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,20 @@
         multi_ns = f" {self.multi_ns}" if " multi:" in mathml else ""
         return (
             f"{prolog}<math {self.mathml_ns}{sbml_ns}{multi_ns}>\n"
             f"{mathml}</math>"
         )
 
     def _print_Number(self, e):
-        res = self._print_int(e)
+        # only try printing as int if it fits int32
+        if isinstance(e, int) and e < 2**31 and e >= -(2**31):
+            res = self._print_int(e)
+        else:
+            res = super()._print_Number(e)
+
         if self.literals_dimensionless:
             res.setAttribute("sbml:units", "dimensionless")
         return res
 
     def _print_Rational(self, e):
         if e.q == 1:
             # don't divide by one
@@ -95,14 +100,17 @@
         res.appendChild(self.dom.createTextNode(f"{e.p} <sep/> {e.q}"))
 
         if self.literals_dimensionless:
             res.setAttribute("sbml:units", "dimensionless")
         return res
 
     def _print_int(self, e):
+        if e >= 2**31 or e < -(2**31):
+            # avoid int32 under/overflow in libsbml and print as float
+            return self._print_Number(e)
         res = super()._print_int(e)
         res.setAttribute("type", "integer")
         if self.literals_dimensionless:
             res.setAttribute("sbml:units", "dimensionless")
         return res
 
     def _print_Float(self, e):
```

### Comparing `sbmlmath-0.0.1/sbmlmath/species_symbol.py` & `sbmlmath-0.0.2/sbmlmath/species_symbol.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/sbmlmath.egg-info/PKG-INFO` & `sbmlmath-0.0.2/sbmlmath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.1
+Version: 0.0.2
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sbmlmath-0.0.1/sbmlmath.egg-info/SOURCES.txt` & `sbmlmath-0.0.2/sbmlmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/tests/test_mathml_parser_sbml_semantic_suite.py` & `sbmlmath-0.0.2/tests/test_mathml_parser_sbml_semantic_suite.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/tests/test_misc.py` & `sbmlmath-0.0.2/tests/test_misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -125,20 +125,63 @@
     """
     sym = SBMLMathMLParser().parse_str(mathml)
     assert isinstance(sym, sp.Function)
     assert sym.definition_url == "http://www.sbml.org/sbml/symbols/delay"
     assert sym.name == "delay"
     assert sym == delay(sp.Symbol("Q"), sp.Integer(1))
 
+
 def test_print_cfunction():
     expected = (
         """<?xml version="1.0" encoding="UTF-8"?>\n<math xmlns="http://www.w3.org/1998/Math/MathML" """
         'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core">\n'
         '<apply><csymbol definitionURL="http://www.sbml.org/sbml/symbols/delay" encoding="text">delay</csymbol>'
         '<ci>Q</ci><cn type="integer" sbml:units="dimensionless">1</cn></apply></math>'
     )
     sym = delay(sp.Symbol("Q"), sp.Integer(1))
     printed_mathml = SBMLMathMLPrinter().doprint(sym)
     assert printed_mathml == expected
 
 
+def test_integer_overflow():
+    """Check whether libsbml still restricts us to 32bit signed integers"""
+
+    def get_mathml(i):
+        return f"""<?xml version="1.0" encoding="UTF-8"?>
+        <math xmlns="http://www.w3.org/1998/Math/MathML" xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core">
+        <cn type="integer">{i}</cn>
+        </math>"""
+
+    i = 2**31 - 1
+    assert (ast_node := libsbml.readMathMLFromString(get_mathml(i))) is not None
+    assert str(i) in libsbml.writeMathMLToString(ast_node)
 
+    # FIXME: change to assert not None, if that restriction is ever lifted
+    i = 2**31
+    assert libsbml.readMathMLFromString(get_mathml(i)) is None
+
+    assert (
+        libsbml.readMathMLFromString(
+            SBMLMathMLPrinter().doprint(sp.Integer(2**31 - 1))
+        )
+        is not None
+    )
+    assert (
+        libsbml.readMathMLFromString(
+            SBMLMathMLPrinter().doprint(sp.Integer(-(2**31)))
+        )
+        is not None
+    )
+
+    # would fail as int32, ensure they are printed in a compatible way
+    assert (
+        libsbml.readMathMLFromString(
+            SBMLMathMLPrinter().doprint(sp.Integer(2**31))
+        )
+        is not None
+    )
+    assert (
+        libsbml.readMathMLFromString(
+            SBMLMathMLPrinter().doprint(sp.Integer(-(2**31) - 1))
+        )
+        is not None
+    )
```

### Comparing `sbmlmath-0.0.1/tests/test_parser.py` & `sbmlmath-0.0.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/tests/test_printer.py` & `sbmlmath-0.0.2/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.1/tests/test_species_symbol.py` & `sbmlmath-0.0.2/tests/test_species_symbol.py`

 * *Files identical despite different names*

