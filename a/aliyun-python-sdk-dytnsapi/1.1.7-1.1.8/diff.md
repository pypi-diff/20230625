# Comparing `tmp/aliyun-python-sdk-dytnsapi-1.1.7.tar.gz` & `tmp/aliyun-python-sdk-dytnsapi-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.7.tar", last modified: Wed May 17 02:24:53 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.8.tar", last modified: Sun Jun 25 06:09:47 2023, max compression
```

## Comparing `aliyun-python-sdk-dytnsapi-1.1.7.tar` & `aliyun-python-sdk-dytnsapi-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-05-17 02:24:53.000000 aliyun-python-sdk-dytnsapi-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-06-25 06:09:47.000000 aliyun-python-sdk-dytnsapi-1.1.8/setup.py
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/LICENSE` & `aliyun-python-sdk-dytnsapi-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.7
+Version: 1.1.8
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/README.rst` & `aliyun-python-sdk-dytnsapi-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.7
+Version: 1.1.8
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/endpoint.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberAnalysisRequest(RpcRequest):
+class TwoElementsVerificationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberAnalysis')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'TwoElementsVerification')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_Rate(self): # Long
-		return self.get_query_params().get('Rate')
-
-	def set_Rate(self, Rate):  # Long
-		self.add_query_param('Rate', Rate)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -52,22 +47,22 @@
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_NumberType(self): # Integer
-		return self.get_query_params().get('NumberType')
-
-	def set_NumberType(self, NumberType):  # Integer
-		self.add_query_param('NumberType', NumberType)
 	def get_AuthCode(self): # String
 		return self.get_query_params().get('AuthCode')
 
 	def set_AuthCode(self, AuthCode):  # String
 		self.add_query_param('AuthCode', AuthCode)
 	def get_InputNumber(self): # String
 		return self.get_query_params().get('InputNumber')
 
 	def set_InputNumber(self, InputNumber):  # String
 		self.add_query_param('InputNumber', InputNumber)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
+
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.8/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class TwoElementsVerificationRequest(RpcRequest):
+class DescribePhoneNumberAnalysisRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'TwoElementsVerification')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberAnalysis')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_Rate(self): # Long
+		return self.get_query_params().get('Rate')
+
+	def set_Rate(self, Rate):  # Long
+		self.add_query_param('Rate', Rate)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -47,22 +52,22 @@
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_NumberType(self): # Long
+		return self.get_query_params().get('NumberType')
+
+	def set_NumberType(self, NumberType):  # Long
+		self.add_query_param('NumberType', NumberType)
 	def get_AuthCode(self): # String
 		return self.get_query_params().get('AuthCode')
 
 	def set_AuthCode(self, AuthCode):  # String
 		self.add_query_param('AuthCode', AuthCode)
 	def get_InputNumber(self): # String
 		return self.get_query_params().get('InputNumber')
 
 	def set_InputNumber(self, InputNumber):  # String
 		self.add_query_param('InputNumber', InputNumber)
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
-
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.7/setup.py` & `aliyun-python-sdk-dytnsapi-1.1.8/setup.py`

 * *Files identical despite different names*

