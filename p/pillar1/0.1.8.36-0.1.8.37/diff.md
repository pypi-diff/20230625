# Comparing `tmp/pillar1-0.1.8.36.tar.gz` & `tmp/pillar1-0.1.8.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.36.tar", last modified: Sun Jun 25 01:07:47 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.37.tar", last modified: Sun Jun 25 01:22:00 2023, max compression
```

## Comparing `pillar1-0.1.8.36.tar` & `pillar1-0.1.8.37.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:07:47.071779 pillar1-0.1.8.36/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:07:47.071643 pillar1-0.1.8.36/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.36/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:07:47.070904 pillar1-0.1.8.36/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.36/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.36/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.36/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5507 2023-06-25 01:07:44.000000 pillar1-0.1.8.36/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:07:47.071446 pillar1-0.1.8.36/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:07:47.000000 pillar1-0.1.8.36/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:07:47.000000 pillar1-0.1.8.36/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:07:47.000000 pillar1-0.1.8.36/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:07:47.000000 pillar1-0.1.8.36/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:07:47.071827 pillar1-0.1.8.36/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:07:46.000000 pillar1-0.1.8.36/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:22:00.043361 pillar1-0.1.8.37/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:22:00.043197 pillar1-0.1.8.37/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.37/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:22:00.042480 pillar1-0.1.8.37/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.37/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.37/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.37/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     5530 2023-06-25 01:21:54.000000 pillar1-0.1.8.37/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:22:00.042989 pillar1-0.1.8.37/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:21:59.000000 pillar1-0.1.8.37/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:22:00.000000 pillar1-0.1.8.37/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:21:59.000000 pillar1-0.1.8.37/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:21:59.000000 pillar1-0.1.8.37/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:22:00.043409 pillar1-0.1.8.37/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:21:59.000000 pillar1-0.1.8.37/setup.py
```

### Comparing `pillar1-0.1.8.36/PKG-INFO` & `pillar1-0.1.8.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.36
+Version: 0.1.8.37
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.36/README.md` & `pillar1-0.1.8.37/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.36/pillar1/constants.py` & `pillar1-0.1.8.37/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.36/pillar1/constants_original.py` & `pillar1-0.1.8.37/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.36/pillar1/pillar1.py` & `pillar1-0.1.8.37/pillar1/pillar1.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,53 +9,54 @@
     STARCODERPLUS = 'starcoderplus'
     STARCHAT_BETA = 'starchat-beta'
     FALCON_40B_INSTRUCT = 'f40b-instruct'
 
 
 MODELS_META = {
     'f40b-instruct': {
-        'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoderplus': {
         'free': {
-            'context': cn.STARCODER_BETA,
             'prepend': 'Given this `claims` table description:',
             'append': '',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', }
         }
     },
     'starchat-beta': {
         'free': {
-            'context': cn.STARCODER_BETA,
             'prepend': '<|user|>Given this `claims` table description:',
             'append': '<|end|>',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/HuggingFaceH4/starchat-beta',
             'replaces': {'': '', }
         }
     }
 }
 
 
 class Model:
     def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 100, verbose: bool = False, api_type: str = 'free',
-                 huggingface_token=''):
+                 huggingface_token='', background: str = ''):
         self.end_point = end_point
         self.prompt = None
         self.result = None
         self.huggingface_token = huggingface_token
         self.cleaned_code = ''
         self.response = None
         self.max_new_tokens = max_new_tokens
         self.verbose = verbose
         self.curr_model = MODELS_META[end_point][api_type]
         self.api_type = api_type
+        if not background:
+            self.background = cn.STARCODER_BETA
+        else:
+            self.background = background
 
         if self.api_type == 'hosted':
             self.client = boto3.client(
                 'sagemaker-runtime',
                 aws_access_key_id=user_name,
                 aws_secret_access_key=password,
                 region_name='us-west-2'
@@ -109,21 +110,21 @@
 
             if self.api_type == 'free':
                 response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
                 self.response = response.json()[0]['generated_text']
                 return self.response
 
         if prompt:
-            prompt = f"{self.curr_model['prepend']}{self.curr_model['context']}The DataBricks-compatible SQL code that will {prompt}{self.curr_model['append']}"
+            prompt = f"{self.curr_model['prepend']}{self.background}The DataBricks-compatible SQL code that will {prompt}{self.curr_model['append']}"
             self.prompt = prompt
             submit_request(self.prompt)
 
         else:
             question = input('What SQL are you looking for: ')
-            prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nAnswer this question: {question}\" {self.curr_model['append']}"
+            prompt = f"{self.curr_model['prepend']}:\n\"{self.background}\"\n\nAnswer this question: {question}\" {self.curr_model['append']}"
             self.prompt = prompt
             submit_request(self.prompt)
 
             # input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             # button = widgets.Button(description='Submit')
             # # display(textarea_bg)
             # display(input_text)
```

### Comparing `pillar1-0.1.8.36/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.37/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.36
+Version: 0.1.8.37
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.36/setup.py` & `pillar1-0.1.8.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.36',
+    version='0.1.8.37',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

