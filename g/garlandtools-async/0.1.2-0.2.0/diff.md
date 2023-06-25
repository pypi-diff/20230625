# Comparing `tmp/garlandtools_async-0.1.2.tar.gz` & `tmp/garlandtools_async-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garlandtools_async-0.1.2.tar", max compression
+gzip compressed data, was "garlandtools_async-0.2.0.tar", max compression
```

## Comparing `garlandtools_async-0.1.2.tar` & `garlandtools_async-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/LICENSE
--rw-r--r--   0        0        0      571 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/__init__.py
--rw-r--r--   0        0        0     2398 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/client.py
--rw-r--r--   0        0        0        0 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/__init__.py
--rw-r--r--   0        0        0      152 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/lang.py
--rw-r--r--   0        0        0        0 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/partials/__init__.py
--rw-r--r--   0        0        0      588 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/partials/item_partial.py
--rw-r--r--   0        0        0      308 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/partials/partial.py
--rw-r--r--   0        0        0     2175 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/records/base_record.py
--rw-r--r--   0        0        0     1253 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/records/factory.py
--rw-r--r--   0        0        0     2782 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/records/item.py
--rw-r--r--   0        0        0      328 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/garlandtools/models/type.py
--rw-r--r--   0        0        0      593 2023-05-13 16:28:23.700816 garlandtools_async-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 garlandtools_async-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/__init__.py
+-rw-r--r--   0        0        0     2640 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/client.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/lang.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/__init__.py
+-rw-r--r--   0        0        0      593 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/item_partial.py
+-rw-r--r--   0        0        0      311 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/partial.py
+-rw-r--r--   0        0        0     2301 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/base_record.py
+-rw-r--r--   0        0        0     1253 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/factory.py
+-rw-r--r--   0        0        0     2820 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/item.py
+-rw-r--r--   0        0        0      328 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/type.py
+-rw-r--r--   0        0        0      848 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 garlandtools_async-0.2.0/PKG-INFO
```

### Comparing `garlandtools_async-0.1.2/LICENSE` & `garlandtools_async-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.2/README.md` & `garlandtools_async-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.2/garlandtools/client.py` & `garlandtools_async-0.2.0/garlandtools/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import Any
 
 from aiohttp import ClientSession
+from cachetools import LFUCache
+from shelved_cache import PersistentCache
+from shelved_cache.decorators import cachedasyncmethod
 
 from garlandtools.models.lang import Lang
 from garlandtools.models.records.base_record import BaseRecord
 from garlandtools.models.records.factory import partial_factory, record_factory
 from garlandtools.models.type import Type
 
+persistent_cache = PersistentCache(LFUCache, filename="data-cache", maxsize=50)
+
 
 class Client:
     base_url = "https://garlandtools.org/api/"
 
     def __init__(
         self,
         session: ClientSession | None = None,
@@ -37,37 +42,38 @@
         :param exact: If the query should be an exact match.
         """
         params = {"text": query}
         if type is not None:
             params["type"] = type.value
         if exact:
             params["exact"] = "true"
-        result = await self._get("search.php", params=params)
+        result = await self._get("search.php", **params)
 
         return [partial_factory(r, client=self) for r in result]
 
     async def _get_by_id(self, id: int, type: Type):
         params = {
             "id": id,
             "type": type.value,
             "lang": self.lang.value,
             "version": 3 if type == type.LEVE or type == type.ITEM else 2,
         }
-        return await self._get("get.php", params=params)
+        return await self._get("get.php", **params)
 
     async def get_by_id(self, id: int, type: Type):
         """Get a record by its ID.
 
         :param id: The ID of the record.
         :param type: The type of the record.
         :param lang: The language of the record.
         """
         result = await self._get_by_id(id, type)
         return record_factory(type, result, self)
 
-    async def _get(self, path: str, params: dict | None = None) -> Any:
+    @cachedasyncmethod(lambda self: persistent_cache)
+    async def _get(self, path: str, **params: dict) -> Any:
         url = self.base_url + path
         async with self.session.get(url, params=params) as response:
             if response.status == 200:
                 return await response.json()
             else:
                 raise Exception(f"Received status code {response.status} from {url}")
```

### Comparing `garlandtools_async-0.1.2/garlandtools/models/records/base_record.py` & `garlandtools_async-0.2.0/garlandtools/models/records/base_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,53 +16,56 @@
     @abstractmethod
     def TYPE(self) -> Type:
         """The type of the record."""
 
     @property
     def id(self) -> int:
         """The ID of the item record."""
-        if self.data is not None:
-            return self.data["id"]
-        if self.partial is not None:
-            return self.partial.id
+        if self._data is not None:
+            return self._data["id"]
+        if self._partial is not None:
+            return self._partial.id
         raise ValueError("Neither data nor partial is set.")
 
     @property
     def name(self) -> str:
         """The name of the item record."""
-        if self.data is not None:
-            return self.data["name"]
-        if self.partial is not None:
-            return self.partial.name
+        if self._data is not None:
+            return self._data["name"]
+        if self._partial is not None:
+            return self._partial.name
         raise ValueError("Neither data nor partial is set.")
 
     def __init__(
         self,
         client: "Client",
         data: dict | None = None,
         partial: ItemPartial | None = None,
         related_records: list["BaseRecord"] = [],
     ):
         if data is None and partial is None:
             raise ValueError("Either data or partial must be provided.")
-        self.client = client
-        self.data = data
-        self.partial = partial
-        self.related_records = related_records
-        self.fetch_lock = asyncio.Lock()
+        self._client = client
+        self._data = data
+        self._partial = partial
+        self._related_records = related_records
+        self._fetch_lock = asyncio.Lock()
 
     async def _get(self, key: str) -> Any | None:
-        if self.data is not None:
-            return self.data[key]
+        if self._data is not None:
+            return self._data[key]
 
-        async with self.fetch_lock:
+        async with self._fetch_lock:
             # Check again in case another coroutine
             # fetched the data while we were waiting
-            if self.data is not None:
-                return self.data[key]
-            record_data = await self.client._get_by_id(self.id, self.TYPE)
-            self.data = record_data[self.TYPE.value]
-            self.related_records = [
-                partial_factory(partial, client=self.client)
+            if self._data is not None:
+                return self._data[key]
+            record_data = await self._client._get_by_id(self.id, self.TYPE)
+            self._data = record_data[self.TYPE.value]
+            self._related_records = [
+                partial_factory(partial, client=self._client)
                 for partial in record_data["partials"]
             ]
-            return self.data[key]
+            return self._data[key]
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} {self.id=}, {self.name=}>"
```

### Comparing `garlandtools_async-0.1.2/garlandtools/models/records/factory.py` & `garlandtools_async-0.2.0/garlandtools/models/records/factory.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.2/garlandtools/models/records/item.py` & `garlandtools_async-0.2.0/garlandtools/models/records/item.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,47 +7,47 @@
     def TYPE(self) -> Type:
         """The type of the record."""
         return Type.ITEM
 
     @property
     def ilvl(self) -> int:
         """The item level of the item."""
-        if self.data is not None:
-            return self.data["ilvl"]
-        if self.partial is not None:
-            return self.partial.ilvl
+        if self._data is not None:
+            return self._data["ilvl"]
+        if self._partial is not None:
+            return self._partial.ilvl
         raise ValueError("Neither data nor partial is set.")
 
     @property
     def icon(self) -> str:
         """The icon of the item."""
-        if self.data is not None:
-            return self.data["icon"]
-        if self.partial is not None:
-            return self.partial.icon
+        if self._data is not None:
+            return self._data["icon"]
+        if self._partial is not None:
+            return self._partial.icon
         raise ValueError("Neither data nor partial is set.")
 
     @property
     def category(self) -> int:
         """The category of the item."""
-        if self.data is not None:
-            return self.data["category"]
-        if self.partial is not None:
-            return self.partial.category
+        if self._data is not None:
+            return self._data["category"]
+        if self._partial is not None:
+            return self._partial.category
         raise ValueError("Neither data nor partial is set.")
 
     @property
     def price(self) -> int:
         """The price of the item."""
-        if self.data is not None:
-            if "price" not in self.data:
+        if self._data is not None:
+            if "price" not in self._data:
                 return 0
-            return self.data["price"]
-        if self.partial is not None:
-            return self.partial.price
+            return self._data["price"]
+        if self._partial is not None:
+            return self._partial.price
         raise ValueError("Neither data nor partial is set.")
 
     @property
     async def description(self) -> str | None:
         """The description of the item."""
         return await self._get("description")
 
@@ -55,21 +55,21 @@
     # async def patch(self) -> int:
     #     return self.data["patch"]  # TODO: return a Patch object
 
     # @property
     # async def patchCategory(self) -> int:
     #     return self.data["patchCategory"]  # TODO: return a PatchCategory object
 
-    # @property
-    # async def tradeable(self) -> bool:
-    #     return bool(self.data["tradeable"])
+    @property
+    async def tradeable(self) -> bool:
+        return bool(await self._get("tradeable"))
 
-    # @property
-    # async def sell_price(self) -> int:
-    #     return self.data["sell_price"]
+    @property
+    async def sell_price(self) -> int:
+        return int(await self._get("sell_price"))  # type: ignore
 
     # @property
     # async def rarity(self) -> int:
     #     return self.data["rarity"]  # TODO: return a Rarity Enum
 
     @property
     async def stack_size(self) -> int | None:
```

### Comparing `garlandtools_async-0.1.2/PKG-INFO` & `garlandtools_async-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: garlandtools-async
-Version: 0.1.2
+Version: 0.2.0
 Summary: A async python wrapper for the https://garlandtools.org/ API
 License: MIT
 Author: Abigail Howe
 Author-email: abby@abigailhowe.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
+Requires-Dist: shelved-cache (>=0.3.1,<0.4.0)
 Description-Content-Type: text/markdown
 
 # garlandtools-py
 
 Work in progress project to provide a async wrapper around the Garland Tools API as detailed here:
 https://www.cyanclay.xyz/info/garland-tools-api-doc-en/
```

