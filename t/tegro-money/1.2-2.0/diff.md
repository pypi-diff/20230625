# Comparing `tmp/tegro_money-1.2.tar.gz` & `tmp/tegro_money-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tegro_money-1.2.tar", last modified: Mon Jun 19 18:34:54 2023, max compression
+gzip compressed data, was "tegro_money-2.0.tar", last modified: Sun Jun 25 15:45:04 2023, max compression
```

## Comparing `tegro_money-1.2.tar` & `tegro_money-2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 18:34:54.000000 tegro_money-1.2/
--rw-rw-rw-   0        0        0      331 2023-06-19 18:34:54.000000 tegro_money-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 18:34:54.000000 tegro_money-1.2/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-06-19 18:32:19.000000 tegro_money-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 18:34:54.000000 tegro_money-1.2/tegro_money/
--rw-rw-rw-   0        0        0       82 2023-06-19 18:33:37.000000 tegro_money-1.2/tegro_money/__init__.py
--rw-rw-rw-   0        0        0      604 2023-06-19 18:31:33.000000 tegro_money-1.2/tegro_money/api.py
--rw-rw-rw-   0        0        0      339 2023-06-19 11:25:31.000000 tegro_money-1.2/tegro_money/build_dict.py
--rw-rw-rw-   0        0        0      411 2023-06-19 11:23:05.000000 tegro_money-1.2/tegro_money/build_headers.py
--rw-rw-rw-   0        0        0      146 2023-06-19 18:08:51.000000 tegro_money-1.2/tegro_money/tegro_config.py
--rw-rw-rw-   0        0        0     4956 2023-06-19 18:30:22.000000 tegro_money-1.2/tegro_money/tegro_money.py
-drwxrwxrwx   0        0        0        0 2023-06-19 18:34:54.000000 tegro_money-1.2/tegro_money.egg-info/
--rw-rw-rw-   0        0        0      331 2023-06-19 18:34:53.000000 tegro_money-1.2/tegro_money.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-06-19 18:34:53.000000 tegro_money-1.2/tegro_money.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 18:34:53.000000 tegro_money-1.2/tegro_money.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 18:34:53.000000 tegro_money-1.2/tegro_money.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 18:34:53.000000 tegro_money-1.2/tegro_money.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 15:45:04.067111 tegro_money-2.0/
+-rw-rw-rw-   0        0        0       56 2023-06-25 15:45:03.988986 tegro_money-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-25 15:45:04.113983 tegro_money-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      117 2023-06-25 11:58:49.000000 tegro_money-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:45:01.645233 tegro_money-2.0/tegro_money/
+-rw-rw-rw-   0        0        0       82 2023-06-19 18:33:37.000000 tegro_money-2.0/tegro_money/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-06-25 15:35:55.000000 tegro_money-2.0/tegro_money/api.py
+-rw-rw-rw-   0        0        0      339 2023-06-19 11:25:31.000000 tegro_money-2.0/tegro_money/build_dict.py
+-rw-rw-rw-   0        0        0      411 2023-06-19 11:23:05.000000 tegro_money-2.0/tegro_money/build_headers.py
+-rw-rw-rw-   0        0        0      146 2023-06-19 18:08:51.000000 tegro_money-2.0/tegro_money/tegro_config.py
+-rw-rw-rw-   0        0        0     4923 2023-06-25 15:43:57.000000 tegro_money-2.0/tegro_money/tegro_money.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:45:03.988986 tegro_money-2.0/tegro_money.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-25 15:44:55.000000 tegro_money-2.0/tegro_money.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-25 15:44:55.000000 tegro_money-2.0/tegro_money.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 15:44:55.000000 tegro_money-2.0/tegro_money.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 15:44:55.000000 tegro_money-2.0/tegro_money.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tegro_money-1.2/tegro_money/api.py` & `tegro_money-2.0/tegro_money/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import requests
 import json
 from typing import Dict
+from .tegro_config import TegroConfig
 from .build_dict import build_dict
 from .build_headers import build_headers
 
 
-def post(shop_id: str, api_key: str, api_url: str, endpoint: str, body: Dict = None) -> Dict:
+def post(config: TegroConfig, endpoint: str, body: Dict = None) -> Dict:
+    api_url, shop_id, api_key = set(config.dict().values())
     url = api_url + endpoint
     body = build_dict(shop_id, body)
     headers = build_headers(api_key, body)
     try:
         response = requests.post(url, data=body, headers=headers)
         response.raise_for_status()
         response_text = json.loads(response.text)
```

### Comparing `tegro_money-1.2/tegro_money/tegro_money.py` & `tegro_money-2.0/tegro_money/tegro_money.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,145 +17,150 @@
                 "order_info": "order",
                 "orders_list": "orders",
                 "create_withdrawal": "createWithdrawal",
                 "withdrawals_list": "withdrawals",
                 "withdrawal_info": "withdrawal"
             }
 
-        self.config = config.dict()
+        self.config = config
         self.endpoints = endpoints or default_endpoints
 
+    def create_order(self, currency: str, order_id: str, payment_system: str, fields: Dict, items: List[Dict]):
+        body = build_dict(self.config.shop_id, 
+            {
+            "currency": currency,
+            "amount": sum([item["price"] for item in items]),
+            "order_id": order_id,
+            "payment_system": payment_system,
+            "fields": fields,
+            "receipt": {"items": items}
+            })
+        result = post(
+            self.config,
+            self.endpoints["create_order"], 
+            body
+            )
+        if result:
+            url = result["data"]["url"]
+            return url
+        else:
+            return None
+
     def shops_list(self) -> List[Dict]:
-        body = build_dict(self.config["shop_id"])
+        body = build_dict(self.config.shop_id)
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["shops_list"], 
             body
             )
         if result:
             shops = result["data"]["shops"]
             return shops
         else:
             return None
         
     def balance(self) -> Dict:
-        body = build_dict(self.config["shop_id"])
+        body = build_dict(self.config.shop_id)
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["balance"], 
             body
             )
         if result:
             balance = result["data"]["balance"]
             return balance
         else:
             return None
 
     def order_info_by_order_id(self, order_id: int) -> Dict:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "order_id": order_id
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["order_info"], 
             body
             )
         if result:
             order_info = result["data"]
             return order_info
         else:
             return None
 
     def order_info_by_payment_id(self, payment_id: str) -> Dict:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "payment_id": payment_id
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config, 
             self.endpoints["order_info"], 
             body
             )
         if result:
             order_info = result["data"]
             return order_info
         else:
             return None
 
     def orders_list(self, page: int = 1) -> List[Dict]:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "page": page
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["orders_list"], 
             body
             )
         if result:
             orders = result["data"]
             return orders
         else:
             return None
     
     def withdrawals_list(self, page: int = 1) -> List[Dict]:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "page": page
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["withdrawals_list"], 
             body
             )
         if result:
             withdrawals = result["data"]
             return withdrawals
         else:
             return None
         
     def withdrawal_info_by_order_id(self, order_id: int) -> Dict:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "order_id": order_id
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["withdrawal_info"], 
             body)
         if result:
             withdrawal_info = result["data"]
             return withdrawal_info
         else:
             return None
 
     def withdrawal_info_by_payment_id(self, payment_id: str) -> Dict:
-        body = build_dict(self.config["shop_id"], 
+        body = build_dict(self.config.shop_id, 
             {
             "payment_id": payment_id
             })
         result = post(
-            self.config["shop_id"], 
-            self.config["api_key"], 
-            self.config["api_url"], 
+            self.config,
             self.endpoints["withdrawal_info"], 
             body
             )
         if result:
             withdrawal_info = result["data"]
             return withdrawal_info
         else:
```

