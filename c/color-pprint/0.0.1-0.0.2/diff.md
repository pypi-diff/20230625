# Comparing `tmp/color-pprint-0.0.1.tar.gz` & `tmp/color-pprint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color-pprint-0.0.1.tar", last modified: Thu Nov 17 19:14:20 2022, max compression
+gzip compressed data, was "color-pprint-0.0.2.tar", last modified: Sat Jun 24 21:46:34 2023, max compression
```

## Comparing `color-pprint-0.0.1.tar` & `color-pprint-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:20.720658 color-pprint-0.0.1/
--rw-rw-rw-   0        0        0     1103 2022-11-17 15:06:57.000000 color-pprint-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       85 2022-11-17 14:36:53.000000 color-pprint-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2665 2022-11-17 19:14:20.725649 color-pprint-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2022-11-17 18:47:11.000000 color-pprint-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:20.632703 color-pprint-0.0.1/color_pprint/
--rw-rw-rw-   0        0        0     1165 2022-11-17 15:06:57.000000 color-pprint-0.0.1/color_pprint/__init__.py
--rw-rw-rw-   0        0        0     5509 2022-11-17 15:07:02.000000 color-pprint-0.0.1/color_pprint/__main__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:20.704661 color-pprint-0.0.1/color_pprint/ansi/
--rw-rw-rw-   0        0        0    11339 2022-11-17 15:07:01.000000 color-pprint-0.0.1/color_pprint/ansi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 19:14:20.699664 color-pprint-0.0.1/color_pprint.egg-info/
--rw-rw-rw-   0        0        0     2665 2022-11-17 19:14:20.000000 color-pprint-0.0.1/color_pprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2022-11-17 19:14:20.000000 color-pprint-0.0.1/color_pprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 19:14:20.000000 color-pprint-0.0.1/color_pprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-11-17 19:14:20.000000 color-pprint-0.0.1/color_pprint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-17 19:14:20.000000 color-pprint-0.0.1/color_pprint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2022-11-17 17:54:03.000000 color-pprint-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-17 19:14:20.751635 color-pprint-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1682 2022-11-17 19:13:38.000000 color-pprint-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.798798 color-pprint-0.0.2/
+-rw-rw-rw-   0        0        0     1103 2022-11-17 15:06:57.000000 color-pprint-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2022-11-17 14:36:53.000000 color-pprint-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2665 2023-06-24 21:46:34.799798 color-pprint-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2022-11-17 18:47:11.000000 color-pprint-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.781809 color-pprint-0.0.2/color_pprint/
+-rw-rw-rw-   0        0        0     1165 2022-11-17 15:06:57.000000 color-pprint-0.0.2/color_pprint/__init__.py
+-rw-rw-rw-   0        0        0     5448 2022-11-18 00:13:51.000000 color-pprint-0.0.2/color_pprint/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.796800 color-pprint-0.0.2/color_pprint/ansi/
+-rw-rw-rw-   0        0        0    11333 2023-06-24 21:33:23.000000 color-pprint-0.0.2/color_pprint/ansi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.794800 color-pprint-0.0.2/color_pprint.egg-info/
+-rw-rw-rw-   0        0        0     2665 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2022-11-17 17:54:03.000000 color-pprint-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:46:34.801796 color-pprint-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-24 21:38:58.000000 color-pprint-0.0.2/setup.py
```

### Comparing `color-pprint-0.0.1/LICENSE` & `color-pprint-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `color-pprint-0.0.1/PKG-INFO` & `color-pprint-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color-pprint
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
 Home-page: https://github.com/mccoderpy/color-pprint
 Author: mccoder.py
 Author-email: mccuber04@outlook.de
 License: MIT
 Project-URL: Source, https://github.com/mccoderpy/color-pprint/
 Project-URL: Support, https://discord.gg/sb69muSqsg
```

### Comparing `color-pprint-0.0.1/README.md` & `color-pprint-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `color-pprint-0.0.1/color_pprint/__init__.py` & `color-pprint-0.0.2/color_pprint/__init__.py`

 * *Files identical despite different names*

### Comparing `color-pprint-0.0.1/color_pprint/__main__.py` & `color-pprint-0.0.2/color_pprint/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,36 +31,29 @@
 import sys
 import json
 from . import *
 from os import PathLike
 
 
 def exit_with_help():
-    sys.exit('''
-    Usage:
-    
-    <python> -m color_pprint [--ansi/-a] [--discord/-d] [--file/-f <FILE_TO_WRITE_TO>] <[value/PATH_TO_READ_FROM,]>
-    
-    Example: "py -m color_pprint --file ./test.json --discord '{\"hello\": \"world\", \"something\": 1234}'"
-    '''
-             )
+    sys.exit(
+        "Usage:\n\n"
+        "<python> -m color_pprint [--ansi/-a] [--discord/-d] [--file/-f <FILE_TO_WRITE_TO>] <[value/PATH_TO_READ_FROM,]>\n\n"
+        "Example: \"py -m color_pprint --file ./test.json --discord '{\"hello\": \"world\", \"something\": 1234}'\""
+    )
 
 
 def open_file(path: PathLike):
     return open(path, "a+", encoding='utf-8')
 
 
 if __name__ == '__main__':
     args: list[str | PathLike] = sys.argv[1:]
     if not args or '--help' in args:
-        print(
-            '''
-            A simple package to pretty-print lists dicts, tuples, etc. with color and highlight - (c) 2022-present mccoderpy
-            '''
-        )
+        print('A simple package to pretty-print lists dicts, tuples, etc. with color and highlight - (c) 2022-present mccoderpy')
         exit_with_help()
 
     values = []
     mode = 'default'
     file = sys.stdout
     kwargs = {}
```

### Comparing `color-pprint-0.0.1/color_pprint/ansi/__init__.py` & `color-pprint-0.0.2/color_pprint/ansi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,20 +36,22 @@
     Any,
     TypeVar
 )
 
 
 if TYPE_CHECKING:
     from _typeshed import SupportsWrite
-    from re import Pattern
+
 
 import json
 import colorama
 import multidict
+from re import Pattern
 import collections.abc
+
 from pprint import saferepr
 
 __all__ = (
     'highlight_values',
     'color_dict',
     'color_dumps',
     'cprint'
@@ -259,15 +261,15 @@
             separators=(', ', f'{FORE.RED}:{FORE.RESET} '),
             **kwargs
         )
     except Exception as exc:
         print(exc)
         return str(result)
     else:
-        return as_str.replace('\\u001b', '\033').replace('"', '')
+        return as_str.replace('\\u001b', '\033').strip('"')
 
 
 def cprint(
         *values: object,
         highlight: Sequence[Union[str, Pattern]] = None,
         highlight_groups: Sequence[str] = [],
         key_color: Union[FORE, BACK] = FORE.LIGHTRED_EX,
```

### Comparing `color-pprint-0.0.1/color_pprint.egg-info/PKG-INFO` & `color-pprint-0.0.2/color_pprint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color-pprint
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
 Home-page: https://github.com/mccoderpy/color-pprint
 Author: mccoder.py
 Author-email: mccuber04@outlook.de
 License: MIT
 Project-URL: Source, https://github.com/mccoderpy/color-pprint/
 Project-URL: Support, https://discord.gg/sb69muSqsg
```

### Comparing `color-pprint-0.0.1/setup.py` & `color-pprint-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as fp:
     long_description = fp.read()
 
 setup(
     name='color-pprint',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/mccoderpy/color-pprint',
     project_urls={
         'Source': 'https://github.com/mccoderpy/color-pprint/',
         'Support': 'https://discord.gg/sb69muSqsg',
         'Issue Tracker': 'https://github.com/mccoderpy/color-pprint/issues'
     },
     license='MIT',
```

