# Comparing `tmp/mathtranslate-2.4.4.tar.gz` & `tmp/mathtranslate-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.4.4.tar", last modified: Mon Jun 19 04:45:41 2023, max compression
+gzip compressed data, was "mathtranslate-3.0.0.tar", last modified: Sun Jun 25 04:59:58 2023, max compression
```

## Comparing `mathtranslate-2.4.4.tar` & `mathtranslate-3.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:45:41.051761 mathtranslate-2.4.4/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 04:45:41.000000 mathtranslate-2.4.4/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:45:41.055761 mathtranslate-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 04:45:28.000000 mathtranslate-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 04:59:58.673064 mathtranslate-3.0.0/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 04:59:58.000000 mathtranslate-3.0.0/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 04:59:58.677064 mathtranslate-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-25 04:59:44.000000 mathtranslate-3.0.0/setup.py
```

### Comparing `mathtranslate-2.4.4/LICENSE` & `mathtranslate-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/PKG-INFO` & `mathtranslate-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.4
+Version: 3.0.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.4 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 3.0.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.4/README.md` & `mathtranslate-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/cache.py` & `mathtranslate-3.0.0/mathtranslate/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from . import ROOT
+from . import app_dir
 import os
 import time
 import hashlib
 import shutil
-ROOT_CACHE = os.path.join(ROOT, 'cache')
-os.makedirs(ROOT_CACHE, exist_ok=True)
+cache_dir = os.path.join(app_dir, 'cache')
+os.makedirs(cache_dir, exist_ok=True)
 time_filename = 'update_time'
 max_cache = 5
 
 
 def deterministic_hash(obj):
     hash_object = hashlib.sha256()
     hash_object.update(str(obj).encode())
     return hash_object.hexdigest()[0:20]
 
 
 def get_dirs():
-    dirs = [os.path.join(ROOT_CACHE, dir) for dir in os.listdir(ROOT_CACHE)]
+    dirs = [os.path.join(cache_dir, dir) for dir in os.listdir(cache_dir)]
     return dirs
 
 
 def get_time(dir):
     timefile = os.path.join(dir, time_filename)
     t = float(open(timefile, encoding='utf-8').read())
     return t
@@ -51,28 +51,28 @@
             break
         times = [get_time(dir) for dir in dirs]
         arg = argmin(times)
         shutil.rmtree(dirs[arg])
 
 
 def is_cached(hash_key):
-    dir = os.path.join(ROOT_CACHE, hash_key)
+    dir = os.path.join(cache_dir, hash_key)
     return os.path.exists(dir)
 
 
 def create_cache(hash_key):
-    dir = os.path.join(ROOT_CACHE, hash_key)
+    dir = os.path.join(cache_dir, hash_key)
     os.makedirs(dir, exist_ok=True)
     write_time(dir)
 
 
 def load_paragraph(hash_key, hash_key_paragraph):
-    filename = os.path.join(ROOT_CACHE, hash_key, hash_key_paragraph)
+    filename = os.path.join(cache_dir, hash_key, hash_key_paragraph)
     if os.path.exists(filename):
         return open(filename, encoding='utf-8').read()
     else:
         return None
 
 
 def write_paragraph(hash_key, hash_key_paragraph, paragraph):
-    filename = os.path.join(ROOT_CACHE, hash_key, hash_key_paragraph)
+    filename = os.path.join(cache_dir, hash_key, hash_key_paragraph)
     print(paragraph, file=open(filename, "w", encoding='utf-8'), end='')
```

### Comparing `mathtranslate-2.4.4/mathtranslate/config.py` & `mathtranslate-3.0.0/mathtranslate/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
-from . import ROOT
+from . import app_dir
+default_dir = os.path.join(app_dir, 'default')
+os.makedirs(default_dir, exist_ok=True)
 
 
 class Config:
     default_engine_path = 'DEFAULT_ENGINE'
     default_language_from_path = 'DEFAULT_LANGUAGE_FROM'
     default_language_to_path = 'DEFAULT_LANGUAGE_TO'
     default_loading_dir_path = 'DEFAULT_LOADING_DIR'
@@ -16,40 +18,40 @@
     default_language_to_default = 'zh-CN'
     default_loading_dir_default = os.path.expanduser("~")
     default_saving_dir_default = os.path.expanduser("~")
     tencent_secret_id_default = None
     tencent_secret_key_default = None
 
     math_code = 'XMATHX'
-    log_file = f'{ROOT}/translate_log'
+    log_file = f'{app_dir}/translate_log'
 
     def __init__(self):
         self.load()
-        if os.path.exists(f'{ROOT}/TEST'):
+        if os.path.exists(f'{app_dir}/TEST'):
             self.test_environment = True
             print('This is a test environment!')
         else:
             self.test_environment = False
 
     @staticmethod
     def read_variable(path, default):
-        if os.path.exists(f'{ROOT}/{path}'):
-            return open(f'{ROOT}/{path}').read().replace(' ', '').replace('\n', '')
+        if os.path.exists(f'{default_dir}/{path}'):
+            return open(f'{default_dir}/{path}').read().replace(' ', '').replace('\n', '')
         else:
             return default
 
     @staticmethod
     def set_variable(path, default):
         var = input().replace(' ', '').replace('\n', '')
         if var != '':
-            print(var, file=open(f'{ROOT}/{path}', 'w'))
+            print(var, file=open(f'{default_dir}/{path}', 'w'))
 
     @staticmethod
     def set_variable_4ui(path, var):
-        print(var, file=open(f'{ROOT}/{path}', 'w'))
+        print(var, file=open(f'{default_dir}/{path}', 'w'))
 
     def load(self):
         self.default_engine = self.read_variable(self.default_engine_path, self.default_engine_default)
         self.default_language_from = self.read_variable(self.default_language_from_path, self.default_language_from_default)
         self.default_language_to = self.read_variable(self.default_language_to_path, self.default_language_to_default)
         self.tencent_secret_id = self.read_variable(self.tencent_secret_id_path, self.tencent_secret_id_default)
         self.tencent_secret_key = self.read_variable(self.tencent_secret_key_path, self.tencent_secret_key_default)
```

### Comparing `mathtranslate-2.4.4/mathtranslate/encoding.py` & `mathtranslate-3.0.0/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/process_file.py` & `mathtranslate-3.0.0/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/process_latex.py` & `mathtranslate-3.0.0/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/process_text.py` & `mathtranslate-3.0.0/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencent.py` & `mathtranslate-3.0.0/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-3.0.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/translate.py` & `mathtranslate-3.0.0/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/translate_arxiv.py` & `mathtranslate-3.0.0/mathtranslate/translate_arxiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import utils
 from . import process_latex
 from . import process_file
 from .translate import translate_single_tex_file
 from .encoding import get_file_encoding
-from . import ROOT
+from . import app_dir
 import os
 import sys
 import shutil
 import gzip
 import zipfile
 import tarfile
 import tempfile
@@ -17,15 +17,15 @@
 def download_source(number, path):
     url = f'https://arxiv.org/e-print/{number}'
     print('trying to download from', url)
     urllib.request.urlretrieve(url, path)
 
 
 def download_source_with_cache(number, path):
-    cache_dir = os.path.join(ROOT, 'cache_arxiv')
+    cache_dir = os.path.join(app_dir, 'cache_arxiv')
     os.makedirs(cache_dir, exist_ok=True)
     cache_path = os.path.join(cache_dir, 'last_downloaded_source')
     cache_number_path = os.path.join(cache_dir, 'last_arxiv_number')
     if os.path.exists(cache_path) and os.path.exists(cache_number_path):
         last_number = open(cache_number_path).read()
         if last_number == number:
             shutil.copyfile(cache_path, path)
```

### Comparing `mathtranslate-2.4.4/mathtranslate/translate_tex.py` & `mathtranslate-3.0.0/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/upload_overleaf.py` & `mathtranslate-3.0.0/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate/utils.py` & `mathtranslate-3.0.0/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-3.0.0/mathtranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.4
+Version: 3.0.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.4 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 3.0.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.4/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-3.0.0/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.4/setup.py` & `mathtranslate-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["mtranslate",
                       "charset-normalizer",
                       "requests",
                       "regex",
                       "tqdm",
+                      "appdata"
                       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
```

