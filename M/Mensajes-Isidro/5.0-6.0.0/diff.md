# Comparing `tmp/Mensajes-Isidro-5.0.tar.gz` & `tmp/Mensajes-Isidro-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/isidro/CursoHektorPython/Modulos y paquetes/dist/.tmp-2fxohrfj/Mensajes-Isidro-5.0.tar", last modified: Sun Jun 25 16:39:16 2023, max compression
+gzip compressed data, was "/home/isidro/CursoHektorPython/Modulos y paquetes/dist/.tmp-z1ot1d8l/Mensajes-Isidro-6.0.0.tar", last modified: Sun Jun 25 17:27:41 2023, max compression
```

## Comparing `Mensajes-Isidro-5.0.tar` & `Mensajes-Isidro-6.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     1066 2023-06-25 16:08:20.000000 Mensajes-Isidro-5.0/LICENSE
--rw-r--r--   0 isidro    (1000) isidro    (1000)       59 2023-06-25 16:08:15.000000 Mensajes-Isidro-5.0/MANIFEST.in
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/
--rw-rw-r--   0 isidro    (1000) isidro    (1000)      573 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/PKG-INFO
--rw-rw-r--   0 isidro    (1000) isidro    (1000)      414 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/SOURCES.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/dependency_links.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       14 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/requires.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       15 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/top_level.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)      573 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/PKG-INFO
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       87 2023-06-25 16:08:18.000000 Mensajes-Isidro-5.0/README.md
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/mensajes/
--rw-r--r--   0 isidro    (1000) isidro    (1000)       38 2022-07-07 17:39:14.000000 Mensajes-Isidro-5.0/mensajes/__init__.py
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/mensajes/adios/
--rw-r--r--   0 isidro    (1000) isidro    (1000)       47 2022-07-07 17:43:51.000000 Mensajes-Isidro-5.0/mensajes/adios/__init__.py
--rw-r--r--   0 isidro    (1000) isidro    (1000)      182 2022-07-07 17:45:52.000000 Mensajes-Isidro-5.0/mensajes/adios/despedidas.py
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/mensajes/hola/
--rw-r--r--   0 isidro    (1000) isidro    (1000)       46 2022-07-07 17:41:56.000000 Mensajes-Isidro-5.0/mensajes/hola/__init__.py
--rw-r--r--   0 isidro    (1000) isidro    (1000)      373 2022-07-08 17:46:25.000000 Mensajes-Isidro-5.0/mensajes/hola/saludos.py
--rw-r--r--   0 isidro    (1000) isidro    (1000)       13 2023-06-21 18:33:27.000000 Mensajes-Isidro-5.0/requirements.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       38 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/setup.cfg
--rw-r--r--   0 isidro    (1000) isidro    (1000)      820 2023-06-25 16:37:04.000000 Mensajes-Isidro-5.0/setup.py
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 16:39:16.000000 Mensajes-Isidro-5.0/tests/
--rw-r--r--   0 isidro    (1000) isidro    (1000)        0 2022-07-08 18:23:47.000000 Mensajes-Isidro-5.0/tests/__init__.py
--rw-r--r--   0 isidro    (1000) isidro    (1000)      268 2022-07-08 18:20:55.000000 Mensajes-Isidro-5.0/tests/test_hola.py
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1066 2023-06-25 16:08:20.000000 Mensajes-Isidro-6.0.0/LICENSE
+-rw-r--r--   0 isidro    (1000) isidro    (1000)       59 2023-06-25 16:08:15.000000 Mensajes-Isidro-6.0.0/MANIFEST.in
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)      575 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/PKG-INFO
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)      414 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/SOURCES.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/dependency_links.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       14 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/requires.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       15 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/top_level.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)      575 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/PKG-INFO
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       87 2023-06-25 16:08:18.000000 Mensajes-Isidro-6.0.0/README.md
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/mensajes/
+-rw-r--r--   0 isidro    (1000) isidro    (1000)       38 2022-07-07 17:39:14.000000 Mensajes-Isidro-6.0.0/mensajes/__init__.py
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/mensajes/adios/
+-rw-r--r--   0 isidro    (1000) isidro    (1000)       47 2022-07-07 17:43:51.000000 Mensajes-Isidro-6.0.0/mensajes/adios/__init__.py
+-rw-r--r--   0 isidro    (1000) isidro    (1000)      182 2022-07-07 17:45:52.000000 Mensajes-Isidro-6.0.0/mensajes/adios/despedidas.py
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/mensajes/hola/
+-rw-r--r--   0 isidro    (1000) isidro    (1000)       46 2023-06-25 16:40:45.000000 Mensajes-Isidro-6.0.0/mensajes/hola/__init__.py
+-rw-r--r--   0 isidro    (1000) isidro    (1000)      378 2023-06-25 17:24:22.000000 Mensajes-Isidro-6.0.0/mensajes/hola/saludos.py
+-rw-r--r--   0 isidro    (1000) isidro    (1000)       13 2023-06-21 18:33:27.000000 Mensajes-Isidro-6.0.0/requirements.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       38 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/setup.cfg
+-rw-r--r--   0 isidro    (1000) isidro    (1000)      822 2023-06-25 17:26:45.000000 Mensajes-Isidro-6.0.0/setup.py
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-06-25 17:27:41.000000 Mensajes-Isidro-6.0.0/tests/
+-rw-r--r--   0 isidro    (1000) isidro    (1000)        0 2022-07-08 18:23:47.000000 Mensajes-Isidro-6.0.0/tests/__init__.py
+-rw-r--r--   0 isidro    (1000) isidro    (1000)      268 2022-07-08 18:20:55.000000 Mensajes-Isidro-6.0.0/tests/test_hola.py
```

### Comparing `Mensajes-Isidro-5.0/LICENSE` & `Mensajes-Isidro-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-Isidro-5.0/Mensajes_Isidro.egg-info/PKG-INFO` & `Mensajes-Isidro-6.0.0/Mensajes_Isidro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Isidro
-Version: 5.0
+Version: 6.0.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.ibcop.com
 Author: Isidro Bellón Cano
 Author-email: isidro.bellon@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `Mensajes-Isidro-5.0/PKG-INFO` & `Mensajes-Isidro-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Isidro
-Version: 5.0
+Version: 6.0.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.ibcop.com
 Author: Isidro Bellón Cano
 Author-email: isidro.bellon@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `Mensajes-Isidro-5.0/setup.py` & `Mensajes-Isidro-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-Isidro',
-    version='5.0',
+    version='6.0.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Isidro Bellón Cano',
     author_email='isidro.bellon@gmail.com',
     url='https://www.ibcop.com',
     license_files=['LICENSE'],
```

