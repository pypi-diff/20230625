# Comparing `tmp/pywss-0.1.8.tar.gz` & `tmp/pywss-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pywss-0.1.8.tar", last modified: Thu Oct 13 12:13:47 2022, max compression
+gzip compressed data, was "dist\pywss-0.1.9.tar", last modified: Tue Nov 15 12:29:27 2022, max compression
```

## Comparing `pywss-0.1.8.tar` & `pywss-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 12:13:47.000000 pywss-0.1.8/
--rw-rw-rw-   0        0        0      381 2022-10-13 12:13:47.000000 pywss-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-13 12:13:47.000000 pywss-0.1.8/pywss/
--rw-rw-rw-   0        0        0      449 2022-09-30 05:41:32.000000 pywss-0.1.8/pywss/closing.py
--rw-rw-rw-   0        0        0     1639 2022-10-01 13:40:15.000000 pywss-0.1.8/pywss/headers.py
--rw-rw-rw-   0        0        0     5514 2022-09-30 05:41:32.000000 pywss-0.1.8/pywss/openapi.py
--rw-rw-rw-   0        0        0      951 2022-09-30 05:41:32.000000 pywss-0.1.8/pywss/routing.py
--rw-rw-rw-   0        0        0     1786 2022-09-30 05:41:32.000000 pywss-0.1.8/pywss/static.py
--rw-rw-rw-   0        0        0     1961 2022-09-30 05:41:32.000000 pywss-0.1.8/pywss/statuscode.py
--rw-rw-rw-   0        0        0     3959 2022-10-01 13:40:15.000000 pywss-0.1.8/pywss/testing.py
--rw-rw-rw-   0        0        0     3054 2022-10-13 12:07:37.000000 pywss-0.1.8/pywss/websocket.py
--rw-rw-rw-   0        0        0    18142 2022-10-13 12:12:51.000000 pywss-0.1.8/pywss/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 12:13:47.000000 pywss-0.1.8/pywss.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-13 12:13:46.000000 pywss-0.1.8/pywss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      381 2022-10-13 12:13:46.000000 pywss-0.1.8/pywss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2022-10-13 12:13:46.000000 pywss-0.1.8/pywss.egg-info/requires.txt
--rw-rw-rw-   0        0        0      338 2022-10-13 12:13:47.000000 pywss-0.1.8/pywss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-10-13 12:13:46.000000 pywss-0.1.8/pywss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8194 2022-10-13 12:07:37.000000 pywss-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2022-10-13 12:13:47.000000 pywss-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1224 2022-09-30 05:41:32.000000 pywss-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-13 12:13:47.000000 pywss-0.1.8/test/
--rw-rw-rw-   0        0        0    21213 2022-10-13 12:07:37.000000 pywss-0.1.8/test/test_base.py
+drwxrwxrwx   0        0        0        0 2022-11-15 12:29:27.000000 pywss-0.1.9/
+-rw-rw-rw-   0        0        0      381 2022-11-15 12:29:27.000000 pywss-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss/
+-rw-rw-rw-   0        0        0      449 2022-09-23 09:07:49.000000 pywss-0.1.9/pywss/closing.py
+-rw-rw-rw-   0        0        0     1639 2022-11-15 11:55:11.000000 pywss-0.1.9/pywss/headers.py
+-rw-rw-rw-   0        0        0     5514 2022-09-23 08:42:03.000000 pywss-0.1.9/pywss/openapi.py
+-rw-rw-rw-   0        0        0      951 2022-09-23 08:42:03.000000 pywss-0.1.9/pywss/routing.py
+-rw-rw-rw-   0        0        0     1786 2022-11-15 11:53:54.000000 pywss-0.1.9/pywss/static.py
+-rw-rw-rw-   0        0        0     1961 2022-09-27 08:32:24.000000 pywss-0.1.9/pywss/statuscode.py
+-rw-rw-rw-   0        0        0     4038 2022-11-15 12:25:54.000000 pywss-0.1.9/pywss/testing.py
+-rw-rw-rw-   0        0        0     3054 2022-10-08 06:13:22.000000 pywss-0.1.9/pywss/websocket.py
+-rw-rw-rw-   0        0        0    18444 2022-11-15 12:27:50.000000 pywss-0.1.9/pywss/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      381 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      338 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2022-11-15 12:29:27.000000 pywss-0.1.9/pywss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9411 2022-10-26 08:38:26.000000 pywss-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-11-15 12:29:27.000000 pywss-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2022-09-23 09:57:30.000000 pywss-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-15 12:29:27.000000 pywss-0.1.9/test/
+-rw-rw-rw-   0        0        0    21213 2022-11-15 12:01:59.000000 pywss-0.1.9/test/test_base.py
```

### Comparing `pywss-0.1.8/pywss/headers.py` & `pywss-0.1.9/pywss/headers.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/openapi.py` & `pywss-0.1.9/pywss/openapi.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/routing.py` & `pywss-0.1.9/pywss/routing.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/static.py` & `pywss-0.1.9/pywss/static.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/statuscode.py` & `pywss-0.1.9/pywss/statuscode.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/testing.py` & `pywss-0.1.9/pywss/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
             header_list.append(f"{k}: {v}")
         header = "\r\n".join(header_list)
         req_message = f"{self.method} {self.path} HTTP/1.1\r\n{header}\r\n\r\n{self.body}"
 
         s, c = socket.socketpair()
         with s, c:
             c.sendall(req_message.encode())
+            c.sendall("GET / HTTP/1.1\r\nConnection: close\r\n\r\n".encode())
             self.app._(s, None)
             resp = c.makefile("rb", -1)
             return HttpTestResponse(resp.readlines())
 
     def get(self, route, headers=None, json=None, data=""):
         return self.request("GET", route, headers, json, data)
```

### Comparing `pywss-0.1.8/pywss/websocket.py` & `pywss-0.1.9/pywss/websocket.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/pywss/__init__.py` & `pywss-0.1.9/pywss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pywss.websocket import WebSocketUpgrade, WebSocketContextWrap
 from pywss.testing import HttpTestRequest, HttpTestResponse
 from pywss.static import NewStaticHandler
 from pywss.closing import Closing
 from pywss.routing import Route
 from pywss.openapi import openapi_ui_template, merge_dict, parameters_filter
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 
 class Context:
     _handler_index = 0
     _flush_header = False
 
     def __init__(self, app, fd, address, log, rfd, method, path, paths, version, headers, route, handlers):
@@ -384,51 +384,55 @@
             openapi_ui_css_url,
         )))
 
     def _(self, request: socket.socket, address: tuple) -> None:
         log = self.log
         try:
             rfd = request.makefile("rb", -1)
-            method, path, version, err = parse_request_line(rfd)
-            if err:
-                request.sendall(b"HTTP/1.1 400 BadRequest\r\n")
-                return
-            log = log.update(method=method, path=path)
-            hes, err = parse_headers(rfd)
-            if err:
-                request.sendall(b"HTTP/1.1 400 BadRequest\r\n")
-                log.error(err)
-                return
-            # full match
-            paths = {}
-            route = f"{method.upper()}/{path.split('?', 1)[0].strip('/')}"
-            handlers = self.full_match_routes.get(route, None)
-            # parser match
-            if not handlers:
-                for r, v in self.parse_match_routes:
-                    fix, ps = r.match(route)
-                    if fix:
-                        route = r.route
-                        handlers = v
-                        paths = ps
-                        break
-            # head match
-            if not handlers:
-                for r, v in self.head_match_routes:
-                    if route.startswith(r):
-                        route = r
-                        handlers = v
-                        break
-            if not handlers:
-                request.sendall(b"HTTP/1.1 404 NotFound\r\n")
-                log.warning("No Handler")
-                return
-            ctx = Context(self, request, address, log, rfd, method, path, paths, version, hes, route, handlers)
-            ctx.next()
-            ctx.flush()
+            while True:
+                method, path, version, err = parse_request_line(rfd)
+                if err:
+                    request.sendall(b"HTTP/1.1 400 BadRequest\r\n")
+                    return
+                log = log.update(method=method, path=path)
+                hes, err = parse_headers(rfd)
+                if err:
+                    request.sendall(b"HTTP/1.1 400 BadRequest\r\n")
+                    log.error(err)
+                    return
+                # check keep alive
+                if hes.get("Connection", "").lower() == "close":
+                    break
+                # full match
+                paths = {}
+                route = f"{method.upper()}/{path.split('?', 1)[0].strip('/')}"
+                handlers = self.full_match_routes.get(route, None)
+                # parser match
+                if not handlers:
+                    for r, v in self.parse_match_routes:
+                        fix, ps = r.match(route)
+                        if fix:
+                            route = r.route
+                            handlers = v
+                            paths = ps
+                            break
+                # head match
+                if not handlers:
+                    for r, v in self.head_match_routes:
+                        if route.startswith(r):
+                            route = r
+                            handlers = v
+                            break
+                if not handlers:
+                    request.sendall(b"HTTP/1.1 404 NotFound\r\n")
+                    log.warning("No Handler")
+                    return
+                ctx = Context(self, request, address, log, rfd, method, path, paths, version, hes, route, handlers)
+                ctx.next()
+                ctx.flush()
         except ConnectionAbortedError:
             log.error("connect abort")
         except:
             log.traceback()
         finally:
             try:
                 request.shutdown(socket.SHUT_WR)
```

### Comparing `pywss-0.1.8/README.md` & `pywss-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,63 @@
 [![codecov](https://codecov.io/gh/czasg/pywss/branch/master/graph/badge.svg?token=JSXIQXY1EQ)](https://codecov.io/gh/czasg/pywss)
 
 > pip3 install pywss
 
 **Pywss 是一个轻量级的 Python Web 框架。**     
 
 主要特性：   
-- [x] websocket upgrade
-- [x] openapi & swagger ui
-- [x] middleware
-- [x] static server
-- [x] api test
+- [x] WebSocket Upgrade
+- [x] OpenAPI & Swagger-UI
+- [x] API Test
+- [x] Middleware
+- [x] Static Server
+
+<details>
+  <summary>重点版本迭代说明</summary>
+
+- 0.1.4
+  * 修复`signal`无法在子线程注册
+- 0.1.3
+  * 支持`openapi`
+  * 支持`swagger ui`
+- 0.1.2
+  * 修复`Content-Length`丢失问题
+- 0.1.1
+  * 项目重构
+
+</details>
+
+<br/>
+
+## 一、快速开始
+
+1、安装 pywss
+```shell
+pip install pywss
+```
+2、创建 main.py，写入以下代码：
+```python
+import pywss
 
-[版本迭代历史](https://github.com/czasg/pywss/wiki/version-history)
+def hello(ctx: pywss.Context):
+  ctx.write("hello world")
 
-## 一、快速使用手册
+if __name__ == '__main__':
+    app = pywss.App()
+    app.get("/hello", hello)
+    app.run()
+```
+3、启动服务
+```shell
+python main.py
+```
+
+<br/>
 
+## 二、进阶使用
 - [1、初始化app](#1初始化app)
 - [2、绑定路由](#2绑定路由)
 - [3、创建子路由](#3创建子路由)
 - [4、使用中间件](#4使用中间件)
 - [5、升级WebSocket](#5升级WebSocket)
 - [6、openapi & swagger ui](#6openapi--swagger-ui)
 - [7、静态文件服务器](#7静态文件服务器)
@@ -36,14 +75,16 @@
 # 启动服务
 app.run(port=8080)  
 ```
 默认:
 - `host="0.0.0.0"`
 - `port=8080`
 
+<br/>
+
 ### 2、绑定路由
 ```python
 import pywss
 
 def hello(ctx: pywss.Context):
     ctx.write({"hello": ctx.paths["name"]})
 
@@ -53,29 +94,34 @@
 app.get("/hello", lambda ctx: ctx.write({"hello": "world"}))
 
 # 注册路由
 app.post("/hello/{name}", hello)
 
 app.run(port=8080)
 ```
-`handler`仅接收一个参数，就是`pywss.Context`。路由支持：  
+路由处理函数`handler`仅接收一个参数，就是`pywss.Context`。
+
+除此之外，路由支持多种匹配方式：  
 - `/hello/world`：精确匹配
-- `/hello/{world}`：局部匹配，路径参数可通过`ctx.paths`获取
-- `/hello/*`：模糊匹配
+- `/hello/{world}`：局部匹配（注意：对应路径参数可通过`ctx.paths["world"]`获取`）
+- `/hello/*`：模糊匹配（注意：路由最后一位必须是`*`）
 
 在终端界面执行：
 ```shell script
 $ curl localhost:8080/hello
 {"hello": "world"}
 
 $ curl -X POST localhost:8080/hello/pywss
 {"hello": "pywss"}
 ```
 
+<br/>
+
 ### 3、创建子路由
+pywss 支持通过`app.party`来实现丰富的路由管理
 ```python
 import pywss
 
 def hello(ctx: pywss.Context):
     ctx.write({"hello": ctx.path})
 
 app = pywss.App()
@@ -101,15 +147,20 @@
 $ curl localhost:8080/api/v2/hello
 {"hello": "v2"}
 
 $ curl -X POST localhost:8080/api/v2/hello/pywss
 {"hello": "/api/v2/hello/pywss"}
 ```
 
+<br/>
+
 ### 4、使用中间件
+pywss 支持通过`use`注册全局中间件，也支持单个路由绑定中间件。  
+
+使用中间件时，注意需要调用`ctx.next()`才能继续执行往后执行，否则会中断此次请求。 
 ```python
 import pywss, time
 
 # 日志中间件，单次请求结束后输出cost耗时 - 根据响应码判断输出不同级别日志
 def log_handler(ctx: pywss.Context):  
     start = time.time()
     ctx.next()  # 调用 next 进入到下一个 handler
@@ -135,18 +186,20 @@
 app.use(log_handler)  
 
 # 中间件也可以直接路由处注册
 app.get("/hello/{name}", auth_handler, lambda ctx: ctx.write({"hello": "world"}))  
 
 app.run()
 ```
-支持 `use` 注册全局中间件，也支持单个路由绑定中间件。    
-使用中间件时需要调用 `ctx.next()` 以便继续执行，否则会中断此次请求。     
+
+<br/>
 
 ### 5、升级WebSocket
+WebSocket 本质基于 HTTP GET 升级实现，Pywss 则通过`WebSocketUpgrade`完成此处升级。    
+
 ```python
 import pywss
 
 def websocket(ctx: pywss.Context):
     # 升级 WebSocket
     err = pywss.WebSocketUpgrade(ctx)
     if err:
@@ -162,15 +215,14 @@
 
 app = pywss.App()
 
 app.get("/websocket", websocket)
 
 app.run()
 ``` 
-WebSocket 本质基于 GET 升级实现，Pywss 则通过 `WebSocketUpgrade` 完成此处升级。    
 测试需要`打开浏览器 -> F12 -> 控制台`，输入以下代码：
 ```
 ws = new WebSocket("ws://127.0.0.1:8080/websocket");
 ws.onmessage = function (ev) {
     console.log(ev.data);
 }
 ws.onclose = function (ev) {
@@ -181,14 +233,16 @@
         ws.send('hello??')
     }
 }
 ```
 
 其他具体使用场景/用例，可以参考 [多人在线协同编辑luckysheet](./demo/luckysheet)、[多人聊天室](./demo/chat)
 
+<br/>
+
 ### 6、openapi & swagger ui
 ```python
 import pywss
 
 @pywss.openapi.docs(
     summary="此处是接口摘要 - 可选",
     description="此处是接口描述 - 可选",
@@ -222,14 +276,16 @@
 
 app.post("/hello/{name}", hello)
 
 app.run()
 ```
 打开浏览器，访问 [localhost:8080/docs](http://localhost:8080/docs)
 
+<br/>
+
 ### 7、静态文件服务器
 ```python
 import pywss
 
 app = pywss.App()
 
 # 注册静态资源，需要指定文件根目录
@@ -241,14 +297,16 @@
 ```text
 - rootDir
     - index.html
     - 200.html
     - 500.html
 ```
 
+<br/>
+
 ### 8、单元测试
 ```python
 import pywss
 
 app = pywss.App()
 
 app.get("/test", lambda ctx: ctx.set_status_code(204))
@@ -259,38 +317,41 @@
 # 发起Get请求，获取resp
 resp = req.get("/test")  
 
 assert resp.status_code == 204
 ```
 可以参考 [pywss单元测试](test/test_base.py)
 
-## 二、参数说明
+<br/>
+
+## 三、参数说明
 ### 1、请求参数
 * Context
     * `ctx.app`: app
-    * `ctx.fd`: socket 句柄
-    * `ctx.method`: 字符串类型，请求方法，如 `GET/POST/PUT/DELETE`
-    * `ctx.path`: 字符串类型，请求路径，如 `/api/v1/query`
-    * `ctx.paths`: 字典类型，请求路径参数，如 `/api/v1/query/{name}`
-    * `ctx.route`: 字符串类型，匹配路由的路径，如 `GET/api/v1/query`
-    * `ctx.cookies`: 字典类型，表示 cookies
-    * `ctx.content`: 原生二进制请求体
-    * `ctx.body()`: 字符串类型。等同于 `ctx.content.decode()`
-    * `ctx.json()`: 获取 json 请求
-    * `ctx.form()`: 获取 form 请求，文件数据也会存放于此
-    * `ctx.params`: 字典类型，获取 url 路由参数，类似 `?code=1&callback=2` 会解析成 `{"code": "1", "callback": "2"}`
-        * 多个同名会以列表形式存放，`?code=1&code=2` 会解析成 `{"code": ["1", "2"]}`
-    * `ctx.headers`: 字典类型，获取 url 请求头
+    * `ctx.fd`: `socket.socket`类型，一般用于写操作
+    * `ctx.rfd`: `socket.makefile`类型，一般用于读操作
+    * `ctx.method`: `str`类型，请求方法，如 `GET/POST/PUT/DELETE`
+    * `ctx.path`: `str`类型，请求路径，如 `/api/v1/query`
+    * `ctx.paths`: `dict`类型，请求路径参数，如 `/api/v1/query/{name}`
+    * `ctx.route`: `str`类型，匹配路由的路径，如 `GET/api/v1/query`
+    * `ctx.cookies`: `dict`类型，用于存储请求`cookies`数据
+    * `ctx.body()`: `bytes`类型，获取用户请求报文`body`
+    * `ctx.json()`: 解析用户请求，等同于`json.loads(self.body())`，需要遵循一定`json`格式
+    * `ctx.form()`: 解析用户请求，需要遵循一定`form`格式
+    * `ctx.params`: `dict`类型，用于存储解析的`query`参数
+        * `http://github.com/czasg/pywss?code=1&callback=2`->`{"code": "1", "callback": "2"}`
+        * `http://github.com/czasg/pywss?code=1&code=2`->`{"code": ["1", "2"]}`
+    * `ctx.headers`: `dict`类型，用于存储解析的`header`参数
 
 ### 2、响应参数
 * Context
-    * `ctx.set_status_code`: -
-    * `ctx.set_header`: -
-    * `ctx.set_content_type`: -
-    * `ctx.set_cookie`: -
-    * `ctx.write`: -
-    * `ctx.write_text`: -
-    * `ctx.write_json`: -
-    * `ctx.write_file`: -
-    * `ctx.ws_read`: WebSocket 专用
-    * `ctx.ws_write`: WebSocket 专用
+    * `ctx.set_status_code`: 设置响应状态码
+    * `ctx.set_header`: 设置响应头
+    * `ctx.set_content_type`: 设置响应类型
+    * `ctx.set_cookie`: 设置响应`cookie`
+    * `ctx.write`: 用于写请求
+    * `ctx.write_text`: 同`ctx.write`
+    * `ctx.write_json`: 同`ctx.write`
+    * `ctx.write_file`: 同`ctx.write`
+    * `ctx.ws_read`: WebSocket 读请求，需要`pywss.WebSocketUpgrade`升级后使用
+    * `ctx.ws_write`: WebSocket 写请求，需要`pywss.WebSocketUpgrade`升级后使用
     * `ctx.flush`: 一般不需要自己调用
```

### Comparing `pywss-0.1.8/setup.py` & `pywss-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pywss-0.1.8/test/test_base.py` & `pywss-0.1.9/test/test_base.py`

 * *Files identical despite different names*

