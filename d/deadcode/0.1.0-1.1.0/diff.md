# Comparing `tmp/deadcode-0.1.0.tar.gz` & `tmp/deadcode-1.1.0.tar.gz`

## Comparing `deadcode-0.1.0.tar` & `deadcode-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/cli.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/data_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/find_python_filenames.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/find_unused_names.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/get_unused_names_error_message.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_abstract_syntax_trees.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_arguments.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_global_names.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/read_files.py
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/classes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/functions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/variables.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/flatten_lists.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/path_matching.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-0.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-0.1.0/LICENSE
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 deadcode-0.1.0/README.md
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 deadcode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/__init__.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/cli.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_abstract_syntax_trees.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_global_names.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/read_files.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/base.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_command_line_argument_parsing.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_count_output.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_ignore_names_by_pattern.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/path_matching.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 deadcode-1.1.0/README.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 deadcode-1.1.0/PKG-INFO
```

### Comparing `deadcode-0.1.0/deadcode/cli.py` & `deadcode-1.1.0/deadcode/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 ) -> Optional[str]:
     args = parse_arguments(command_line_args)
 
     python_filenames = find_python_filenames(args=args)
     files = read_files(python_filenames)
 
     global_names = parse_global_names(files, args=args)
-    abstract_syntax_trees_of_files = parse_abstract_syntax_trees(files)
+    abstract_syntax_trees_of_files = parse_abstract_syntax_trees(files, args=args)
     unused_names = find_unused_names(abstract_syntax_trees_of_files, global_names, args=args)
 
     if error_message := get_unused_names_error_message(unused_names, args=args):
         return error_message
 
-    print("\033[1mWell done!\033[0m ✨ 🚀 ✨")
+    if not args.count and not args.quite:
+        print("\033[1mWell done!\033[0m ✨ 🚀 ✨")
     return None
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `deadcode-0.1.0/deadcode/actions/find_python_filenames.py` & `deadcode-1.1.0/deadcode/actions/find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-0.1.0/deadcode/actions/get_unused_names_error_message.py` & `deadcode-1.1.0/deadcode/actions/get_unused_names_error_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from deadcode.data_types import Args
 
 
 def get_unused_names_error_message(unused_names: Dict[VariableName, Filename], args: Args) -> Optional[str]:
     if not unused_names:
         return None
 
+    if args.quite:
+        return ""
+
+    if args.count:
+        return f"{len(unused_names)}"
+
     if args.no_color:
         return "\n".join([f"{filename} DC100 Global {name} is never used" for name, filename in unused_names.items()])
 
     return "\n".join(
         [
             f"{filename} \033[91mDC100\033[0m Global \033[1m{name}\033[0m is never used"
             for name, filename in unused_names.items()
```

### Comparing `deadcode-0.1.0/deadcode/actions/parse_abstract_syntax_trees.py` & `deadcode-1.1.0/deadcode/actions/parse_abstract_syntax_trees.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import ast
 from typing import Dict
 
-from deadcode.data_types import FileContent, Filename, AbstractSyntaxTree
+from deadcode.data_types import Args, FileContent, Filename, AbstractSyntaxTree
 
 
-def parse_abstract_syntax_trees(files: Dict[Filename, FileContent]) -> Dict[Filename, AbstractSyntaxTree]:
+def parse_abstract_syntax_trees(files: Dict[Filename, FileContent], args: Args) -> Dict[Filename, AbstractSyntaxTree]:
     """Did my code coverage just increased? Answer is no: a doc string was ignored :tada:"""
     abstract_syntax_trees_for_files = {}
     for filename, file_content in files.items():
         try:
             abstract_syntax_trees_for_files[filename] = ast.dump(ast.parse(file_content))  # Note: indent=1 for debug
         except:  # noqa: E722
-            print(f"Error: Failed to parse {filename} file, ignoring it.")
+            if not args.count and not args.quite:
+                print(f"Error: Failed to parse {filename} file, ignoring it.")
             abstract_syntax_trees_for_files[filename] = ""
     return abstract_syntax_trees_for_files
```

### Comparing `deadcode-0.1.0/deadcode/actions/parse_arguments.py` & `deadcode-1.1.0/deadcode/actions/parse_arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,26 @@
     )
     parser.add_argument(
         "--no-color",
         help="Turn off colors in the output",
         action="store_true",
         default=False,
     )
+    parser.add_argument(
+        "--quite",
+        help="Does not output anything. Makefile still fails with exit code 1 if unused names are found.",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
+        "--count",
+        help="Provides the count of the detected unused names instead of printing them all out.",
+        action="store_true",
+        default=False,
+    )
 
     parsed_args = parser.parse_args(args).__dict__
 
     for field_name in ["exclude", "ignore_names", "ignore_names_in_files"]:
         parsed_args[field_name] = flatten_lists_of_comma_separated_values(parsed_args.get(field_name))
 
     # Extend the Args with the values provided in the pyproject.toml
```

### Comparing `deadcode-0.1.0/deadcode/actions/parse_global_names.py` & `deadcode-1.1.0/deadcode/actions/parse_global_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-0.1.0/deadcode/utils/flatten_lists.py` & `deadcode-1.1.0/deadcode/utils/flatten_lists.py`

 * *Files identical despite different names*

### Comparing `deadcode-0.1.0/.gitignore` & `deadcode-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-0.1.0/LICENSE` & `deadcode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadcode-0.1.0/README.md` & `deadcode-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,64 @@
 # deadcode
 `deadcode` package implements `DC100` - `unused-global-name` check for detecting
 variable/function/class names which are never used in a whole code base.
 Only globally defined names are being checked.
-Unused local names can be detected by other tools like `ruff`.
+Unused local names can be detected by other tools like [ruff](https://pypi.org/project/ruff/).
 
 ## Installation
 ```shell
 pip install deadcode
 ```
 
 ## Usage
 ```shell
 deadcode .
 ```
 
 Or with command line options:
 ```
-deadcode . --exclude=venv,tests --ignore-names=BaseTestCase --ignore-names-in-files=migrations
+deadcode . --exclude=venv,tests --ignore-names=BaseTestCase,.*Mixin --ignore-names-in-files=migrations
 ```
 
 The same options can be provided in `pyproject.toml` settings file:
 ```
 [tool.deadcode]
 exclude = ["venv", "tests"]
 ignore-names = ["BaseTestCase"]
 ignore-names-in-files = ["migrations"]
 ```
 
 Command line options:
-| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Type  | Meaning  |
-|---------------------------|-------|----------|
-|`--exclude`                | list | Path expressions to completely skips files from being analysed. |
-|`--ignore-names`           | list | Removes provided list of names from the error output. |
-|`--ignore-names-in-files`  | list | Unused names from files matching provided path expressions. |
-|`--no-color`               | None | Removes colors from the output. |
+
+| Option                            | Type | Meaning  |
+|-----------------------------------|------|----------|
+|<pre>--exclude</pre>               | list | Path expressions to completely skip files from being analysed. |
+|<pre>--ignore-names</pre>          | list | Removes provided list of names from the error output. Regexp expressions to match multiple names can also be provided, e.g. `.*Mixin` will match all classes ending with `Mixin`. |
+|<pre>--ignore-names-in-files</pre> | list | Unused names from files matching provided path expressions. |
+|<pre>--no-color</pre>              | None | Removes colors from the output. |
+|<pre>--count</pre>                 | None | Provides the count of the detected unused names instead of printing them all out. |
+|<pre>--quite</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
+
 
 ## Contributing
 - `make check` - runs unit tests and other checks using virtual environment.
 
 ## Rationale
-`ruff` and `flake8` - don't have rules for unused global code detection, only for local ones `F823`, `F841`, `F842`.
-`deadcode` package tries to add a new `DC100` check for detecting variables/functions/classes which are not used in a whole code base.
-
-There is an alternative `vulture` package, which provides many false positives. `deadcode` - tries to find less, but findings are with higher confidence.
+[ruff](https://pypi.org/project/ruff/) and
+[flake8](https://pypi.org/project/flake8/) - don't have rules for unused global
+code detection, only for local ones `F823`, `F841`, `F842`. `deadcode` package
+tries to add a new `DC100` check for detecting variables/functions/classes
+which are not used in a whole code base.
+
+There is an alternative [vulture](https://pypi.org/project/vulture/) package,
+which provides many false positives.
+`deadcode` - tries to find less, but findings are with higher confidence.
 `deadcode` - is supposed to be used inline with other static code checkers like `ruff`.
 
 ## Known limitations
 If the same unused name is repeated in several files - it wont be detected.
 
-Files with syntax errors will be ignored, because `deadcode` uses `ast` to build abstract syntax tree for name usage detection.
+Files with syntax errors will be ignored, because `deadcode` uses `ast` to
+build abstract syntax tree for name usage detection.
 
-It is assumed that `deadcode` will be run using the same Python version as the checked code base is implemented in.
+It is assumed that `deadcode` will be run using the same Python version as the
+checked code base is implemented in.
```

### Comparing `deadcode-0.1.0/pyproject.toml` & `deadcode-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "0.1.0"
+version = "1.1.0"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
@@ -65,8 +65,8 @@
 [tool.black]
 max_line_length = 120
 line_length = 120
 target_version = ["py38"]
 
 
 [tool.pytest.ini_options]
-addopts = "--cov=. --cov-fail-under=90.0"
+addopts = "--cov=. --cov-fail-under=92.0"
```

### Comparing `deadcode-0.1.0/PKG-INFO` & `deadcode-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadcode
-Version: 0.1.0
+Version: 1.1.0
 Summary: Find and remove dead code.
 Project-URL: Homepage, https://github.com/albertas/deadcode
 Project-URL: Documentation, https://deadcode.readthedocs.io/
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -18,56 +18,67 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # deadcode
 `deadcode` package implements `DC100` - `unused-global-name` check for detecting
 variable/function/class names which are never used in a whole code base.
 Only globally defined names are being checked.
-Unused local names can be detected by other tools like `ruff`.
+Unused local names can be detected by other tools like [ruff](https://pypi.org/project/ruff/).
 
 ## Installation
 ```shell
 pip install deadcode
 ```
 
 ## Usage
 ```shell
 deadcode .
 ```
 
 Or with command line options:
 ```
-deadcode . --exclude=venv,tests --ignore-names=BaseTestCase --ignore-names-in-files=migrations
+deadcode . --exclude=venv,tests --ignore-names=BaseTestCase,.*Mixin --ignore-names-in-files=migrations
 ```
 
 The same options can be provided in `pyproject.toml` settings file:
 ```
 [tool.deadcode]
 exclude = ["venv", "tests"]
 ignore-names = ["BaseTestCase"]
 ignore-names-in-files = ["migrations"]
 ```
 
 Command line options:
-| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Type  | Meaning  |
-|---------------------------|-------|----------|
-|`--exclude`                | list | Path expressions to completely skips files from being analysed. |
-|`--ignore-names`           | list | Removes provided list of names from the error output. |
-|`--ignore-names-in-files`  | list | Unused names from files matching provided path expressions. |
-|`--no-color`               | None | Removes colors from the output. |
+
+| Option                            | Type | Meaning  |
+|-----------------------------------|------|----------|
+|<pre>--exclude</pre>               | list | Path expressions to completely skip files from being analysed. |
+|<pre>--ignore-names</pre>          | list | Removes provided list of names from the error output. Regexp expressions to match multiple names can also be provided, e.g. `.*Mixin` will match all classes ending with `Mixin`. |
+|<pre>--ignore-names-in-files</pre> | list | Unused names from files matching provided path expressions. |
+|<pre>--no-color</pre>              | None | Removes colors from the output. |
+|<pre>--count</pre>                 | None | Provides the count of the detected unused names instead of printing them all out. |
+|<pre>--quite</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
+
 
 ## Contributing
 - `make check` - runs unit tests and other checks using virtual environment.
 
 ## Rationale
-`ruff` and `flake8` - don't have rules for unused global code detection, only for local ones `F823`, `F841`, `F842`.
-`deadcode` package tries to add a new `DC100` check for detecting variables/functions/classes which are not used in a whole code base.
-
-There is an alternative `vulture` package, which provides many false positives. `deadcode` - tries to find less, but findings are with higher confidence.
+[ruff](https://pypi.org/project/ruff/) and
+[flake8](https://pypi.org/project/flake8/) - don't have rules for unused global
+code detection, only for local ones `F823`, `F841`, `F842`. `deadcode` package
+tries to add a new `DC100` check for detecting variables/functions/classes
+which are not used in a whole code base.
+
+There is an alternative [vulture](https://pypi.org/project/vulture/) package,
+which provides many false positives.
+`deadcode` - tries to find less, but findings are with higher confidence.
 `deadcode` - is supposed to be used inline with other static code checkers like `ruff`.
 
 ## Known limitations
 If the same unused name is repeated in several files - it wont be detected.
 
-Files with syntax errors will be ignored, because `deadcode` uses `ast` to build abstract syntax tree for name usage detection.
+Files with syntax errors will be ignored, because `deadcode` uses `ast` to
+build abstract syntax tree for name usage detection.
 
-It is assumed that `deadcode` will be run using the same Python version as the checked code base is implemented in.
+It is assumed that `deadcode` will be run using the same Python version as the
+checked code base is implemented in.
```

