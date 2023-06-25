# Comparing `tmp/gcloud-secret-configure-0.0.3.tar.gz` & `tmp/gcloud-secret-configure-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud-secret-configure-0.0.3.tar", last modified: Sun Jun 25 17:47:02 2023, max compression
+gzip compressed data, was "gcloud-secret-configure-1.0.0.tar", last modified: Sun Jun 25 17:55:23 2023, max compression
```

## Comparing `gcloud-secret-configure-0.0.3.tar` & `gcloud-secret-configure-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-25 15:20:19.000000 gcloud-secret-configure-0.0.3/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/PKG-INFO
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.545891 gcloud-secret-configure-0.0.3/gcloud_secret_configure/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 13:43:23.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2767 2023-06-25 17:18:11.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/config.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1283 2023-06-25 17:43:04.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/secret.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.549890 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      464 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       30 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      673 2023-06-25 17:46:49.000000 gcloud-secret-configure-0.0.3/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 14:59:34.000000 gcloud-secret-configure-0.0.3/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2426 2023-06-25 17:24:09.000000 gcloud-secret-configure-0.0.3/tests/test_config_get.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1244 2023-06-25 16:07:25.000000 gcloud-secret-configure-0.0.3/tests/test_config_integration.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1926 2023-06-25 14:54:53.000000 gcloud-secret-configure-0.0.3/tests/test_config_parse.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1721 2023-06-25 14:58:19.000000 gcloud-secret-configure-0.0.3/tests/test_config_repository.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      965 2023-06-25 17:44:08.000000 gcloud-secret-configure-0.0.3/tests/test_secret.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:55:23.647031 gcloud-secret-configure-1.0.0/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-25 15:20:19.000000 gcloud-secret-configure-1.0.0/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      528 2023-06-25 17:55:23.647031 gcloud-secret-configure-1.0.0/PKG-INFO
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:55:23.643031 gcloud-secret-configure-1.0.0/gcloud_secret_configure/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 13:43:23.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2767 2023-06-25 17:18:11.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure/config.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1283 2023-06-25 17:43:04.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure/secret.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:55:23.647031 gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      528 2023-06-25 17:55:23.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      464 2023-06-25 17:55:23.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-25 17:55:23.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       30 2023-06-25 17:55:23.000000 gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-25 17:55:23.647031 gcloud-secret-configure-1.0.0/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      681 2023-06-25 17:55:18.000000 gcloud-secret-configure-1.0.0/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:55:23.647031 gcloud-secret-configure-1.0.0/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 14:59:34.000000 gcloud-secret-configure-1.0.0/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2426 2023-06-25 17:24:09.000000 gcloud-secret-configure-1.0.0/tests/test_config_get.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1244 2023-06-25 16:07:25.000000 gcloud-secret-configure-1.0.0/tests/test_config_integration.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1926 2023-06-25 14:54:53.000000 gcloud-secret-configure-1.0.0/tests/test_config_parse.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1721 2023-06-25 14:58:19.000000 gcloud-secret-configure-1.0.0/tests/test_config_repository.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      965 2023-06-25 17:44:08.000000 gcloud-secret-configure-1.0.0/tests/test_secret.py
```

### Comparing `gcloud-secret-configure-0.0.3/LICENSE` & `gcloud-secret-configure-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/PKG-INFO` & `gcloud-secret-configure-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gcloud-secret-configure
-Version: 0.0.3
+Version: 1.0.0
 Summary: A package to configure environment variables from Google Cloud Secret Manager
 Home-page: https://github.com/masatoEmata/cloud_secret_configure
 Author: Masato Emata
 Keywords: google cloud secret manager environment variables
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `gcloud-secret-configure-0.0.3/gcloud_secret_configure/config.py` & `gcloud-secret-configure-1.0.0/gcloud_secret_configure/config.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/gcloud_secret_configure/secret.py` & `gcloud-secret-configure-1.0.0/gcloud_secret_configure/secret.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/PKG-INFO` & `gcloud-secret-configure-1.0.0/gcloud_secret_configure.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gcloud-secret-configure
-Version: 0.0.3
+Version: 1.0.0
 Summary: A package to configure environment variables from Google Cloud Secret Manager
 Home-page: https://github.com/masatoEmata/cloud_secret_configure
 Author: Masato Emata
 Keywords: google cloud secret manager environment variables
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `gcloud-secret-configure-0.0.3/setup.py` & `gcloud-secret-configure-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name="gcloud-secret-configure",
-    version="0.0.3",
+    version="1.0.0",
     description="A package to configure environment variables from Google Cloud Secret Manager",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # https://pypi.org/classifiers/
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     author="Masato Emata",
     url="https://github.com/masatoEmata/cloud_secret_configure",
     keywords="google cloud secret manager environment variables",
```

### Comparing `gcloud-secret-configure-0.0.3/tests/test_config_get.py` & `gcloud-secret-configure-1.0.0/tests/test_config_get.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/tests/test_config_integration.py` & `gcloud-secret-configure-1.0.0/tests/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/tests/test_config_parse.py` & `gcloud-secret-configure-1.0.0/tests/test_config_parse.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/tests/test_config_repository.py` & `gcloud-secret-configure-1.0.0/tests/test_config_repository.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.3/tests/test_secret.py` & `gcloud-secret-configure-1.0.0/tests/test_secret.py`

 * *Files identical despite different names*

