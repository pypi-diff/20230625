# Comparing `tmp/ko2kana-1.1.tar.gz` & `tmp/ko2kana-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ko2kana-1.1.tar", last modified: Sun Jun 25 17:18:40 2023, max compression
+gzip compressed data, was "ko2kana-1.2.tar", last modified: Sun Jun 25 17:22:28 2023, max compression
```

## Comparing `ko2kana-1.1.tar` & `ko2kana-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:18:40.066390 ko2kana-1.1/
--rw-rw-rw-   0        0        0     1090 2023-06-19 12:49:08.000000 ko2kana-1.1/LICENSE
--rw-rw-rw-   0        0        0     1674 2023-06-25 17:18:40.065391 ko2kana-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-06-25 17:15:39.000000 ko2kana-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 17:18:40.058285 ko2kana-1.1/ko2kana/
--rw-rw-rw-   0        0        0       36 2023-06-25 14:01:53.000000 ko2kana-1.1/ko2kana/__init__.py
--rw-rw-rw-   0        0        0     2675 2023-06-25 12:28:30.000000 ko2kana-1.1/ko2kana/japanese.py
--rw-rw-rw-   0        0        0     2212 2023-06-25 17:12:10.000000 ko2kana-1.1/ko2kana/ko2kana.py
--rw-rw-rw-   0        0        0    14528 2023-06-25 12:40:12.000000 ko2kana-1.1/ko2kana/korean.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:18:40.064390 ko2kana-1.1/ko2kana.egg-info/
--rw-rw-rw-   0        0        0     1674 2023-06-25 17:18:39.000000 ko2kana-1.1/ko2kana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-25 17:18:39.000000 ko2kana-1.1/ko2kana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:18:39.000000 ko2kana-1.1/ko2kana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-25 17:18:39.000000 ko2kana-1.1/ko2kana.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 17:18:39.000000 ko2kana-1.1/ko2kana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 17:18:40.066390 ko2kana-1.1/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-06-25 17:17:55.000000 ko2kana-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:22:28.416379 ko2kana-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-19 12:49:08.000000 ko2kana-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1674 2023-06-25 17:22:28.415378 ko2kana-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-06-25 17:15:39.000000 ko2kana-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 17:22:28.395349 ko2kana-1.2/ko2kana/
+-rw-rw-rw-   0        0        0       36 2023-06-25 14:01:53.000000 ko2kana-1.2/ko2kana/__init__.py
+-rw-rw-rw-   0        0        0     2675 2023-06-25 12:28:30.000000 ko2kana-1.2/ko2kana/japanese.py
+-rw-rw-rw-   0        0        0     2212 2023-06-25 17:12:10.000000 ko2kana-1.2/ko2kana/ko2kana.py
+-rw-rw-rw-   0        0        0    14528 2023-06-25 12:40:12.000000 ko2kana-1.2/ko2kana/korean.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:22:28.414373 ko2kana-1.2/ko2kana.egg-info/
+-rw-rw-rw-   0        0        0     1674 2023-06-25 17:22:28.000000 ko2kana-1.2/ko2kana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-25 17:22:28.000000 ko2kana-1.2/ko2kana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:22:28.000000 ko2kana-1.2/ko2kana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-25 17:22:28.000000 ko2kana-1.2/ko2kana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 17:22:28.000000 ko2kana-1.2/ko2kana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:22:28.416379 ko2kana-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-06-25 17:22:26.000000 ko2kana-1.2/setup.py
```

### Comparing `ko2kana-1.1/LICENSE` & `ko2kana-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ko2kana-1.1/PKG-INFO` & `ko2kana-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ko2kana
-Version: 1.1
+Version: 1.2
 Summary: Korean to Katakana
 Home-page: https://github.com/kdrkdrkdr/ko2kana
 Author: kdr
 Author-email: kdrhacker1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ko2kana-1.1/README.md` & `ko2kana-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ko2kana-1.1/ko2kana/japanese.py` & `ko2kana-1.2/ko2kana/japanese.py`

 * *Files identical despite different names*

### Comparing `ko2kana-1.1/ko2kana/ko2kana.py` & `ko2kana-1.2/ko2kana/ko2kana.py`

 * *Files identical despite different names*

### Comparing `ko2kana-1.1/ko2kana/korean.py` & `ko2kana-1.2/ko2kana/korean.py`

 * *Files identical despite different names*

### Comparing `ko2kana-1.1/ko2kana.egg-info/PKG-INFO` & `ko2kana-1.2/ko2kana.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ko2kana
-Version: 1.1
+Version: 1.2
 Summary: Korean to Katakana
 Home-page: https://github.com/kdrkdrkdr/ko2kana
 Author: kdr
 Author-email: kdrhacker1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ko2kana-1.1/setup.py` & `ko2kana-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="ko2kana",
-    version="1.1",
+    version="1.2",
     license='MIT',
     author="kdr",
     author_email="kdrhacker1234@gmail.com",
     description="Korean to Katakana",
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/kdrkdrkdr/ko2kana",
@@ -20,11 +20,12 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'g2pk2',
         'jamo',
         'cmake',
+        'jaconv',
         'pyopenjtalk',
     ],
     py_modules = ['ko2kana']
 )
```

