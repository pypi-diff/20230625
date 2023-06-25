# Comparing `tmp/noseOfYeti-2.4.1.tar.gz` & `tmp/noseOfYeti-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noseOfYeti-2.4.1.tar", last modified: Sun Dec  4 01:04:50 2022, max compression
+gzip compressed data, was "noseOfYeti-2.4.2.tar", last modified: Sun Jun 25 02:53:20 2023, max compression
```

## Comparing `noseOfYeti-2.4.1.tar` & `noseOfYeti-2.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.031963 noseOfYeti-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2022-12-04 01:04:50.031963 noseOfYeti-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.023962 noseOfYeti-2.4.1/noseOfYeti/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.027962 noseOfYeti-2.4.1/noseOfYeti/black/
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/black/Grammar.noy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/black/noy_black.pth
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.027962 noseOfYeti-2.4.1/noseOfYeti/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/black_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/nosetests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/pylama.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/pyls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/plugins/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.031963 noseOfYeti-2.4.1/noseOfYeti/tokeniser/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/chooser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/spec_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/tokeniser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    20947 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/noseOfYeti/tokeniser/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 01:04:50.027962 noseOfYeti-2.4.1/noseOfYeti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2022-12-04 01:04:49.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-04 01:04:50.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 01:04:50.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-04 01:04:50.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-04 01:04:50.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-04 01:04:50.000000 noseOfYeti-2.4.1/noseOfYeti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-04 01:04:50.031963 noseOfYeti-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2022-12-04 01:04:46.000000 noseOfYeti-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.152031 noseOfYeti-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-25 02:53:20.152031 noseOfYeti-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.148031 noseOfYeti-2.4.2/noseOfYeti/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.148031 noseOfYeti-2.4.2/noseOfYeti/black/
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/black/Grammar.noy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/black/noy_black.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.148031 noseOfYeti-2.4.2/noseOfYeti/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/black_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/nosetests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/pylama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/plugins/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.152031 noseOfYeti-2.4.2/noseOfYeti/tokeniser/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/chooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/spec_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/tokeniser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/noseOfYeti/tokeniser/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:53:20.148031 noseOfYeti-2.4.2/noseOfYeti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 02:53:20.000000 noseOfYeti-2.4.2/noseOfYeti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 02:53:20.152031 noseOfYeti-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-25 02:53:14.000000 noseOfYeti-2.4.2/setup.py
```

### Comparing `noseOfYeti-2.4.1/LICENSE` & `noseOfYeti-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/PKG-INFO` & `noseOfYeti-2.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: noseOfYeti
-Version: 2.4.1
+Version: 2.4.2
 Summary: A custom pyton codec that provides an RSpec style dsl for python
 Home-page: https://github.com/delfick/nose-of-yeti
 Author: Stephen Moore
 Author-email: delfick755@gmail.com
 License: MIT
 Keywords: bdd rspec spec
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: tests
 Provides-Extra: black
 License-File: LICENSE
@@ -49,9 +48,7 @@
 
 It is recommended any .pyc files are removed when NoseOfYeti is upgraded.
 
 The Python interpreter skips the translation process if it
 sees a .pyc file (unless the .py file has changed since the .pyc file was
 created). This means that any changes in the translation process won't apply
 until either the .pyc files are removed or all the .py files have been changed.
-
-
```

### Comparing `noseOfYeti-2.4.1/README.rst` & `noseOfYeti-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/black/Grammar.noy.txt` & `noseOfYeti-2.4.2/noseOfYeti/black/Grammar.noy.txt`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/plugins/black_compat.py` & `noseOfYeti-2.4.2/noseOfYeti/plugins/black_compat.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/plugins/nosetests.py` & `noseOfYeti-2.4.2/noseOfYeti/plugins/nosetests.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/plugins/pylama.py` & `noseOfYeti-2.4.2/noseOfYeti/plugins/pylama.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/plugins/pyls.py` & `noseOfYeti-2.4.2/noseOfYeti/plugins/pyls.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/plugins/pytest.py` & `noseOfYeti-2.4.2/noseOfYeti/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/chooser.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/chooser.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/containers.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/containers.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/spec_codec.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/spec_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         """
         data = []
         try:
             # We pass in the data variable as an argument so that we
             # get partial output even in the case of an exception.
             self.tokeniser.translate(readline, data, **kwargs)
         except:
-            lines = ['msg = """']
+            lines = ['msg = r"""']
             for line in traceback.format_exception(*sys.exc_info()):
                 lines.append(line.strip())
             lines.append('"""')
             lines.append(r'raise Exception(f"--- internal spec codec error --- \n{msg}")')
             data = "\n".join(lines)
         else:
             # At this point, data is a list of tokens
```

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/support.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/support.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/tokeniser.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/tokeniser.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/tokens.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/tokens.py`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/noseOfYeti/tokeniser/tracker.py` & `noseOfYeti-2.4.2/noseOfYeti/tokeniser/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,19 +213,23 @@
         # Hence current group isn't empty !
         if found_content and not created_group:
             self.groups.empty = False
 
         # Just append if token should be
         if just_append:
             # Make sure comments are indented appropriately
+            add_dedent = False
             if tokenum == COMMENT and not self.in_container:
                 indent = self.indent_type * (self.current.scol - self.groups.level)
                 self.result.append((INDENT, indent))
+                add_dedent = True
 
             self.result.append([tokenum, value])
+            if add_dedent:
+                self.result.append((DEDENT, ""))
 
     ########################
     ###   UTILITY
     ########################
 
     def add_tokens(self, tokens):
         """Add tokens to result"""
```

### Comparing `noseOfYeti-2.4.1/noseOfYeti.egg-info/PKG-INFO` & `noseOfYeti-2.4.2/noseOfYeti.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: noseOfYeti
-Version: 2.4.1
+Version: 2.4.2
 Summary: A custom pyton codec that provides an RSpec style dsl for python
 Home-page: https://github.com/delfick/nose-of-yeti
 Author: Stephen Moore
 Author-email: delfick755@gmail.com
 License: MIT
 Keywords: bdd rspec spec
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: tests
 Provides-Extra: black
 License-File: LICENSE
@@ -49,9 +48,7 @@
 
 It is recommended any .pyc files are removed when NoseOfYeti is upgraded.
 
 The Python interpreter skips the translation process if it
 sees a .pyc file (unless the .py file has changed since the .pyc file was
 created). This means that any changes in the translation process won't apply
 until either the .pyc files are removed or all the .py files have been changed.
-
-
```

### Comparing `noseOfYeti-2.4.1/noseOfYeti.egg-info/SOURCES.txt` & `noseOfYeti-2.4.2/noseOfYeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noseOfYeti-2.4.1/setup.py` & `noseOfYeti-2.4.2/setup.py`

 * *Files identical despite different names*

