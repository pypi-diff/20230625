# Comparing `tmp/datawise-0.0.21.tar.gz` & `tmp/datawise-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.21.tar", max compression
+gzip compressed data, was "datawise-0.0.22.tar", max compression
```

## Comparing `datawise-0.0.21.tar` & `datawise-0.0.22.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.21/LICENSE
--rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.21/README.md
--rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.21/datawise/__init__.py
--rw-r--r--   0        0        0      704 2023-06-25 18:46:09.256341 datawise-0.0.21/datawise/exceptions.py
--rw-r--r--   0        0        0      589 2023-06-25 18:50:43.652759 datawise-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.22/LICENSE
+-rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.22/README.md
+-rw-r--r--   0        0        0     8384 2023-06-25 19:37:03.295583 datawise-0.0.22/datawise/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-25 18:46:09.256341 datawise-0.0.22/datawise/exceptions.py
+-rw-r--r--   0        0        0      589 2023-06-25 19:40:35.826780 datawise-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.22/PKG-INFO
```

### Comparing `datawise-0.0.21/LICENSE` & `datawise-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.21/README.md` & `datawise-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `datawise-0.0.21/datawise/__init__.py` & `datawise-0.0.22/datawise/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,15 +34,14 @@
       Example:
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to transformed dataframes or not.
     """
     return self._sql(query, dataframes, code=code)
 
-
   @retry(exceptions=(RequestException, DataWiseInternalError), tries=3, delay=2)
   def _sql(self, query, dataframes, error=None, code=False, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
     if num_retries >= 2:
       logging.error(f"We couldn't translate your query. Here is python code we attempted to generate: \n{prev_code}")
       raise TranslationError()
 
@@ -82,15 +81,85 @@
         return_df = self._sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
     except Exception as e:
       num_retries += 1
       data["error"] = f"Threw exception: `{e}`"
       return_df = self._sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
     
     return return_df
+
+
+
+  def transform(self, prompt, dataframes, code=False):
+    """
+    Transforms given dataframes based on based on given prompt.
+
+    Parameters:
+    -----------
+    prompt: str
+      Prompt to be used for transformation.
+    dataframes: Pandas dataframes
+      Dictionary of dataframes to be transformed.
+      The key is the dataframe name and the value is the dataframe itself.
+      Example:
+      {"customers_df": customers_df, "employees_df": employees_df}
+    Code: bool
+      Whether to print/log the pandas code used to generate visualization or not.
+    """
+    return self._transform(prompt, dataframes, code=code)
   
+  @retry(exceptions=(RequestException, DataWiseInternalError), tries=3, delay=2)
+  def _transform(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
+    if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
+
+    if num_retries >= 2:
+      logging.error(f"We couldn't translate your prompt. Here is python code we attempted to generate: \n{prev_code}")
+      raise TranslationError()
+    
+    data = {
+      "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns={value.columns.tolist()} {'and index=[' + value.index.name + ']' if value.index.name else ''}." for idx, (key, value) in enumerate(dataframes.items())]),
+      "nl": prompt,
+      "error": error
+    }
+
+    response = requests.post(
+      self.api_base + "/nl2pandas", 
+      data=json.dumps(data), 
+      headers={
+        "Authorization": "Bearer " + self.api_key,
+        "content-type": "application/json"
+      }
+    )
+
+    if (response.status_code == 400): raise BadRequestError(response.text)
+    if (response.status_code == 401): raise AuthorizationError()
+    if (response.status_code >= 500): raise DataWiseInternalError()
+
+    python_code = response.json()
+
+    import pandas as pd
+    import numpy as np
+    globals = { "np": np, "pd": pd }
+    locals = dataframes.copy()
+    try:
+      exec(python_code, globals, locals)
+      if isinstance(locals["return_df"], pd.DataFrame):
+        return_df=locals["return_df"].reset_index(drop=True)
+        if code: logging.info(f"Given prompt: \n{prompt} \nOutput code: \n{python_code}\n")
+      else:
+        num_retries += 1
+        data["error"] = "Is not a pandas dataframe. Please return dataframe."
+        return_df = self._transform(prompt, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
+    except Exception as e:
+      num_retries += 1
+      data["error"] = f"Threw exception: `{e}`"
+      return_df = self._transform(prompt, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
+    
+    return return_df
+
+
   def viz(self, prompt, dataframes, code=False):
     """
     Creates visualization based on given prompt.
 
     Parameters:
     -----------
     prompt: str
```

### Comparing `datawise-0.0.21/datawise/exceptions.py` & `datawise-0.0.22/datawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.21/pyproject.toml` & `datawise-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.21"
+version = "0.0.22"
 description = "AI Assistant for Python Data Analytics"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.21/PKG-INFO` & `datawise-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.21
+Version: 0.0.22
 Summary: AI Assistant for Python Data Analytics
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

