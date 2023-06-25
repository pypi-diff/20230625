# Comparing `tmp/spark_acl_tools-0.1.0.tar.gz` & `tmp/spark_acl_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_acl_tools-0.1.0.tar", last modified: Sun Jun 25 09:27:46 2023, max compression
+gzip compressed data, was "spark_acl_tools-0.2.0.tar", last modified: Sun Jun 25 20:28:44 2023, max compression
```

## Comparing `spark_acl_tools-0.1.0.tar` & `spark_acl_tools-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_acl_tools-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       41 2023-06-25 06:14:15.000000 spark_acl_tools-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5704 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4949 2023-06-25 09:26:52.000000 spark_acl_tools-0.1.0/README.md
--rw-rw-rw-   0        0        0      633 2023-06-25 06:52:01.000000 spark_acl_tools-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-25 09:27:46.728812 spark_acl_tools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-06-25 09:21:42.000000 spark_acl_tools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.697560 spark_acl_tools-0.1.0/spark_acl_tools/
--rw-rw-rw-   0        0        0     1428 2023-06-25 08:40:18.000000 spark_acl_tools-0.1.0/spark_acl_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/spark_acl_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_acl_tools-0.1.0/spark_acl_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    19121 2023-06-25 09:15:50.000000 spark_acl_tools-0.1.0/spark_acl_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/spark_acl_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_acl_tools-0.1.0/spark_acl_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_acl_tools-0.1.0/spark_acl_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/spark_acl_tools/utils/files/
--rw-rw-rw-   0        0        0    24641 2023-06-24 17:38:32.000000 spark_acl_tools-0.1.0/spark_acl_tools/utils/files/acl.xlsx
--rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_acl_tools-0.1.0/spark_acl_tools/utils/files/ns.csv
-drwxrwxrwx   0        0        0        0 2023-06-25 09:27:46.713187 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/
--rw-rw-rw-   0        0        0     5704 2023-06-25 09:27:46.000000 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-06-25 09:27:46.000000 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 09:27:46.000000 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-06-25 09:27:46.000000 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-25 09:27:46.000000 spark_acl_tools-0.1.0/spark_acl_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.156263 spark_acl_tools-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-06-25 06:14:15.000000 spark_acl_tools-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5704 2023-06-25 20:28:44.156263 spark_acl_tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4949 2023-06-25 09:26:52.000000 spark_acl_tools-0.2.0/README.md
+-rw-rw-rw-   0        0        0      633 2023-06-25 06:52:01.000000 spark_acl_tools-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-25 20:28:44.158264 spark_acl_tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-06-25 20:28:28.000000 spark_acl_tools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.114251 spark_acl_tools-0.2.0/spark_acl_tools/
+-rw-rw-rw-   0        0        0     1428 2023-06-25 08:40:18.000000 spark_acl_tools-0.2.0/spark_acl_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.134255 spark_acl_tools-0.2.0/spark_acl_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/spark_acl_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    19184 2023-06-25 20:28:12.000000 spark_acl_tools-0.2.0/spark_acl_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.144257 spark_acl_tools-0.2.0/spark_acl_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.155263 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/
+-rw-rw-rw-   0        0        0    24641 2023-06-24 17:38:32.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/acl.xlsx
+-rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/ns.csv
+drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.133255 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/
+-rw-rw-rw-   0        0        0     5704 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/top_level.txt
```

### Comparing `spark_acl_tools-0.1.0/LICENSE` & `spark_acl_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/PKG-INFO` & `spark_acl_tools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_acl_tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: spark_acl_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_acl_tools-0.1.0/README.md` & `spark_acl_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/pyproject.toml` & `spark_acl_tools-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/setup.py` & `spark_acl_tools-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_acl_tools',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.2.0',
     description='spark_acl_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_datax_tools/',
     download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
```

### Comparing `spark_acl_tools-0.1.0/spark_acl_tools/__init__.py` & `spark_acl_tools-0.2.0/spark_acl_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/spark_acl_tools/functions/generator.py` & `spark_acl_tools-0.2.0/spark_acl_tools/functions/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         lambda x: get_replace_value(acl_name="ACL_INGESTA_MASTER", col=x["Group"], uuaa_master=uuaa_master, ns=ns),
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_INGESTA_MASTER", col=x["Path"], uuaa_master=uuaa_master, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_PROJECT_INGESTA_MASTER', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_INGESTA_MASTER", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -140,15 +140,15 @@
         lambda x: get_replace_value(acl_name="ACL_INGESTA_RAW", col=x["Group"], uuaa_raw=uuaa_raw, ns=ns),
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_INGESTA_RAW", col=x["Path"], uuaa_raw=uuaa_raw, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_PROJECT_INGESTA_RAW', uuaa_raw)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_INGESTA_RAW", uuaa_raw)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_raw}'))
     print(f'create file for acl: {path_filename}')
@@ -181,15 +181,15 @@
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_PROCESAMIENTO_MASTER", col=x["Path"],
                                     uuaa_master=uuaa_master, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_PROJECT_PROCESAMIENTO', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_PROCESAMIENTO", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -225,15 +225,15 @@
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_RAW", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_raw=uuaa_raw, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_RAW', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_RAW", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -269,15 +269,15 @@
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_STAGING", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_staging=uuaa_staging, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_STAGING', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_STAGING", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -313,15 +313,15 @@
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_READ", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_master_read=uuaa_master_read, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_READ', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_READ", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -350,15 +350,15 @@
         lambda x: get_replace_value(acl_name="ACL_MONITORING", col=x["Group"], uuaa_master=uuaa_master),
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_MONITORING", col=x["Path"], uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_ARGOS', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_ARGOS", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -387,15 +387,15 @@
         lambda x: get_replace_value(acl_name="ACL_DATAPROC", col=x["Group"], uuaa_master=uuaa_master),
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_DATAPROC", col=x["Path"], uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_DATAPROC', uuaa_master)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_DATAPROC", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
@@ -428,15 +428,15 @@
         axis=1)
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_SANDBOX", col=x["Path"],
                                     uuaa_sandbox=uuaa_sandbox, uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
-    path_directory = os.path.join('DIRECTORY_ACL_RUTA_SANDBOXLIVE', uuaa_sandbox)
+    path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_SANDBOXLIVE", uuaa_sandbox)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_sandbox}'))
     print(f'create file for acl: {path_filename}')
```

### Comparing `spark_acl_tools-0.1.0/spark_acl_tools/utils/files/acl.xlsx` & `spark_acl_tools-0.2.0/spark_acl_tools/utils/files/acl.xlsx`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/spark_acl_tools/utils/files/ns.csv` & `spark_acl_tools-0.2.0/spark_acl_tools/utils/files/ns.csv`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.1.0/spark_acl_tools.egg-info/PKG-INFO` & `spark_acl_tools-0.2.0/spark_acl_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-acl-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: spark_acl_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

