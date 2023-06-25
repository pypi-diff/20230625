# Comparing `tmp/pandasai-0.6.3.tar.gz` & `tmp/pandasai-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.3.tar", max compression
+gzip compressed data, was "pandasai-0.6.4.tar", max compression
```

## Comparing `pandasai-0.6.3.tar` & `pandasai-0.6.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-23 13:57:34.498989 pandasai-0.6.3/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-23 13:57:34.498989 pandasai-0.6.3/README.md
--rw-r--r--   0        0        0    24332 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     4369 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4119 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-23 13:57:34.510990 pandasai-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-25 17:11:19.104006 pandasai-0.6.4/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-25 17:11:19.104006 pandasai-0.6.4/README.md
+-rw-r--r--   0        0        0    24578 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4119 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10606 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1712 2023-06-25 17:11:19.116006 pandasai-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.4/PKG-INFO
```

### Comparing `pandasai-0.6.3/LICENSE` & `pandasai-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/README.md` & `pandasai-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/__init__.py` & `pandasai-0.6.4/pandasai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,26 @@
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 
+def get_version():
+    """
+    Get the version from the package metadata
+    """
+    from importlib.metadata import version
+
+    return version("pandasai")
+
+
+__version__ = get_version()
+
+
 class PandasAI(Shortcuts):
     """
     PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
     This is an entry point of `pandasai` object. This class consists of methods
     to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
@@ -330,14 +342,15 @@
                         "df_head": heads,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
+                    df_head = df_head.to_csv(index=False)
 
                     generate_code_instruction = self._non_default_prompts.get(
                         "generate_python_code", GeneratePythonCodePrompt
                     )(
                         prompt=prompt,
                         df_head=df_head,
                         num_rows=data_frame.shape[0],
```

### Comparing `pandasai-0.6.3/pandasai/constants.py` & `pandasai-0.6.4/pandasai/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-"""
-Constants used in the pandasai package.
-
-It includes Start & End Code tags, Whitelisted Python Packages and
-While List Builtin Methods.
-
-"""
-
-START_CODE_TAG = "<startCode>"
-END_CODE_TAG = "<endCode>"
-
 # List of Python builtin libraries that are added to the environment by default.
 WHITELISTED_BUILTINS = [
     "abs",
     "all",
     "any",
     "ascii",
     "bin",
```

### Comparing `pandasai-0.6.3/pandasai/exceptions.py` & `pandasai-0.6.4/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/_optional.py` & `pandasai-0.6.4/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/anonymizer.py` & `pandasai-0.6.4/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/cache.py` & `pandasai-0.6.4/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/from_excel.py` & `pandasai-0.6.4/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/notebook.py` & `pandasai-0.6.4/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/helpers/save_chart.py` & `pandasai-0.6.4/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/azure_openai.py` & `pandasai-0.6.4/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/base.py` & `pandasai-0.6.4/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
 import openai
 import requests
 
-from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 from ..helpers._optional import import_dependency
 from ..prompts.base import Prompt
@@ -103,21 +102,14 @@
         Raises:
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
         """
         code = response
-        match = re.search(
-            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
-            code,
-            re.DOTALL,
-        )
-        if match:
-            code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
```

### Comparing `pandasai-0.6.3/pandasai/llm/fake.py` & `pandasai-0.6.4/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/falcon.py` & `pandasai-0.6.4/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/google_palm.py` & `pandasai-0.6.4/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/langchain.py` & `pandasai-0.6.4/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/open_assistant.py` & `pandasai-0.6.4/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/openai.py` & `pandasai-0.6.4/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/llm/starcoder.py` & `pandasai-0.6.4/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/middlewares/base.py` & `pandasai-0.6.4/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/middlewares/charts.py` & `pandasai-0.6.4/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/middlewares/streamlit.py` & `pandasai-0.6.4/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/prompts/base.py` & `pandasai-0.6.4/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.3/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.4/pandasai/prompts/correct_error_prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,22 +11,19 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above
-mentioned error. Do not generate the same code again. Make sure to prefix the requested python
-code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
+mentioned error. Do not generate the same code again.
 ```
 """  # noqa: E501
 from datetime import date
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
 
     text: str = """
@@ -41,17 +38,11 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 """  # noqa: E501
 
     def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
-            today_date=date.today()
-        )
+        super().__init__(**kwargs, today_date=date.today())
```

### Comparing `pandasai-0.6.3/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.4/pandasai/prompts/correct_multiples_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """ Prompt to correct error """
 
 import pandas as pd
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class CorrectMultipleDataframesErrorPrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
@@ -34,14 +32,13 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 """  # noqa: E501
 
         self.text += instruction
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.6.3/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.4/pandasai/prompts/generate_python_code.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,40 +2,31 @@
 ```
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the
-dataframe `df`. Using the provided dataframe, df, return the python code and make sure to prefix
-the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG}
-exactly to get the answer to the following question:
+dataframe `df`. Using the provided dataframe, df, return the python code to get the answer to the following question:
 ```
 """  # noqa: E501
 
 from datetime import date
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class GeneratePythonCodePrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the dataframe `df`.
-Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
+Using the provided dataframe, df, return the python code to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
-            today_date=date.today()
-        )
+        super().__init__(**kwargs, today_date=date.today())
```

### Comparing `pandasai-0.6.3/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.4/pandasai/prompts/multiple_dataframes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """ Prompt to generate Python code for multiple dataframes """
 
 from datetime import date
 
 import pandas as pd
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class MultipleDataframesPrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
-Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
+Using the provided dataframes and no other dataframes, return the python code to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
         )
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.6.3/pyproject.toml` & `pandasai-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.3"
+version = "0.6.4"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.3/PKG-INFO` & `pandasai-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

