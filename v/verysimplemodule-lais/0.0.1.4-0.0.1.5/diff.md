# Comparing `tmp/verysimplemodule_lais-0.0.1.4.tar.gz` & `tmp/verysimplemodule_lais-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodule_lais-0.0.1.4.tar", last modified: Sun Jun 25 14:51:57 2023, max compression
+gzip compressed data, was "verysimplemodule_lais-0.0.1.5.tar", last modified: Sun Jun 25 14:56:11 2023, max compression
```

## Comparing `verysimplemodule_lais-0.0.1.4.tar` & `verysimplemodule_lais-0.0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 14:51:57.152599 verysimplemodule_lais-0.0.1.4/
--rw-rw-rw-   0        0        0      528 2023-06-25 14:51:57.152599 verysimplemodule_lais-0.0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-25 14:51:57.152599 verysimplemodule_lais-0.0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-06-25 14:50:44.000000 verysimplemodule_lais-0.0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 14:51:57.090101 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais/
--rw-rw-rw-   0        0        0       43 2023-06-23 19:00:28.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-25 14:44:01.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais/baixar_arquivo.py
-drwxrwxrwx   0        0        0        0 2023-06-25 14:51:57.136979 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/
--rw-rw-rw-   0        0        0      528 2023-06-25 14:51:56.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-25 14:51:56.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 14:51:56.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 14:51:56.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-25 14:51:56.000000 verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 14:56:11.698700 verysimplemodule_lais-0.0.1.5/
+-rw-rw-rw-   0        0        0      528 2023-06-25 14:56:11.698700 verysimplemodule_lais-0.0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-25 14:56:11.698700 verysimplemodule_lais-0.0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-06-25 14:55:52.000000 verysimplemodule_lais-0.0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 14:56:11.651826 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais/
+-rw-rw-rw-   0        0        0       50 2023-06-25 14:55:20.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-25 14:44:01.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais/baixar_arquivo.py
+drwxrwxrwx   0        0        0        0 2023-06-25 14:56:11.698700 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-06-25 14:56:11.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-25 14:56:11.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 14:56:11.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 14:56:11.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-25 14:56:11.000000 verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/top_level.txt
```

### Comparing `verysimplemodule_lais-0.0.1.4/PKG-INFO` & `verysimplemodule_lais-0.0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodule_lais
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Pacote para baixar arquivo
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `verysimplemodule_lais-0.0.1.4/setup.py` & `verysimplemodule_lais-0.0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1.4' 
+VERSION = '0.0.1.5' 
 DESCRIPTION = 'Pacote para baixar arquivo'
 LONG_DESCRIPTION = 'Pacote em Python para baixar um PDF'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="verysimplemodule_lais",
```

### Comparing `verysimplemodule_lais-0.0.1.4/verysimplemodule_lais.egg-info/PKG-INFO` & `verysimplemodule_lais-0.0.1.5/verysimplemodule_lais.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodule-lais
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Pacote para baixar arquivo
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

