# Comparing `tmp/fix8-0.1.7.tar.gz` & `tmp/fix8-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fix8-0.1.7.tar", last modified: Sat Jun 17 18:23:52 2023, max compression
+gzip compressed data, was "fix8-0.1.8.tar", last modified: Sun Jun 25 12:34:32 2023, max compression
```

## Comparing `fix8-0.1.7.tar` & `fix8-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:23:52.606634 fix8-0.1.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-17 18:23:52.606634 fix8-0.1.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-17 18:23:43.000000 fix8-0.1.7/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:23:52.606634 fix8-0.1.7/fix8.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      229 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/zip-safe
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    14750 2023-06-17 18:23:43.000000 fix8-0.1.7/fix8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-17 18:23:52.606634 fix8-0.1.7/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1543 2023-06-17 18:23:43.000000 fix8-0.1.7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:34:32.411961 fix8-0.1.8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-25 12:34:32.411961 fix8-0.1.8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-25 12:34:23.000000 fix8-0.1.8/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 12:34:32.411961 fix8-0.1.8/fix8.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      229 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 12:34:32.000000 fix8-0.1.8/fix8.egg-info/zip-safe
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15616 2023-06-25 12:34:23.000000 fix8-0.1.8/fix8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-06-25 12:34:32.411961 fix8-0.1.8/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1543 2023-06-25 12:34:23.000000 fix8-0.1.8/setup.py
```

### Comparing `fix8-0.1.7/PKG-INFO` & `fix8-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
```

### Comparing `fix8-0.1.7/README.md` & `fix8-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fix8-0.1.7/fix8.egg-info/PKG-INFO` & `fix8-0.1.8/fix8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
```

### Comparing `fix8-0.1.7/fix8.py` & `fix8-0.1.8/fix8.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 
 class CodeLine(NamedTuple):
     text: str
     line: int
     col: int
 
 
+class FixResult(NamedTuple):
+    new_content: str
+    fixed: list[ErrorDetail]
+
+
 Position = Tuple[int, int]
 Span = Tuple[Position, Position]
 
 # TODO: currently we return the new string, we should move to instead returning
 # a description of the edit.
 LineFixer = Callable[[CodeLine], str]
 TLineFixer = TypeVar('TLineFixer', bound=LineFixer)
@@ -414,15 +419,15 @@
         # Note: the wrapper will close our buffer when it gets closed, so need to
         # get the value while it's still alive.
         output = buffer.getvalue().decode()
 
     return parse_flake8_output(output)
 
 
-def process_errors(messages: list[ErrorDetail], content: str) -> str:
+def process_errors(messages: list[ErrorDetail], content: str) -> FixResult:
     lines = content.splitlines()
     modified = False
 
     for message in sorted(messages, reverse=True):
         line_fixer_fn = LINE_FIXERS.get(message.code)
         if not line_fixer_fn:
             continue
@@ -436,43 +441,64 @@
 
         lines[lineno] = new_line
         modified = True
 
     if modified:
         content = ''.join(x.rstrip() + '\n' for x in lines)
 
+    fixed: list[ErrorDetail] = []
+
     for code, fixer_fn in FILE_FIXERS.items():
         relevant_messages = [x for x in messages if x.code == code]
         if relevant_messages:
             content = fixer_fn(relevant_messages, content)
+            fixed += relevant_messages
 
-    return content
+    return FixResult(content, fixed)
 
 
 def run(args: argparse.Namespace) -> None:
     all_error_details = run_flake8(args.flake8_args)
 
     for filepath, error_details in all_error_details.items():
         if error_details[0].code == 'E999':
             print(error_details[0].render(filepath))
             continue
 
         with filepath.open(mode='r+') as f:
             content = f.read()
-            new_content = process_errors(error_details, content)
+            new_content, fixed_errors = process_errors(error_details, content)
+
+            fixed_set = set(fixed_errors)
+
+            if args.verbose:
+                print('--')
 
             if new_content != content:
                 print(f"Fixing {filepath}")
                 f.seek(0)
                 f.write(new_content)
                 f.truncate()
 
+            if args.verbose:
+                remaining = [x for x in error_details if x not in fixed_set]
+                fixed = [x for x in error_details if x in fixed_set]
+                if remaining:
+                    print("Remaining:")
+                    for detail in remaining:
+                        print(" ", detail.render(filepath))
+                if fixed:
+                    print("Fixed:")
+                    for detail in fixed:
+                        print(" ", detail.render(filepath))
+
 
 def parse_args(argv: list[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
+    parser.add_argument('--verbose', action='store_true')
     parser.add_argument('flake8_args', metavar='FLAKE8_ARG', nargs='*')
     return parser.parse_args(argv)
 
 
 def main(argv: list[str] = sys.argv[1:]) -> None:
     return run(parse_args(argv))
```

### Comparing `fix8-0.1.7/setup.cfg` & `fix8-0.1.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 	build,
 	debian,
 	script
 ignore = 
 	C401
 	W503
 max_line_length = 90
+per-file-ignores = 
+	tests.py:E501
+noqa-require-code = true
 
 [isort]
 atomic = True
 indent = 4
 multi_line_output = 3
 use_parentheses = True
 include_trailing_comma = True
```

### Comparing `fix8-0.1.7/setup.py` & `fix8-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup  # type: ignore[import]
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='fix8',
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/PeterJCLaw/fix8',
     project_urls={
         'Documentation': 'https://github.com/PeterJCLaw/fix8/blob/master/README.md',
         'Code': 'https://github.com/PeterJCLaw/fix8',
         'Issue tracker': 'https://github.com/PeterJCLaw/fix8/issues',
     },
     description="Automatic fix for Python linting issues found by Flake8",
```

