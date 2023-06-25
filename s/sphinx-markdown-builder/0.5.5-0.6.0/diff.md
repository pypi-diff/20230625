# Comparing `tmp/sphinx-markdown-builder-0.5.5.tar.gz` & `tmp/sphinx-markdown-builder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-markdown-builder-0.5.5.tar", last modified: Sat Jan  8 15:31:19 2022, max compression
+gzip compressed data, was "sphinx-markdown-builder-0.6.0.tar", last modified: Sun Jun 25 12:09:52 2023, max compression
```

## Comparing `sphinx-markdown-builder-0.5.5.tar` & `sphinx-markdown-builder-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 clayrisser  (1000) clayrisser  (1001)        0 2022-01-08 15:31:19.924679 sphinx-markdown-builder-0.5.5/
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)     4959 2022-01-08 15:31:19.924679 sphinx-markdown-builder-0.5.5/PKG-INFO
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)     3311 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/README.md
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)       67 2022-01-08 15:31:19.924679 sphinx-markdown-builder-0.5.5/setup.cfg
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)     1642 2022-01-08 15:28:53.000000 sphinx-markdown-builder-0.5.5/setup.py
-drwxr-xr-x   0 clayrisser  (1000) clayrisser  (1001)        0 2022-01-08 15:31:19.924679 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)      100 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/__init__.py
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)      758 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/depth.py
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)    25213 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/doctree2md.py
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)     2222 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/markdown_builder.py
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)    10504 2022-01-08 15:27:25.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/markdown_writer.py
-drwxr-xr-x   0 clayrisser  (1000) clayrisser  (1001)        0 2022-01-08 15:31:19.924679 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)     4959 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/PKG-INFO
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)      506 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/SOURCES.txt
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)        1 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/dependency_links.txt
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)       54 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/entry_points.txt
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)       35 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/requires.txt
--rw-r--r--   0 clayrisser  (1000) clayrisser  (1001)       24 2022-01-08 15:31:19.000000 sphinx-markdown-builder-0.5.5/sphinx_markdown_builder.egg-info/top_level.txt
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.0/CONTRIBUTING.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2670 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1961 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/README.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1865 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/
+-rw-rw-r--   0 liran     (1000) liran     (1000)      484 2023-06-25 12:07:13.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2813 2023-06-25 11:47:26.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5547 2023-06-25 11:53:29.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/contexts.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    23402 2023-06-25 11:56:31.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/translator.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1421 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/writer.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2670 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      514 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-06-25 12:09:52.000000 sphinx-markdown-builder-0.6.0/sphinx_markdown_builder.egg-info/top_level.txt
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-06-25 12:09:52.125374 sphinx-markdown-builder-0.6.0/tests/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1345 2023-06-25 11:01:32.000000 sphinx-markdown-builder-0.6.0/tests/test_builder.py
```

### Comparing `sphinx-markdown-builder-0.5.5/sphinx_markdown_builder/markdown_builder.py` & `sphinx-markdown-builder-0.6.0/sphinx_markdown_builder/builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,83 @@
-from .markdown_writer import MarkdownWriter, MarkdownTranslator
+"""
+docutils XML to markdown translator.
+"""
+import os
+from typing import Set
+
+from docutils import nodes
 from docutils.io import StringOutput
-from io import open
-from os import path
+from sphinx.application import Sphinx
 from sphinx.builders import Builder
+from sphinx.environment import BuildEnvironment
 from sphinx.locale import __
 from sphinx.util import logging
 from sphinx.util.osutil import ensuredir, os_path
 
+from sphinx_markdown_builder.translator import MarkdownTranslator
+from sphinx_markdown_builder.writer import MarkdownWriter
+
 logger = logging.getLogger(__name__)
 
+
+def get_mod_time_if_exists(file_path):
+    try:
+        return os.path.getmtime(file_path)
+    except OSError as err:
+        logger.warning(__("error reading file %s: %s"), file_path, err)
+        return 0
+
+
 class MarkdownBuilder(Builder):
-    name = 'markdown'
-    format = 'markdown'
-    epilog = __('The markdown files are in %(outdir)s.')
+    name = "markdown"
+    format = "markdown"
+    epilog = __("The markdown files are in %(outdir)s.")
 
-    out_suffix = '.md'
     allow_parallel = True
     default_translator_class = MarkdownTranslator
 
-    current_docname = None
+    out_suffix = ".md"
 
-    markdown_http_base = 'https://localhost'
+    def __init__(self, app: Sphinx, env: BuildEnvironment = None):
+        super().__init__(app, env)
+        self.writer = None
+        self.sec_numbers = None
+        self.current_doc_name = None
 
     def init(self):
-        self.secnumbers = {}
+        self.sec_numbers = {}
 
     def get_outdated_docs(self):
-        for docname in self.env.found_docs:
-            if docname not in self.env.all_docs:
-                yield docname
+        for doc_name in self.env.found_docs:
+            if doc_name not in self.env.all_docs:
+                yield doc_name
                 continue
-            targetname = path.join(self.outdir, docname + self.out_suffix)
-            try:
-                targetmtime = path.getmtime(targetname)
-            except Exception:
-                targetmtime = 0
-            try:
-                srcmtime = path.getmtime(self.env.doc2path(docname))
-                if srcmtime > targetmtime:
-                    yield docname
-            except EnvironmentError:
-                pass
-
-    def get_target_uri(self, docname: str, typ=None):
-        # Returns the target markdown file name
-        return f"{docname}.md"
+            target_name = os.path.join(self.outdir, doc_name + self.out_suffix)
+            target_mtime = get_mod_time_if_exists(target_name)
+            src_mtime = get_mod_time_if_exists(self.env.doc2path(doc_name))
+            if src_mtime > target_mtime:
+                yield doc_name
+
+    def get_target_uri(self, docname: str, typ: str = None):
+        """
+        Returns the target file name.
+        By default, we link to the currently generated markdown files.
+        But, we also support linking to external document (e.g., an html web page).
+        """
+        return f"{docname}{self.config.markdown_uri_doc_suffix}"
 
-    def prepare_writing(self, docnames):
+    def prepare_writing(self, docnames: Set[str]):
         self.writer = MarkdownWriter(self)
 
-    def write_doc(self, docname, doctree):
-        self.current_docname = docname
-        self.secnumbers = self.env.toc_secnumbers.get(docname, {})
-        destination = StringOutput(encoding='utf-8')
+    def write_doc(self, docname: str, doctree: nodes.document):
+        self.current_doc_name = docname
+        self.sec_numbers = self.env.toc_secnumbers.get(docname, {})
+        destination = StringOutput(encoding="utf-8")
         self.writer.write(doctree, destination)
-        outfilename = path.join(
-            self.outdir,
-            os_path(docname) + self.out_suffix
-        )
-        ensuredir(path.dirname(outfilename))
+        out_filename = os.path.join(self.outdir, f"{os_path(docname)}{self.out_suffix}")
+        ensuredir(os.path.dirname(out_filename))
+
         try:
-            with open(outfilename, 'w', encoding='utf-8') as f:  # type: ignore
-                f.write(self.writer.output)
+            with open(out_filename, "w", encoding="utf-8") as file:
+                file.write(self.writer.output)
         except (IOError, OSError) as err:
-            logger.warning(__('error writing file %s: %s'), outfilename, err)
-
-    def finish(self):
-        pass
+            logger.warning(__("error writing file %s: %s"), out_filename, err)
```

