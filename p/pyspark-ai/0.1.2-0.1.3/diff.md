# Comparing `tmp/pyspark_ai-0.1.2.tar.gz` & `tmp/pyspark_ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.2.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.3.tar", max compression
```

## Comparing `pyspark_ai-0.1.2.tar` & `pyspark_ai-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.2/LICENSE
--rw-r--r--   0        0        0     3735 2023-06-24 22:36:00.071711 pyspark_ai-0.1.2/README.md
--rw-r--r--   0        0        0      978 2023-06-24 22:36:23.297554 pyspark_ai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.2/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.2/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.2/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.2/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.2/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.2/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     8878 2023-06-24 17:39:22.580299 pyspark_ai-0.1.2/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    16248 2023-06-24 17:39:22.580986 pyspark_ai-0.1.2/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.2/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 pyspark_ai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3735 2023-06-24 22:36:00.071711 pyspark_ai-0.1.3/README.md
+-rw-r--r--   0        0        0      978 2023-06-25 04:09:18.391176 pyspark_ai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.3/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.3/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.3/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.3/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.3/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.3/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     8878 2023-06-24 17:39:22.580299 pyspark_ai-0.1.3/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    17498 2023-06-25 04:04:32.148887 pyspark_ai-0.1.3/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.3/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 pyspark_ai-0.1.3/PKG-INFO
```

### Comparing `pyspark_ai-0.1.2/LICENSE` & `pyspark_ai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/README.md` & `pyspark_ai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyproject.toml` & `pyspark_ai-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.2"
+version = "0.1.3"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyspark_ai-0.1.2/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.3/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/cache.py` & `pyspark_ai-0.1.3/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.3/pyspark_ai/code_logger.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.3/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.3/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/prompt.py` & `pyspark_ai-0.1.3/pyspark_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.3/pyspark_ai/pyspark_ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import contextlib
+import io
 import os
 import re
 import pandas as pd  # noqa: F401
 
 from typing import Callable, Optional, List
 from urllib.parse import urlparse
 
@@ -230,16 +232,39 @@
         pattern = r"#\d+"
 
         # Remove matching patterns
         trimmed_plan = re.sub(pattern, "", analyzed_plan)
 
         return trimmed_plan
 
+    @staticmethod
+    def _parse_explain_string(df: DataFrame) -> str:
+        """
+        Helper function to parse the content of the extended explain
+        string to extract the analyzed logical plan. As Spark does not provide
+        access to the logical plane without accessing the query execution object
+        directly, the value is extracted from the explain text representation.
+
+        :param df: The dataframe to extract the logical plan from.
+        :return: The analyzed logical plan.
+        """
+        with contextlib.redirect_stdout(io.StringIO()) as f:
+            df.explain(extended=True)
+        explain = f.getvalue()
+        splitted = explain.split("\n")
+        # The two index operations will fail if Spark changes the textual
+        # plan representation.
+        begin = splitted.index("== Analyzed Logical Plan ==")
+        end = splitted.index("== Optimized Logical Plan ==")
+        # The analyzed logical plan starts two lines after the section marker.
+        # The first line is the output schema.
+        return "\n".join(splitted[begin + 2:end])
+
     def _get_df_explain(self, df: DataFrame, cache: bool) -> str:
-        raw_analyzed_str = df._jdf.queryExecution().analyzed().toString()
+        raw_analyzed_str = self._parse_explain_string(df)
         tags = self._get_tags(cache)
         return self._explain_chain.run(
             tags=tags, input=self._trim_hash_id(raw_analyzed_str)
         )
 
     def _get_tags(self, cache: bool) -> Optional[List[str]]:
         if self._enable_cache and not cache:
@@ -273,23 +298,23 @@
             self.log(f"HTTP error occurred: {http_err}")
             return
         except Exception as err:
             self.log(f"Other error occurred: {err}")
             return
 
         soup = BeautifulSoup(response.text, "html.parser")
-        
+
         # add url and page content to cache
         if cache:
             if self._cache.lookup(key=url):
                 page_content = self._cache.lookup(key=url)
             else:
                 page_content = soup.get_text()
                 self._cache.update(key=url, val=page_content)
-        
+
         # If the input is a URL link, use the title of web page as the dataset's description.
         if is_url:
             desc = soup.title.string
         return self._create_dataframe_with_llm(
             page_content, desc, columns, cache
         )
 
@@ -393,14 +418,17 @@
         return locals_[udf_name]
 
     def activate(self):
         """
         Activates AI utility functions for Spark DataFrame.
         """
         DataFrame.ai = AIUtils(self)
+        # Patch the Spark Connect DataFrame as well.
+        from pyspark.sql.connect.dataframe import DataFrame as CDataFrame
+        CDataFrame.ai = AIUtils(self)
 
     def commit(self):
         """
         Commit the staging in-memory cache into persistent cache, if cache is enabled.
         """
         if self._cache is not None:
             self._cache.commit()
```

### Comparing `pyspark_ai-0.1.2/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.3/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.2/PKG-INFO` & `pyspark_ai-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

