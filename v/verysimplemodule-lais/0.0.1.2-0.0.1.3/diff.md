# Comparing `tmp/verysimplemodule_lais-0.0.1.2.tar.gz` & `tmp/verysimplemodule_lais-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodule_lais-0.0.1.2.tar", last modified: Fri Jun 23 19:46:30 2023, max compression
+gzip compressed data, was "verysimplemodule_lais-0.0.1.3.tar", last modified: Sun Jun 25 14:22:56 2023, max compression
```

## Comparing `verysimplemodule_lais-0.0.1.2.tar` & `verysimplemodule_lais-0.0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.513112 verysimplemodule_lais-0.0.1.2/
--rw-rw-rw-   0        0        0      544 2023-06-23 19:46:30.497491 verysimplemodule_lais-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-23 19:46:30.513112 verysimplemodule_lais-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-06-23 19:44:37.000000 verysimplemodule_lais-0.0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.481878 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/
--rw-rw-rw-   0        0        0       43 2023-06-23 19:00:28.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/__init__.py
--rw-rw-rw-   0        0        0      374 2023-06-23 19:00:35.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/baixar_arquivo.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.497491 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/
--rw-rw-rw-   0        0        0      544 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 14:22:56.973020 verysimplemodule_lais-0.0.1.3/
+-rw-rw-rw-   0        0        0      528 2023-06-25 14:22:56.973020 verysimplemodule_lais-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-25 14:22:56.973020 verysimplemodule_lais-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1091 2023-06-25 14:21:08.000000 verysimplemodule_lais-0.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 14:22:56.910524 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais/
+-rw-rw-rw-   0        0        0       43 2023-06-23 19:00:28.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-25 14:18:38.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais/baixar_arquivo.py
+drwxrwxrwx   0        0        0        0 2023-06-25 14:22:56.973020 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-06-25 14:22:56.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-25 14:22:56.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 14:22:56.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 14:22:56.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-06-25 14:22:56.000000 verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/top_level.txt
```

### Comparing `verysimplemodule_lais-0.0.1.2/PKG-INFO` & `verysimplemodule_lais-0.0.1.3/verysimplemodule_lais.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: verysimplemodule_lais
-Version: 0.0.1.2
-Summary: Meu primeiro pacote em Python
+Name: verysimplemodule-lais
+Version: 0.0.1.3
+Summary: Pacote para baixar arquivo
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
-Meu primeiro pacote em Python para baixar um PDF
+Pacote em Python para baixar um PDF
```

### Comparing `verysimplemodule_lais-0.0.1.2/setup.py` & `verysimplemodule_lais-0.0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1.2' 
-DESCRIPTION = 'Meu primeiro pacote em Python'
-LONG_DESCRIPTION = 'Meu primeiro pacote em Python para baixar um PDF'
+VERSION = '0.0.1.3' 
+DESCRIPTION = 'Pacote para baixar arquivo'
+LONG_DESCRIPTION = 'Pacote em Python para baixar um PDF'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="verysimplemodule_lais", 
         version=VERSION,
         author="Lais Sousa",
```

### Comparing `verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/PKG-INFO` & `verysimplemodule_lais-0.0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: verysimplemodule-lais
-Version: 0.0.1.2
-Summary: Meu primeiro pacote em Python
+Name: verysimplemodule_lais
+Version: 0.0.1.3
+Summary: Pacote para baixar arquivo
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
-Meu primeiro pacote em Python para baixar um PDF
+Pacote em Python para baixar um PDF
```

