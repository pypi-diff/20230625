# Comparing `tmp/jmcomic-2.0.7.tar.gz` & `tmp/jmcomic-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.0.7.tar", last modified: Sat Jun 24 09:47:42 2023, max compression
+gzip compressed data, was "jmcomic-2.0.8.tar", last modified: Sun Jun 25 04:33:25 2023, max compression
```

## Comparing `jmcomic-2.0.7.tar` & `jmcomic-2.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.676393 jmcomic-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-24 09:47:28.000000 jmcomic-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-24 09:47:42.676393 jmcomic-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-24 09:47:28.000000 jmcomic-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:47:42.676393 jmcomic-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-24 09:47:28.000000 jmcomic-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.672393 jmcomic-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.672393 jmcomic-2.0.7/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.676393 jmcomic-2.0.7/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:33:25.815193 jmcomic-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 04:33:15.000000 jmcomic-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-25 04:33:25.815193 jmcomic-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-25 04:33:15.000000 jmcomic-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 04:33:25.815193 jmcomic-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-25 04:33:15.000000 jmcomic-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:33:25.811193 jmcomic-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:33:25.815193 jmcomic-2.0.8/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-06-25 04:33:15.000000 jmcomic-2.0.8/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:33:25.815193 jmcomic-2.0.8/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-25 04:33:25.000000 jmcomic-2.0.8/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-25 04:33:25.000000 jmcomic-2.0.8/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 04:33:25.000000 jmcomic-2.0.8/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 04:33:25.000000 jmcomic-2.0.8/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 04:33:25.000000 jmcomic-2.0.8/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.7/LICENSE` & `jmcomic-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/PKG-INFO` & `jmcomic-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.7/README.md` & `jmcomic-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/setup.py` & `jmcomic-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/api.py` & `jmcomic-2.0.8/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.8/src/jmcomic/jm_client_impl.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.8/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_config.py` & `jmcomic-2.0.8/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_entity.py` & `jmcomic-2.0.8/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_option.py` & `jmcomic-2.0.8/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.7/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.8/src/jmcomic/jm_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     def parse_to_photo_id(cls, text) -> str:
         if isinstance(text, int):
             return str(text)
 
         if not isinstance(text, str):
             raise AssertionError(f"无法解析jm车号, 参数类型为: {type(text)}")
 
+        # 43210
+        if text.isdigit():
+            return text
+
+        # Jm43210
         if len(text) <= 2:
             raise AssertionError(f"无法解析jm车号, 文本为: {text}")
 
         # text: JM12341
         c0 = text[0]
         c1 = text[1]
         if (c0 == 'J' or c0 == 'j') and (c1 == 'M' or c1 == 'm'):
```

### Comparing `jmcomic-2.0.7/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.8/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

