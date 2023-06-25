# Comparing `tmp/gcloud-secret-configure-0.0.2.tar.gz` & `tmp/gcloud-secret-configure-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud-secret-configure-0.0.2.tar", last modified: Sun Jun 25 17:25:00 2023, max compression
+gzip compressed data, was "gcloud-secret-configure-0.0.3.tar", last modified: Sun Jun 25 17:47:02 2023, max compression
```

## Comparing `gcloud-secret-configure-0.0.2.tar` & `gcloud-secret-configure-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:25:00.557664 gcloud-secret-configure-0.0.2/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-25 15:20:19.000000 gcloud-secret-configure-0.0.2/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:25:00.557664 gcloud-secret-configure-0.0.2/PKG-INFO
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:25:00.553663 gcloud-secret-configure-0.0.2/gcloud_secret_configure/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 13:43:23.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2767 2023-06-25 17:18:11.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure/config.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1107 2023-06-25 17:17:22.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure/secret.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:25:00.553663 gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:25:00.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      464 2023-06-25 17:25:00.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-25 17:25:00.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       30 2023-06-25 17:25:00.000000 gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-25 17:25:00.557664 gcloud-secret-configure-0.0.2/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      673 2023-06-25 17:24:58.000000 gcloud-secret-configure-0.0.2/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:25:00.557664 gcloud-secret-configure-0.0.2/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 14:59:34.000000 gcloud-secret-configure-0.0.2/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2426 2023-06-25 17:24:09.000000 gcloud-secret-configure-0.0.2/tests/test_config_get.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1244 2023-06-25 16:07:25.000000 gcloud-secret-configure-0.0.2/tests/test_config_integration.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1926 2023-06-25 14:54:53.000000 gcloud-secret-configure-0.0.2/tests/test_config_parse.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1721 2023-06-25 14:58:19.000000 gcloud-secret-configure-0.0.2/tests/test_config_repository.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      822 2023-06-25 15:10:49.000000 gcloud-secret-configure-0.0.2/tests/test_secret.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-25 15:20:19.000000 gcloud-secret-configure-0.0.3/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/PKG-INFO
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.545891 gcloud-secret-configure-0.0.3/gcloud_secret_configure/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 13:43:23.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2767 2023-06-25 17:18:11.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/config.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1283 2023-06-25 17:43:04.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure/secret.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.549890 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      520 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      464 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       30 2023-06-25 17:47:02.000000 gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      673 2023-06-25 17:46:49.000000 gcloud-secret-configure-0.0.3/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 17:47:02.553890 gcloud-secret-configure-0.0.3/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-25 14:59:34.000000 gcloud-secret-configure-0.0.3/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2426 2023-06-25 17:24:09.000000 gcloud-secret-configure-0.0.3/tests/test_config_get.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1244 2023-06-25 16:07:25.000000 gcloud-secret-configure-0.0.3/tests/test_config_integration.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1926 2023-06-25 14:54:53.000000 gcloud-secret-configure-0.0.3/tests/test_config_parse.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1721 2023-06-25 14:58:19.000000 gcloud-secret-configure-0.0.3/tests/test_config_repository.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      965 2023-06-25 17:44:08.000000 gcloud-secret-configure-0.0.3/tests/test_secret.py
```

### Comparing `gcloud-secret-configure-0.0.2/LICENSE` & `gcloud-secret-configure-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/PKG-INFO` & `gcloud-secret-configure-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-secret-configure
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to configure environment variables from Google Cloud Secret Manager
 Home-page: https://github.com/masatoEmata/cloud_secret_configure
 Author: Masato Emata
 Keywords: google cloud secret manager environment variables
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gcloud-secret-configure-0.0.2/gcloud_secret_configure/config.py` & `gcloud-secret-configure-0.0.3/gcloud_secret_configure/config.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/gcloud_secret_configure/secret.py` & `gcloud-secret-configure-0.0.3/gcloud_secret_configure/secret.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from io import StringIO
 from typing import Optional
 
 import google.auth
 from google.auth.exceptions import DefaultCredentialsError
 from google.cloud import secretmanager
 
 
@@ -17,15 +18,21 @@
 
 
 class GoogleSecretFetcher(SecretFetcher):
     """
     Concrete implementation for fetching secrets from Google Cloud.
     """
 
-    def fetch_secret(self, secret_label="env_file", version="latest") -> Optional[str]:
+    def fetch_secret(
+        self, secret_label="env_file", version="latest"
+    ) -> Optional[StringIO]:
+        """
+        Fetches the secret from Google Secret Manager
+        and returns it as a StringIO object.
+        """
         try:
             _, project_id = google.auth.default()
         except DefaultCredentialsError:
             project_id = None
 
         if project_id is None:
             return None
@@ -35,8 +42,8 @@
         gcloud_secret_name = (
             f"projects/{project_id}/secrets/{secret_label}/versions/{version}"
         )
 
         payload = client.access_secret_version(
             name=gcloud_secret_name
         ).payload.data.decode("UTF-8")
-        return payload
+        return StringIO(payload)
```

### Comparing `gcloud-secret-configure-0.0.2/gcloud_secret_configure.egg-info/PKG-INFO` & `gcloud-secret-configure-0.0.3/gcloud_secret_configure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-secret-configure
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to configure environment variables from Google Cloud Secret Manager
 Home-page: https://github.com/masatoEmata/cloud_secret_configure
 Author: Masato Emata
 Keywords: google cloud secret manager environment variables
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gcloud-secret-configure-0.0.2/setup.py` & `gcloud-secret-configure-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="gcloud-secret-configure",
-    version="0.0.2",
+    version="0.0.3",
     description="A package to configure environment variables from Google Cloud Secret Manager",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # https://pypi.org/classifiers/
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gcloud-secret-configure-0.0.2/tests/test_config_get.py` & `gcloud-secret-configure-0.0.3/tests/test_config_get.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/tests/test_config_integration.py` & `gcloud-secret-configure-0.0.3/tests/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/tests/test_config_parse.py` & `gcloud-secret-configure-0.0.3/tests/test_config_parse.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/tests/test_config_repository.py` & `gcloud-secret-configure-0.0.3/tests/test_config_repository.py`

 * *Files identical despite different names*

### Comparing `gcloud-secret-configure-0.0.2/tests/test_secret.py` & `gcloud-secret-configure-0.0.3/tests/test_secret.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import StringIO
 from unittest.mock import patch
 
 from google.auth.exceptions import DefaultCredentialsError
 
 from gcloud_secret_configure.secret import GoogleSecretFetcher
 
 
@@ -10,13 +11,15 @@
 def test_fetch_secret(mock_auth_default, mock_secret_client):
     # Test for normal operation
     mock_auth_default.return_value = (None, "test_project")
     mock_secret_client.return_value.access_secret_version.return_value.payload.data.decode.return_value = (
         "test_secret"
     )
     fetcher = GoogleSecretFetcher()
-    assert fetcher.fetch_secret() == "test_secret"
+    result = fetcher.fetch_secret()
+    assert isinstance(result, StringIO)  # assert the return type
+    assert result.getvalue() == "test_secret"  # assert the content
 
     # english: Test for authentication error
     mock_auth_default.side_effect = DefaultCredentialsError("Error")
     fetcher = GoogleSecretFetcher()
     assert fetcher.fetch_secret() is None
```

