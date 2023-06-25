# Comparing `tmp/dk_google-0.0.3.tar.gz` & `tmp/dk_google-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dk_google-0.0.3.tar", last modified: Sun Jun 25 16:47:12 2023, max compression
+gzip compressed data, was "dk_google-0.0.31.tar", last modified: Sun Jun 25 16:48:46 2023, max compression
```

## Comparing `dk_google-0.0.3.tar` & `dk_google-0.0.31.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 16:47:12.453946 dk_google-0.0.3/
--rw-rw-rw-   0        0        0      237 2023-06-25 16:47:12.453946 dk_google-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-24 13:34:34.000000 dk_google-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 16:47:12.444544 dk_google-0.0.3/dk_google/
--rw-rw-rw-   0        0        0     8709 2023-06-24 17:56:33.000000 dk_google-0.0.3/dk_google/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:47:12.449752 dk_google-0.0.3/dk_google/cloud/
--rw-rw-rw-   0        0        0     4495 2023-06-20 14:22:42.000000 dk_google-0.0.3/dk_google/cloud/__init__.py
--rw-rw-rw-   0        0        0     4036 2023-05-31 15:58:52.000000 dk_google-0.0.3/dk_google/cloud/bigquery.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:47:12.452948 dk_google-0.0.3/dk_google/cloud/iam/
--rw-rw-rw-   0        0        0      116 2023-06-23 15:19:35.000000 dk_google-0.0.3/dk_google/cloud/iam/__init__.py
--rw-rw-rw-   0        0        0     3962 2023-06-23 15:06:06.000000 dk_google-0.0.3/dk_google/cloud/iam/account_client.py
--rw-rw-rw-   0        0        0    10044 2023-06-23 14:54:46.000000 dk_google-0.0.3/dk_google/cloud/iam/account_object.py
--rw-rw-rw-   0        0        0     5164 2023-06-23 22:46:25.000000 dk_google-0.0.3/dk_google/cloud/iam/helpers.py
--rw-rw-rw-   0        0        0     2638 2023-06-23 15:08:06.000000 dk_google-0.0.3/dk_google/cloud/iam/key_client.py
--rw-rw-rw-   0        0        0     3151 2023-06-23 11:34:23.000000 dk_google-0.0.3/dk_google/config.py
--rw-rw-rw-   0        0        0     6094 2023-06-23 21:36:46.000000 dk_google-0.0.3/dk_google/github.py
--rw-rw-rw-   0        0        0     8350 2023-06-20 17:04:15.000000 dk_google-0.0.3/dk_google/helpers.py
--rw-rw-rw-   0        0        0     7356 2023-06-20 13:27:00.000000 dk_google-0.0.3/dk_google/local.py
--rw-rw-rw-   0        0        0      210 2023-05-24 21:18:35.000000 dk_google-0.0.3/dk_google/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:47:12.448098 dk_google-0.0.3/dk_google.egg-info/
--rw-rw-rw-   0        0        0      237 2023-06-25 16:47:12.000000 dk_google-0.0.3/dk_google.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-06-25 16:47:12.000000 dk_google-0.0.3/dk_google.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 16:47:12.000000 dk_google-0.0.3/dk_google.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1575 2023-06-25 16:47:12.000000 dk_google-0.0.3/dk_google.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-25 16:47:12.000000 dk_google-0.0.3/dk_google.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 16:47:12.454948 dk_google-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-06-25 16:46:58.000000 dk_google-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:48:46.045374 dk_google-0.0.31/
+-rw-rw-rw-   0        0        0      238 2023-06-25 16:48:46.045374 dk_google-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-24 13:34:34.000000 dk_google-0.0.31/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 16:48:46.036110 dk_google-0.0.31/dk_google/
+-rw-rw-rw-   0        0        0     8709 2023-06-24 17:56:33.000000 dk_google-0.0.31/dk_google/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:48:46.041682 dk_google-0.0.31/dk_google/cloud/
+-rw-rw-rw-   0        0        0     4495 2023-06-20 14:22:42.000000 dk_google-0.0.31/dk_google/cloud/__init__.py
+-rw-rw-rw-   0        0        0     4036 2023-05-31 15:58:52.000000 dk_google-0.0.31/dk_google/cloud/bigquery.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:48:46.045374 dk_google-0.0.31/dk_google/cloud/iam/
+-rw-rw-rw-   0        0        0      116 2023-06-23 15:19:35.000000 dk_google-0.0.31/dk_google/cloud/iam/__init__.py
+-rw-rw-rw-   0        0        0     3962 2023-06-23 15:06:06.000000 dk_google-0.0.31/dk_google/cloud/iam/account_client.py
+-rw-rw-rw-   0        0        0    10044 2023-06-23 14:54:46.000000 dk_google-0.0.31/dk_google/cloud/iam/account_object.py
+-rw-rw-rw-   0        0        0     5164 2023-06-23 22:46:25.000000 dk_google-0.0.31/dk_google/cloud/iam/helpers.py
+-rw-rw-rw-   0        0        0     2638 2023-06-23 15:08:06.000000 dk_google-0.0.31/dk_google/cloud/iam/key_client.py
+-rw-rw-rw-   0        0        0     3151 2023-06-23 11:34:23.000000 dk_google-0.0.31/dk_google/config.py
+-rw-rw-rw-   0        0        0     6094 2023-06-23 21:36:46.000000 dk_google-0.0.31/dk_google/github.py
+-rw-rw-rw-   0        0        0     8350 2023-06-20 17:04:15.000000 dk_google-0.0.31/dk_google/helpers.py
+-rw-rw-rw-   0        0        0     7356 2023-06-20 13:27:00.000000 dk_google-0.0.31/dk_google/local.py
+-rw-rw-rw-   0        0        0      210 2023-05-24 21:18:35.000000 dk_google-0.0.31/dk_google/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:48:46.039689 dk_google-0.0.31/dk_google.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-06-25 16:48:45.000000 dk_google-0.0.31/dk_google.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-06-25 16:48:45.000000 dk_google-0.0.31/dk_google.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:48:45.000000 dk_google-0.0.31/dk_google.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1575 2023-06-25 16:48:45.000000 dk_google-0.0.31/dk_google.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 16:48:45.000000 dk_google-0.0.31/dk_google.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 16:48:46.046999 dk_google-0.0.31/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-06-25 16:48:37.000000 dk_google-0.0.31/setup.py
```

### Comparing `dk_google-0.0.3/dk_google/__init__.py` & `dk_google-0.0.31/dk_google/__init__.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/__init__.py` & `dk_google-0.0.31/dk_google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/bigquery.py` & `dk_google-0.0.31/dk_google/cloud/bigquery.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/iam/account_client.py` & `dk_google-0.0.31/dk_google/cloud/iam/account_client.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/iam/account_object.py` & `dk_google-0.0.31/dk_google/cloud/iam/account_object.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/iam/helpers.py` & `dk_google-0.0.31/dk_google/cloud/iam/helpers.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/cloud/iam/key_client.py` & `dk_google-0.0.31/dk_google/cloud/iam/key_client.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/config.py` & `dk_google-0.0.31/dk_google/config.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/github.py` & `dk_google-0.0.31/dk_google/github.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/helpers.py` & `dk_google-0.0.31/dk_google/helpers.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google/local.py` & `dk_google-0.0.31/dk_google/local.py`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google.egg-info/SOURCES.txt` & `dk_google-0.0.31/dk_google.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/dk_google.egg-info/requires.txt` & `dk_google-0.0.31/dk_google.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dk_google-0.0.3/setup.py` & `dk_google-0.0.31/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pip._internal.req import parse_requirements
 
 install_reqs = list(parse_requirements('requirements.txt', session = 'dummy'))
 reqs = [str(ir.requirement) for ir in install_reqs if ir.requirement.find('win') < 0]
 
 setup(
     name = 'dk_google',
-    version = '0.0.3',
+    version = '0.0.31',
     author = 'Dzmitry Kobzarau',
     author_email = 'kobzaraydzmitry@gmail.com',
     description = 'Data Engineering helping tools on Google-Cloud',
     long_description = '',
     url = 'https://github.com/dmitry-kobzarev/dk_google',
     packages = find_namespace_packages(include = ['dk_google', 'dk_google.*']),    
     install_requires = reqs,
```

