# Comparing `tmp/deadcode-1.1.1.tar.gz` & `tmp/deadcode-1.1.2.tar.gz`

## Comparing `deadcode-1.1.1.tar` & `deadcode-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/__init__.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/cli.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/data_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/find_python_filenames.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/find_unused_names.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/get_unused_names_error_message.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_abstract_syntax_trees.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_arguments.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/parse_global_names.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/actions/read_files.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/base.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_command_line_argument_parsing.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_count_output.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/test_ignore_names_by_pattern.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/classes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/functions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/variables.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/tests/files/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/flatten_lists.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.1/deadcode/utils/path_matching.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.1/LICENSE
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 deadcode-1.1.1/README.md
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 deadcode-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/cli.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_abstract_syntax_trees.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/parse_global_names.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/actions/read_files.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/base.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_command_line_argument_parsing.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_ignore_names_by_pattern.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/test_output.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-1.1.2/deadcode/utils/path_matching.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-1.1.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 deadcode-1.1.2/README.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 deadcode-1.1.2/PKG-INFO
```

### Comparing `deadcode-1.1.1/deadcode/cli.py` & `deadcode-1.1.2/deadcode/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     python_filenames = find_python_filenames(args=args)
     files = read_files(python_filenames)
 
     global_names = parse_global_names(files, args=args)
     abstract_syntax_trees_of_files = parse_abstract_syntax_trees(files, args=args)
     unused_names = find_unused_names(abstract_syntax_trees_of_files, global_names, args=args)
 
-    if error_message := get_unused_names_error_message(unused_names, args=args):
+    if (error_message := get_unused_names_error_message(unused_names, args=args)) is not None:
         return error_message
 
     if not args.count and not args.quiet:
         print("\033[1mWell done!\033[0m ✨ 🚀 ✨")
     return None
```

### Comparing `deadcode-1.1.1/deadcode/actions/find_python_filenames.py` & `deadcode-1.1.2/deadcode/actions/find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/actions/find_unused_names.py` & `deadcode-1.1.2/deadcode/actions/find_unused_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/actions/get_unused_names_error_message.py` & `deadcode-1.1.2/deadcode/actions/get_unused_names_error_message.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/actions/parse_abstract_syntax_trees.py` & `deadcode-1.1.2/deadcode/actions/parse_abstract_syntax_trees.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/actions/parse_arguments.py` & `deadcode-1.1.2/deadcode/actions/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/actions/parse_global_names.py` & `deadcode-1.1.2/deadcode/actions/parse_global_names.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/tests/test_command_line_argument_parsing.py` & `deadcode-1.1.2/deadcode/tests/test_command_line_argument_parsing.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/tests/test_deadcode.py` & `deadcode-1.1.2/deadcode/tests/test_deadcode.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,59 +33,14 @@
             unused_names,
             (
                 "tests/files/classes.py:1:6: DC100 Global UnusedClass is never used\n"
                 "tests/files/classes.py:13:6: DC100 Global AnotherUnusedClass is never used"
             ),
         )
 
-    def test_colorful_output(self):
-        self.read_files_mock = self.patch("deadcode.cli.read_files")
-        self.read_files_mock.return_value = {
-            "tests/files/variables.py": """\
-unused_global_variable = True
-ANOTHER_GLOBAL_VARIABLE = "This variable is unused"
-third_global_varialbe3 = 12 * 25
-THIS_ONE_IS_USED = "World"
-print(THIS_ONE_IS_USED)"""
-        }
-        unused_names = main(["tests/files/variables.py"])
-
-        self.assertEqual(
-            unused_names,
-            (
-                "tests/files/variables.py:1:0: \x1b[91mDC100\x1b[0m Global "
-                "\x1b[1munused_global_variable\x1b[0m is never used\n"
-                "tests/files/variables.py:2:0: \x1b[91mDC100\x1b[0m Global "
-                "\x1b[1mANOTHER_GLOBAL_VARIABLE\x1b[0m is never used\n"
-                "tests/files/variables.py:3:0: \x1b[91mDC100\x1b[0m Global "
-                "\x1b[1mthird_global_varialbe3\x1b[0m is never used"
-            ),
-        )
-
-    def test_unused_variable_name_found_file_content_patched(self):
-        self.read_files_mock = self.patch("deadcode.cli.read_files")
-        self.read_files_mock.return_value = {
-            "tests/files/variables.py": """\
-unused_global_variable = True
-ANOTHER_GLOBAL_VARIABLE = "This variable is unused"
-third_global_varialbe3 = 12 * 25
-THIS_ONE_IS_USED = "World"
-print(THIS_ONE_IS_USED)"""
-        }
-        unused_names = main(["tests/files/variables.py", "--no-color"])
-
-        self.assertEqual(
-            unused_names,
-            (
-                "tests/files/variables.py:1:0: DC100 Global unused_global_variable is never used\n"
-                "tests/files/variables.py:2:0: DC100 Global ANOTHER_GLOBAL_VARIABLE is never used\n"
-                "tests/files/variables.py:3:0: DC100 Global third_global_varialbe3 is never used"
-            ),
-        )
-
     def test_invalid_python_file_found(self):
         self.read_files_mock = self.patch("deadcode.cli.read_files")
         self.read_files_mock.return_value = {"tests/files/invalid_file.py": """This is invalid python file content."""}
         unused_names = main(["tests/files/invalid_file.py", "--no-color"])
 
         self.assertEqual(unused_names, None)
```

### Comparing `deadcode-1.1.1/deadcode/tests/test_ignore_names_by_pattern.py` & `deadcode-1.1.2/deadcode/tests/test_ignore_names_by_pattern.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/deadcode/utils/flatten_lists.py` & `deadcode-1.1.2/deadcode/utils/flatten_lists.py`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/.gitignore` & `deadcode-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/LICENSE` & `deadcode-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadcode-1.1.1/pyproject.toml` & `deadcode-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
```

