# Comparing `tmp/mathtranslate-3.0.0.tar.gz` & `tmp/mathtranslate-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-3.0.0.tar", last modified: Sun Jun 25 04:59:58 2023, max compression
+gzip compressed data, was "mathtranslate-3.0.1.tar", last modified: Sun Jun 25 06:56:12 2023, max compression
```

## Comparing `mathtranslate-3.0.0.tar` & `mathtranslate-3.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.107079 mathtranslate-3.0.1/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.107079 mathtranslate-3.0.1/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:56:12.107079 mathtranslate-3.0.1/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 06:56:12.000000 mathtranslate-3.0.1/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:56:12.111079 mathtranslate-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-25 06:55:56.000000 mathtranslate-3.0.1/setup.py
```

### Comparing `mathtranslate-3.0.0/LICENSE` & `mathtranslate-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/__init__.py` & `mathtranslate-3.0.1/mathtranslate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __author__ = "MathTranslate developers"
 import os
 from appdata import AppDataPaths
 app_paths = AppDataPaths('mathtranslate')
 app_dir = app_paths.app_data_path
 os.makedirs(app_dir, exist_ok=True)
```

### Comparing `mathtranslate-3.0.0/mathtranslate/cache.py` & `mathtranslate-3.0.1/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/config.py` & `mathtranslate-3.0.1/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/encoding.py` & `mathtranslate-3.0.1/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/process_file.py` & `mathtranslate-3.0.1/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/process_latex.py` & `mathtranslate-3.0.1/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/process_text.py` & `mathtranslate-3.0.1/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencent.py` & `mathtranslate-3.0.1/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-3.0.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/translate.py` & `mathtranslate-3.0.1/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/translate_arxiv.py` & `mathtranslate-3.0.1/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/translate_tex.py` & `mathtranslate-3.0.1/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/upload_overleaf.py` & `mathtranslate-3.0.1/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate/utils.py` & `mathtranslate-3.0.1/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-3.0.1/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-3.0.0/setup.py` & `mathtranslate-3.0.1/setup.py`

 * *Files identical despite different names*

