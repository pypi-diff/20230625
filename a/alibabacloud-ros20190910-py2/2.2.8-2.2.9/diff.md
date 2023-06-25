# Comparing `tmp/alibabacloud_ros20190910_py2-2.2.8.tar.gz` & `tmp/alibabacloud_ros20190910_py2-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ros20190910_py2-2.2.8.tar", last modified: Thu Jul 21 07:55:11 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ros20190910_py2-2.2.9.tar", last modified: Mon Sep  5 01:32:20 2022, max compression
```

## Comparing `alibabacloud_ros20190910_py2-2.2.8.tar` & `alibabacloud_ros20190910_py2-2.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/
--rw-r--r--   0 root         (0) root         (0)     2980 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2499 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/__init__.py
--rw-r--r--   0 root         (0) root         (0)   122377 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/client.py
--rw-r--r--   0 root         (0) root         (0)   594644 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2499 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2930 2022-07-21 07:55:11.000000 alibabacloud_ros20190910_py2-2.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/
+-rw-r--r--   0 root         (0) root         (0)     3064 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2499 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122883 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/client.py
+-rw-r--r--   0 root         (0) root         (0)   607057 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2499 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2930 2022-09-05 01:32:20.000000 alibabacloud_ros20190910_py2-2.2.9/setup.py
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/ChangeLog.md` & `alibabacloud_ros20190910_py2-2.2.9/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-07-21 Version: 2.2.8
+- GetTemplateSummary support Parameters and ClientToken.
+
 2022-07-13 Version: 2.2.7
 - PreviewStack adds StackId and returns Action to support preview stack update.
 
 2022-06-30 Version: 2.2.6
 - ValidateTemplate returns ResourceTypes.
 - GetStackResource supports ResourceAttributes.
 - GetStack supports LogOption and returns ResourceLogs.
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/LICENSE` & `alibabacloud_ros20190910_py2-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910_py2-2.2.8/PKG-INFO` & `alibabacloud_ros20190910_py2-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ros20190910_py2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/README-CN.md` & `alibabacloud_ros20190910_py2-2.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910_py2-2.2.8/README.md` & `alibabacloud_ros20190910_py2-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/client.py` & `alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2154,27 +2154,33 @@
             self.call_api(params, req, runtime)
         )
 
     def move_resource_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.move_resource_group_with_options(request, runtime)
 
-    def preview_stack_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
+    def preview_stack_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = ros20190910_models.PreviewStackShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.resource_config_rules):
+            request.resource_config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_config_rules, 'ResourceConfigRules', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.disable_rollback):
             query['DisableRollback'] = request.disable_rollback
         if not UtilClient.is_unset(request.parallelism):
             query['Parallelism'] = request.parallelism
         if not UtilClient.is_unset(request.parameters):
             query['Parameters'] = request.parameters
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_config_rules_shrink):
+            query['ResourceConfigRules'] = request.resource_config_rules_shrink
         if not UtilClient.is_unset(request.stack_id):
             query['StackId'] = request.stack_id
         if not UtilClient.is_unset(request.stack_name):
             query['StackName'] = request.stack_name
         if not UtilClient.is_unset(request.stack_policy_body):
             query['StackPolicyBody'] = request.stack_policy_body
         if not UtilClient.is_unset(request.stack_policy_url):
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910/models.py` & `alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4163,48 +4163,80 @@
         if m.get('SupportedResourceTypes') is not None:
             for k in m.get('SupportedResourceTypes'):
                 temp_model = GetFeatureDetailsResponseBodyTemplateScratchSupportedResourceTypes()
                 self.supported_resource_types.append(temp_model.from_map(k))
         return self
 
 
+class GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk(TeaModel):
+    def __init__(self, delete_stack=None):
+        self.delete_stack = delete_stack  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.delete_stack is not None:
+            result['DeleteStack'] = self.delete_stack
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DeleteStack') is not None:
+            self.delete_stack = m.get('DeleteStack')
+        return self
+
+
 class GetFeatureDetailsResponseBodyTerraformSupportedResourceTypes(TeaModel):
-    def __init__(self, custom_tag=None, estimate_cost=None, resource_group=None, system_tag=None):
+    def __init__(self, custom_tag=None, estimate_cost=None, resource_group=None, stack_operation_risk=None,
+                 system_tag=None):
         self.custom_tag = custom_tag  # type: list[str]
         self.estimate_cost = estimate_cost  # type: list[str]
         self.resource_group = resource_group  # type: list[str]
+        self.stack_operation_risk = stack_operation_risk  # type: GetFeatureDetailsResponseBodyTerraformSupportedResourceTypesStackOperationRisk
         self.system_tag = system_tag  # type: list[str]
 
     def validate(self):
-        pass
+        if self.stack_operation_risk:
+            self.stack_operation_risk.validate()
 
     def to_map(self):
         _map = super(GetFeatureDetailsResponseBodyTerraformSupportedResourceTypes, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, provider_name=None, supported_versions=None):
@@ -11899,15 +11931,14 @@
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class MoveResourceGroupResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # Id of the request
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(MoveResourceGroupResponseBody, self).to_map()
@@ -11990,24 +12021,59 @@
         if m.get('ParameterKey') is not None:
             self.parameter_key = m.get('ParameterKey')
         if m.get('ParameterValue') is not None:
             self.parameter_value = m.get('ParameterValue')
         return self
 
 
+class PreviewStackRequestResourceConfigRules(TeaModel):
+    def __init__(self, identifier=None, input_parameters=None, resource_type=None):
+        self.identifier = identifier  # type: str
+        self.input_parameters = input_parameters  # type: dict[str, any]
+        self.resource_type = resource_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(PreviewStackRequestResourceConfigRules, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.identifier is not None:
+            result['Identifier'] = self.identifier
+        if self.input_parameters is not None:
+            result['InputParameters'] = self.input_parameters
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Identifier') is not None:
+            self.identifier = m.get('Identifier')
+        if m.get('InputParameters') is not None:
+            self.input_parameters = m.get('InputParameters')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
 class PreviewStackRequest(TeaModel):
     def __init__(self, client_token=None, disable_rollback=None, parallelism=None, parameters=None, region_id=None,
-                 stack_id=None, stack_name=None, stack_policy_body=None, stack_policy_url=None, template_body=None,
-                 template_id=None, template_scratch_id=None, template_scratch_region_id=None, template_url=None,
-                 template_version=None, timeout_in_minutes=None):
+                 resource_config_rules=None, stack_id=None, stack_name=None, stack_policy_body=None, stack_policy_url=None,
+                 template_body=None, template_id=None, template_scratch_id=None, template_scratch_region_id=None,
+                 template_url=None, template_version=None, timeout_in_minutes=None):
         self.client_token = client_token  # type: str
         self.disable_rollback = disable_rollback  # type: bool
         self.parallelism = parallelism  # type: long
         self.parameters = parameters  # type: list[PreviewStackRequestParameters]
         self.region_id = region_id  # type: str
+        self.resource_config_rules = resource_config_rules  # type: list[PreviewStackRequestResourceConfigRules]
         self.stack_id = stack_id  # type: str
         self.stack_name = stack_name  # type: str
         self.stack_policy_body = stack_policy_body  # type: str
         self.stack_policy_url = stack_policy_url  # type: str
         self.template_body = template_body  # type: str
         self.template_id = template_id  # type: str
         self.template_scratch_id = template_scratch_id  # type: str
@@ -12017,14 +12083,18 @@
         self.timeout_in_minutes = timeout_in_minutes  # type: long
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
+        if self.resource_config_rules:
+            for k in self.resource_config_rules:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(PreviewStackRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -12036,14 +12106,18 @@
             result['Parallelism'] = self.parallelism
         result['Parameters'] = []
         if self.parameters is not None:
             for k in self.parameters:
                 result['Parameters'].append(k.to_map() if k else None)
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        result['ResourceConfigRules'] = []
+        if self.resource_config_rules is not None:
+            for k in self.resource_config_rules:
+                result['ResourceConfigRules'].append(k.to_map() if k else None)
         if self.stack_id is not None:
             result['StackId'] = self.stack_id
         if self.stack_name is not None:
             result['StackName'] = self.stack_name
         if self.stack_policy_body is not None:
             result['StackPolicyBody'] = self.stack_policy_body
         if self.stack_policy_url is not None:
@@ -12075,14 +12149,163 @@
         self.parameters = []
         if m.get('Parameters') is not None:
             for k in m.get('Parameters'):
                 temp_model = PreviewStackRequestParameters()
                 self.parameters.append(temp_model.from_map(k))
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        self.resource_config_rules = []
+        if m.get('ResourceConfigRules') is not None:
+            for k in m.get('ResourceConfigRules'):
+                temp_model = PreviewStackRequestResourceConfigRules()
+                self.resource_config_rules.append(temp_model.from_map(k))
+        if m.get('StackId') is not None:
+            self.stack_id = m.get('StackId')
+        if m.get('StackName') is not None:
+            self.stack_name = m.get('StackName')
+        if m.get('StackPolicyBody') is not None:
+            self.stack_policy_body = m.get('StackPolicyBody')
+        if m.get('StackPolicyURL') is not None:
+            self.stack_policy_url = m.get('StackPolicyURL')
+        if m.get('TemplateBody') is not None:
+            self.template_body = m.get('TemplateBody')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateScratchId') is not None:
+            self.template_scratch_id = m.get('TemplateScratchId')
+        if m.get('TemplateScratchRegionId') is not None:
+            self.template_scratch_region_id = m.get('TemplateScratchRegionId')
+        if m.get('TemplateURL') is not None:
+            self.template_url = m.get('TemplateURL')
+        if m.get('TemplateVersion') is not None:
+            self.template_version = m.get('TemplateVersion')
+        if m.get('TimeoutInMinutes') is not None:
+            self.timeout_in_minutes = m.get('TimeoutInMinutes')
+        return self
+
+
+class PreviewStackShrinkRequestParameters(TeaModel):
+    def __init__(self, parameter_key=None, parameter_value=None):
+        self.parameter_key = parameter_key  # type: str
+        self.parameter_value = parameter_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(PreviewStackShrinkRequestParameters, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.parameter_key is not None:
+            result['ParameterKey'] = self.parameter_key
+        if self.parameter_value is not None:
+            result['ParameterValue'] = self.parameter_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ParameterKey') is not None:
+            self.parameter_key = m.get('ParameterKey')
+        if m.get('ParameterValue') is not None:
+            self.parameter_value = m.get('ParameterValue')
+        return self
+
+
+class PreviewStackShrinkRequest(TeaModel):
+    def __init__(self, client_token=None, disable_rollback=None, parallelism=None, parameters=None, region_id=None,
+                 resource_config_rules_shrink=None, stack_id=None, stack_name=None, stack_policy_body=None, stack_policy_url=None,
+                 template_body=None, template_id=None, template_scratch_id=None, template_scratch_region_id=None,
+                 template_url=None, template_version=None, timeout_in_minutes=None):
+        self.client_token = client_token  # type: str
+        self.disable_rollback = disable_rollback  # type: bool
+        self.parallelism = parallelism  # type: long
+        self.parameters = parameters  # type: list[PreviewStackShrinkRequestParameters]
+        self.region_id = region_id  # type: str
+        self.resource_config_rules_shrink = resource_config_rules_shrink  # type: str
+        self.stack_id = stack_id  # type: str
+        self.stack_name = stack_name  # type: str
+        self.stack_policy_body = stack_policy_body  # type: str
+        self.stack_policy_url = stack_policy_url  # type: str
+        self.template_body = template_body  # type: str
+        self.template_id = template_id  # type: str
+        self.template_scratch_id = template_scratch_id  # type: str
+        self.template_scratch_region_id = template_scratch_region_id  # type: str
+        self.template_url = template_url  # type: str
+        self.template_version = template_version  # type: str
+        self.timeout_in_minutes = timeout_in_minutes  # type: long
+
+    def validate(self):
+        if self.parameters:
+            for k in self.parameters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(PreviewStackShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.disable_rollback is not None:
+            result['DisableRollback'] = self.disable_rollback
+        if self.parallelism is not None:
+            result['Parallelism'] = self.parallelism
+        result['Parameters'] = []
+        if self.parameters is not None:
+            for k in self.parameters:
+                result['Parameters'].append(k.to_map() if k else None)
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_config_rules_shrink is not None:
+            result['ResourceConfigRules'] = self.resource_config_rules_shrink
+        if self.stack_id is not None:
+            result['StackId'] = self.stack_id
+        if self.stack_name is not None:
+            result['StackName'] = self.stack_name
+        if self.stack_policy_body is not None:
+            result['StackPolicyBody'] = self.stack_policy_body
+        if self.stack_policy_url is not None:
+            result['StackPolicyURL'] = self.stack_policy_url
+        if self.template_body is not None:
+            result['TemplateBody'] = self.template_body
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_scratch_id is not None:
+            result['TemplateScratchId'] = self.template_scratch_id
+        if self.template_scratch_region_id is not None:
+            result['TemplateScratchRegionId'] = self.template_scratch_region_id
+        if self.template_url is not None:
+            result['TemplateURL'] = self.template_url
+        if self.template_version is not None:
+            result['TemplateVersion'] = self.template_version
+        if self.timeout_in_minutes is not None:
+            result['TimeoutInMinutes'] = self.timeout_in_minutes
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DisableRollback') is not None:
+            self.disable_rollback = m.get('DisableRollback')
+        if m.get('Parallelism') is not None:
+            self.parallelism = m.get('Parallelism')
+        self.parameters = []
+        if m.get('Parameters') is not None:
+            for k in m.get('Parameters'):
+                temp_model = PreviewStackShrinkRequestParameters()
+                self.parameters.append(temp_model.from_map(k))
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceConfigRules') is not None:
+            self.resource_config_rules_shrink = m.get('ResourceConfigRules')
         if m.get('StackId') is not None:
             self.stack_id = m.get('StackId')
         if m.get('StackName') is not None:
             self.stack_name = m.get('StackName')
         if m.get('StackPolicyBody') is not None:
             self.stack_policy_body = m.get('StackPolicyBody')
         if m.get('StackPolicyURL') is not None:
@@ -12195,37 +12418,84 @@
         if m.get('ParameterKey') is not None:
             self.parameter_key = m.get('ParameterKey')
         if m.get('ParameterValue') is not None:
             self.parameter_value = m.get('ParameterValue')
         return self
 
 
+class PreviewStackResponseBodyStackResourcesConfigRuleEvaluations(TeaModel):
+    def __init__(self, annotation=None, compliance_type=None, help_url=None, identifier=None):
+        self.annotation = annotation  # type: str
+        self.compliance_type = compliance_type  # type: str
+        self.help_url = help_url  # type: str
+        self.identifier = identifier  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(PreviewStackResponseBodyStackResourcesConfigRuleEvaluations, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.annotation is not None:
+            result['Annotation'] = self.annotation
+        if self.compliance_type is not None:
+            result['ComplianceType'] = self.compliance_type
+        if self.help_url is not None:
+            result['HelpUrl'] = self.help_url
+        if self.identifier is not None:
+            result['Identifier'] = self.identifier
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Annotation') is not None:
+            self.annotation = m.get('Annotation')
+        if m.get('ComplianceType') is not None:
+            self.compliance_type = m.get('ComplianceType')
+        if m.get('HelpUrl') is not None:
+            self.help_url = m.get('HelpUrl')
+        if m.get('Identifier') is not None:
+            self.identifier = m.get('Identifier')
+        return self
+
+
 class PreviewStackResponseBodyStackResources(TeaModel):
-    def __init__(self, action=None, description=None, logical_resource_id=None, properties=None, replacement=None,
-                 required_by=None, resource_type=None, stack=None):
+    def __init__(self, action=None, config_rule_evaluations=None, description=None, logical_resource_id=None,
+                 properties=None, replacement=None, required_by=None, resource_type=None, stack=None):
         self.action = action  # type: str
+        self.config_rule_evaluations = config_rule_evaluations  # type: list[PreviewStackResponseBodyStackResourcesConfigRuleEvaluations]
         self.description = description  # type: str
         self.logical_resource_id = logical_resource_id  # type: str
         self.properties = properties  # type: dict[str, any]
         self.replacement = replacement  # type: str
         self.required_by = required_by  # type: list[str]
         self.resource_type = resource_type  # type: str
         self.stack = stack  # type: dict[str, any]
 
     def validate(self):
-        pass
+        if self.config_rule_evaluations:
+            for k in self.config_rule_evaluations:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(PreviewStackResponseBodyStackResources, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.action is not None:
             result['Action'] = self.action
+        result['ConfigRuleEvaluations'] = []
+        if self.config_rule_evaluations is not None:
+            for k in self.config_rule_evaluations:
+                result['ConfigRuleEvaluations'].append(k.to_map() if k else None)
         if self.description is not None:
             result['Description'] = self.description
         if self.logical_resource_id is not None:
             result['LogicalResourceId'] = self.logical_resource_id
         if self.properties is not None:
             result['Properties'] = self.properties
         if self.replacement is not None:
@@ -12238,14 +12508,19 @@
             result['Stack'] = self.stack
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Action') is not None:
             self.action = m.get('Action')
+        self.config_rule_evaluations = []
+        if m.get('ConfigRuleEvaluations') is not None:
+            for k in m.get('ConfigRuleEvaluations'):
+                temp_model = PreviewStackResponseBodyStackResourcesConfigRuleEvaluations()
+                self.config_rule_evaluations.append(temp_model.from_map(k))
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('LogicalResourceId') is not None:
             self.logical_resource_id = m.get('LogicalResourceId')
         if m.get('Properties') is not None:
             self.properties = m.get('Properties')
         if m.get('Replacement') is not None:
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/alibabacloud_ros20190910_py2.egg-info/PKG-INFO` & `alibabacloud_ros20190910_py2-2.2.9/alibabacloud_ros20190910_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros20190910-py2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910_py2-2.2.8/setup.py` & `alibabacloud_ros20190910_py2-2.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ros20190910_py2.
 
-Created on 21/07/2022
+Created on 05/09/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ros20190910"
 NAME = "alibabacloud_ros20190910_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python2"
```

