# Comparing `tmp/superpowered-sdk-0.1.8.tar.gz` & `tmp/superpowered-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.8.tar", last modified: Wed Jun 14 21:54:24 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.9.tar", last modified: Sun Jun 25 18:05:55 2023, max compression
```

## Comparing `superpowered-sdk-0.1.8.tar` & `superpowered-sdk-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.575136 superpowered-sdk-0.1.8/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/superpowered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.575136 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:05:55.911498 superpowered-sdk-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-25 18:05:55.911498 superpowered-sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-25 18:05:41.000000 superpowered-sdk-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:05:55.911498 superpowered-sdk-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-25 18:05:41.000000 superpowered-sdk-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:05:55.911498 superpowered-sdk-0.1.9/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-25 18:05:41.000000 superpowered-sdk-0.1.9/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-25 18:05:41.000000 superpowered-sdk-0.1.9/superpowered/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-25 18:05:41.000000 superpowered-sdk-0.1.9/superpowered/superpowered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:05:55.911498 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-25 18:05:55.000000 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-25 18:05:55.000000 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:05:55.000000 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 18:05:55.000000 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 18:05:55.000000 superpowered-sdk-0.1.9/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.8/PKG-INFO` & `superpowered-sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.9 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

### Comparing `superpowered-sdk-0.1.8/README.md` & `superpowered-sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.8/setup.py` & `superpowered-sdk-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.8/superpowered/__init__.py` & `superpowered-sdk-0.1.9/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.8/superpowered/exceptions.py` & `superpowered-sdk-0.1.9/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.8/superpowered/superpowered.py` & `superpowered-sdk-0.1.9/superpowered/superpowered.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             try:
                 raise ERRORS[error_code]['python_sdk_exception'](resp_json, resp.status_code)
             except KeyError:
                 raise Exception(resp_json, resp.status_code)
         else:
             raise Exception(resp_json, resp.status_code)
     elif not resp.ok:
-        print(args)
         raise Exception(resp_json, resp.status_code)
     else:
         return resp_json
 
 
 def get_total_storage():
     """
@@ -140,61 +139,65 @@
         'method': 'DELETE',
         'url': f'{get_base_url()}/knowledge_bases/{knowledge_base_id}',
         'auth': auth(),
     }
     return make_api_call(args)
 
 
-def create_document_via_text(knowledge_base_id: str, content: str, title: str = None, link_to_source: str = None, description: str = None, supp_id: str = None) -> dict:
+def create_document_via_text(knowledge_base_id: str, content: str, title: str = None, link_to_source: str = None, description: str = None, supp_id: str = None, chunk_header: str = None) -> dict:
     """
     POST /knowledge_bases/{knowledge_base_id}/documents/raw_text
     """
     data = {
         'content': content,
     }
     if title:
         data['title'] = title
     if description:
         data['description'] = description
     if supp_id:
         data['supp_id'] = supp_id
     if link_to_source:
         data['link_to_source'] = link_to_source
+    if chunk_header:
+        data['chunk_header'] = chunk_header
     args = {
         'method': 'POST',
         'url': f'{get_base_url()}/knowledge_bases/{knowledge_base_id}/documents/raw_text',
         'json': data,
         'auth': auth(),
     }
     return make_api_call(args)
 
 
-def create_document_via_url(knowledge_base_id: str, url: str, title: str = None, description: str = None, supp_id: str = None) -> dict:
+def create_document_via_url(knowledge_base_id: str, url: str, title: str = None, description: str = None, supp_id: str = None, chunk_header: str = None) -> dict:
     """
     POST /knowledge_bases/{knowledge_base_id}/documents/url
     """
     data = {
         'url': url,
     }
     if title:
         data['title'] = title
     if description:
         data['description'] = description
     if supp_id:
         data['supp_id'] = supp_id
+    if chunk_header:
+        data['chunk_header'] = chunk_header
     args = {
         'method': 'POST',
         'url': f'{get_base_url()}/knowledge_bases/{knowledge_base_id}/documents/url',
         'json': data,
         'auth': auth(),
     }
     return make_api_call(args)
 
 
-def create_document_via_file(knowledge_base_id: str, file_path: str, description: str = None, supp_id: str = None) -> dict:
+def create_document_via_file(knowledge_base_id: str, file_path: str, description: str = None, supp_id: str = None, chunk_header: str = None) -> dict:
     """
     POST /knowledge_bases/{knowledge_base_id}/documents/request_signed_file_url
     +
     PUT response['temporary_url']
     """
     # read the file and get the encoded md5 for the presigned url request
     with open(file_path, 'rb') as f:
@@ -208,14 +211,16 @@
         'method': 'PUT',
         'encoded_md5': encoded_md5,
     }
     if description:
         data['description'] = description
     if supp_id:
         data['supp_id'] = supp_id
+    if chunk_header:
+        data['chunk_header'] = chunk_header
 
     args = {
         'method': 'POST',
         'url': f'{get_base_url()}/knowledge_bases/{knowledge_base_id}/documents/request_signed_file_url',
         'json': data,
         'auth': auth(),
     }
```

### Comparing `superpowered-sdk-0.1.8/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.9/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.9 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

