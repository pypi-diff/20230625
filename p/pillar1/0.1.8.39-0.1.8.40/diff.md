# Comparing `tmp/pillar1-0.1.8.39.tar.gz` & `tmp/pillar1-0.1.8.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.39.tar", last modified: Sun Jun 25 01:41:08 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.40.tar", last modified: Sun Jun 25 02:13:48 2023, max compression
```

## Comparing `pillar1-0.1.8.39.tar` & `pillar1-0.1.8.40.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.594061 pillar1-0.1.8.39/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:41:08.593919 pillar1-0.1.8.39/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.39/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.593160 pillar1-0.1.8.39/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.39/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.39/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.39/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6168 2023-06-25 01:41:00.000000 pillar1-0.1.8.39/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 01:41:08.593719 pillar1-0.1.8.39/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 01:41:08.594103 pillar1-0.1.8.39/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 01:41:08.000000 pillar1-0.1.8.39/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.114672 pillar1-0.1.8.40/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:13:48.114534 pillar1-0.1.8.40/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.40/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.113615 pillar1-0.1.8.40/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.40/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      805 2023-06-25 01:03:17.000000 pillar1-0.1.8.40/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.40/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6500 2023-06-25 01:55:56.000000 pillar1-0.1.8.40/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 02:13:48.114338 pillar1-0.1.8.40/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 02:13:48.000000 pillar1-0.1.8.40/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 02:13:48.114719 pillar1-0.1.8.40/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 02:13:47.000000 pillar1-0.1.8.40/setup.py
```

### Comparing `pillar1-0.1.8.39/PKG-INFO` & `pillar1-0.1.8.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.39
+Version: 0.1.8.40
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.39/README.md` & `pillar1-0.1.8.40/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.39/pillar1/constants.py` & `pillar1-0.1.8.40/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.39/pillar1/constants_original.py` & `pillar1-0.1.8.40/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.39/pillar1/pillar1.py` & `pillar1-0.1.8.40/pillar1/pillar1.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,22 @@
             'prepend': 'Given this `claims` table description:',
             'append': '',
             'stop_token': '<|end|>',
             'API_URL': 'https://api-inference.huggingface.co/models/bigcode/starcoderplus',
             'replaces': {'': '', },
             'placeholder_beg': {'pattern': '```sql', 'index': 1},
             'placeholder_end': {'pattern': '```', 'index': 0}
+        },
+        'hosted': {
+            'prepend': 'Given this `claims` table description:',
+            'append': '',
+            'stop_token': '<|end|>',
+            'replaces': {'': '', },
+            'placeholder_beg': {'pattern': '```sql', 'index': 1},
+            'placeholder_end': {'pattern': '```', 'index': 0}
         }
     },
     'starchat-beta': {
         'free': {
             'prepend': '<|user|>Given this `claims` table description:',
             'append': '<|end|>',
             'stop_token': '<|end|>',
@@ -114,15 +122,15 @@
             if self.api_type == "hosted":
                 response = self.client.invoke_endpoint(
                     EndpointName=self.end_point,
                     ContentType='application/json',
                     Body=json.dumps(payload)
                 )
                 self.response = json.loads(response['Body'].read())[0]['generated_text']
-                self.code()
+                return self.response
 
             if self.api_type == 'free':
                 response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
                 self.response = response.json()[0]['generated_text']
                 return self.response
 
         if prompt:
```

### Comparing `pillar1-0.1.8.39/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.40/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.39
+Version: 0.1.8.40
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.39/setup.py` & `pillar1-0.1.8.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.39',
+    version='0.1.8.40',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

