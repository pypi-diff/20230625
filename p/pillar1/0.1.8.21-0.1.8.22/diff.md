# Comparing `tmp/pillar1-0.1.8.21.tar.gz` & `tmp/pillar1-0.1.8.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.21.tar", last modified: Sat Jun 24 23:25:31 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.22.tar", last modified: Sat Jun 24 23:46:13 2023, max compression
```

## Comparing `pillar1-0.1.8.21.tar` & `pillar1-0.1.8.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.818911 pillar1-0.1.8.21/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:25:31.818763 pillar1-0.1.8.21/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.21/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.817188 pillar1-0.1.8.21/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.21/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.21/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.21/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     4621 2023-06-24 23:25:19.000000 pillar1-0.1.8.21/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:25:31.818560 pillar1-0.1.8.21/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-24 23:25:31.818957 pillar1-0.1.8.21/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-24 23:25:31.000000 pillar1-0.1.8.21/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:46:13.081771 pillar1-0.1.8.22/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:46:13.081643 pillar1-0.1.8.22/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.22/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:46:13.080945 pillar1-0.1.8.22/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.22/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.22/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.22/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4857 2023-06-24 23:46:09.000000 pillar1-0.1.8.22/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-24 23:46:13.081462 pillar1-0.1.8.22/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-24 23:46:13.000000 pillar1-0.1.8.22/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-24 23:46:13.000000 pillar1-0.1.8.22/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-24 23:46:13.000000 pillar1-0.1.8.22/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-24 23:46:13.000000 pillar1-0.1.8.22/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-24 23:46:13.081813 pillar1-0.1.8.22/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-24 23:46:12.000000 pillar1-0.1.8.22/setup.py
```

### Comparing `pillar1-0.1.8.21/PKG-INFO` & `pillar1-0.1.8.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.21
+Version: 0.1.8.22
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.21/README.md` & `pillar1-0.1.8.22/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.21/pillar1/constants.py` & `pillar1-0.1.8.22/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.21/pillar1/constants_original.py` & `pillar1-0.1.8.22/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.21/pillar1/pillar1.py` & `pillar1-0.1.8.22/pillar1/pillar1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 import json
 import boto3
 from pyspark.sql import SparkSession
 import pillar1.constants as cn
+import requests
 
 
 class MODELS:
     STARCHAT_BETA = 'starchat-beta'
     FALCON_40B_INSTRUCT = 'f40b-instruct'
 
 
 MODELS_META = {
     'f40b-instruct': {
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starchat-beta': {
-        'context': cn.STARCODER_BETA,
-        'prepend': '<|user|>Given this `claim_item` table description:',
-        'append': '(only return DataBricks-compatible SQL code)<|end|>',
-        'stop_token': '<|end|>',
-        'replaces': {'': '', }
-    },
-    'starcoder-alpha': {
-        'context': cn.STARCODER_BETA,
-        'prepend': '<|user|>Given this `claim_item` table description:',
-        'append': '(only return DataBricks-compatible SQL code)<|end|>',
-        'stop_token': '<|end|>',
-        'replaces': {'': '', }
+        'free': {
+            'context': cn.STARCODER_BETA,
+            'prepend': '<|user|>Given this `claim_item` table description:',
+            'append': '(only return DataBricks-compatible SQL code)<|end|>',
+            'stop_token': '<|end|>',
+            'API_URL': '',
+            'replaces': {'': '', }
+        }
     }
 }
 
 
 class Model:
-    def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 100, verbose: bool = False):
+    def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 100, verbose: bool = False, api_type: str = 'free',
+                 huggingface_token=''):
         self.end_point = end_point
         self.prompt = None
         self.result = None
+        self.huggingface_token = huggingface_token
         self.cleaned_code = ''
         self.response = None
         self.max_new_tokens = max_new_tokens
         self.verbose = verbose
+        self.curr_model = MODELS_META[end_point][api_type]
+        self.api_type = api_type
 
-        self.client = boto3.client(
-            'sagemaker-runtime',
-            aws_access_key_id=user_name,
-            aws_secret_access_key=password,
-            region_name='us-west-2'
-        )
+        if self.api_type == 'hosted':
+            self.client = boto3.client(
+                'sagemaker-runtime',
+                aws_access_key_id=user_name,
+                aws_secret_access_key=password,
+                region_name='us-west-2'
+            )
 
     def code(self):
         self.cleaned_code = self.response.replace(self.prompt, '').strip()
         ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
         for curr_el_to_remove in ELS_TO_REMOVE:
             self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
 
         # self.cleaned_code = self.cleaned_code.split('<|assistant|>')[1].split('<|end|>')[0].strip().replace(' claim_item;', ' uc_beesbridge.abacus.claim_item;').replace(
         #    ' claim_item ',
         #    ' uc_beesbridge.abacus.claim_item ').replace(
         #    ' claim_item\n', ' uc_beesbridge.abacus.claim_item\n')
+
         self.cleaned_code = self.cleaned_code.strip()
         print(self.cleaned_code)
 
     def execute(self):
         spark = SparkSession.builder.getOrCreate()
         self.result = spark.sql(self.cleaned_code)
         return self.result
@@ -73,38 +76,41 @@
                 "parameters": {
                     "do_sample": True,
                     "top_p": 0.7,
                     "temperature": 0.7,
                     "top_k": 50,
                     "max_new_tokens": self.max_new_tokens,
                     "repetition_penalty": 1.03,
-                    "stop": [MODELS_META[self.end_point].get('stop_token')]
+                    "stop": [self.curr_model['stop_token']]
                 }
             }
 
             if self.verbose:
                 print(f"Submit payload: {payload}")
 
-            response = self.client.invoke_endpoint(
-                EndpointName=self.end_point,
-                ContentType='application/json',
-                Body=json.dumps(payload)
-            )
+            if self.api_type == "hosted":
+                response = self.client.invoke_endpoint(
+                    EndpointName=self.end_point,
+                    ContentType='application/json',
+                    Body=json.dumps(payload)
+                )
+
+            if self.api_type == 'free':
+                response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
+                return response.json()
 
             self.response = json.loads(response['Body'].read())[0]['generated_text']
             self.code()
 
         if prompt:
             self.prompt = prompt
             submit_request(self.prompt)
         else:
             question = input('What SQL are you looking for: ')
-            prompt = f"{MODELS_META[self.end_point].get('prepend', '')}:" \
-                     f"\n\"{MODELS_META[self.end_point].get('context', '')}\"\n\nAnswer this question: " \
-                     f"\"{question}\" {MODELS_META[self.end_point].get('append', '')}"
+            prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nAnswer this question: {question}\" {self.curr_model['append']}"
             self.prompt = prompt
             submit_request(self.prompt)
 
             # input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             # button = widgets.Button(description='Submit')
             # # display(textarea_bg)
             # display(input_text)
```

### Comparing `pillar1-0.1.8.21/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.22/pillar1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.21
+Version: 0.1.8.22
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.21/setup.py` & `pillar1-0.1.8.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.21',
+    version='0.1.8.22',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

