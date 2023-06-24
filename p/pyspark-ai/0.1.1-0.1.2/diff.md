# Comparing `tmp/pyspark_ai-0.1.1.tar.gz` & `tmp/pyspark_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.1.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.2.tar", max compression
```

## Comparing `pyspark_ai-0.1.1.tar` & `pyspark_ai-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.1/LICENSE
--rw-r--r--   0        0        0     3397 2023-06-23 22:14:14.463218 pyspark_ai-0.1.1/README.md
--rw-r--r--   0        0        0      978 2023-06-23 23:50:06.264450 pyspark_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.1/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.1/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.1/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.1/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.1/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.1/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     8879 2023-06-23 22:14:14.485908 pyspark_ai-0.1.1/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    15941 2023-06-23 23:49:27.968706 pyspark_ai-0.1.1/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.1/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 pyspark_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3735 2023-06-24 22:36:00.071711 pyspark_ai-0.1.2/README.md
+-rw-r--r--   0        0        0      978 2023-06-24 22:36:23.297554 pyspark_ai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.2/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.2/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.2/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.2/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.2/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.2/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     8878 2023-06-24 17:39:22.580299 pyspark_ai-0.1.2/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    16248 2023-06-24 17:39:22.580986 pyspark_ai-0.1.2/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.2/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 pyspark_ai-0.1.2/PKG-INFO
```

### Comparing `pyspark_ai-0.1.1/LICENSE` & `pyspark_ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/README.md` & `pyspark_ai-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,25 @@
 from pyspark_ai import SparkAI
 
 spark_ai = SparkAI()
 spark_ai.activate()  # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
+If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
+```
+Otherwise, you can ingest data via URL:
+```python
+auto_df = spark_ai.create_df("https://www.carpro.com/blog/full-year-2022-national-auto-sales-by-brand")
+```
+
+Take a look at the data:
+```python
 auto_df.show(n=5)
 ```
 | rank | brand     | us_sales_2022 | sales_change_vs_2021 |
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
@@ -46,15 +55,15 @@
 To plot with an instruction:
 ```python
 auto_df.ai.plot("pie chart for US sales market shares, show the top 5 brands and the sum of others")
 ```
 ![2022 USA national auto sales_market_share by brand](docs/_static/auto_sales_pie_char.png)
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=auto_df.ai.transform("top brand with the highest growth")
+auto_top_growth_df=auto_df.ai.transform("brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
 ### DataFrame Explanation
```

### Comparing `pyspark_ai-0.1.1/pyproject.toml` & `pyspark_ai-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.1"
+version = "0.1.2"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -21,18 +21,18 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 requests = "^2.31.0"
 tiktoken = "0.4.0"
 beautifulsoup4 = "^4.12.2"
-pyspark = "^3.4.0"
 openai = "^0.27.8"
 langchain = "^0.0.201"
 pandas = "^2.0.2"
 pygments = "^2.15.1"
 google-api-python-client = "^2.90.0"
 chispa = "^0.9.2"
 
 
 [tool.poetry.dev-dependencies]
+pyspark = "^3.4.0"
```

### Comparing `pyspark_ai-0.1.1/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.2/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/pyspark_ai/cache.py` & `pyspark_ai-0.1.2/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.2/pyspark_ai/code_logger.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.2/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.2/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/pyspark_ai/prompt.py` & `pyspark_ai-0.1.2/pyspark_ai/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,17 +122,18 @@
 
 The output columns of `df`:
 {columns}
 
 And an explanation of `df`: {explain}
 
 Write python code to visualize the result of `df` using plotly.
-Your code should NOT include the method 'append'. 
+Your code must NOT include the method 'append'. 
 There is no need to install any package with pip. 
 Display the plot directly, instead of saving into an HTML.
+
 Ensure that your code is correct.
 {instruction}
 """
 
 PLOT_PROMPT = PromptTemplate(
     input_variables=["columns", "explain", "instruction"], template=PLOT_PROMPT_TEMPLATE
 )
```

### Comparing `pyspark_ai-0.1.1/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.2/pyspark_ai/pyspark_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,19 +273,28 @@
             self.log(f"HTTP error occurred: {http_err}")
             return
         except Exception as err:
             self.log(f"Other error occurred: {err}")
             return
 
         soup = BeautifulSoup(response.text, "html.parser")
+        
+        # add url and page content to cache
+        if cache:
+            if self._cache.lookup(key=url):
+                page_content = self._cache.lookup(key=url)
+            else:
+                page_content = soup.get_text()
+                self._cache.update(key=url, val=page_content)
+        
         # If the input is a URL link, use the title of web page as the dataset's description.
         if is_url:
             desc = soup.title.string
         return self._create_dataframe_with_llm(
-            soup.get_text(), desc, columns, cache
+            page_content, desc, columns, cache
         )
 
     def transform_df(
         self, df: DataFrame, desc: str, cache: bool = True
     ) -> DataFrame:
         """
         This method applies a transformation to a provided Spark DataFrame, the specifics of which are determined by the 'desc' parameter.
```

### Comparing `pyspark_ai-0.1.1/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.2/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.1/PKG-INFO` & `pyspark_ai-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: chispa (>=0.9.2,<0.10.0)
 Requires-Dist: google-api-python-client (>=2.90.0,<3.0.0)
 Requires-Dist: langchain (>=0.0.201,<0.0.202)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
-Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (==0.4.0)
 Description-Content-Type: text/markdown
 
 # English SDK for Apache Spark
 
 <div align="center">
@@ -53,16 +49,25 @@
 from pyspark_ai import SparkAI
 
 spark_ai = SparkAI()
 spark_ai.activate()  # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
+If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
+```
+Otherwise, you can ingest data via URL:
+```python
+auto_df = spark_ai.create_df("https://www.carpro.com/blog/full-year-2022-national-auto-sales-by-brand")
+```
+
+Take a look at the data:
+```python
 auto_df.show(n=5)
 ```
 | rank | brand     | us_sales_2022 | sales_change_vs_2021 |
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
@@ -78,15 +83,15 @@
 To plot with an instruction:
 ```python
 auto_df.ai.plot("pie chart for US sales market shares, show the top 5 brands and the sum of others")
 ```
 ![2022 USA national auto sales_market_share by brand](docs/_static/auto_sales_pie_char.png)
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=auto_df.ai.transform("top brand with the highest growth")
+auto_top_growth_df=auto_df.ai.transform("brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
 ### DataFrame Explanation
```

