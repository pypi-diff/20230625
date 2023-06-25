# Comparing `tmp/zingmp3py-0.3.1.tar.gz` & `tmp/zingmp3py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zingmp3py-0.3.1.tar", last modified: Mon Sep 19 07:28:35 2022, max compression
+gzip compressed data, was "zingmp3py-0.3.2.tar", last modified: Sun Jun 25 15:35:03 2023, max compression
```

## Comparing `zingmp3py-0.3.1.tar` & `zingmp3py-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-19 07:28:35.546338 zingmp3py-0.3.1/
--rw-rw-rw-   0        0        0    10751 2022-09-15 12:40:26.000000 zingmp3py-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1373 2022-09-19 07:28:35.542839 zingmp3py-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      946 2022-09-18 07:05:57.000000 zingmp3py-0.3.1/README.md
--rw-rw-rw-   0        0        0      539 2022-09-19 07:26:45.000000 zingmp3py-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-19 07:28:35.546838 zingmp3py-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      292 2022-09-19 07:26:45.000000 zingmp3py-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-19 07:28:35.488336 zingmp3py-0.3.1/zingmp3py/
--rw-rw-rw-   0        0        0      189 2022-09-19 07:26:45.000000 zingmp3py-0.3.1/zingmp3py/__init__.py
--rw-rw-rw-   0        0        0     3294 2022-09-18 07:12:20.000000 zingmp3py-0.3.1/zingmp3py/sobj.py
--rw-rw-rw-   0        0        0     1025 2022-09-17 03:12:41.000000 zingmp3py-0.3.1/zingmp3py/util.py
--rw-rw-rw-   0        0        0     3497 2022-09-19 07:26:45.000000 zingmp3py-0.3.1/zingmp3py/zasync.py
--rw-rw-rw-   0        0        0     2744 2022-09-18 03:36:59.000000 zingmp3py-0.3.1/zingmp3py/zsync.py
-drwxrwxrwx   0        0        0        0 2022-09-19 07:28:35.540838 zingmp3py-0.3.1/zingmp3py.egg-info/
--rw-rw-rw-   0        0        0     1373 2022-09-19 07:28:35.000000 zingmp3py-0.3.1/zingmp3py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2022-09-19 07:28:35.000000 zingmp3py-0.3.1/zingmp3py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-19 07:28:35.000000 zingmp3py-0.3.1/zingmp3py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-09-19 07:28:35.000000 zingmp3py-0.3.1/zingmp3py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-19 07:28:35.000000 zingmp3py-0.3.1/zingmp3py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:03.154270 zingmp3py-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-25 15:35:03.154270 zingmp3py-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:35:03.154270 zingmp3py-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:03.154270 zingmp3py-0.3.2/zingmp3py/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/zingmp3py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/zingmp3py/sobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/zingmp3py/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/zingmp3py/zasync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-25 15:34:53.000000 zingmp3py-0.3.2/zingmp3py/zsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:03.154270 zingmp3py-0.3.2/zingmp3py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-25 15:35:03.000000 zingmp3py-0.3.2/zingmp3py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-25 15:35:03.000000 zingmp3py-0.3.2/zingmp3py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:35:03.000000 zingmp3py-0.3.2/zingmp3py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 15:35:03.000000 zingmp3py-0.3.2/zingmp3py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-25 15:35:03.000000 zingmp3py-0.3.2/zingmp3py.egg-info/top_level.txt
```

### Comparing `zingmp3py-0.3.1/LICENSE` & `zingmp3py-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zingmp3py-0.3.1/PKG-INFO` & `zingmp3py-0.3.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-Metadata-Version: 2.1
-Name: zingmp3py
-Version: 0.3.1
-Summary: A Python library for the ZingMp3 API
-Author: The DT
-Author-email: The DT <duongtuan30306@gmail.com>
-Project-URL: Homepage, https://github.com/thedtvn/zingmp3py
-Project-URL: Bug Tracker, https://github.com/thedtvn/zingmp3py/issues
-Keywords: zingmp3,music,api,vietnam
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# zingmp3py
-#### A light weight Python library for the ZingMp3 API
-##### *all functions are return dict or ZingMp3 Object
-
-# Sync :
-```py
-from zingmp3py import ZingMp3
-
-zi = ZingMp3()
-zi.getDetailPlaylist("67ZFO8DZ")
-zi.getDetailArtist("Cammie")
-zi.getRadioInfo("IWZ979CW")
-zi.getSongInfo("ZWAF6UFD")
-zi.getSongStreaming("ZWAF6UFD")
-zi.getTop100()
-zi.search("rick roll")
-```
-
-# Async
-```py
-import asyncio
-from zingmp3py import ZingMp3Async
-
-async def main():
-    zi = ZingMp3Async()
-    await zi.getDetailPlaylist("67ZFO8DZ")
-    await zi.getDetailArtist("Cammie")
-    await zi.getSongInfo("ZWAF6UFD")
-    await zi.getSongStreaming("ZWAF6UFD")
-    await zi.getTop100()
-    await zi.search("rick roll")
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-```
-
-## Get Type And ID
-
-```py
-from zingmp3py import getUrlTypeAndID
-
-getUrlTypeAndID("https://zingmp3.vn/liveradio/IWZ979CW.html")
-```
+Metadata-Version: 2.1
+Name: zingmp3py
+Version: 0.3.2
+Summary: A light weight Python library for the ZingMp3 API
+Author: The DT
+Author-email: duongtuan30306@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# zingmp3py
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
+#### A light weight Python library for the ZingMp3 API
+##### *all functions are return dict or ZingMp3 Object
+
+# install 
+
+## pypi
+```
+pip install zingmp3py
+```
+
+## Git (version in development)
+```
+pip install git+https://github.com/thedtvn/zingmp3py.git
+```
+
+
+# Sync :
+```py
+from zingmp3py import ZingMp3
+
+zi = ZingMp3()
+zi.getDetailPlaylist("67ZFO8DZ")
+zi.getDetailArtist("Cammie")
+zi.getRadioInfo("IWZ979CW")
+zi.getSongInfo("ZWAF6UFD")
+zi.getSongStreaming("ZWAF6UFD")
+zi.getTop100()
+zi.search("rick roll")
+```
+
+# Async
+```py
+import asyncio
+from zingmp3py import ZingMp3Async
+
+async def main():
+    zi = ZingMp3Async()
+    await zi.getDetailPlaylist("67ZFO8DZ")
+    await zi.getDetailArtist("Cammie")
+    await zi.getSongInfo("ZWAF6UFD")
+    await zi.getSongStreaming("ZWAF6UFD")
+    await zi.getTop100()
+    await zi.search("rick roll")
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+## Get Type And ID
+
+```py
+from zingmp3py import getUrlTypeAndID
+
+getUrlTypeAndID("https://zingmp3.vn/liveradio/IWZ979CW.html")
+```
```

### Comparing `zingmp3py-0.3.1/zingmp3py/zasync.py` & `zingmp3py-0.3.2/zingmp3py/zasync.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,108 @@
-import aiohttp
-import time
-import re
-from .util import *
-from .zsync import ZingMp3
-from .sobj import *
-
-cooke = {"cookies": {}, "last_updated": 0}
-apikey = {}
-async def get_ck(request: aiohttp.ClientSession):
-    if int(time.time() - 60) < int(time.time()):
-        async with request.get("https://zingmp3.vn") as r:
-            cooke["cookies"] = r.cookies
-            cooke["last_updated"] = int(time.time())
-            return cooke["cookies"]
-    else:
-        return cooke["cookies"]
-
-async def get_key():
-    if not apikey:
-        async with aiohttp.ClientSession() as s:
-            async with s.get("https://zjs.zmdcdn.me/zmp3-desktop/releases/v1.7.34/static/js/main.min.js") as r:
-                data = await r.text()
-            key = re.findall(r',h="(.*?)",p=\["ctime","id","type","page","count","version"\]', data)[0]
-            skey = re.findall(r"return d\(\)\(t\+r,\"(.*?)\"\)", data)[0]
-            apikey.update({"data": [key, skey]})
-            return [key, skey]
-    else:
-        return apikey["data"]
-
-async def requestZing(path, qs={}, haveParam=0):
-    apikey, skey = await get_key()
-    param = "&".join([f"{i}={k}" for i,k in qs.items()])
-    sig = hashParam(skey, path, param, haveParam)
-    qs.update({"apiKey": apikey})
-    qs.update({"ctime": sig[1]})
-    qs.update({"sig": sig[0]})
-    url = "https://zingmp3.vn" + path
-    async with aiohttp.ClientSession() as s:
-        ck = await get_ck(s)
-        async with s.get(url, params=qs, cookies=ck) as r:
-            data = await r.json()
-            if data['err'] != 0:
-                raise ZingMp3Error(data)
-            return data
-
-class Stream(Stream):
-    async def download(self, *args, **kwargs):
-        if not self.isVIP:
-            async with aiohttp.ClientSession() as s:
-                async with s.get(self.url, raise_for_status=True) as r:
-                    kwargs["mode"] = "wb"
-                    with open(*args, **kwargs) as streamfile:
-                        streamfile.write(await r.content.read())
-        else:
-            print("VIP Video Can Not Download")
-
-class Song(Song):
-    async def getStreaming(self):
-        return await self.client.getSongStreaming(self.id)
-
-
-class ZingMp3Async(ZingMp3):
-    async def getDetailPlaylist(self, id):
-        data = await requestZing("/api/v2/page/get/playlist", {"id": id})
-        return Playlist(data["data"], client=self)
-
-    async def getDetailArtist(self, alias):
-        data = await requestZing("/api/v2/page/get/artist", {"alias": alias}, 1)
-        return Artist(data["data"])
-
-    async def getRadioInfo(self, id):
-        data = await requestZing("/api/v2/livestream/get/info", {"id": id})
-        return LiveRadio(data["data"])
-
-    async def getSongInfo(self, id):
-        data = await requestZing("/api/v2/song/get/info", {"id": id})
-        return Song(data["data"], client=self)
-
-    async def getSongStreaming(self, id):
-        data = await requestZing("/api/v2/song/get/streaming", {"id": id})
-        return [Stream(i, c) for i, c in data["data"].items()]
-
-    async def getTop100(self):
-        data = await requestZing("/api/v2/page/get/top-100", haveParam=1)
-        dat = data["data"]
-        return [Playlist(j, client=self) for i in dat for j in i["items"]]
-
-    async def search(self, search):
-        data = await requestZing("/api/v2/search/multi", {"q": search}, 1)
-        return Search(data["data"], client=self)
+import aiohttp
+import time
+import re
+from .util import *
+from .zsync import ZingMp3
+from .sobj import *
+
+cooke = {"cookies": {}, "last_updated": 0}
+apikey = {}
+async def get_ck(request: aiohttp.ClientSession):
+    if int(cooke["last_updated"] + 60) < int(time.time()):
+        async with request.get("https://zingmp3.vn") as r:
+            cooke["cookies"] = r.cookies
+            cooke["last_updated"] = int(time.time())
+            return cooke["cookies"]
+    else:
+        return cooke["cookies"]
+
+async def get_key():
+    if not apikey:
+        async with aiohttp.ClientSession() as s:
+            async with s.get("https://zjs.zmdcdn.me/zmp3-desktop/releases/v1.7.34/static/js/main.min.js") as r:
+                data = await r.text()
+            key = re.findall(r',h="(.*?)",p=\["ctime","id","type","page","count","version"\]', data)[0]
+            skey = re.findall(r"return d\(\)\(t\+r,\"(.*?)\"\)", data)[0]
+            apikey.update({"data": [key, skey]})
+            return [key, skey]
+    else:
+        return apikey["data"]
+
+async def requestZing(path, qs={}, haveParam=0):
+    apikey, skey = await get_key()
+    param = "&".join([f"{i}={k}" for i,k in qs.items()])
+    sig = hashParam(skey, path, param, haveParam)
+    qs.update({"apiKey": apikey})
+    qs.update({"ctime": sig[1]})
+    qs.update({"sig": sig[0]})
+    url = "https://zingmp3.vn" + path
+    async with aiohttp.ClientSession() as s:
+        ck = await get_ck(s)
+        async with s.get(url, params=qs, cookies=ck) as r:
+            data = await r.json()
+            if data['err'] != 0:
+                raise ZingMp3Error(data)
+            return data
+
+class Stream(Stream):
+    async def download(self, *args, **kwargs):
+        if not self.isVIP:
+            async with aiohttp.ClientSession() as s:
+                async with s.get(self.url, raise_for_status=True) as r:
+                    kwargs["mode"] = "wb"
+                    with open(*args, **kwargs) as streamfile:
+                        streamfile.write(await r.content.read())
+        else:
+            print("VIP Video Can Not Download")
+
+class Song(Song):
+    async def getStreaming(self):
+        return await self.client.getSongStreaming(self.id)
+
+class Playlist(Playlist):
+    __slots__ = [
+        "id",
+        "title",
+        "indata",
+        "client"
+    ]
+
+    def __init__(self, indata, client):
+        self.id = indata["encodeId"]
+        self.indata = indata
+        self.title = indata['title']
+        self.client = client
+
+    @property
+    def songs(self):
+        return [Song(song, self.client) for song in self.indata['song']["items"]]
+
+class ZingMp3Async(ZingMp3):
+    async def getDetailPlaylist(self, id):
+        data = await requestZing("/api/v2/page/get/playlist", {"id": id})
+        return Playlist(data["data"], client=self)
+
+    async def getDetailArtist(self, alias):
+        data = await requestZing("/api/v2/page/get/artist", {"alias": alias}, 1)
+        return Artist(data["data"])
+
+    async def getRadioInfo(self, id):
+        data = await requestZing("/api/v2/livestream/get/info", {"id": id})
+        return LiveRadio(data["data"])
+
+    async def getSongInfo(self, id):
+        data = await requestZing("/api/v2/song/get/info", {"id": id})
+        return Song(data["data"], client=self)
+
+    async def getSongStreaming(self, id):
+        data = await requestZing("/api/v2/song/get/streaming", {"id": id})
+        return [Stream(i, c) for i, c in data["data"].items()]
+
+    async def getTop100(self):
+        data = await requestZing("/api/v2/page/get/top-100", haveParam=1)
+        dat = data["data"]
+        return [Playlist(j, client=self) for i in dat for j in i["items"]]
+
+    async def search(self, search):
+        data = await requestZing("/api/v2/search/multi", {"q": search}, 1)
+        return Search(data["data"], client=self)
```

### Comparing `zingmp3py-0.3.1/zingmp3py/zsync.py` & `zingmp3py-0.3.2/zingmp3py/zsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-import requests
-import re
-from .util import *
-from .sobj import *
-
-cooke = {"cookies": {}, "last_updated": 0}
-apikey = {}
-
-def get_ck(request: requests.Session):
-    if int(time.time() - 60) < int(time.time()):
-        with request.get("https://zingmp3.vn") as r:
-            cooke["cookies"] = r.cookies
-            cooke["last_updated"] = int(time.time())
-            return cooke["cookies"]
-    else:
-        return cooke["cookies"]
-
-def get_key():
-    if not apikey:
-        with requests.Session() as s:
-            with s.get("https://zjs.zmdcdn.me/zmp3-desktop/releases/v1.7.34/static/js/main.min.js") as r:
-                data = r.text
-            key = re.findall(r',h="(.*?)",p=\["ctime","id","type","page","count","version"\]', data)[0]
-            skey = re.findall(r"return d\(\)\(t\+r,\"(.*?)\"\)", data)[0]
-            apikey.update({"data": [key, skey]})
-            return [key, skey]
-    else:
-        return apikey["data"]
-
-def requestZing(path, qs={}, haveParam=0):
-    apikey, skey = get_key()
-    param = "&".join([f"{i}={k}" for i,k in qs.items()])
-    sig = hashParam(skey, path, param, haveParam)
-    qs.update({"apiKey": apikey})
-    qs.update({"ctime": sig[1]})
-    qs.update({"sig": sig[0]})
-    url = "https://zingmp3.vn" + path
-    with requests.Session() as s:
-        with s.get(url, params=qs, cookies=get_ck(s)) as r:
-            data = r.json()
-            if data['err'] != 0:
-                raise ZingMp3Error(data)
-            print(r.url)
-            return data
-
-class ZingMp3:
-    def __init__(self):
-        pass
-
-    def getDetailPlaylist(self, id):
-        data = requestZing("/api/v2/page/get/playlist", {"id": id})
-        return Playlist(data["data"], client=self)
-
-    def getDetailArtist(self, alias):
-        data = requestZing("/api/v2/page/get/artist", {"alias": alias}, 1)
-        return Artist(data["data"])
-
-    def getRadioInfo(self, id):
-        data = requestZing("/api/v2/livestream/get/info", {"id": id})
-        return LiveRadio(data["data"])
-
-    def getSongInfo(self, id):
-        data = requestZing("/api/v2/song/get/info", {"id": id})
-        return Song(data["data"], client=self)
-
-    def getSongStreaming(self, id):
-        data = requestZing("/api/v2/song/get/streaming", {"id": id})
-        return [Stream(i, c) for i, c in data["data"].items()]
-
-    def getTop100(self):
-        data = requestZing("/api/v2/page/get/top-100", haveParam=1)
-        dat = data["data"]
-        return [Playlist(j, client=self) for i in dat for j in i["items"]]
-
-    def search(self, search):
-        data = requestZing("/api/v2/search/multi", {"q": search}, 1)
-        return Search(data["data"], client=self)
-
-
+import requests
+import re
+from .util import *
+from .sobj import *
+
+cooke = {"cookies": {}, "last_updated": 0}
+apikey = {}
+
+def get_ck(request: requests.Session):
+    if int(cooke["last_updated"] - 60) < int(time.time()):
+        with request.get("https://zingmp3.vn") as r:
+            cooke["cookies"] = r.cookies
+            cooke["last_updated"] = int(time.time())
+            return cooke["cookies"]
+    else:
+        return cooke["cookies"]
+
+def get_key():
+    if not apikey:
+        with requests.Session() as s:
+            with s.get("https://zjs.zmdcdn.me/zmp3-desktop/releases/v1.7.34/static/js/main.min.js") as r:
+                data = r.text
+            key = re.findall(r',h="(.*?)",p=\["ctime","id","type","page","count","version"\]', data)[0]
+            skey = re.findall(r"return d\(\)\(t\+r,\"(.*?)\"\)", data)[0]
+            apikey.update({"data": [key, skey]})
+            return [key, skey]
+    else:
+        return apikey["data"]
+
+def requestZing(path, qs={}, haveParam=0):
+    apikey, skey = get_key()
+    param = "&".join([f"{i}={k}" for i,k in qs.items()])
+    sig = hashParam(skey, path, param, haveParam)
+    qs.update({"apiKey": apikey})
+    qs.update({"ctime": sig[1]})
+    qs.update({"sig": sig[0]})
+    url = "https://zingmp3.vn" + path
+    with requests.Session() as s:
+        with s.get(url, params=qs, cookies=get_ck(s)) as r:
+            data = r.json()
+            if data['err'] != 0:
+                raise ZingMp3Error(data)
+            return data
+
+class ZingMp3:
+    def __init__(self):
+        pass
+
+    def getDetailPlaylist(self, id):
+        data = requestZing("/api/v2/page/get/playlist", {"id": id})
+        return Playlist(data["data"], client=self)
+
+    def getDetailArtist(self, alias):
+        data = requestZing("/api/v2/page/get/artist", {"alias": alias}, 1)
+        return Artist(data["data"])
+
+    def getRadioInfo(self, id):
+        data = requestZing("/api/v2/livestream/get/info", {"id": id})
+        return LiveRadio(data["data"])
+
+    def getSongInfo(self, id):
+        data = requestZing("/api/v2/song/get/info", {"id": id})
+        return Song(data["data"], client=self)
+
+    def getSongStreaming(self, id):
+        data = requestZing("/api/v2/song/get/streaming", {"id": id})
+        return [Stream(i, c) for i, c in data["data"].items()]
+
+    def getTop100(self):
+        data = requestZing("/api/v2/page/get/top-100", haveParam=1)
+        dat = data["data"]
+        return [Playlist(j, client=self) for i in dat for j in i["items"]]
+
+    def search(self, search):
+        data = requestZing("/api/v2/search/multi", {"q": search}, 1)
+        return Search(data["data"], client=self)
+
+
```

### Comparing `zingmp3py-0.3.1/zingmp3py.egg-info/PKG-INFO` & `zingmp3py-0.3.2/zingmp3py.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-Metadata-Version: 2.1
-Name: zingmp3py
-Version: 0.3.1
-Summary: A Python library for the ZingMp3 API
-Author: The DT
-Author-email: The DT <duongtuan30306@gmail.com>
-Project-URL: Homepage, https://github.com/thedtvn/zingmp3py
-Project-URL: Bug Tracker, https://github.com/thedtvn/zingmp3py/issues
-Keywords: zingmp3,music,api,vietnam
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# zingmp3py
-#### A light weight Python library for the ZingMp3 API
-##### *all functions are return dict or ZingMp3 Object
-
-# Sync :
-```py
-from zingmp3py import ZingMp3
-
-zi = ZingMp3()
-zi.getDetailPlaylist("67ZFO8DZ")
-zi.getDetailArtist("Cammie")
-zi.getRadioInfo("IWZ979CW")
-zi.getSongInfo("ZWAF6UFD")
-zi.getSongStreaming("ZWAF6UFD")
-zi.getTop100()
-zi.search("rick roll")
-```
-
-# Async
-```py
-import asyncio
-from zingmp3py import ZingMp3Async
-
-async def main():
-    zi = ZingMp3Async()
-    await zi.getDetailPlaylist("67ZFO8DZ")
-    await zi.getDetailArtist("Cammie")
-    await zi.getSongInfo("ZWAF6UFD")
-    await zi.getSongStreaming("ZWAF6UFD")
-    await zi.getTop100()
-    await zi.search("rick roll")
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-```
-
-## Get Type And ID
-
-```py
-from zingmp3py import getUrlTypeAndID
-
-getUrlTypeAndID("https://zingmp3.vn/liveradio/IWZ979CW.html")
-```
+Metadata-Version: 2.1
+Name: zingmp3py
+Version: 0.3.2
+Summary: A light weight Python library for the ZingMp3 API
+Author: The DT
+Author-email: duongtuan30306@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# zingmp3py
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
+#### A light weight Python library for the ZingMp3 API
+##### *all functions are return dict or ZingMp3 Object
+
+# install 
+
+## pypi
+```
+pip install zingmp3py
+```
+
+## Git (version in development)
+```
+pip install git+https://github.com/thedtvn/zingmp3py.git
+```
+
+
+# Sync :
+```py
+from zingmp3py import ZingMp3
+
+zi = ZingMp3()
+zi.getDetailPlaylist("67ZFO8DZ")
+zi.getDetailArtist("Cammie")
+zi.getRadioInfo("IWZ979CW")
+zi.getSongInfo("ZWAF6UFD")
+zi.getSongStreaming("ZWAF6UFD")
+zi.getTop100()
+zi.search("rick roll")
+```
+
+# Async
+```py
+import asyncio
+from zingmp3py import ZingMp3Async
+
+async def main():
+    zi = ZingMp3Async()
+    await zi.getDetailPlaylist("67ZFO8DZ")
+    await zi.getDetailArtist("Cammie")
+    await zi.getSongInfo("ZWAF6UFD")
+    await zi.getSongStreaming("ZWAF6UFD")
+    await zi.getTop100()
+    await zi.search("rick roll")
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+## Get Type And ID
+
+```py
+from zingmp3py import getUrlTypeAndID
+
+getUrlTypeAndID("https://zingmp3.vn/liveradio/IWZ979CW.html")
+```
```

