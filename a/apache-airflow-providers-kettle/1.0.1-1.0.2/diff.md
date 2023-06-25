# Comparing `tmp/apache_airflow_providers_kettle-1.0.1.tar.gz` & `tmp/apache_airflow_providers_kettle-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_kettle-1.0.1.tar", last modified: Sun Jun 25 21:27:24 2023, max compression
+gzip compressed data, was "apache_airflow_providers_kettle-1.0.2.tar", last modified: Sun Jun 25 21:42:32 2023, max compression
```

## Comparing `apache_airflow_providers_kettle-1.0.1.tar` & `apache_airflow_providers_kettle-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/
--rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.1/LICENSE
--rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:00:40.000000 apache_airflow_providers_kettle-1.0.1/README.md
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/
--rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/SOURCES.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/dependency_links.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/entry_points.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/requires.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-06-25 21:27:24.000000 apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/top_level.txt
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/kettle_provider/
--rw-rw-r--   0 bop       (1000) bop       (1000)      420 2023-06-25 21:26:32.000000 apache_airflow_providers_kettle-1.0.1/kettle_provider/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/kettle_provider/hooks/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.1/kettle_provider/hooks/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/kettle_provider/operators/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.1/kettle_provider/operators/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)     8598 2023-06-25 20:10:05.000000 apache_airflow_providers_kettle-1.0.1/kettle_provider/operators/kettle_operator.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/kettle_provider/sensors/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.1/kettle_provider/sensors/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-06-25 21:27:24.554455 apache_airflow_providers_kettle-1.0.1/setup.cfg
--rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-06-25 21:26:13.000000 apache_airflow_providers_kettle-1.0.1/setup.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/
+-rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.2/LICENSE
+-rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:00:40.000000 apache_airflow_providers_kettle-1.0.2/README.md
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/
+-rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/SOURCES.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/dependency_links.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/entry_points.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/requires.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-06-25 21:42:32.000000 apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/top_level.txt
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/kettle_provider/
+-rw-rw-r--   0 bop       (1000) bop       (1000)      386 2023-06-25 21:42:20.000000 apache_airflow_providers_kettle-1.0.2/kettle_provider/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/kettle_provider/hooks/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.2/kettle_provider/hooks/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/kettle_provider/operators/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.2/kettle_provider/operators/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)     8598 2023-06-25 20:10:05.000000 apache_airflow_providers_kettle-1.0.2/kettle_provider/operators/kettle_operator.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/kettle_provider/sensors/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.2/kettle_provider/sensors/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-06-25 21:42:32.409113 apache_airflow_providers_kettle-1.0.2/setup.cfg
+-rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-06-25 21:42:02.000000 apache_airflow_providers_kettle-1.0.2/setup.py
```

### Comparing `apache_airflow_providers_kettle-1.0.1/LICENSE` & `apache_airflow_providers_kettle-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.1/apache_airflow_providers_kettle.egg-info/SOURCES.txt` & `apache_airflow_providers_kettle-1.0.2/apache_airflow_providers_kettle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.1/kettle_provider/operators/kettle_operator.py` & `apache_airflow_providers_kettle-1.0.2/kettle_provider/operators/kettle_operator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.1/setup.py` & `apache_airflow_providers_kettle-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 """Perform the package airflow-provider-kettle-operator setup."""
 setup(
     name="apache_airflow_providers_kettle",
     version=__version__,
     description="A simple Apache Airflow Kettle Operator that can invoke jobs and transformations for Linux based systems.",
     long_description=long_description,
@@ -20,9 +20,9 @@
     author="Robert Bryśkiewicz",
     author_email="bryskiewiczr@pm.me",
     url="",
     classifiers=[
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
     ],
-    python_requires="~=3.8",
+    python_requires="~=3.7",
 )
```

