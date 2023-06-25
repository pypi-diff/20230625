# Comparing `tmp/Digital_Farming_Solution-0.1.0.tar.gz` & `tmp/Digital_Farming_Solution-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.0.tar", last modified: Sun Jun 25 06:43:53 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.1.tar", last modified: Sun Jun 25 17:01:12 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.0.tar` & `Digital_Farming_Solution-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:43:53.683386 Digital_Farming_Solution-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:43:53.597391 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     2509 2023-06-25 06:43:04.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        0 2023-06-23 10:43:31.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:43:53.670139 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      425 2023-06-25 06:43:52.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-25 06:43:53.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:43:52.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-25 06:43:52.000000 Digital_Farming_Solution-0.1.0/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2023-06-25 06:43:53.679049 Digital_Farming_Solution-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-25 06:43:53.684507 Digital_Farming_Solution-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-06-23 11:57:11.000000 Digital_Farming_Solution-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.559445 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     4450 2023-06-25 17:00:31.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:01:11.807277 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-25 17:01:10.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-25 17:01:08.000000 Digital_Farming_Solution-0.1.1/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:01:11.815259 Digital_Farming_Solution-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-06-25 10:53:53.000000 Digital_Farming_Solution-0.1.1/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.0/setup.py` & `Digital_Farming_Solution-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.0",
+    version="0.1.1",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
-    description=" The packages are helps to the DFS Teams to perform some of the task easily by importing this packages.",
+    description=" The packages are helps to the DFS Teams to perform some of the task easily.",
+    long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
+    long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

