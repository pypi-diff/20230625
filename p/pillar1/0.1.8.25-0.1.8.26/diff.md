# Comparing `tmp/pillar1-0.1.8.25.tar.gz` & `tmp/pillar1-0.1.8.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.25.tar", last modified: Sun Jun 25 00:21:36 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.26.tar", last modified: Sun Jun 25 00:23:44 2023, max compression
```

## Comparing `pillar1-0.1.8.25.tar` & `pillar1-0.1.8.26.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:21:36.792926 pillar1-0.1.8.25/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:21:36.792793 pillar1-0.1.8.25/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.25/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:21:36.792125 pillar1-0.1.8.25/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.25/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.25/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.25/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     4968 2023-06-25 00:21:34.000000 pillar1-0.1.8.25/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:21:36.792617 pillar1-0.1.8.25/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:21:36.000000 pillar1-0.1.8.25/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:21:36.000000 pillar1-0.1.8.25/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:21:36.000000 pillar1-0.1.8.25/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:21:36.000000 pillar1-0.1.8.25/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:21:36.792966 pillar1-0.1.8.25/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:21:36.000000 pillar1-0.1.8.25/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:23:44.787915 pillar1-0.1.8.26/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:23:44.787773 pillar1-0.1.8.26/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.26/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:23:44.786937 pillar1-0.1.8.26/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.26/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2249 2023-06-23 19:09:33.000000 pillar1-0.1.8.26/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.26/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4996 2023-06-25 00:23:33.000000 pillar1-0.1.8.26/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 00:23:44.787553 pillar1-0.1.8.26/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 00:23:44.000000 pillar1-0.1.8.26/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 00:23:44.000000 pillar1-0.1.8.26/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 00:23:44.000000 pillar1-0.1.8.26/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 00:23:44.000000 pillar1-0.1.8.26/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 00:23:44.787957 pillar1-0.1.8.26/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 00:23:44.000000 pillar1-0.1.8.26/setup.py
```

### Comparing `pillar1-0.1.8.25/PKG-INFO` & `pillar1-0.1.8.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.25
+Version: 0.1.8.26
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.25/README.md` & `pillar1-0.1.8.26/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.25/pillar1/constants.py` & `pillar1-0.1.8.26/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.25/pillar1/constants_original.py` & `pillar1-0.1.8.26/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.25/pillar1/pillar1.py` & `pillar1-0.1.8.26/pillar1/pillar1.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,23 +89,22 @@
 
             if self.api_type == "hosted":
                 response = self.client.invoke_endpoint(
                     EndpointName=self.end_point,
                     ContentType='application/json',
                     Body=json.dumps(payload)
                 )
+                self.response = json.loads(response['Body'].read())[0]['generated_text']
+                self.code()
 
             if self.api_type == 'free':
                 response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
-                self.response = response.json()
+                self.response = response.json()[0]['generated_text']
                 return self.response
 
-            self.response = json.loads(response['Body'].read())[0]['generated_text']
-            self.code()
-
         if prompt:
             self.prompt = prompt
             submit_request(self.prompt)
         else:
             question = input('What SQL are you looking for: ')
             prompt = f"{self.curr_model['prepend']}:\n\"{self.curr_model['context']}\"\n\nAnswer this question: {question}\" {self.curr_model['append']}"
             self.prompt = prompt
```

### Comparing `pillar1-0.1.8.25/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.26/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.25
+Version: 0.1.8.26
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.25/setup.py` & `pillar1-0.1.8.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.25',
+    version='0.1.8.26',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

