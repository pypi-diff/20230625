# Comparing `tmp/spark_datax_tools-0.3.1.tar.gz` & `tmp/spark_datax_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_datax_tools-0.3.1.tar", last modified: Sat Jun 17 22:17:42 2023, max compression
+gzip compressed data, was "spark_datax_tools-0.3.2.tar", last modified: Sun Jun 25 06:15:11 2023, max compression
```

## Comparing `spark_datax_tools-0.3.1.tar` & `spark_datax_tools-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.156921 spark_datax_tools-0.3.1/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4266 2023-06-17 22:17:42.157922 spark_datax_tools-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.3.1/README.md
--rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-17 22:17:42.158923 spark_datax_tools-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-17 22:17:26.000000 spark_datax_tools-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.114911 spark_datax_tools-0.3.1/spark_datax_tools/
--rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.3.1/spark_datax_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.134916 spark_datax_tools-0.3.1/spark_datax_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/spark_datax_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    50486 2023-06-17 22:17:00.000000 spark_datax_tools-0.3.1/spark_datax_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.150920 spark_datax_tools-0.3.1/spark_datax_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.156921 spark_datax_tools-0.3.1/spark_datax_tools/utils/files/
--rw-rw-rw-   0        0        0     1911 2023-06-08 10:10:52.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/files/ns.csv
--rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.133916 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/
--rw-rw-rw-   0        0        0     4266 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.868221 spark_datax_tools-0.3.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4266 2023-06-25 06:15:11.868221 spark_datax_tools-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.3.2/README.md
+-rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-25 06:15:11.869223 spark_datax_tools-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-25 06:08:46.000000 spark_datax_tools-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.826899 spark_datax_tools-0.3.2/spark_datax_tools/
+-rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.3.2/spark_datax_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.857803 spark_datax_tools-0.3.2/spark_datax_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/spark_datax_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    50486 2023-06-17 22:17:00.000000 spark_datax_tools-0.3.2/spark_datax_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.866805 spark_datax_tools-0.3.2/spark_datax_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.866805 spark_datax_tools-0.3.2/spark_datax_tools/utils/files/
+-rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/files/ns.csv
+-rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.849801 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/
+-rw-rw-rw-   0        0        0     4266 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/top_level.txt
```

### Comparing `spark_datax_tools-0.3.1/LICENSE` & `spark_datax_tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/PKG-INFO` & `spark_datax_tools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_datax_tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.1/README.md` & `spark_datax_tools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/pyproject.toml` & `spark_datax_tools-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/setup.py` & `spark_datax_tools-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_datax_tools',
     packages=find_packages(),
-    version='0.3.1',
+    version='0.3.2',
     description='spark_datax_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_datax_tools/',
     download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
```

### Comparing `spark_datax_tools-0.3.1/spark_datax_tools/__init__.py` & `spark_datax_tools-0.3.2/spark_datax_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/spark_datax_tools/functions/generator.py` & `spark_datax_tools-0.3.2/spark_datax_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/spark_datax_tools/utils/utils.py` & `spark_datax_tools-0.3.2/spark_datax_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.1/spark_datax_tools.egg-info/PKG-INFO` & `spark_datax_tools-0.3.2/spark_datax_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-datax-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.1/spark_datax_tools.egg-info/SOURCES.txt` & `spark_datax_tools-0.3.2/spark_datax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

