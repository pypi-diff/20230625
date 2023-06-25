# Comparing `tmp/drupaljsonapiclient-1.0.3.tar.gz` & `tmp/drupaljsonapiclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.3.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.4.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.3.tar` & `drupaljsonapiclient-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/README.md
--rw-r--r--   0        0        0      156 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26340 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28104 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-24 13:39:22.573047 drupaljsonapiclient-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-06-25 01:43:49.049449 drupaljsonapiclient-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1244 2023-06-25 01:43:49.049449 drupaljsonapiclient-1.0.4/README.md
+-rw-r--r--   0        0        0      156 2023-06-25 01:43:49.049449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26345 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28104 2023-06-25 01:43:49.050449 drupaljsonapiclient-1.0.4/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1008 2023-06-25 01:43:49.052449 drupaljsonapiclient-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.4/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.3/LICENSE` & `drupaljsonapiclient-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/README.md` & `drupaljsonapiclient-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/resourceobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
         # If no resources are returned (which is the case when 202 (Accepted)
         # is received for PATCH, for example).
         self.mark_clean()
 
         if status in (HttpStatus.ACCEPTED_202, HttpStatus.CREATED_201):
             return self.session.read(result, location, no_cache=True).resource
         else:
-            return resource
+            return self.resource
 
     async def _commit_async(self, url: str= '', meta=None) -> None:
         self.session.assert_async()
         if self._delete:
             return await self._perform_delete_async(url)
 
         url = self._pre_commit(url)
```

### Comparing `drupaljsonapiclient-1.0.3/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.4/drupaljsonapiclient/session.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.3/pyproject.toml` & `drupaljsonapiclient-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.3"
+version = "1.0.4"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
```

### Comparing `drupaljsonapiclient-1.0.3/PKG-INFO` & `drupaljsonapiclient-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

