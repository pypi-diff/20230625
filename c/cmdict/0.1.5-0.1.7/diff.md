# Comparing `tmp/cmdict-0.1.5.tar.gz` & `tmp/cmdict-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdict-0.1.5.tar", max compression
+gzip compressed data, was "cmdict-0.1.7.tar", max compression
```

## Comparing `cmdict-0.1.5.tar` & `cmdict-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-06-18 11:48:39.310220 cmdict-0.1.5/LICENSE
--rw-r--r--   0        0        0     2717 2023-06-18 11:48:39.310220 cmdict-0.1.5/README.md
--rw-r--r--   0        0        0     1298 2023-06-18 11:48:39.314220 cmdict-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/__init__.py
--rw-r--r--   0        0        0      112 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/__main__.py
--rw-r--r--   0        0        0     2558 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/ecdict_connector.py
--rw-r--r--   0        0        0     1423 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/history.py
--rw-r--r--   0        0        0     4530 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/pdf_tools.py
--rw-r--r--   0        0        0     6129 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/run_script.py
--rw-r--r--   0        0        0      463 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/txt_tools.py
--rw-r--r--   0        0        0      384 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/utils.py
--rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 cmdict-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-25 09:02:28.422962 cmdict-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2717 2023-06-25 09:02:28.422962 cmdict-0.1.7/README.md
+-rw-r--r--   0        0        0     1298 2023-06-25 09:02:28.422962 cmdict-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/__main__.py
+-rw-r--r--   0        0        0     2558 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/ecdict_connector.py
+-rw-r--r--   0        0        0     1423 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/history.py
+-rw-r--r--   0        0        0     4685 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/pdf_tools.py
+-rw-r--r--   0        0        0     6901 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/run_script.py
+-rw-r--r--   0        0        0      463 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/txt_tools.py
+-rw-r--r--   0        0        0      384 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/utils.py
+-rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 cmdict-0.1.7/PKG-INFO
```

### Comparing `cmdict-0.1.5/LICENSE` & `cmdict-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.5/README.md` & `cmdict-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.5/pyproject.toml` & `cmdict-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdict"
-version = "0.1.5"
+version = "0.1.7"
 description = "A command line dictionary toolset."
 authors = ["zequnyu <zequnyu11@gmail.com>", "edxu96 <edxu96@outlook.com>"]
 license = "GPL-3.0"
 exclude = ["src/cmdict/data/*"]
 readme = "README.md"
 repository = "https://github.com/pastydev/cmdict"
```

### Comparing `cmdict-0.1.5/src/cmdict/ecdict_connector.py` & `cmdict-0.1.7/src/cmdict/ecdict_connector.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.5/src/cmdict/history.py` & `cmdict-0.1.7/src/cmdict/history.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.5/src/cmdict/pdf_tools.py` & `cmdict-0.1.7/src/cmdict/pdf_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Functions to handle highlights in PDF files."""
 from cmdict.ecdict_connector import ECDICTConnector
 from cmdict.utils import remove_punctuation
 
 PDF_FEATURES: bool
 """If the features for PDF are enabled."""
 try:
-    import fitz
-except ImportError:
+    # ``import fitz`` still works, if the directory where it comes from
+    # is empty, so the following command must be used.
+    from fitz import open
+except (ImportError, ModuleNotFoundError):
     PDF_FEATURES = False
 else:
     PDF_FEATURES = True
 
 PREVIEW_COLORS = {
     "yellow": [250, 205, 90],
     "green": [124, 200, 104],
@@ -33,15 +35,15 @@
     Returns:
         list[str]: list of found words.
     """
     if color.lower() not in PREVIEW_COLORS:
         return []
 
     res = set()
-    document = fitz.open(file_path)
+    document = open(file_path)
     for annot in _iterate_filtered_annotations(document, color):
         # annotation may contain several rectangles in different rows
         word_list = []
         rect_counts = len(annot.vertices) // 4
         for i in range(rect_counts):
             for word_block in _iterate_all_word_blocks(document):
                 if _check_contain(
```

### Comparing `cmdict-0.1.5/src/cmdict/run_script.py` & `cmdict-0.1.7/src/cmdict/run_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,39 @@
 _init_colorama(autoreset=True)
 
 _db_dir = os.path.join(str(pathlib.Path(__file__).parent), "data")
 _db_file = os.path.join(_db_dir, "stardict.db")
 _db_path = pathlib.Path(_db_file)
 
 
-@click.group()
+class ActiveFlagCommand(click.Group):
+    """Add a keyword argument that can optionally disable a command.
+
+    Based on https://stackoverflow.com/a/55379716/10181743.
+    """
+
+    def command(self, *args, active=True, **kwargs):
+        """Add a command to CLI if ``active`` is true.
+
+        Args:
+            *args: other arguments.
+            active: if the command is active. Defaults to True.
+            **kwargs: other keyword arguments.
+
+        Returns:
+            Decorated function by ``click``, if ``active`` is true. The
+            original function, otherwise.
+        """
+        if active:
+            return super(ActiveFlagCommand, self).command(*args, **kwargs)
+        else:
+            return lambda f: f
+
+
+@click.group(cls=ActiveFlagCommand)
 def cli():
     """Command line interface."""
 
 
 @cli.command()
 def download():
     """Download necessary database before using cmdict."""
@@ -108,15 +132,15 @@
         words = scan_words(txt_path)
         for i, word in enumerate(words):
             _echo_item(word, db_engine.query(word))
     else:
         _echo_warn_download()
 
 
-@cli.command()
+@cli.command(active=PDF_FEATURES)
 @click.argument("pdf_path", type=click.Path(exists=True))
 @click.option(
     "--color",
     default="yellow",
     help="Which color the highlights are in.",
     show_default=True,
 )
```

### Comparing `cmdict-0.1.5/PKG-INFO` & `cmdict-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdict
-Version: 0.1.5
+Version: 0.1.7
 Summary: A command line dictionary toolset.
 Home-page: https://github.com/pastydev/cmdict
 License: GPL-3.0
 Author: zequnyu
 Author-email: zequnyu11@gmail.com
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

