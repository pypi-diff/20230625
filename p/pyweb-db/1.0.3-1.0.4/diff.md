# Comparing `tmp/pyweb_db-1.0.3.tar.gz` & `tmp/pyweb_db-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweb_db-1.0.3.tar", last modified: Sun Jun 25 10:35:32 2023, max compression
+gzip compressed data, was "pyweb_db-1.0.4.tar", last modified: Sun Jun 25 16:24:30 2023, max compression
```

## Comparing `pyweb_db-1.0.3.tar` & `pyweb_db-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.968711 pyweb_db-1.0.3/
--rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      590 2023-06-25 10:35:32.968711 pyweb_db-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.941240 pyweb_db-1.0.3/pyweb_db/
--rw-rw-rw-   0        0        0     8464 2023-06-25 10:34:33.000000 pyweb_db-1.0.3/pyweb_db/__init__.py
--rw-rw-rw-   0        0        0     4707 2023-06-25 10:34:39.000000 pyweb_db-1.0.3/pyweb_db/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.966395 pyweb_db-1.0.3/pyweb_db.egg-info/
--rw-rw-rw-   0        0        0      590 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-25 10:35:32.971191 pyweb_db-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-06-25 10:34:50.000000 pyweb_db-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.787114 pyweb_db-1.0.4/
+-rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-06-25 16:24:30.788116 pyweb_db-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.749631 pyweb_db-1.0.4/pyweb_db/
+-rw-rw-rw-   0        0        0     8764 2023-06-25 16:24:18.000000 pyweb_db-1.0.4/pyweb_db/__init__.py
+-rw-rw-rw-   0        0        0     4707 2023-06-25 10:34:39.000000 pyweb_db-1.0.4/pyweb_db/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.785569 pyweb_db-1.0.4/pyweb_db.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-06-25 16:24:30.790110 pyweb_db-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-06-25 16:24:23.000000 pyweb_db-1.0.4/setup.py
```

### Comparing `pyweb_db-1.0.3/LICENSE` & `pyweb_db-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.3/PKG-INFO` & `pyweb_db-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb_db
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.3/pyweb_db/__init__.py` & `pyweb_db-1.0.4/pyweb_db/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,35 +8,35 @@
         
         self.path = database_path
         
         if not os.path.isfile(self.path):
             self.create_empty_database()
     
     def create_empty_database(self):
-        with open(self.path, 'w') as file:
+        with open(self.path, 'w', encoding='utf-8') as file:
             json.dump({}, file)
     
     async def load_data(self):
-        async with aiofiles.open(self.path, 'r') as file:
+        async with aiofiles.open(self.path, 'r', encoding='utf-8') as file:
             return json.loads(await file.read())
     
     async def save_data(self, data):
-        async with aiofiles.open(self.path, 'w') as file:
+        async with aiofiles.open(self.path, 'w', encoding='utf-8') as file:
             await file.write(json.dumps(data))
     
     async def create_table(self, table_name: str):
         db_content = await self.load_data()
         if table_name not in db_content:
             db_content[table_name] = []
             await self.save_data(db_content)
     
     async def create_tables(self, table_names: list):
         db_content = await self.load_data()
         if type(table_names) != list:
-            print('INCORRECT TYPE!')
+            print(f'INCORRECT TYPE!\n{table_names}')
             return
         for table_name in table_names:
             if table_name not in db_content:
                 db_content[table_name] = []
                 await self.save_data(db_content)
 
     async def insert_into_table(self, table_name: str, data, unique: bool = False):
@@ -48,15 +48,15 @@
             elif unique == False:
                 db_content[table_name].append(data)
                 await self.save_data(db_content)
     
     async def insert_datas_into_table(self, table_name: str, datas: list, unique: bool = False):
         db_content = await self.load_data()
         if not type(datas) == list:
-            print('INCORRECT TYPE!')
+            print(f'INCORRECT TYPE!\n{datas}')
             return
         if table_name in db_content:
             for data in datas:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
                     await self.save_data(db_content)
                 elif unique == False:
@@ -74,15 +74,15 @@
         db_content = await self.load_data()
         if table_name in db_content:
             del db_content[table_name]
             await self.save_data(db_content)
     
     async def delete_tables(self, table_names: list):
         if type(table_names) != list:
-            print('INCORRECT TYPE!')
+            print(f'INCORRECT TYPE!\n{table_names}')
             return
         db_content = await self.load_data()
         for table_name in table_names:
             if table_name in db_content:
                 del db_content[table_name]
                 await self.save_data(db_content)
     
@@ -102,107 +102,107 @@
     def __init__(self, database_path: str = None):
         if database_path is None:
             raise ValueError('ERROR! INCORRECT DATABASE PATH!')
         
         self.path = database_path
         
         if not os.path.isfile(self.path):
-            with open(self.path, 'w') as file:
+            with open(self.path, 'w', encoding='utf-8') as file:
                 json.dump({}, file)
     
     def create_table(self, table_name: str):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name not in db_content:
                 db_content[table_name] = []
                 file.seek(0)
                 json.dump(db_content, file)
     
     def create_tables(self, table_names: list):
         if type(table_names) != list:
-            print('INCORRECT TYPE!')
+            print(f'INCORRECT TYPE!\n{table_names}')
             return
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             for table_name in table_names:
                 if table_name not in db_content:
                     db_content[table_name] = []
                     file.seek(0)
                     json.dump(db_content, file)
 
     def insert_into_table(self, table_name: str, data, unique: bool = False):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
                     file.seek(0)
                     json.dump(db_content, file)
                 elif unique == False:
                     db_content[table_name].append(data)
                     file.seek(0)
                     json.dump(db_content, file)
     
     def insert_datas_into_table(self, table_name: str, datas: list, unique: bool = False):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if not type(datas) == list:
-                print('INCORRECT TYPE!')
+                print(f'INCORRECT TYPE!\n{datas}')
                 return
             if table_name in db_content:
                 for data in datas:
                     if (not data in db_content[table_name] and unique == True):
                         db_content[table_name].append(data)
                         file.seek(0)
                         json.dump(db_content, file)
                     elif unique == False:
                         db_content[table_name].append(data)
                         file.seek(0)
                         json.dump(db_content, file)
 
     def delete_from_table(self, table_name: str, data):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 if data in db_content[table_name]:
                     db_content[table_name].remove(data)
                     file.seek(0)
                     json.dump(db_content, file)
                     file.truncate()
     
     def delete_table(self, table_name: str):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 del db_content[table_name]
                 file.seek(0)
                 json.dump(db_content, file)
                 file.truncate()
     
     def delete_tables(self, table_names: list):
         if type(table_names) != list:
-            print('INCORRECT TYPE!')
+            print(f'INCORRECT TYPE!\n{table_names}')
             return
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             for table_name in table_names:
                 if table_name in db_content:
                     del db_content[table_name]
                     file.seek(0)
                     json.dump(db_content, file)
                     file.truncate()
     
     def update_data(self, table_name: str, data, replace_data):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content and data in db_content[table_name]:
                 index4replace = db_content[table_name].index(data)
                 db_content[table_name][index4replace] = replace_data
                 file.seek(0)
                 json.dump(db_content, file)
                 file.truncate()
     
     def get_data(self, table_name: str):
-        with open(self.path, 'r+') as file:
+        with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 return db_content[table_name]
```

### Comparing `pyweb_db-1.0.3/pyweb_db/main.py` & `pyweb_db-1.0.4/pyweb_db/main.py`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.3/pyweb_db.egg-info/PKG-INFO` & `pyweb_db-1.0.4/pyweb_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb-db
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.3/setup.py` & `pyweb_db-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='pyweb_db',
-  version='1.0.3',
+  version='1.0.4',
   author='PyWebSol',
   author_email='pywebsol@gmail.com',
   description='This is a simple JSON-based database library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['aiofiles'],
```

