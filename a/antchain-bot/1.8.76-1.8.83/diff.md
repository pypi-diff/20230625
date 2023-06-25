# Comparing `tmp/antchain_bot-1.8.76.tar.gz` & `tmp/antchain_bot-1.8.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.76.tar", last modified: Tue Jun 13 05:41:26 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.83.tar", last modified: Sun Jun 25 09:02:42 2023, max compression
```

## Comparing `antchain_bot-1.8.76.tar` & `antchain_bot-1.8.83.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   425326 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1132219 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   436652 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1161657 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/setup.py
```

### Comparing `antchain_bot-1.8.76/LICENSE` & `antchain_bot-1.8.83/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.76/PKG-INFO` & `antchain_bot-1.8.83/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_bot
-Version: 1.8.76
+Version: 1.8.83
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.76/README-CN.md` & `antchain_bot-1.8.83/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.76/README.md` & `antchain_bot-1.8.83/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.76/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.83/antchain_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-bot
-Version: 1.8.76
+Version: 1.8.83
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.76/antchain_sdk_bot/client.py` & `antchain_bot-1.8.83/antchain_sdk_bot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.76',
+                    'sdk_version': '1.8.83',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.76',
+                    'sdk_version': '1.8.83',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -4505,14 +4505,182 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.NotifyThirddeviceMessageResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.thirddevice.message.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def register_iotbasic_corpjoin(
+        self,
+        request: bot_models.RegisterIotbasicCorpjoinRequest,
+    ) -> bot_models.RegisterIotbasicCorpjoinResponse:
+        """
+        Description: Iotbasic-厂商入驻
+        Summary: Iotbasic-厂商入驻
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.register_iotbasic_corpjoin_ex(request, headers, runtime)
+
+    async def register_iotbasic_corpjoin_async(
+        self,
+        request: bot_models.RegisterIotbasicCorpjoinRequest,
+    ) -> bot_models.RegisterIotbasicCorpjoinResponse:
+        """
+        Description: Iotbasic-厂商入驻
+        Summary: Iotbasic-厂商入驻
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.register_iotbasic_corpjoin_ex_async(request, headers, runtime)
+
+    def register_iotbasic_corpjoin_ex(
+        self,
+        request: bot_models.RegisterIotbasicCorpjoinRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.RegisterIotbasicCorpjoinResponse:
+        """
+        Description: Iotbasic-厂商入驻
+        Summary: Iotbasic-厂商入驻
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.RegisterIotbasicCorpjoinResponse(),
+            self.do_request('1.0', 'blockchain.bot.iotbasic.corpjoin.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def register_iotbasic_corpjoin_ex_async(
+        self,
+        request: bot_models.RegisterIotbasicCorpjoinRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.RegisterIotbasicCorpjoinResponse:
+        """
+        Description: Iotbasic-厂商入驻
+        Summary: Iotbasic-厂商入驻
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.RegisterIotbasicCorpjoinResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.iotbasic.corpjoin.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_txtransaction_device(
+        self,
+        request: bot_models.QueryTxtransactionDeviceRequest,
+    ) -> bot_models.QueryTxtransactionDeviceResponse:
+        """
+        Description: IoT设备平台-查询设备链上资产详情
+        Summary: IoT设备平台-查询设备链上资产详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_txtransaction_device_ex(request, headers, runtime)
+
+    async def query_txtransaction_device_async(
+        self,
+        request: bot_models.QueryTxtransactionDeviceRequest,
+    ) -> bot_models.QueryTxtransactionDeviceResponse:
+        """
+        Description: IoT设备平台-查询设备链上资产详情
+        Summary: IoT设备平台-查询设备链上资产详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_txtransaction_device_ex_async(request, headers, runtime)
+
+    def query_txtransaction_device_ex(
+        self,
+        request: bot_models.QueryTxtransactionDeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryTxtransactionDeviceResponse:
+        """
+        Description: IoT设备平台-查询设备链上资产详情
+        Summary: IoT设备平台-查询设备链上资产详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryTxtransactionDeviceResponse(),
+            self.do_request('1.0', 'blockchain.bot.txtransaction.device.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_txtransaction_device_ex_async(
+        self,
+        request: bot_models.QueryTxtransactionDeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryTxtransactionDeviceResponse:
+        """
+        Description: IoT设备平台-查询设备链上资产详情
+        Summary: IoT设备平台-查询设备链上资产详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryTxtransactionDeviceResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.txtransaction.device.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_txtransaction_chaindata(
+        self,
+        request: bot_models.QueryTxtransactionChaindataRequest,
+    ) -> bot_models.QueryTxtransactionChaindataResponse:
+        """
+        Description: IoT设备平台-查询业务数据链上资产详情
+        Summary: IoT设备平台-查询业务数据链上资产详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_txtransaction_chaindata_ex(request, headers, runtime)
+
+    async def query_txtransaction_chaindata_async(
+        self,
+        request: bot_models.QueryTxtransactionChaindataRequest,
+    ) -> bot_models.QueryTxtransactionChaindataResponse:
+        """
+        Description: IoT设备平台-查询业务数据链上资产详情
+        Summary: IoT设备平台-查询业务数据链上资产详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_txtransaction_chaindata_ex_async(request, headers, runtime)
+
+    def query_txtransaction_chaindata_ex(
+        self,
+        request: bot_models.QueryTxtransactionChaindataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryTxtransactionChaindataResponse:
+        """
+        Description: IoT设备平台-查询业务数据链上资产详情
+        Summary: IoT设备平台-查询业务数据链上资产详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryTxtransactionChaindataResponse(),
+            self.do_request('1.0', 'blockchain.bot.txtransaction.chaindata.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_txtransaction_chaindata_ex_async(
+        self,
+        request: bot_models.QueryTxtransactionChaindataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryTxtransactionChaindataResponse:
+        """
+        Description: IoT设备平台-查询业务数据链上资产详情
+        Summary: IoT设备平台-查询业务数据链上资产详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryTxtransactionChaindataResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.txtransaction.chaindata.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_iotplatform_purchaseorder(
         self,
         request: bot_models.QueryIotplatformPurchaseorderRequest,
     ) -> bot_models.QueryIotplatformPurchaseorderResponse:
         """
         Description: 根据设备串号查询采购设备
         Summary: 根据设备串号查询采购设备
@@ -9713,14 +9881,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.ConfirmCollectorUploadfileResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.collector.uploadfile.confirm', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_thingmodel_event(
+        self,
+        request: bot_models.CreateThingmodelEventRequest,
+    ) -> bot_models.CreateThingmodelEventResponse:
+        """
+        Description: 创建物模型事件
+        Summary: 创建物模型事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_thingmodel_event_ex(request, headers, runtime)
+
+    async def create_thingmodel_event_async(
+        self,
+        request: bot_models.CreateThingmodelEventRequest,
+    ) -> bot_models.CreateThingmodelEventResponse:
+        """
+        Description: 创建物模型事件
+        Summary: 创建物模型事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_thingmodel_event_ex_async(request, headers, runtime)
+
+    def create_thingmodel_event_ex(
+        self,
+        request: bot_models.CreateThingmodelEventRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateThingmodelEventResponse:
+        """
+        Description: 创建物模型事件
+        Summary: 创建物模型事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateThingmodelEventResponse(),
+            self.do_request('1.0', 'blockchain.bot.thingmodel.event.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_thingmodel_event_ex_async(
+        self,
+        request: bot_models.CreateThingmodelEventRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateThingmodelEventResponse:
+        """
+        Description: 创建物模型事件
+        Summary: 创建物模型事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateThingmodelEventResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.thingmodel.event.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_thingmodel_event(
+        self,
+        request: bot_models.QueryThingmodelEventRequest,
+    ) -> bot_models.QueryThingmodelEventResponse:
+        """
+        Description: 查询物模型事件
+        Summary: 查询物模型事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_thingmodel_event_ex(request, headers, runtime)
+
+    async def query_thingmodel_event_async(
+        self,
+        request: bot_models.QueryThingmodelEventRequest,
+    ) -> bot_models.QueryThingmodelEventResponse:
+        """
+        Description: 查询物模型事件
+        Summary: 查询物模型事件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_thingmodel_event_ex_async(request, headers, runtime)
+
+    def query_thingmodel_event_ex(
+        self,
+        request: bot_models.QueryThingmodelEventRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryThingmodelEventResponse:
+        """
+        Description: 查询物模型事件
+        Summary: 查询物模型事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryThingmodelEventResponse(),
+            self.do_request('1.0', 'blockchain.bot.thingmodel.event.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_thingmodel_event_ex_async(
+        self,
+        request: bot_models.QueryThingmodelEventRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryThingmodelEventResponse:
+        """
+        Description: 查询物模型事件
+        Summary: 查询物模型事件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryThingmodelEventResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.thingmodel.event.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def exec_thingsdid_oneapi(
         self,
         request: bot_models.ExecThingsdidOneapiRequest,
     ) -> bot_models.ExecThingsdidOneapiResponse:
         """
         Description: 信物链oneapi
         Summary: 信物链oneapi
```

### Comparing `antchain_bot-1.8.76/antchain_sdk_bot/models.py` & `antchain_bot-1.8.83/antchain_sdk_bot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -777,14 +777,89 @@
         if m.get('gateway_private_key') is not None:
             self.gateway_private_key = m.get('gateway_private_key')
         if m.get('gateway_public_key') is not None:
             self.gateway_public_key = m.get('gateway_public_key')
         return self
 
 
+class QueryChainDataTransactionResultData(TeaModel):
+    def __init__(
+        self,
+        biz_id: str = None,
+        biz_scene: str = None,
+        data_scene: str = None,
+        asset_id: str = None,
+        tenant_id: str = None,
+        asset_data: str = None,
+        timestamp: int = None,
+    ):
+        # 业务ID
+        self.biz_id = biz_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 数据资产类型
+        self.data_scene = data_scene
+        # 资产ID
+        self.asset_id = asset_id
+        # 租户id
+        self.tenant_id = tenant_id
+        # 资产数据
+        self.asset_data = asset_data
+        # 时间
+        self.timestamp = timestamp
+
+    def validate(self):
+        self.validate_required(self.biz_id, 'biz_id')
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.data_scene, 'data_scene')
+        self.validate_required(self.asset_id, 'asset_id')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.asset_data, 'asset_data')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_id is not None:
+            result['biz_id'] = self.biz_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.data_scene is not None:
+            result['data_scene'] = self.data_scene
+        if self.asset_id is not None:
+            result['asset_id'] = self.asset_id
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.asset_data is not None:
+            result['asset_data'] = self.asset_data
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('biz_id') is not None:
+            self.biz_id = m.get('biz_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('data_scene') is not None:
+            self.data_scene = m.get('data_scene')
+        if m.get('asset_id') is not None:
+            self.asset_id = m.get('asset_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('asset_data') is not None:
+            self.asset_data = m.get('asset_data')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        return self
+
+
 class BaiGoodsPointIdentificationResult(TeaModel):
     def __init__(
         self,
         point_name: str = None,
         sub_point_name: str = None,
         result: str = None,
         grade: str = None,
@@ -2267,14 +2342,93 @@
         if m.get('instance_id') is not None:
             self.instance_id = m.get('instance_id')
         if m.get('instance_name') is not None:
             self.instance_name = m.get('instance_name')
         return self
 
 
+class QueryTransactionResultInfo(TeaModel):
+    def __init__(
+        self,
+        block_hash: str = None,
+        parent_block_hash: str = None,
+        timestamp: str = None,
+        gas: int = None,
+        from_: str = None,
+        to: str = None,
+        tx_type: str = None,
+        data: QueryChainDataTransactionResultData = None,
+    ):
+        # 区块hash
+        self.block_hash = block_hash
+        # 父区块hash
+        self.parent_block_hash = parent_block_hash
+        # 交易时间戳
+        self.timestamp = timestamp
+        # 该交易所能消耗的最大gas
+        self.gas = gas
+        # 交易发起方账户
+        self.from_ = from_
+        # 交易接收方账户
+        self.to = to
+        # 交易类型
+        self.tx_type = tx_type
+        # 交易返回的数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.block_hash is not None:
+            result['block_hash'] = self.block_hash
+        if self.parent_block_hash is not None:
+            result['parent_block_hash'] = self.parent_block_hash
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        if self.gas is not None:
+            result['gas'] = self.gas
+        if self.from_ is not None:
+            result['from'] = self.from_
+        if self.to is not None:
+            result['to'] = self.to
+        if self.tx_type is not None:
+            result['tx_type'] = self.tx_type
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('block_hash') is not None:
+            self.block_hash = m.get('block_hash')
+        if m.get('parent_block_hash') is not None:
+            self.parent_block_hash = m.get('parent_block_hash')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        if m.get('gas') is not None:
+            self.gas = m.get('gas')
+        if m.get('from') is not None:
+            self.from_ = m.get('from')
+        if m.get('to') is not None:
+            self.to = m.get('to')
+        if m.get('tx_type') is not None:
+            self.tx_type = m.get('tx_type')
+        if m.get('data') is not None:
+            temp_model = QueryChainDataTransactionResultData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
 class DeviceDisableData(TeaModel):
     def __init__(
         self,
         device_sn: str = None,
         corp_name: str = None,
     ):
         # 设备sn号
@@ -7377,14 +7531,111 @@
         if m.get('biz_type') is not None:
             self.biz_type = m.get('biz_type')
         if m.get('content') is not None:
             self.content = m.get('content')
         return self
 
 
+class QueryDeviceTransactionResultData(TeaModel):
+    def __init__(
+        self,
+        corp_name: str = None,
+        scene: str = None,
+        device_imei: str = None,
+        device_sn: str = None,
+        price: str = None,
+        device_did: str = None,
+        device_tuid: str = None,
+        device_specs: str = None,
+        tenant_id: str = None,
+        account_name: str = None,
+    ):
+        # 设备所属厂商
+        self.corp_name = corp_name
+        # 场景码,所属项目
+        self.scene = scene
+        # IMEI
+        self.device_imei = device_imei
+        # 设备sn
+        self.device_sn = device_sn
+        # 设备金额
+        self.price = price
+        # 设备分布式身份did
+        self.device_did = device_did
+        # 设备终端唯一ID
+        self.device_tuid = device_tuid
+        # 设备参数:品类+型号+规格
+        self.device_specs = device_specs
+        # 所属租户
+        self.tenant_id = tenant_id
+        # 所属账号
+        self.account_name = account_name
+
+    def validate(self):
+        self.validate_required(self.corp_name, 'corp_name')
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.device_sn, 'device_sn')
+        self.validate_required(self.device_did, 'device_did')
+        self.validate_required(self.device_specs, 'device_specs')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.account_name, 'account_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_name is not None:
+            result['corp_name'] = self.corp_name
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.device_imei is not None:
+            result['device_imei'] = self.device_imei
+        if self.device_sn is not None:
+            result['device_sn'] = self.device_sn
+        if self.price is not None:
+            result['price'] = self.price
+        if self.device_did is not None:
+            result['device_did'] = self.device_did
+        if self.device_tuid is not None:
+            result['device_tuid'] = self.device_tuid
+        if self.device_specs is not None:
+            result['device_specs'] = self.device_specs
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.account_name is not None:
+            result['account_name'] = self.account_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corp_name') is not None:
+            self.corp_name = m.get('corp_name')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('device_imei') is not None:
+            self.device_imei = m.get('device_imei')
+        if m.get('device_sn') is not None:
+            self.device_sn = m.get('device_sn')
+        if m.get('price') is not None:
+            self.price = m.get('price')
+        if m.get('device_did') is not None:
+            self.device_did = m.get('device_did')
+        if m.get('device_tuid') is not None:
+            self.device_tuid = m.get('device_tuid')
+        if m.get('device_specs') is not None:
+            self.device_specs = m.get('device_specs')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('account_name') is not None:
+            self.account_name = m.get('account_name')
+        return self
+
+
 class CorporateReqModel(TeaModel):
     def __init__(
         self,
         address: str = None,
         business_address: str = None,
         business_scope: str = None,
         certify_date: str = None,
@@ -18199,14 +18450,431 @@
         if m.get('success') is not None:
             self.success = m.get('success')
         if m.get('command') is not None:
             self.command = m.get('command')
         return self
 
 
+class RegisterIotbasicCorpjoinRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        corp_code: str = None,
+        corp_name: str = None,
+        product_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 厂商value
+        self.corp_code = corp_code
+        # 厂商名称
+        self.corp_name = corp_name
+        # 厂商签约产品码
+        self.product_code = product_code
+
+    def validate(self):
+        self.validate_required(self.corp_code, 'corp_code')
+        self.validate_required(self.corp_name, 'corp_name')
+        self.validate_required(self.product_code, 'product_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.corp_code is not None:
+            result['corp_code'] = self.corp_code
+        if self.corp_name is not None:
+            result['corp_name'] = self.corp_name
+        if self.product_code is not None:
+            result['product_code'] = self.product_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('corp_code') is not None:
+            self.corp_code = m.get('corp_code')
+        if m.get('corp_name') is not None:
+            self.corp_name = m.get('corp_name')
+        if m.get('product_code') is not None:
+            self.product_code = m.get('product_code')
+        return self
+
+
+class RegisterIotbasicCorpjoinResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryTxtransactionDeviceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        device_did: str = None,
+        device_signature: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 设备did
+        self.device_did = device_did
+        # 设备签名
+        self.device_signature = device_signature
+
+    def validate(self):
+        self.validate_required(self.device_did, 'device_did')
+        self.validate_required(self.device_signature, 'device_signature')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.device_did is not None:
+            result['device_did'] = self.device_did
+        if self.device_signature is not None:
+            result['device_signature'] = self.device_signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('device_did') is not None:
+            self.device_did = m.get('device_did')
+        if m.get('device_signature') is not None:
+            self.device_signature = m.get('device_signature')
+        return self
+
+
+class QueryTxtransactionDeviceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        block_hash: str = None,
+        parent_block_hash: str = None,
+        timestamp: str = None,
+        gas: int = None,
+        from_: str = None,
+        to: str = None,
+        tx_type: str = None,
+        data: QueryDeviceTransactionResultData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求结果
+        self.success = success
+        # 区块hash
+        self.block_hash = block_hash
+        # 父区块hash
+        self.parent_block_hash = parent_block_hash
+        # 交易时间戳
+        self.timestamp = timestamp
+        # 该交易所能消耗的最大gas
+        self.gas = gas
+        # 交易发起方账户
+        self.from_ = from_
+        # 交易接收方账户
+        self.to = to
+        # 交易类型
+        self.tx_type = tx_type
+        # 交易返回的数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.block_hash is not None:
+            result['block_hash'] = self.block_hash
+        if self.parent_block_hash is not None:
+            result['parent_block_hash'] = self.parent_block_hash
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        if self.gas is not None:
+            result['gas'] = self.gas
+        if self.from_ is not None:
+            result['from'] = self.from_
+        if self.to is not None:
+            result['to'] = self.to
+        if self.tx_type is not None:
+            result['tx_type'] = self.tx_type
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('block_hash') is not None:
+            self.block_hash = m.get('block_hash')
+        if m.get('parent_block_hash') is not None:
+            self.parent_block_hash = m.get('parent_block_hash')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        if m.get('gas') is not None:
+            self.gas = m.get('gas')
+        if m.get('from') is not None:
+            self.from_ = m.get('from')
+        if m.get('to') is not None:
+            self.to = m.get('to')
+        if m.get('tx_type') is not None:
+            self.tx_type = m.get('tx_type')
+        if m.get('data') is not None:
+            temp_model = QueryDeviceTransactionResultData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class QueryTxtransactionChaindataRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tx_hash: str = None,
+        request_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 上链hash值，和request_id必须有一个有值
+        self.tx_hash = tx_hash
+        # 上链请求消息id，和tx_hash必须有一个有值
+        self.request_id = request_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.tx_hash is not None:
+            result['tx_hash'] = self.tx_hash
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tx_hash') is not None:
+            self.tx_hash = m.get('tx_hash')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        return self
+
+
+class QueryTxtransactionChaindataResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        block_hash: str = None,
+        parent_block_hash: str = None,
+        timestamp: str = None,
+        gas: int = None,
+        from_: str = None,
+        to: str = None,
+        tx_type: str = None,
+        data: QueryChainDataTransactionResultData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求结果
+        self.success = success
+        # 区块hash
+        self.block_hash = block_hash
+        # 父区块hash
+        self.parent_block_hash = parent_block_hash
+        # 交易时间戳
+        self.timestamp = timestamp
+        # 该交易所能消耗的最大gas
+        self.gas = gas
+        # 交易发起方账户
+        self.from_ = from_
+        # 交易接收方账户
+        self.to = to
+        # 交易类型
+        self.tx_type = tx_type
+        # 交易返回的数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.block_hash is not None:
+            result['block_hash'] = self.block_hash
+        if self.parent_block_hash is not None:
+            result['parent_block_hash'] = self.parent_block_hash
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        if self.gas is not None:
+            result['gas'] = self.gas
+        if self.from_ is not None:
+            result['from'] = self.from_
+        if self.to is not None:
+            result['to'] = self.to
+        if self.tx_type is not None:
+            result['tx_type'] = self.tx_type
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('block_hash') is not None:
+            self.block_hash = m.get('block_hash')
+        if m.get('parent_block_hash') is not None:
+            self.parent_block_hash = m.get('parent_block_hash')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        if m.get('gas') is not None:
+            self.gas = m.get('gas')
+        if m.get('from') is not None:
+            self.from_ = m.get('from')
+        if m.get('to') is not None:
+            self.to = m.get('to')
+        if m.get('tx_type') is not None:
+            self.tx_type = m.get('tx_type')
+        if m.get('data') is not None:
+            temp_model = QueryChainDataTransactionResultData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
 class QueryIotplatformPurchaseorderRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         tenant_id: str = None,
         serial_number: str = None,
@@ -23007,15 +23675,14 @@
     def validate(self):
         self.validate_required(self.content, 'content')
         if self.content:
             for k in self.content:
                 if k:
                     k.validate()
         self.validate_required(self.nonce, 'nonce')
-        self.validate_required(self.wait_check_and_hash, 'wait_check_and_hash')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -23141,15 +23808,14 @@
         self.validate_required(self.data_model_id, 'data_model_id')
         self.validate_required(self.nonce, 'nonce')
         self.validate_required(self.content, 'content')
         if self.content:
             for k in self.content:
                 if k:
                     k.validate()
-        self.validate_required(self.wait_check_and_hash, 'wait_check_and_hash')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -29650,14 +30316,209 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class CreateThingmodelEventRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        thing_model_event_json: str = None,
+        data_demo: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 物模型事件json
+        self.thing_model_event_json = thing_model_event_json
+        # 数据样例
+        self.data_demo = data_demo
+
+    def validate(self):
+        self.validate_required(self.thing_model_event_json, 'thing_model_event_json')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.thing_model_event_json is not None:
+            result['thing_model_event_json'] = self.thing_model_event_json
+        if self.data_demo is not None:
+            result['data_demo'] = self.data_demo
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('thing_model_event_json') is not None:
+            self.thing_model_event_json = m.get('thing_model_event_json')
+        if m.get('data_demo') is not None:
+            self.data_demo = m.get('data_demo')
+        return self
+
+
+class CreateThingmodelEventResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        event_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 物模型事件ID
+        self.event_id = event_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.event_id is not None:
+            result['event_id'] = self.event_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('event_id') is not None:
+            self.event_id = m.get('event_id')
+        return self
+
+
+class QueryThingmodelEventRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        event_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 物模型事件ID
+        self.event_id = event_id
+
+    def validate(self):
+        self.validate_required(self.event_id, 'event_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.event_id is not None:
+            result['event_id'] = self.event_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('event_id') is not None:
+            self.event_id = m.get('event_id')
+        return self
+
+
+class QueryThingmodelEventResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        thing_model_event_json: str = None,
+        data_demo: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 物模型事件json
+        # 
+        self.thing_model_event_json = thing_model_event_json
+        # 数据样例
+        self.data_demo = data_demo
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.thing_model_event_json is not None:
+            result['thing_model_event_json'] = self.thing_model_event_json
+        if self.data_demo is not None:
+            result['data_demo'] = self.data_demo
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('thing_model_event_json') is not None:
+            self.thing_model_event_json = m.get('thing_model_event_json')
+        if m.get('data_demo') is not None:
+            self.data_demo = m.get('data_demo')
+        return self
+
+
 class ExecThingsdidOneapiRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_content: str = None,
     ):
```

### Comparing `antchain_bot-1.8.76/setup.py` & `antchain_bot-1.8.83/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 13/06/2023
+Created on 25/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

