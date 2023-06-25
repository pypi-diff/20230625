# Comparing `tmp/alibabacloud_ros20190910-3.2.8.tar.gz` & `tmp/alibabacloud_ros20190910-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ros20190910-3.2.8.tar", last modified: Thu Jul 21 07:55:32 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ros20190910-3.2.9.tar", last modified: Wed Aug 17 02:25:02 2022, max compression
```

## Comparing `alibabacloud_ros20190910-3.2.8.tar` & `alibabacloud_ros20190910-3.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/
--rw-r--r--   0 root         (0) root         (0)     3932 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/__init__.py
--rw-r--r--   0 root         (0) root         (0)   285305 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/client.py
--rw-r--r--   0 root         (0) root         (0)   589773 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2637 2022-07-21 07:55:32.000000 alibabacloud_ros20190910-3.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/
+-rw-r--r--   0 root         (0) root         (0)     4016 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2355 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   285305 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/client.py
+-rw-r--r--   0 root         (0) root         (0)   591054 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2355 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2022-08-17 02:25:02.000000 alibabacloud_ros20190910-3.2.9/setup.py
```

### Comparing `alibabacloud_ros20190910-3.2.8/ChangeLog.md` & `alibabacloud_ros20190910-3.2.9/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-07-21 Version: 3.2.8
+- GetTemplateSummary support Parameters and ClientToken.
+
 2022-07-13 Version: 3.2.7
 - PreviewStack adds StackId and returns Action to support preview stack update.
 
 2022-06-30 Version: 3.2.6
 - ValidateTemplate returns ResourceTypes.
 - GetStackResource supports ResourceAttributes.
 - GetStack supports LogOption and returns ResourceLogs.
```

### Comparing `alibabacloud_ros20190910-3.2.8/LICENSE` & `alibabacloud_ros20190910-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.2.8/PKG-INFO` & `alibabacloud_ros20190910-3.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ros20190910
-Version: 3.2.8
+Version: 3.2.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910-3.2.8/README-CN.md` & `alibabacloud_ros20190910-3.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.2.8/README.md` & `alibabacloud_ros20190910-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/client.py` & `alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910/models.py` & `alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4718,54 +4718,89 @@
         if m.get('SupportedResourceTypes') is not None:
             for k in m.get('SupportedResourceTypes'):
                 temp_model = GetFeatureDetailsResponseBodyTemplateScratchSupportedResourceTypes()
                 self.supported_resource_types.append(temp_model.from_map(k))
         return self
 
 
+class GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk(TeaModel):
+    def __init__(
+        self,
+        delete_stack: List[str] = None,
+    ):
+        self.delete_stack = delete_stack
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.delete_stack is not None:
+            result['DeleteStack'] = self.delete_stack
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeleteStack') is not None:
+            self.delete_stack = m.get('DeleteStack')
+        return self
+
+
 class GetFeatureDetailsResponseBodyTerraformSupportedResourceTypes(TeaModel):
     def __init__(
         self,
         custom_tag: List[str] = None,
         estimate_cost: List[str] = None,
         resource_group: List[str] = None,
+        stack_operation_risk: GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk = None,
         system_tag: List[str] = None,
     ):
         self.custom_tag = custom_tag
         self.estimate_cost = estimate_cost
         self.resource_group = resource_group
+        self.stack_operation_risk = stack_operation_risk
         self.system_tag = system_tag
 
     def validate(self):
-        pass
+        if self.stack_operation_risk:
+            self.stack_operation_risk.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.custom_tag is not None:
             result['CustomTag'] = self.custom_tag
         if self.estimate_cost is not None:
             result['EstimateCost'] = self.estimate_cost
         if self.resource_group is not None:
             result['ResourceGroup'] = self.resource_group
+        if self.stack_operation_risk is not None:
+            result['StackOperationRisk'] = self.stack_operation_risk.to_map()
         if self.system_tag is not None:
             result['SystemTag'] = self.system_tag
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CustomTag') is not None:
             self.custom_tag = m.get('CustomTag')
         if m.get('EstimateCost') is not None:
             self.estimate_cost = m.get('EstimateCost')
         if m.get('ResourceGroup') is not None:
             self.resource_group = m.get('ResourceGroup')
+        if m.get('StackOperationRisk') is not None:
+            temp_model = GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk()
+            self.stack_operation_risk = temp_model.from_map(m['StackOperationRisk'])
         if m.get('SystemTag') is not None:
             self.system_tag = m.get('SystemTag')
         return self
 
 
 class GetFeatureDetailsResponseBodyTerraformSupportedVersionsProviderVersions(TeaModel):
     def __init__(
@@ -13492,15 +13527,14 @@
 
 
 class MoveResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_ros20190910-3.2.8/alibabacloud_ros20190910.egg-info/PKG-INFO` & `alibabacloud_ros20190910-3.2.9/alibabacloud_ros20190910.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros20190910
-Version: 3.2.8
+Version: 3.2.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910-3.2.8/setup.py` & `alibabacloud_ros20190910-3.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ros20190910.
 
-Created on 21/07/2022
+Created on 17/08/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ros20190910"
 NAME = "alibabacloud_ros20190910" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python"
```

