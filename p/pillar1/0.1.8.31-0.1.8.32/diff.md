# Comparing `tmp/pillar1-0.1.8.31.tar.gz` & `tmp/pillar1-0.1.8.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.31.tar", last modified: Sun Jun 25 00:43:50 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.32.tar", last modified: Sun Jun 25 00:57:27 2023, max compression
```

## Comparing `pillar1-0.1.8.31.tar` & `pillar1-0.1.8.32.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:43:50.594510 pillar1-0.1.8.31/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:43:50.594361 pillar1-0.1.8.31/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.31/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:43:50.593647 pillar1-0.1.8.31/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.31/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      815 2023-06-25 00:35:52.000000 pillar1-0.1.8.31/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.31/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     5615 2023-06-25 00:43:48.000000 pillar1-0.1.8.31/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:43:50.594168 pillar1-0.1.8.31/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:43:50.000000 pillar1-0.1.8.31/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:43:50.000000 pillar1-0.1.8.31/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:43:50.000000 pillar1-0.1.8.31/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:43:50.000000 pillar1-0.1.8.31/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:43:50.594565 pillar1-0.1.8.31/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:43:50.000000 pillar1-0.1.8.31/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:57:27.980339 pillar1-0.1.8.32/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:57:27.980210 pillar1-0.1.8.32/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.32/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:57:27.979477 pillar1-0.1.8.32/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.32/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      804 2023-06-25 00:55:55.000000 pillar1-0.1.8.32/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.32/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     5633 2023-06-25 00:57:23.000000 pillar1-0.1.8.32/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:57:27.980010 pillar1-0.1.8.32/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:57:27.000000 pillar1-0.1.8.32/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:57:27.000000 pillar1-0.1.8.32/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:57:27.000000 pillar1-0.1.8.32/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:57:27.000000 pillar1-0.1.8.32/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:57:27.980378 pillar1-0.1.8.32/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:57:27.000000 pillar1-0.1.8.32/setup.py
```

### Comparing `pillar1-0.1.8.31/PKG-INFO` & `pillar1-0.1.8.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.31
+Version: 0.1.8.32
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.31/README.md` & `pillar1-0.1.8.32/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.31/pillar1/constants.py` & `pillar1-0.1.8.32/pillar1/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,13 +26,10 @@
 PatientFirstName,string,
 PatientLastName,string,
 PatientGender,string,
 PatientDateOfBirth,date,
 PatientAddress,string,
 PatientState,string,
 PatientZIP,int,
-PatientID,string,
-
+PatientID,string.
 """
-STARCODER_BETA += """
- When answering the request use the information listed above only, do not make up column names and do not place additional conditions
-    """
+STARCODER_BETA += " When answering the request use the information listed above only, do not make up column names and do not place additional conditions"
```

### Comparing `pillar1-0.1.8.31/pillar1/constants_original.py` & `pillar1-0.1.8.32/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.31/pillar1/pillar1.py` & `pillar1-0.1.8.32/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'f40b-instruct': {
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoderplus': {
         'free': {
             'context': cn.STARCODER_BETA,
-            'prepend': '<|user|>Given this `claim_item` table description:',
+            'prepend': '<|user|>Given this `claims` table description:',
             'append': '(only return DataBricks-compatible SQL code)<|end|>',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', }
         }
     },
     'starchat-beta': {
@@ -109,15 +109,15 @@
 
             if self.api_type == 'free':
                 response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
                 self.response = response.json()[0]['generated_text']
                 return self.response
 
         if prompt:
-            prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nGive me the SQL code that will: {prompt}\" {self.curr_model['append']}"
+            prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nGive me the DataBricks-compatible SQL code that will: {prompt}\" {self.curr_model['append']}"
             self.prompt = prompt
             submit_request(self.prompt)
 
         else:
             question = input('What SQL are you looking for: ')
             prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nAnswer this question: {question}\" {self.curr_model['append']}"
             self.prompt = prompt
```

### Comparing `pillar1-0.1.8.31/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.32/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.31
+Version: 0.1.8.32
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.31/setup.py` & `pillar1-0.1.8.32/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.31',
+    version='0.1.8.32',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

