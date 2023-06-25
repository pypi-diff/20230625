# Comparing `tmp/drupaljsonapiclient-1.0.5.tar.gz` & `tmp/drupaljsonapiclient-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.5.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.6.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.5.tar` & `drupaljsonapiclient-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/README.md
--rw-r--r--   0        0        0      156 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26336 2023-06-25 02:37:20.452324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28104 2023-06-25 02:37:20.453324 drupaljsonapiclient-1.0.5/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-25 02:37:20.454324 drupaljsonapiclient-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-06-25 05:48:13.209717 drupaljsonapiclient-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1244 2023-06-25 05:48:13.209717 drupaljsonapiclient-1.0.6/README.md
+-rw-r--r--   0        0        0      156 2023-06-25 05:48:13.209717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-25 05:48:13.209717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-06-25 05:48:13.209717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26334 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28104 2023-06-25 05:48:13.210717 drupaljsonapiclient-1.0.6/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1008 2023-06-25 05:48:13.211717 drupaljsonapiclient-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.6/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.5/LICENSE` & `drupaljsonapiclient-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/README.md` & `drupaljsonapiclient-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/resourceobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                                                      resource=resource)
                 elif 'relation' in field_spec:
                     pass  # Special handling for relationships
                 else:
                     self[field_name] = data.pop(field_name, field_spec.get('default'))
 
             if data:
-                logger.warning('There was extra data (not specified in schema): %s',
+                logger.debug('There was extra data (not specified in schema): %s',
                                data)
         # If not, we will use the source data as it is.
         if data:
             self.update(data)
             for key, value in data.items():
                 if isinstance(value, dict):
                     self[key] = AttributeDict(data=value, name=key, parent=self, resource=resource)
```

### Comparing `drupaljsonapiclient-1.0.5/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.6/drupaljsonapiclient/session.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.5/pyproject.toml` & `drupaljsonapiclient-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.5"
+version = "1.0.6"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
```

### Comparing `drupaljsonapiclient-1.0.5/PKG-INFO` & `drupaljsonapiclient-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.5
+Version: 1.0.6
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

