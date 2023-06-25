# Comparing `tmp/pyweb_db-1.0.4.tar.gz` & `tmp/pyweb_db-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweb_db-1.0.4.tar", last modified: Sun Jun 25 16:24:30 2023, max compression
+gzip compressed data, was "pyweb_db-1.0.5.tar", last modified: Sun Jun 25 20:13:40 2023, max compression
```

## Comparing `pyweb_db-1.0.4.tar` & `pyweb_db-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.787114 pyweb_db-1.0.4/
--rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      590 2023-06-25 16:24:30.788116 pyweb_db-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.749631 pyweb_db-1.0.4/pyweb_db/
--rw-rw-rw-   0        0        0     8764 2023-06-25 16:24:18.000000 pyweb_db-1.0.4/pyweb_db/__init__.py
--rw-rw-rw-   0        0        0     4707 2023-06-25 10:34:39.000000 pyweb_db-1.0.4/pyweb_db/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:24:30.785569 pyweb_db-1.0.4/pyweb_db.egg-info/
--rw-rw-rw-   0        0        0      590 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 16:24:30.000000 pyweb_db-1.0.4/pyweb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-25 16:24:30.790110 pyweb_db-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-06-25 16:24:23.000000 pyweb_db-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.230163 pyweb_db-1.0.5/
+-rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-06-25 20:13:40.231431 pyweb_db-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.188022 pyweb_db-1.0.5/pyweb_db/
+-rw-rw-rw-   0        0        0     8573 2023-06-25 20:13:23.000000 pyweb_db-1.0.5/pyweb_db/__init__.py
+-rw-rw-rw-   0        0        0     4707 2023-06-25 19:54:48.000000 pyweb_db-1.0.5/pyweb_db/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.228080 pyweb_db-1.0.5/pyweb_db.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-25 20:13:40.000000 pyweb_db-1.0.5/pyweb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-06-25 20:13:40.234382 pyweb_db-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-06-25 19:55:06.000000 pyweb_db-1.0.5/setup.py
```

### Comparing `pyweb_db-1.0.4/LICENSE` & `pyweb_db-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.4/PKG-INFO` & `pyweb_db-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb_db
-Version: 1.0.4
+Version: 1.0.5
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.4/pyweb_db/__init__.py` & `pyweb_db-1.0.5/pyweb_db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import json, os, aiofiles, asyncio
 
-
 class async_connection:
     def __init__(self, database_path: str = None):
         if database_path is None:
             raise ValueError('ERROR! INCORRECT DATABASE PATH!')
-        
         self.path = database_path
-        
         if not os.path.isfile(self.path):
             self.create_empty_database()
     
     def create_empty_database(self):
         with open(self.path, 'w', encoding='utf-8') as file:
             json.dump({}, file)
     
@@ -54,18 +51,17 @@
         if not type(datas) == list:
             print(f'INCORRECT TYPE!\n{datas}')
             return
         if table_name in db_content:
             for data in datas:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
-                    await self.save_data(db_content)
                 elif unique == False:
                     db_content[table_name].append(data)
-                    await self.save_data(db_content)
+            await self.save_data(db_content)
 
     async def delete_from_table(self, table_name: str, data):
         db_content = await self.load_data()
         if table_name in db_content:
             if data in db_content[table_name]:
                 db_content[table_name].remove(data)
                 await self.save_data(db_content)
@@ -148,20 +144,18 @@
             if not type(datas) == list:
                 print(f'INCORRECT TYPE!\n{datas}')
                 return
             if table_name in db_content:
                 for data in datas:
                     if (not data in db_content[table_name] and unique == True):
                         db_content[table_name].append(data)
-                        file.seek(0)
-                        json.dump(db_content, file)
                     elif unique == False:
                         db_content[table_name].append(data)
-                        file.seek(0)
-                        json.dump(db_content, file)
+                file.seek(0)
+                json.dump(db_content, file)
 
     def delete_from_table(self, table_name: str, data):
         with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 if data in db_content[table_name]:
                     db_content[table_name].remove(data)
```

### Comparing `pyweb_db-1.0.4/pyweb_db/main.py` & `pyweb_db-1.0.5/pyweb_db/main.py`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.4/pyweb_db.egg-info/PKG-INFO` & `pyweb_db-1.0.5/pyweb_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb-db
-Version: 1.0.4
+Version: 1.0.5
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.4/setup.py` & `pyweb_db-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='pyweb_db',
-  version='1.0.4',
+  version='1.0.5',
   author='PyWebSol',
   author_email='pywebsol@gmail.com',
   description='This is a simple JSON-based database library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['aiofiles'],
```

