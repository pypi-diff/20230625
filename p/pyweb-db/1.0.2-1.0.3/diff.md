# Comparing `tmp/pyweb_db-1.0.2.tar.gz` & `tmp/pyweb_db-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweb_db-1.0.2.tar", last modified: Sat Jun 24 17:06:07 2023, max compression
+gzip compressed data, was "pyweb_db-1.0.3.tar", last modified: Sun Jun 25 10:35:32 2023, max compression
```

## Comparing `pyweb_db-1.0.2.tar` & `pyweb_db-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.137228 pyweb_db-1.0.2/
--rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1895 2023-06-24 17:06:07.137228 pyweb_db-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1448 2023-06-24 13:41:47.000000 pyweb_db-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.094624 pyweb_db-1.0.2/pyweb_db/
--rw-rw-rw-   0        0        0     7874 2023-06-24 17:01:00.000000 pyweb_db-1.0.2/pyweb_db/__init__.py
--rw-rw-rw-   0        0        0     4707 2023-06-24 17:04:39.000000 pyweb_db-1.0.2/pyweb_db/main.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.135253 pyweb_db-1.0.2/pyweb_db.egg-info/
--rw-rw-rw-   0        0        0     1895 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-24 17:06:07.140253 pyweb_db-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-06-24 17:05:21.000000 pyweb_db-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.968711 pyweb_db-1.0.3/
+-rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-06-25 10:35:32.968711 pyweb_db-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.941240 pyweb_db-1.0.3/pyweb_db/
+-rw-rw-rw-   0        0        0     8464 2023-06-25 10:34:33.000000 pyweb_db-1.0.3/pyweb_db/__init__.py
+-rw-rw-rw-   0        0        0     4707 2023-06-25 10:34:39.000000 pyweb_db-1.0.3/pyweb_db/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 10:35:32.966395 pyweb_db-1.0.3/pyweb_db.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 10:35:32.000000 pyweb_db-1.0.3/pyweb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-06-25 10:35:32.971191 pyweb_db-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-06-25 10:34:50.000000 pyweb_db-1.0.3/setup.py
```

### Comparing `pyweb_db-1.0.2/LICENSE` & `pyweb_db-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.2/pyweb_db/__init__.py` & `pyweb_db-1.0.3/pyweb_db/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,17 @@
         db_content = await self.load_data()
         if table_name not in db_content:
             db_content[table_name] = []
             await self.save_data(db_content)
     
     async def create_tables(self, table_names: list):
         db_content = await self.load_data()
+        if type(table_names) != list:
+            print('INCORRECT TYPE!')
+            return
         for table_name in table_names:
             if table_name not in db_content:
                 db_content[table_name] = []
                 await self.save_data(db_content)
 
     async def insert_into_table(self, table_name: str, data, unique: bool = False):
         db_content = await self.load_data()
@@ -44,14 +47,17 @@
                 await self.save_data(db_content)
             elif unique == False:
                 db_content[table_name].append(data)
                 await self.save_data(db_content)
     
     async def insert_datas_into_table(self, table_name: str, datas: list, unique: bool = False):
         db_content = await self.load_data()
+        if not type(datas) == list:
+            print('INCORRECT TYPE!')
+            return
         if table_name in db_content:
             for data in datas:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
                     await self.save_data(db_content)
                 elif unique == False:
                     db_content[table_name].append(data)
@@ -67,14 +73,17 @@
     async def delete_table(self, table_name: str):
         db_content = await self.load_data()
         if table_name in db_content:
             del db_content[table_name]
             await self.save_data(db_content)
     
     async def delete_tables(self, table_names: list):
+        if type(table_names) != list:
+            print('INCORRECT TYPE!')
+            return
         db_content = await self.load_data()
         for table_name in table_names:
             if table_name in db_content:
                 del db_content[table_name]
                 await self.save_data(db_content)
     
     async def update_data(self, table_name: str, data, replace_data):
@@ -105,14 +114,17 @@
             db_content = json.load(file)
             if table_name not in db_content:
                 db_content[table_name] = []
                 file.seek(0)
                 json.dump(db_content, file)
     
     def create_tables(self, table_names: list):
+        if type(table_names) != list:
+            print('INCORRECT TYPE!')
+            return
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             for table_name in table_names:
                 if table_name not in db_content:
                     db_content[table_name] = []
                     file.seek(0)
                     json.dump(db_content, file)
@@ -129,14 +141,17 @@
                     db_content[table_name].append(data)
                     file.seek(0)
                     json.dump(db_content, file)
     
     def insert_datas_into_table(self, table_name: str, datas: list, unique: bool = False):
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
+            if not type(datas) == list:
+                print('INCORRECT TYPE!')
+                return
             if table_name in db_content:
                 for data in datas:
                     if (not data in db_content[table_name] and unique == True):
                         db_content[table_name].append(data)
                         file.seek(0)
                         json.dump(db_content, file)
                     elif unique == False:
@@ -160,14 +175,17 @@
             if table_name in db_content:
                 del db_content[table_name]
                 file.seek(0)
                 json.dump(db_content, file)
                 file.truncate()
     
     def delete_tables(self, table_names: list):
+        if type(table_names) != list:
+            print('INCORRECT TYPE!')
+            return
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             for table_name in table_names:
                 if table_name in db_content:
                     del db_content[table_name]
                     file.seek(0)
                     json.dump(db_content, file)
```

### Comparing `pyweb_db-1.0.2/pyweb_db/main.py` & `pyweb_db-1.0.3/pyweb_db/main.py`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.2/setup.py` & `pyweb_db-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='pyweb_db',
-  version='1.0.2',
+  version='1.0.3',
   author='PyWebSol',
   author_email='pywebsol@gmail.com',
   description='This is a simple JSON-based database library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['aiofiles'],
```

