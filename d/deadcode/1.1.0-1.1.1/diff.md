# Comparing `tmp/deadcode-1.1.0.tar.gz` & `tmp/deadcode-1.1.1.tar.gz`

## Comparing `deadcode-1.1.0.tar` & `deadcode-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/__init__.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/cli.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/data_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/find_python_filenames.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/find_unused_names.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/get_unused_names_error_message.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_abstract_syntax_trees.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_arguments.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/parse_global_names.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/actions/read_files.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/base.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_command_line_argument_parsing.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_count_output.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/test_ignore_names_by_pattern.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/classes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/functions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/variables.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/tests/files/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/flatten_lists.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.0/deadcode/utils/path_matching.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.0/LICENSE
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 deadcode-1.1.0/README.md
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 deadcode-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/__init__.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/cli.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_abstract_syntax_trees.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_global_names.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/read_files.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/base.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_command_line_argument_parsing.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_count_output.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_ignore_names_by_pattern.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/path_matching.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 deadcode-1.1.1/README.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 deadcode-1.1.1/PKG-INFO
```

### Comparing `deadcode-1.1.0/deadcode/cli.py` & `deadcode-1.1.1/deadcode/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
     global_names = parse_global_names(files, args=args)
     abstract_syntax_trees_of_files = parse_abstract_syntax_trees(files, args=args)
     unused_names = find_unused_names(abstract_syntax_trees_of_files, global_names, args=args)
 
     if error_message := get_unused_names_error_message(unused_names, args=args):
         return error_message
 
-    if not args.count and not args.quite:
+    if not args.count and not args.quiet:
         print("\033[1mWell done!\033[0m ✨ 🚀 ✨")
     return None
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `deadcode-1.1.0/deadcode/actions/find_python_filenames.py` & `deadcode-1.1.1/deadcode/actions/find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/actions/find_unused_names.py` & `deadcode-1.1.1/deadcode/actions/find_unused_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/actions/get_unused_names_error_message.py` & `deadcode-1.1.1/deadcode/actions/get_unused_names_error_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from deadcode.data_types import Args
 
 
 def get_unused_names_error_message(unused_names: Dict[VariableName, Filename], args: Args) -> Optional[str]:
     if not unused_names:
         return None
 
-    if args.quite:
+    if args.quiet:
         return ""
 
     if args.count:
         return f"{len(unused_names)}"
 
     if args.no_color:
         return "\n".join([f"{filename} DC100 Global {name} is never used" for name, filename in unused_names.items()])
```

### Comparing `deadcode-1.1.0/deadcode/actions/parse_abstract_syntax_trees.py` & `deadcode-1.1.1/deadcode/actions/parse_abstract_syntax_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 def parse_abstract_syntax_trees(files: Dict[Filename, FileContent], args: Args) -> Dict[Filename, AbstractSyntaxTree]:
     """Did my code coverage just increased? Answer is no: a doc string was ignored :tada:"""
     abstract_syntax_trees_for_files = {}
     for filename, file_content in files.items():
         try:
             abstract_syntax_trees_for_files[filename] = ast.dump(ast.parse(file_content))  # Note: indent=1 for debug
         except:  # noqa: E722
-            if not args.count and not args.quite:
+            if not args.count and not args.quiet:
                 print(f"Error: Failed to parse {filename} file, ignoring it.")
             abstract_syntax_trees_for_files[filename] = ""
     return abstract_syntax_trees_for_files
```

### Comparing `deadcode-1.1.0/deadcode/actions/parse_arguments.py` & `deadcode-1.1.1/deadcode/actions/parse_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     parser.add_argument(
         "--no-color",
         help="Turn off colors in the output",
         action="store_true",
         default=False,
     )
     parser.add_argument(
-        "--quite",
+        "--quiet",
         help="Does not output anything. Makefile still fails with exit code 1 if unused names are found.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "--count",
         help="Provides the count of the detected unused names instead of printing them all out.",
```

### Comparing `deadcode-1.1.0/deadcode/actions/parse_global_names.py` & `deadcode-1.1.1/deadcode/actions/parse_global_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/tests/test_command_line_argument_parsing.py` & `deadcode-1.1.1/deadcode/tests/test_command_line_argument_parsing.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/tests/test_count_output.py` & `deadcode-1.1.1/deadcode/tests/test_count_output.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/tests/test_deadcode.py` & `deadcode-1.1.1/deadcode/tests/test_deadcode.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/tests/test_ignore_names_by_pattern.py` & `deadcode-1.1.1/deadcode/tests/test_ignore_names_by_pattern.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/deadcode/utils/flatten_lists.py` & `deadcode-1.1.1/deadcode/utils/flatten_lists.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/.gitignore` & `deadcode-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/LICENSE` & `deadcode-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.0/README.md` & `deadcode-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 | Option                            | Type | Meaning  |
 |-----------------------------------|------|----------|
 |<pre>--exclude</pre>               | list | Path expressions to completely skip files from being analysed. |
 |<pre>--ignore-names</pre>          | list | Removes provided list of names from the error output. Regexp expressions to match multiple names can also be provided, e.g. `.*Mixin` will match all classes ending with `Mixin`. |
 |<pre>--ignore-names-in-files</pre> | list | Unused names from files matching provided path expressions. |
 |<pre>--no-color</pre>              | None | Removes colors from the output. |
 |<pre>--count</pre>                 | None | Provides the count of the detected unused names instead of printing them all out. |
-|<pre>--quite</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
+|<pre>--quiet</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
 
 
 ## Contributing
 - `make check` - runs unit tests and other checks using virtual environment.
 
 ## Rationale
 [ruff](https://pypi.org/project/ruff/) and
```

### Comparing `deadcode-1.1.0/pyproject.toml` & `deadcode-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
```

### Comparing `deadcode-1.1.0/PKG-INFO` & `deadcode-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadcode
-Version: 1.1.0
+Version: 1.1.1
 Summary: Find and remove dead code.
 Project-URL: Homepage, https://github.com/albertas/deadcode
 Project-URL: Documentation, https://deadcode.readthedocs.io/
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -52,15 +52,15 @@
 | Option                            | Type | Meaning  |
 |-----------------------------------|------|----------|
 |<pre>--exclude</pre>               | list | Path expressions to completely skip files from being analysed. |
 |<pre>--ignore-names</pre>          | list | Removes provided list of names from the error output. Regexp expressions to match multiple names can also be provided, e.g. `.*Mixin` will match all classes ending with `Mixin`. |
 |<pre>--ignore-names-in-files</pre> | list | Unused names from files matching provided path expressions. |
 |<pre>--no-color</pre>              | None | Removes colors from the output. |
 |<pre>--count</pre>                 | None | Provides the count of the detected unused names instead of printing them all out. |
-|<pre>--quite</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
+|<pre>--quiet</pre>                 | None | Does not output anything. Makefile still fails with exit code 1 if unused names are found. |
 
 
 ## Contributing
 - `make check` - runs unit tests and other checks using virtual environment.
 
 ## Rationale
 [ruff](https://pypi.org/project/ruff/) and
```

