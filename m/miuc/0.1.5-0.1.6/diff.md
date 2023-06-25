# Comparing `tmp/miuc-0.1.5.tar.gz` & `tmp/miuc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.5.tar", max compression
+gzip compressed data, was "miuc-0.1.6.tar", max compression
```

## Comparing `miuc-0.1.5.tar` & `miuc-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.5/LICENSE
--rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.5/miuc/__init__.py
--rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.5/miuc/main.py
--rw-r--r--   0        0        0    23066 2023-06-23 15:00:31.533250 miuc-0.1.5/miuc/site_processor.py
--rw-r--r--   0        0        0     1888 2023-06-23 17:43:34.626260 miuc-0.1.5/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-23 17:44:03.181976 miuc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1334 2023-06-23 17:31:22.612187 miuc-0.1.5/README.md
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 miuc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.6/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.6/miuc/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.6/miuc/main.py
+-rw-r--r--   0        0        0    24888 2023-06-24 15:19:04.030351 miuc-0.1.6/miuc/site_processor.py
+-rw-r--r--   0        0        0     2125 2023-06-24 15:20:57.077677 miuc-0.1.6/miuc/utils.py
+-rw-r--r--   0        0        0     2047 2023-06-24 14:45:49.745689 miuc-0.1.6/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-24 15:54:39.149265 miuc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1463 2023-06-24 15:24:40.722303 miuc-0.1.6/README.md
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 miuc-0.1.6/PKG-INFO
```

### Comparing `miuc-0.1.5/LICENSE` & `miuc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `miuc-0.1.5/miuc/main.py` & `miuc-0.1.6/miuc/main.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.5/miuc/site_processor.py` & `miuc-0.1.6/miuc/site_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,15 @@
 *@Github: luzhixing12345
 """
 
 import re
 import requests
 import urllib
 import json
-
-
-def guess_name_by_url(url):
-    """
-    when could not access the website or get the html, guess the name by url
-    """
-    url_title = re.sub(r"^https?://", "", url)
-    urls = url_title.split(".")
-    if urls[0] == 'www':
-        urls = urls[1:-1]
-    else:
-        urls = urls[:-1]
-    # remove top domains
-    url_title = ".".join(urls)
-    return f"[{url_title}]({url})"
+from .utils import guess_name_by_url
 
 
 class Error(Exception):
     def __init__(self, url: str, class_name: str, message: str = None) -> None:  # pragma: no cover
         super().__init__()
         self.url = url
         self.class_name = class_name
@@ -48,14 +34,16 @@
             "Content-Type": "text/html;charset=utf-8",
         }
 
     def __call__(self, url: str):
         self.url: str = url
         self.parse()
         title = self.format()
+        if title is None or title == "":  # pragma: no cover
+            return guess_name_by_url(self.url)
         return f"[{title}]({self.url})"
 
     def parse(self) -> str:  # pragma: no cover
         """
         override this function for a specific site processor
 
         parse the url
@@ -79,56 +67,69 @@
 
     def get_html(self):
         """
         call this function if could not parse only by url
         """
         response = requests.get(self.url, headers=self.headers, timeout=self.max_time_limit)
         if response.status_code != 200:
-            self.error(f"connect {self.url} failed: status code [{response.status_code}]")
+            self.error(
+                f"connect {self.url} failed: status code [{response.status_code}]"
+            )  # pragma: no cover
         return response.text
 
+    def _debug(self, html):  # pragma: no cover
+        """
+        only work for me to debug
+        """
+        with open("a.html", "w", encoding="utf-8") as f:
+            f.write(html)
+
 
 class GithubProcessor(Processor):
     # https://github.com/microsoft/vscode
 
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
 
         self.site = "Github"
         self.user_name = None
         self.repo_name = None
-        self.repo_function = None # issues | pull | actions
-        self.repo_function_name = None # issue name
+        self.repo_function = None  # issues | pull | actions
+        self.repo_function_name = None  # issue name
         self.branch_name = None
         self.file_name = None
         self.tab_name = None
         self.routine = None
-        
 
         self.urls_re = [
             re.compile(r"^https://github\.com/?$"),
             re.compile(r"^https://github\.com/(?P<user>[^/]*?)\?tab=(?P<tab>.*?)/?$"),
             re.compile(r"^https://github\.com/(?P<user>[^/]*?)$/?"),
             re.compile(r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/?$"),
-            
             re.compile(
                 r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/blob/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
             ),
             re.compile(
                 r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/files/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
             ),
             re.compile(
                 r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/tree/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
             ),
             re.compile(
                 r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/commits?/(?P<commit>.*)$"
             ),
-            re.compile(r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/\?]*?)/?$"),
-            re.compile(r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)\?.*$"),
-            re.compile(r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)/(?P<routine>.*?)(?:#.*)?$")   
+            re.compile(
+                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/\?]*?)/?$"
+            ),
+            re.compile(
+                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)\?.*$"
+            ),
+            re.compile(
+                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)/(?P<routine>.*?)(?:#.*)?$"
+            ),
         ]
 
         # "https://github.com/{user}"
         # "https://github.com/{user}/{repo}"
         # "https://github.com/{user}/{repo}/blob/{branch}/({folder_name}/)?{file_name}"
         # "https://github.com/{user}/{repo}/tree/{branch}"
         # "https://github.com/{user}/{repo}/tree/{branch}/({folder_name}/)?{file_name}"
@@ -138,53 +139,53 @@
         for url_re in self.urls_re:
             res = url_re.match(self.url)
             if res:
                 if "user" in res.groupdict():
                     self.user_name = res.group("user")
                 if "repo" in res.groupdict():
                     self.repo_name = res.group("repo")
-                    if 'commit' in res.groupdict("commit"):
-                        self.repo_name += ' commit'
-                if 'function' in res.groupdict():
-                    self.repo_function = res.group('function')
-                    if 'routine' in res.groupdict():
-                        self.routine = res.group('routine')
-                        has_id = self.routine.split('/')[0].isdigit()
+                    if "commit" in res.groupdict("commit"):
+                        self.repo_name += " commit"
+                if "function" in res.groupdict():
+                    self.repo_function = res.group("function")
+                    if "routine" in res.groupdict():
+                        self.routine = res.group("routine")
+                        has_id = self.routine.split("/")[0].isdigit()
                         if has_id:
                             html = self.get_html()
                             # for issue and pull
-                            pattern = re.compile(r'<bdi class="js-issue-title markdown-title">(.*?)</bdi>')
+                            pattern = re.compile(
+                                r'<bdi class="js-issue-title markdown-title">(.*?)</bdi>'
+                            )
                             self.repo_function_name = pattern.search(html).group(1)
                         else:
-                            self.repo_function_name = self.routine.split('/')[-1]
+                            self.repo_function_name = self.routine.split("/")[-1]
                 if "branch" in res.groupdict():
                     self.branch_name = res.group("branch")
                 if "file" in res.groupdict():
                     self.file_name = res.group("file").split("/")[-1]
                 if "tab" in res.groupdict():
                     self.tab_name = res.group("tab")
                 return
 
         # should never reach here
         self.error()  # pragma: no cover
 
     def format(self):
         if self.repo_name is None and self.user_name is None:
-            return self.site
-
+            title = self.site
+        title = ""
         if self.repo_name:
             title = self.repo_name
             if self.repo_function:
-                title += f' {self.repo_function}'
+                title += f" {self.repo_function}"
                 if self.repo_function_name:
                     title = self.repo_function_name
             elif self.file_name:
                 title += f" {self.file_name}"
-            elif self.routine:
-                title = self.routine
         else:
             title = self.user_name
             if self.tab_name:
                 title += f" {self.tab_name}"
 
         return title
 
@@ -214,15 +215,15 @@
                     self.user_name = res.group("user")
                 if "repo" in res.groupdict():
                     self.repo_name = res.group("repo")
                 if "routine" in res.groupdict():
                     origin_routine = res.group("routine").split("/")[-1]
                     self.routine = urllib.parse.unquote(origin_routine)
                 return
-        self.error("unknown url")
+        self.error("unknown url")  # pragma: no cover
 
     def format(self):
         if self.repo_name is None:
             title = f"{self.user_name}'s blog"
         else:
             if self.routine is None:
                 title = f"{self.repo_name} document"
@@ -295,16 +296,14 @@
 
     def format(self):
         title = ""
         if self.question_name:
             title = self.question_name
             if self.is_answer:
                 title += " [answer]"
-            else:
-                title += " [question]"
         elif self.tag_name:
             title = f"{self.tag_name} tag"
         elif self.user_name:
             title = f"{self.user_name}"
         else:
             # pure https://stackoverflow.com/
             title = self.site
@@ -359,20 +358,20 @@
 
         return title
 
 
 class ZhihuProcessor(Processor):
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
-        self.site = "Zhihu"
+        self.site = "知乎"
         self.type_name = None
         self.title = None
 
         self.urls_re = [
-            re.compile(r"^https://www\.zhihu\.com/?$"),
+            re.compile(r"(?P<site>^https://www\.zhihu\.com)/?$"),
             re.compile(r"^https://www\.zhihu\.com/question/\d+/(?P<type>.*?)/(?P<id>.*?)/?$"),
             re.compile(r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/(?P<sub_type>.*?)/?$"),
             re.compile(r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$"),
             re.compile(r"^https://zhuanlan\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$"),
         ]
 
         self.sub_types = {
@@ -393,16 +392,16 @@
 
         # https://www.zhihu.com/collection/86788003
 
     def parse(self) -> str:
         for url_re in self.urls_re:
             res = url_re.match(self.url)
             if res:
-                if "type" not in res.groupdict():
-                    self.title = "知乎"
+                if "site" in res.groupdict():
+                    self.title = self.site
                     return
                 self.type_name = res.group("type")
 
                 # following parse need page html elements
                 html = self.get_html()
 
                 if self.type_name == "question":
@@ -455,30 +454,29 @@
         self.site = "bilibli"
         self.type_name = None
         self.user_name = None
         self.id = None
         self.name = None
 
         self.urls_re = [
-            re.compile(r"^https://www\.bilibili\.com/?$"),
+            re.compile(r"(?P<site>^https://www\.bilibili\.com)/?$"),
             re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*?)\?.*$"),
             re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*)$"),
         ]
 
         # https://www.bilibili.com/video/BV1ah4y1X73M
         # https://www.bilibili.com/opus/806593844580712449?spm_id_from=333.999.0.0
         # https://www.bilibili.com/read/cv23285665?spm_id_from=333.999.0.0
 
     def parse(self) -> str:
         for url_re in self.urls_re:
             res = url_re.match(self.url)
 
             if res:
-                if "type" not in res.groupdict():
-                    # pure bilibili
+                if "site" in res.groupdict():
                     return
                 self.type_name = res.group("type")
                 self.id = res.group("id")
                 # bilibili url often following with "spm_id_from=333.999.0.0 ..."
                 # clean the url
                 self.url = f"https://www.bilibili.com/{self.type_name}/{self.id}"
 
@@ -517,15 +515,15 @@
         self.site = "csdn"
         self.user_id = None
         self.user_name = None
         self.article_id = None
         self.article_name = None
 
         self.urls_re = [
-            re.compile(r"^https://blog\.csdn\.net/?$"),
+            re.compile(r"(?P<site>^https://blog\.csdn\.net)/?$"),
             re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)/(?P<category>.*?)\.html$"),
             re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)\?type=.*$"),
             re.compile(
                 r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)\?.*$"
             ),
             re.compile(
                 r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)$"
@@ -533,17 +531,16 @@
             re.compile(r"^http://t\.csdn\.cn/(?P<short_id>.*?)$"),
         ]
 
     def parse(self) -> str:
         for url_re in self.urls_re:
             res = url_re.match(self.url)
             if res:
-                if "user_id" not in res.groupdict() and "short_id" not in res.groupdict():
+                if "site" in res.groupdict():
                     return
-
                 html = self.get_html()
                 # with open("a.txt",'w',encoding='utf-8') as f:
                 #     f.write(html)
 
                 if "article_id" in res.groupdict():
                     self.user_id = res.group("user_id")
                     self.article_id = res.group("article_id")
@@ -572,7 +569,60 @@
             title = self.site
         else:
             if self.article_name:
                 title = self.article_name
             else:
                 title = self.user_name
         return title
+
+
+class Githubusercontent(Processor):
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
+
+    def parse(self) -> str:
+        return
+
+    def format(self):
+        return "image"
+
+
+class CNblog(Processor):
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
+        self.site = "博客园"
+        self.author_name = None
+        self.article_name = None
+
+        self.urls_re = [
+            re.compile(r"(?P<site>^https://www\.cnblogs\.com)/?$"),
+            re.compile(r"^https://www\.cnblogs\.com/(?P<author>.*?)/p/(?P<article>.*?)/?$"),
+            re.compile(r"^https://www\.cnblogs\.com/(?P<author>.*?)/?$"),
+        ]
+
+    def parse(self) -> str:
+        for url_re in self.urls_re:
+            res = url_re.match(self.url)
+            if res:
+                if "site" in res.groupdict():
+                    return
+                self.author_name = res.group("author")
+                html = self.get_html()
+                if "article" in res.groupdict():
+                    pattern = re.compile(r'<span role="heading" aria-level="2">(.*?)</span>')
+                    self.article_name = pattern.search(html).group(1)
+                else:
+                    pattern = re.compile(
+                        r'<a id="Header1_HeaderTitle" class="headermaintitle HeaderMainTitle" href="https://www.cnblogs.com/.*">(.*?)</a>'
+                    )
+                    self.author_name = pattern.search(html).group(1)
+
+    def format(self):
+        if self.author_name is None:
+            title = self.site
+        else:
+            if self.article_name:
+                title = self.article_name
+            else:
+                title = self.author_name
+
+        return title
```

### Comparing `miuc-0.1.5/miuc/web_parser.py` & `miuc-0.1.6/miuc/web_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,31 +12,35 @@
     GithubProcessor,
     StackoverflowProcessor,
     ZhihuProcessor,
     BilibiliProcessor,
     GithubioProcessor,
     YoutubeProcessor,
     CSDNProcessor,
+    Githubusercontent,
+    CNblog
 )
-from .site_processor import guess_name_by_url
+from .utils import guess_name_by_url
 
 # some frequently pages
 
 SPECIFIC_SITES = {
     # url: page_processor
     r"^https://github\.com.*": GithubProcessor,
     r"^https://.*?\.github\.io.*": GithubioProcessor,
     r"^https://stackoverflow\.com.*": StackoverflowProcessor,
     r"^https://www\.youtube\.com.*$": YoutubeProcessor,
     r"^https://youtu\.be/.*": YoutubeProcessor,
     r"^https://zhuanlan\.zhihu\.com.*": ZhihuProcessor,
     r"^https://www\.zhihu\.com.*": ZhihuProcessor,
     r"^https://www\.bilibili\.com.*": BilibiliProcessor,
     r"^https://blog\.csdn\.net.*": CSDNProcessor,
-    r"^http://t\.csdn\.cn/.*": CSDNProcessor
+    r"^http://t\.csdn\.cn/.*": CSDNProcessor,
+    r"^https://raw\.githubusercontent\.com.*": Githubusercontent,
+    r"^https://www\.cnblogs\.com.*": CNblog
 }
 
 
 def parse_url(url: str, max_time_limit: int = 5) -> str:
     """
     parse url and return the tite for the page
     """
@@ -44,22 +48,22 @@
     # first check the url whether in specific sites
     # if so,
     try:
         for specific_page_url in SPECIFIC_SITES:
             if re.match(specific_page_url, url):
                 return SPECIFIC_SITES[specific_page_url](max_time_limit)(url)
 
-        response = requests.get(url, timeout=max_time_limit)
-        if response.status_code != 200:
+        # response = requests.get(url, timeout=max_time_limit)
+        # if response.status_code != 200:
             # 404 or other unusual error
-            return guess_name_by_url(url)
-
+            # return guess_name_by_url(url)
+        # print('ok')
         return guess_name_by_url(url)
     except Exception as e:
-        
         return guess_name_by_url(url)
 
+
 def parse_html(html: str) -> str:
     """
     parse html and return the title
     """
     return html
```

### Comparing `miuc-0.1.5/README.md` & `miuc-0.1.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # miuc
 
+[![codecov](https://codecov.io/gh/luzhixing12345/miuc/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/miuc)
+
 Markdown Intelligence Url Complete
 
 Paste URL by <kbd>ctrl</kbd> + <kbd>v</kbd>, miuc will complete the title for you
 
 ## Features
 
 ![action](https://raw.githubusercontent.com/learner-lu/picbed/master/action.gif)
```

### Comparing `miuc-0.1.5/PKG-INFO` & `miuc-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,16 @@
 Requires-Dist: requests
 Project-URL: Documentation, https://luzhixing12345.github.io/miuc/
 Project-URL: Repository, https://github.com/luzhixing12345/miuc
 Description-Content-Type: text/markdown
 
 # miuc
 
+[![codecov](https://codecov.io/gh/luzhixing12345/miuc/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/miuc)
+
 Markdown Intelligence Url Complete
 
 Paste URL by <kbd>ctrl</kbd> + <kbd>v</kbd>, miuc will complete the title for you
 
 ## Features
 
 ![action](https://raw.githubusercontent.com/learner-lu/picbed/master/action.gif)
```

