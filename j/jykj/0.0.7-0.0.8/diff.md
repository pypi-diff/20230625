# Comparing `tmp/jykj-0.0.7.tar.gz` & `tmp/jykj-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.7.tar", last modified: Sun Jun 25 06:47:55 2023, max compression
+gzip compressed data, was "jykj-0.0.8.tar", last modified: Sun Jun 25 07:36:41 2023, max compression
```

## Comparing `jykj-0.0.7.tar` & `jykj-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.067578 jykj-0.0.7/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-25 06:47:55.067578 jykj-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.049577 jykj-0.0.7/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.7/jykj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.065575 jykj-0.0.7/jykj/business_model/
--rw-rw-rw-   0        0        0    17264 2023-06-25 06:46:54.000000 jykj-0.0.7/jykj/business_model/SHE.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.7/jykj/business_model/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.7/jykj/business_model/prevention.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.7/jykj/business_model/production.py
--rw-rw-rw-   0        0        0    14683 2023-06-25 06:46:56.000000 jykj-0.0.7/jykj/business_model/security.py
--rw-rw-rw-   0        0        0    28542 2023-06-25 01:35:15.000000 jykj-0.0.7/jykj/business_model/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:47:55.059575 jykj-0.0.7/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 06:47:54.000000 jykj-0.0.7/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 06:47:55.068576 jykj-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-25 06:47:43.000000 jykj-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.707391 jykj-0.0.8/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-25 07:36:41.707391 jykj-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.673390 jykj-0.0.8/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.8/jykj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.705406 jykj-0.0.8/jykj/business_model/
+-rw-rw-rw-   0        0        0    17264 2023-06-25 06:46:54.000000 jykj-0.0.8/jykj/business_model/SHE.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.8/jykj/business_model/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.8/jykj/business_model/prevention.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.8/jykj/business_model/production.py
+-rw-rw-rw-   0        0        0    14683 2023-06-25 06:46:56.000000 jykj-0.0.8/jykj/business_model/security.py
+-rw-rw-rw-   0        0        0    28571 2023-06-25 07:34:18.000000 jykj-0.0.8/jykj/business_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.693390 jykj-0.0.8/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:36:41.708391 jykj-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-25 07:36:35.000000 jykj-0.0.8/setup.py
```

### Comparing `jykj-0.0.7/LICENSE` & `jykj-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jykj-0.0.7/jykj/business_model/SHE.py` & `jykj-0.0.8/jykj/business_model/SHE.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.7/jykj/business_model/security.py` & `jykj-0.0.8/jykj/business_model/security.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.7/jykj/business_model/utils.py` & `jykj-0.0.8/jykj/business_model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 
         resolution (list):  [width, height]
     
     返回:
         list: 绝对坐标
     '''
     coords = np.array(coords)
+    single = False
 
     if len(coords.shape) == 1:
+        single = True
         coords = coords[np.newaxis, :]
 
     if (coords.dtype == float) and (coords <= 1).all():
         w, h = resolution
         coords[:, ::2] *= w
         coords[:, 1::2] *= h
     coords = coords.astype(int)
 
-    if coords.shape[0] == 1:
+    if single:
         coords = coords[0]
 
     return coords.tolist()
 
 
 def pnpoly(verts: list, testx: int, testy: int) -> bool:
     '''
```

### Comparing `jykj-0.0.7/setup.py` & `jykj-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jykj",
-    version="0.0.7",
+    version="0.0.8",
     author="jykj",
     author_email="renshuai@jylink.com",
     description="",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

