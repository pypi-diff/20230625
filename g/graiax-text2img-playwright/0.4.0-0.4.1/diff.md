# Comparing `tmp/graiax-text2img-playwright-0.4.0.tar.gz` & `tmp/graiax_text2img_playwright-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graiax-text2img-playwright-0.4.0.tar", last modified: Sun Mar 26 14:37:53 2023, max compression
+gzip compressed data, was "graiax_text2img_playwright-0.4.1.tar", last modified: Sun Jun 25 10:54:31 2023, max compression
```

## Comparing `graiax-text2img-playwright-0.4.0.tar` & `graiax_text2img_playwright-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-03-26 14:37:39.694522 graiax-text2img-playwright-0.4.0/LICENSE
--rw-r--r--   0        0        0     2406 2023-03-26 14:37:39.694522 graiax-text2img-playwright-0.4.0/README.md
--rw-r--r--   0        0        0     1154 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      709 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/__init__.py
--rw-r--r--   0        0        0     3661 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/converter.py
--rw-r--r--   0        0        0        0 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/__init__.py
--rw-r--r--   0        0        0      360 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/container.css
--rw-r--r--   0        0        0    23531 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/github.css
--rw-r--r--   0        0        0     5895 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/one-dark.css
--rw-r--r--   0        0        0      279 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/reset.css
--rw-r--r--   0        0        0        0 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/__init__.py
--rw-r--r--   0        0        0     3188 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/__init__.py
--rw-r--r--   0        0        0     1772 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/highlight_lines.py
--rw-r--r--   0        0        0     1094 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/highlighter.py
--rw-r--r--   0        0        0     2202 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/language_resolver.py
--rw-r--r--   0        0        0     2683 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/container.py
--rw-r--r--   0        0        0     9067 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/renderer.py
--rw-r--r--   0        0        0     1300 2023-03-26 14:37:39.698522 graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/utils.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 graiax-text2img-playwright-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2406 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/README.md
+-rw-r--r--   0        0        0     1469 2023-06-25 10:54:31.276335 graiax_text2img_playwright-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/__init__.py
+-rw-r--r--   0        0        0     3661 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/converter.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/container.css
+-rw-r--r--   0        0        0    23531 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/github.css
+-rw-r--r--   0        0        0     5895 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/one-dark.css
+-rw-r--r--   0        0        0      279 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/reset.css
+-rw-r--r--   0        0        0        0 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/__init__.py
+-rw-r--r--   0        0        0     3188 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/highlight_lines.py
+-rw-r--r--   0        0        0     1094 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/highlighter.py
+-rw-r--r--   0        0        0     2202 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/language_resolver.py
+-rw-r--r--   0        0        0     2683 2023-06-25 10:54:16.708020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/container.py
+-rw-r--r--   0        0        0     9296 2023-06-25 10:54:16.712020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/renderer.py
+-rw-r--r--   0        0        0     2002 2023-06-25 10:54:16.712020 graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/utils.py
+-rw-r--r--   0        0        0     3405 1970-01-01 00:00:00.000000 graiax_text2img_playwright-0.4.1/PKG-INFO
```

### Comparing `graiax-text2img-playwright-0.4.0/LICENSE` & `graiax_text2img_playwright-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/README.md` & `graiax_text2img_playwright-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/__init__.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/converter.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/converter.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/github.css` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/github.css`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/css/one-dark.css` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/css/one-dark.css`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/__init__.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/__init__.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/highlight_lines.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/highlight_lines.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/highlighter.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/highlighter.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/code/language_resolver.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/code/language_resolver.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/plugins/container.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/plugins/container.py`

 * *Files identical despite different names*

### Comparing `graiax-text2img-playwright-0.4.0/src/graiax/text2img/playwright/renderer.py` & `graiax_text2img_playwright-0.4.1/src/graiax/text2img/playwright/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from graiax.playwright import PlaywrightBrowser, PlaywrightContext
 from graiax.playwright.interface import Parameters as PageOption
 from launart import Launart
 from playwright.async_api import Browser, BrowserContext, Page
 from playwright.async_api._generated import Locator
 from typing_extensions import TypedDict
 
+from .utils import run_always_await
+
 
 class FloatRect(TypedDict):
     x: float
     y: float
     width: float
     height: float
 
@@ -85,35 +87,35 @@
     Args:
         page_option (PageOption, optional): 截图时使用的页面设置.
             参数介绍详见：https://playwright.dev/python/docs/api/class-browser#browser-new-page
         screenshot_option (ScreenshotOption, optional): 截图设置.
         css (Sequence[Union[BuiltinCSS, str]], optional): 要加载的 CSS.
             默认包含 Reset CSS、GitHub Markdown 样式、One Dark 代码高亮主题、VitePress 样式的 container CSS.
             如有不需要或想覆盖这些默认 CSS，则传入一个包含 CSS 字符串的列表.
-        page_modifiers (List[Callable[[Page], Awaitable]], optional): 接受 Page 实例的方法/函数.
+        page_modifiers (List[Callable[[Page], Union[Awaitable[None], None]]], optional): 接受 Page 实例的方法/函数.
             用于对 Page 本身进行额外的修改，如: 使用 page.route 重定向资源文件到本地文件.
     """
 
     page_option: PageOption
     screenshot_option: ScreenshotOption
     style: str
-    page_modifiers: List[Callable[[Page], Awaitable]]
+    page_modifiers: List[Callable[[Page], Union[Awaitable[None], None]]]
 
     def __init__(
         self,
         page_option: Optional[PageOption] = None,
         screenshot_option: Optional[ScreenshotOption] = None,
         *,
         css: Sequence[Union[BuiltinCSS, str]] = (
             BuiltinCSS.reset,
             BuiltinCSS.github,
             BuiltinCSS.one_dark,
             BuiltinCSS.container,
         ),
-        page_modifiers: Optional[List[Callable[[Page], Awaitable]]] = None,
+        page_modifiers: Optional[List[Callable[[Page], Union[Awaitable[None], None]]]] = None,
     ):
         if isinstance(css, str):
             css = [css]
         page_option = page_option or {}
         screenshot_option = screenshot_option or {}
         screenshot_option = {"full_page": True, "type": "jpeg", **screenshot_option}
 
@@ -125,62 +127,64 @@
     @overload
     async def render(
         self,
         content: str,
         *,
         extra_screenshot_option: Optional[ScreenshotOption] = None,
         extra_page_option: Optional[PageOption] = None,
-        extra_page_modifiers: Optional[List[Callable[[Page], Awaitable]]] = None,
+        extra_page_modifiers: Optional[List[Callable[[Page], Union[Awaitable[None], None]]]] = None,
         browser: Optional[Browser] = None,
     ) -> bytes:
         ...
 
     @overload
     async def render(
         self,
         content: str,
         *,
         extra_screenshot_option: Optional[ScreenshotOption] = None,
-        extra_page_modifiers: Optional[List[Callable[[Page], Awaitable]]] = None,
+        extra_page_modifiers: Optional[List[Callable[[Page], Union[Awaitable[None], None]]]] = None,
         context: BrowserContext,
     ) -> bytes:
         ...
 
     async def render(
         self,
         content: str,
         *,
         extra_screenshot_option: Optional[ScreenshotOption] = None,
         extra_page_option: Optional[PageOption] = None,
-        extra_page_modifiers: Optional[List[Callable[[Page], Awaitable]]] = None,
+        extra_page_modifiers: Optional[List[Callable[[Page], Union[Awaitable[None], None]]]] = None,
         browser: Optional[Browser] = None,
         context: Optional[BrowserContext] = None,
     ) -> bytes:
         """渲染 HTML 代码为图片
 
         Args:
             content (str): 要渲染的 HTML 代码
             extra_screenshot_option (Optional[ScreenshotOption], optional): 额外的截图选项.
             extra_page_option (Optional[PageOption], optional): 额外的页面设置.
-            extra_page_modifiers (List[Callable[[Page], Awaitable]], optional): 接受 `Page` 实例的方法/函数.
+            extra_page_modifiers (List[Callable[[Page], Union[Awaitable[None], None]]], optional): 接受 `Page` 实例的方法/函数.
                 用于对 Page 本身进行额外的修改，如: 使用 `page.route` 重定向资源文件到本地文件.
                 仅本次截图使用.
             browser (Optional[Browser], optional): Playwright 异步浏览器实例，
                 如果 `context` 和 `browser` 都不传入则会通过 `Launart` 自动获取.
                 当使用持久上下文（Persistence Context）模式启动 Playwright 时，
                 不支持 `page_option` 和 `extra_page_option`.
             context (Optional[BrowserContext], optional): Playwright 浏览器上下文实例，
                 如果 `context` 和 `browser` 都不传入则会通过 `Launart` 自动获取.
                 与 `browser` 参数互斥，且不支持 `page_option` 和 `extra_page_option`.
 
         Returns:
             bytes: 渲染结果图的 bytes 数据
         """
         screenshot_option: ScreenshotOption = {**self.screenshot_option, **(extra_screenshot_option or {})}
-        page_modifiers: List[Callable[[Page], Awaitable]] = self.page_modifiers + (extra_page_modifiers or [])
+        page_modifiers: List[Callable[[Page], Union[Awaitable[None], None]]] = self.page_modifiers + (
+            extra_page_modifiers or []
+        )
 
         launart = Launart.current()
         page_option: PageOption = {**self.page_option, **(extra_page_option or {})}
 
         if browser is None:
             if context is None:
                 context = launart.get_interface(PlaywrightContext)
@@ -198,15 +202,15 @@
             browser = browser or launart.get_interface(PlaywrightBrowser)
             page_option: PageOption = {**self.page_option, **(extra_page_option or {})}
             page = await browser.new_page(**page_option)
         else:
             raise ValueError("Argument `browser` and `context` conflict with each other.")
 
         for modifier in page_modifiers:
-            await modifier(page)
+            await run_always_await(modifier, page)
 
         await page.set_content(
             '<html><head><meta name="viewport" content="width=device-width,initial-scale=1.0">'
             f"<style>{self.style}</style></head><body>{content}<body></html>"
         )
         result = await page.screenshot(**screenshot_option)
         await page.close()
```

### Comparing `graiax-text2img-playwright-0.4.0/PKG-INFO` & `graiax_text2img_playwright-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 Metadata-Version: 2.1
 Name: graiax-text2img-playwright
-Version: 0.4.0
+Version: 0.4.1
 Summary: 基于 Playwright 的适用于 Graia 的文转图工具
+Keywords: graia graiax text2img playwright
+Author-Email: Redlnn <w731347477@gmail.com>, BlueGlassBlock <blueglassblock@outlook.com>
 License: MIT
-Keywords: graia,graiax,text2img,playwright
-Author-email: Redlnn <w731347477@gmail.com>,BlueGlassBlock <blueglassblock@outlook.com>
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/GraiaCommunity/graiax-text2img-playwright
 Requires-Python: >=3.8.1
-Project-URL: repository, https://github.com/GraiaCommunity/graiax-text2img-playwright
+Requires-Dist: graiax-playwright<0.3.0,>=0.2.3
+Requires-Dist: launart<0.7.0,>=0.6.3
+Requires-Dist: markdown-it-py[linkify,plugins]<4.0.0,>=3.0.0
+Requires-Dist: pygments>=2.13.0
+Requires-Dist: typing-extensions
+Requires-Dist: mdit-py-emoji>=0.1.1
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # GraiaX TextToImage (Playwright)
 
 *基于 Playwright 的适用于 Graia 的文转图工具*
@@ -73,8 +86,7 @@
 ## 预览
 
 ![预览图](preview.jpg)
 
 ## 许可证
 
 本项目使用 [`MIT`](./LICENSE) 许可证进行许可。
-
```

