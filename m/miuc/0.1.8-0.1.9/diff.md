# Comparing `tmp/miuc-0.1.8.tar.gz` & `tmp/miuc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.8.tar", max compression
+gzip compressed data, was "miuc-0.1.9.tar", max compression
```

## Comparing `miuc-0.1.8.tar` & `miuc-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.8/LICENSE
--rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.8/miuc/__init__.py
--rw-r--r--   0        0        0     1091 2023-06-25 03:33:01.484702 miuc-0.1.8/miuc/main.py
--rw-r--r--   0        0        0    26107 2023-06-25 01:17:31.758549 miuc-0.1.8/miuc/site_processor.py
--rw-r--r--   0        0        0     2258 2023-06-25 01:14:57.116556 miuc-0.1.8/miuc/utils.py
--rw-r--r--   0        0        0     2179 2023-06-25 01:17:49.848313 miuc-0.1.8/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-25 03:33:14.927747 miuc-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1543 2023-06-24 17:29:12.273734 miuc-0.1.8/README.md
--rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 miuc-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.9/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.9/miuc/__init__.py
+-rw-r--r--   0        0        0     1091 2023-06-25 03:33:01.484702 miuc-0.1.9/miuc/main.py
+-rw-r--r--   0        0        0    25283 2023-06-25 04:12:15.095140 miuc-0.1.9/miuc/site_processor.py
+-rw-r--r--   0        0        0     2258 2023-06-25 01:14:57.116556 miuc-0.1.9/miuc/utils.py
+-rw-r--r--   0        0        0     2179 2023-06-25 01:17:49.848313 miuc-0.1.9/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-25 04:13:43.712769 miuc-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1543 2023-06-24 17:29:12.273734 miuc-0.1.9/README.md
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 miuc-0.1.9/PKG-INFO
```

### Comparing `miuc-0.1.8/LICENSE` & `miuc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miuc-0.1.8/miuc/main.py` & `miuc-0.1.9/miuc/main.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.8/miuc/site_processor.py` & `miuc-0.1.9/miuc/site_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 
 class Processor:
     def __init__(self, max_time_limit: int = 5) -> None:
         self.class_name = self.__class__.__name__
         self.url = None
         self.max_time_limit = max_time_limit
         self.urls_re = [
-            # re.compile(...)
+            # ...
         ]
         self.headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
             "Accept-Encoding": "gzip",
             "Connection": "keep-alive",
             "Content-Type": "text/html;charset=utf-8",
         }
 
     def __call__(self, url: str):
         self.url: str = url
-        if len(self.urls_re) == 0: # pragma: no cover
+        if len(self.urls_re) == 0:  # pragma: no cover
             self.error("finish urls_re in your processor class")
         for url_re in self.urls_re:
-            res = url_re.match(self.url)
+            res = re.compile(url_re).match(self.url)
             if res:
                 self.parse(res)
                 break
         title = self.format()
         if title is None or title == "":  # pragma: no cover
             return guess_name_by_url(self.url)
         return f"[{title}]({self.url})"
@@ -84,15 +84,16 @@
             self.error(
                 f"connect {self.url} failed: status code [{response.status_code}]"
             )  # pragma: no cover
         return response.text
 
     def get_element_match(self, pattern: re.Pattern):
         html = self.get_html()
-        return pattern.search(html).group(1)
+        # self._debug(html)
+        return re.compile(pattern).search(html).group(1)
 
     def _debug(self, html):  # pragma: no cover
         """
         only work for me to debug
         """
         with open("a.html", "w", encoding="utf-8") as f:
             f.write(html)
@@ -112,40 +113,26 @@
         self.branch_name = None
         self.file_name = None
         self.tab_name = None
         self.routine = None
         self.search_name = None
 
         self.urls_re = [
-            re.compile(r"^https://github\.com/?$"),
-            re.compile(r"^https://github\.com/(?P<user>[^/]*?)\?tab=(?P<tab>.*?)/?$"),
-            re.compile(r"^https://github\.com/(?P<user>[^/\?]*?)$/?"),
-            re.compile(r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/?$"),
-            re.compile(
-                r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/blob/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
-            ),
-            re.compile(
-                r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/files/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
-            ),
-            re.compile(
-                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/tree/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$"
-            ),
-            re.compile(
-                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/commits?/(?P<commit>.*)$"
-            ),
-            re.compile(
-                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/\?]*?)/?$"
-            ),
-            re.compile(
-                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)\?.*$"
-            ),
-            re.compile(
-                r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)/(?P<routine>.*?)(?:#.*)?$"
-            ),
-            re.compile(r"^https://github\.com/search\?q=(?P<search>.*?)((&.*)|(:.*))?/?$"),
+            r"^https://github\.com/?$",
+            r"^https://github\.com/(?P<user>[^/]*?)\?tab=(?P<tab>.*?)/?$",
+            r"^https://github\.com/(?P<user>[^/\?]*?)$/?",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/?$",
+            r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/blob/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$",
+            r"^https://github.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/files/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/tree/(?P<branch>[^/]*?)/?(?P<file>.*?)?/?$",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/commits?/(?P<commit>.*)$",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/\?]*?)/?$",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)\?.*$",
+            r"^https://github\.com/(?P<user>[^/]*?)/(?P<repo>[^/]*?)/(?P<function>[^/]*?)/(?P<routine>.*?)(?:#.*)?$",
+            r"^https://github\.com/search\?q=(?P<search>.*?)((&.*)|(:.*))?/?$",
         ]
 
         # "https://github.com/{user}"
         # "https://github.com/{user}/{repo}"
         # "https://github.com/{user}/{repo}/blob/{branch}/({folder_name}/)?{file_name}"
         # "https://github.com/{user}/{repo}/tree/{branch}"
         # "https://github.com/{user}/{repo}/tree/{branch}/({folder_name}/)?{file_name}"
@@ -161,15 +148,15 @@
         if "function" in res.groupdict():
             self.repo_function = res.group("function")
             if "routine" in res.groupdict():
                 self.routine = res.group("routine")
                 has_id = self.routine.split("/")[0].isdigit()
                 if has_id:
                     # for issue and pull
-                    pattern = re.compile(r'<bdi class="js-issue-title markdown-title">(.*?)</bdi>')
+                    pattern = r'<bdi class="js-issue-title markdown-title">(.*?)</bdi>'
                     self.repo_function_name = self.get_element_match(pattern)
                 else:
                     self.repo_function_name = self.routine.split("/")[-1]
         if "branch" in res.groupdict():
             self.branch_name = res.group("branch")
         if "file" in res.groupdict():
             self.file_name = res.group("file").split("/")[-1]
@@ -208,17 +195,17 @@
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.user_name = None
         self.repo_name = None
         self.routine = None
 
         self.urls_re = [
-            re.compile(r"^https://(?P<user>.*?)\.github\.io/?$"),  # blog / resume
-            re.compile(r"^https://(?P<user>.*?)\.github\.io/(?P<repo>.*?)/(?P<routine>.+?)/?$"),
-            re.compile(r"^https://(?P<user>.*?)\.github\.io/(?P<repo>.*?)/?$"),  # github repo
+            r"^https://(?P<user>.*?)\.github\.io/?$",  # blog / resume
+            r"^https://(?P<user>.*?)\.github\.io/(?P<repo>.*?)/(?P<routine>.+?)/?$",
+            r"^https://(?P<user>.*?)\.github\.io/(?P<repo>.*?)/?$",  # github repo
         ]
 
     def parse(self, res: Match) -> str:
         if "user" in res.groupdict():
             self.user_name = res.group("user")
         if "repo" in res.groupdict():
             self.repo_name = res.group("repo")
@@ -247,19 +234,17 @@
         self.tag_name = None
         self.user_name = None
 
         self.question_name = None
         self.is_answer = False
 
         self.urls_re = [
-            re.compile(r"^https://stackoverflow\.com/?$"),
-            re.compile(r"^https://stackoverflow\.com/(?P<type>[^/]*?)/tagged/(?P<tag>.*?)/?$"),
-            re.compile(
-                r"^https://stackoverflow\.com/(?P<type>[^/]*?)/(?P<id>[^/]*?)/(?P<question>.*?)/?$"
-            ),
+            r"^https://stackoverflow\.com/?$",
+            r"^https://stackoverflow\.com/(?P<type>[^/]*?)/tagged/(?P<tag>.*?)/?$",
+            r"^https://stackoverflow\.com/(?P<type>[^/]*?)/(?P<id>[^/]*?)/(?P<question>.*?)/?$",
         ]
 
         # https://stackoverflow.com/questions/tagged/python
         # https://stackoverflow.com/users/5740428/jan-schultke
 
     def parse(self, res: Match) -> str:
         if "type" not in res.groupdict():
@@ -275,21 +260,21 @@
                 self.id = res.group("id")
             if "question" in res.groupdict():
                 # stackoverflow question name use `-` to replace ' '
                 self.question_name = res.group("question").replace("-", " ")
 
             if self.question_name is None or self.question_name.isdigit():
                 # could not get question name from url
-                pattern = re.compile(r'<a .*class="question-hyperlink">(.*?)</a>')
+                pattern = r'<a .*class="question-hyperlink">(.*?)</a>'
                 self.question_name = self.get_element_match(pattern)
         elif self.type_name == "a":
             # answer
             # https://stackoverflow.com/a/601989/17869889
 
-            pattern = re.compile(r'<a .*class="question-hyperlink">(.*?)</a>')
+            pattern = r'<a .*class="question-hyperlink">(.*?)</a>'
             self.question_name = self.get_element_match(pattern)
             self.is_answer = True
         elif self.type_name == "users":
             # https://stackoverflow.com/users/5740428/jan-schultke
             self.user_name = res.group("question")
         else:
             self.error("unknown type")  # pragma: no cover
@@ -315,19 +300,19 @@
 class Youtube(Processor):
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "youtube"
         self.user_name = None
         self.video_name = None
         self.urls_re = [
-            re.compile(r"^https://www\.youtube\.com/?$"),
-            re.compile(r"^https://www\.youtube\.com/\@(?P<user>.*?)/?$"),
-            re.compile(r"^https://www\.youtube\.com/\@(?P<user>.*?)/.*$"),
-            re.compile(r"^https://www\.youtube\.com/watch\?v=(?P<id>.*?)/?$"),
-            re.compile(r"^https://youtu\.be/(?P<id>.*?)/?"),
+            r"^https://www\.youtube\.com/?$",
+            r"^https://www\.youtube\.com/\@(?P<user>.*?)/?$",
+            r"^https://www\.youtube\.com/\@(?P<user>.*?)/.*$",
+            r"^https://www\.youtube\.com/watch\?v=(?P<id>.*?)/?$",
+            r"^https://youtu\.be/(?P<id>.*?)/?",
         ]
 
         # https://www.youtube.com/watch?v=ErV-2tlf9Ls
 
     def _get_youtube_title(self):
         # could not directly get youtube video title, instead use the following method
         # https://stackoverflow.com/a/52664178/17869889
@@ -361,19 +346,19 @@
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "知乎"
         self.type_name = None
         self.title = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://www\.zhihu\.com)/?$"),
-            re.compile(r"^https://www\.zhihu\.com/question/\d+/(?P<type>.*?)/(?P<id>.*?)/?$"),
-            re.compile(r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/(?P<sub_type>.*?)/?$"),
-            re.compile(r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$"),
-            re.compile(r"^https://zhuanlan\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$"),
+            r"(?P<site>^https://www\.zhihu\.com)/?$",
+            r"^https://www\.zhihu\.com/question/\d+/(?P<type>.*?)/(?P<id>.*?)/?$",
+            r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/(?P<sub_type>.*?)/?$",
+            r"^https://www\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$",
+            r"^https://zhuanlan\.zhihu\.com/(?P<type>.*?)/(?P<id>.*?)/?$",
         ]
 
         self.sub_types = {
             "answers": "回答",
             "zvideos": "视频",
             "asks": "提问",
             "posts": "文章",
@@ -396,42 +381,42 @@
             return
         self.type_name = res.group("type")
 
         # following parse need page html elements
 
         if self.type_name == "question":
             # https://www.zhihu.com/question/446988424
-            pattern = re.compile(r'<h1 class="QuestionHeader-title">(.*?)</h1>')
+            pattern = r'<h1 class="QuestionHeader-title">(.*?)</h1>'
             self.title = self.get_element_match(pattern)
         elif self.type_name == "p":
             # https://zhuanlan.zhihu.com/p/347552573
-            pattern = re.compile(r'<h1 class="Post-Title">(.*?)</h1>')
+            pattern = r'<h1 class="Post-Title">(.*?)</h1>'
             self.title = self.get_element_match(pattern)
         elif self.type_name == "answer":
             # https://www.zhihu.com/question/21099081/answer/119347251
             # https://www.zhihu.com/question/367357782/answer/3066947505 Anonymous user
-            pattern = re.compile(r'<h1 class="QuestionHeader-title">(.*?)</h1>')
+            pattern = r'<h1 class="QuestionHeader-title">(.*?)</h1>'
             self.title = self.get_element_match(pattern) + "的回答"
         elif self.type_name == "people":
             # https://www.zhihu.com/people/hinus
 
-            pattern = re.compile(r'<span class="ProfileHeader-name">(.*?)</span')
+            pattern = r'<span class="ProfileHeader-name">(.*?)</span'
             # sometimes there will be <style ...> inside, remove it
             user_name = re.sub(r"<style.*>", "", self.get_element_match(pattern))
             self.title = user_name + "的主页"
             if "sub_type" in res.groupdict():
                 # https://www.zhihu.com/people/hinus/collections
                 self.title = f'{user_name}的{self.sub_types[res.group("sub_type")]}'
         elif self.type_name == "collection":
             # https://www.zhihu.com/collection/86788003
-            pattern = re.compile(r'<div class="CollectionDetailPageHeader-title">(.*?)</div>')
+            pattern = r'<div class="CollectionDetailPageHeader-title">(.*?)</div>'
             self.title = self.get_element_match(pattern) + " 收藏夹"
         elif self.type_name == "column":
             # https://www.zhihu.com/column/hinus
-            pattern = re.compile(r'<div class="css-zyehvu">(.*?)</div>')
+            pattern = r'<div class="css-zyehvu">(.*?)</div>'
             self.title = self.get_element_match(pattern) + " 专栏"
 
     def format(self):
         return self.title
 
 
 class Bilibili(Processor):
@@ -440,17 +425,17 @@
         self.site = "bilibli"
         self.type_name = None
         self.user_name = None
         self.id = None
         self.name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://www\.bilibili\.com)/?$"),
-            re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*?)\?.*$"),
-            re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*)$"),
+            r"(?P<site>^https://www\.bilibili\.com)/?$",
+            r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*?)\?.*$",
+            r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*)$",
         ]
 
         # https://www.bilibili.com/video/BV1ah4y1X73M
         # https://www.bilibili.com/opus/806593844580712449?spm_id_from=333.999.0.0
         # https://www.bilibili.com/read/cv23285665?spm_id_from=333.999.0.0
 
     def parse(self, res: Match) -> str:
@@ -459,20 +444,20 @@
         self.type_name = res.group("type")
         self.id = res.group("id")
         # bilibili url often following with "spm_id_from=333.999.0.0 ..."
         # clean the url
         self.url = f"https://www.bilibili.com/{self.type_name}/{self.id}"
 
         if self.type_name == "video":
-            pattern = re.compile(r"<h1 .*>(.*?)</h1>")
+            pattern = r"<h1 .*>(.*?)</h1>"
             self.name = self.get_element_match(pattern)
         elif self.type_name == "opus":
             pass
         elif self.type_name == "read":
-            pattern = re.compile(r'<title data-vue-meta="true">(.*?)</title>')
+            pattern = r'<title data-vue-meta="true">(.*?)</title>'
             self.name = self.get_element_match(pattern).replace(" - 哔哩哔哩", "")
 
     def format(self):
         if self.type_name is None:
             # pure bilibili
             title = self.site
         else:
@@ -494,50 +479,46 @@
         self.site = "csdn"
         self.user_id = None
         self.user_name = None
         self.article_id = None
         self.article_name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://blog\.csdn\.net)/?$"),
-            re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)/(?P<category>.*?)\.html$"),
-            re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)\?type=.*$"),
-            re.compile(
-                r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)\?.*$"
-            ),
-            re.compile(
-                r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)$"
-            ),
-            re.compile(r"^http://t\.csdn\.cn/(?P<short_id>.*?)$"),
+            r"(?P<site>^https://blog\.csdn\.net)/?$",
+            r"^https://blog\.csdn\.net/(?P<user_id>.*?)/(?P<category>.*?)\.html$",
+            r"^https://blog\.csdn\.net/(?P<user_id>.*?)\?type=.*$",
+            r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)\?.*$",
+            r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)$",
+            r"^http://t\.csdn\.cn/(?P<short_id>.*?)$",
         ]
 
     def parse(self, res: Match) -> str:
         if "site" in res.groupdict():
             return
 
         # self._debug(html)
 
         if "article_id" in res.groupdict():
             self.user_id = res.group("user_id")
             self.article_id = res.group("article_id")
             # clean the url
             self.url = f"https://blog.csdn.net/{self.user_id}/article/details/{self.article_id}"
-            pattern = re.compile(r'<h1 class="title-article" id="articleContentId">(.*?)</h1>')
+            pattern = r'<h1 class="title-article" id="articleContentId">(.*?)</h1>'
             self.article_name = self.get_element_match(pattern)
         elif "category" in res.groupdict():
-            pattern = re.compile(r'<h3 class="column_title oneline" title=.*>(.*?)</h3>')
+            pattern = r'<h3 class="column_title oneline" title=.*>(.*?)</h3>'
             self.article_name = self.get_element_match(pattern)
         elif "short_id" in res.groupdict():
             # for short url
 
-            pattern = re.compile(r'<meta name="keywords" content="(.*?)">')
+            pattern = r'<meta name="keywords" content="(.*?)">'
             self.article_name = self.get_element_match(pattern)
         else:
             # for user home page
-            pattern = re.compile(r'data-nickname="(.*?)"')
+            pattern = r'data-nickname="(.*?)"'
             self.user_name = self.get_element_match(pattern)
 
     def format(self) -> str:
         if self.user_name is None and self.article_name is None:
             title = self.site
         else:
             if self.article_name:
@@ -547,15 +528,15 @@
         return title
 
 
 class Githubusercontent(Processor):
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
 
-        self.urls_re = [re.compile(r"^https://raw\.githubusercontent\.com.*$")]
+        self.urls_re = [r"^https://raw\.githubusercontent\.com.*$"]
 
     def parse(self, res: Match) -> str:
         return
 
     def format(self):
         return "image"
 
@@ -564,35 +545,39 @@
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "博客园"
         self.author_name = None
         self.article_name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://www\.cnblogs\.com)/?$"),
-            re.compile(r"^https://www\.cnblogs\.com/(?P<author>.*?)/p/(?P<article>.*?)/?$"),
-            re.compile(r"^https://www\.cnblogs\.com/(?P<author>.*?)/?$"),
+            r"(?P<site>^https://www\.cnblogs\.com)/?$",
+            r"^https://www\.cnblogs\.com/(?P<author>.*?)/p/(?P<article>.*?)/?$",
+            r"^https://www\.cnblogs\.com/(?P<archive>.*?)/archive/.*$",
+            r"^https://www\.cnblogs\.com/(?P<author>.*?)/?$",
         ]
 
     def parse(self, res: Match) -> str:
         if "site" in res.groupdict():
             return
-        self.author_name = res.group("author")
 
         if "article" in res.groupdict():
-            pattern = re.compile(r'<span role="heading" aria-level="2">(.*?)</span>')
+            pattern = r'<span role="heading" aria-level="2">(.*?)</span>'
             self.article_name = self.get_element_match(pattern)
-        else:
+        elif "archive" in res.groupdict():
+            pattern = r'<span role="heading" aria-level="2">(.*?)</span>'
+            self.article_name = self.get_element_match(pattern)
+        elif "author" in res.groupdict():
+            # only author
             pattern = re.compile(
                 r'<a id="Header1_HeaderTitle" class="headermaintitle HeaderMainTitle" href="https://www.cnblogs.com/.*">(.*?)</a>'
             )
             self.author_name = self.get_element_match(pattern)
 
     def format(self):
-        if self.author_name is None:
+        if self.author_name is None and self.article_name is None:
             title = self.site
         else:
             if self.article_name:
                 title = self.article_name
             else:
                 title = self.author_name
 
@@ -603,28 +588,28 @@
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "简书"
         self.article_name = None
         self.user_name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://www\.jianshu\.com)/?$"),
-            re.compile(r"^https://www\.jianshu\.com/p/(?P<article>.*?)/?$"),
-            re.compile(r"^https://www\.jianshu\.com/u/(?P<user>.*?)/?$"),
+            r"(?P<site>^https://www\.jianshu\.com)/?$",
+            r"^https://www\.jianshu\.com/p/(?P<article>.*?)/?$",
+            r"^https://www\.jianshu\.com/u/(?P<user>.*?)/?$",
         ]
 
     def parse(self, res: Match) -> str:
         if "site" in res.groupdict():
             return
 
         if "article" in res.groupdict():
-            pattern = re.compile(r'<h1 class="_1RuRku">(.*?)</h1>')
+            pattern = r'<h1 class="_1RuRku">(.*?)</h1>'
             self.article_name = self.get_element_match(pattern)
         if "user" in res.groupdict():
-            pattern = re.compile(r'<a class="name" href=.*?>(.*?)</a>')
+            pattern = r'<a class="name" href=.*?>(.*?)</a>'
             self.user_name = self.get_element_match(pattern)
 
     def format(self):
         title = self.site
         if self.article_name:
             title = self.article_name
         elif self.user_name:
@@ -636,28 +621,28 @@
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "tencent cloud"
         self.article_name = None
         self.user_name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>^https://cloud.tencent.com)/?$"),
-            re.compile(r"^https://cloud.tencent.com/developer/article/(?P<article>.*?)/?$"),
-            re.compile(r"^https://cloud.tencent.com/developer/user/(?P<user>.*?)/?$"),
+            r"(?P<site>^https://cloud.tencent.com)/?$",
+            r"^https://cloud.tencent.com/developer/article/(?P<article>.*?)/?$",
+            r"^https://cloud.tencent.com/developer/user/(?P<user>.*?)/?$",
         ]
 
     def parse(self, res: Match) -> str:
         if "site" in res.groupdict():
             return
 
         if "article" in res.groupdict():
-            pattern = re.compile(r'<h2 class="title-text">(.*?)</h2>')
+            pattern = r'<h2 class="title-text">(.*?)</h2>'
             self.article_name = self.get_element_match(pattern)
         elif "user" in res.groupdict():
-            pattern = re.compile(r'<h3 class="uc-hero-name">(.*?)</h3>')
+            pattern = r'<h3 class="uc-hero-name">(.*?)</h3>'
             self.user_name = self.get_element_match(pattern)
 
     def format(self):
         title = self.site
 
         if self.article_name:
             title = self.article_name
@@ -670,23 +655,23 @@
 class Douban(Processor):
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "豆瓣"
         self.book_name = None
 
         self.urls_re = [
-            re.compile(r"(?P<site>https://book\.douban\.com)/?$"),
-            re.compile(r"^https://book\.douban\.com/subject/(?P<id>.*?)(\?.*)?/?$"),
+            r"(?P<site>https://book\.douban\.com)/?$",
+            r"^https://book\.douban\.com/subject/(?P<id>.*?)(\?.*)?/?$",
         ]
 
     def parse(self, res: Match) -> str:
         if "site" in res.groupdict():
             return
 
-        pattern = re.compile(r'<span property="v:itemreviewed">(.*?)</span>')
+        pattern = r'<span property="v:itemreviewed">(.*?)</span>'
         self.book_name = self.get_element_match(pattern)
 
     def format(self):
         title = self.site
         if self.book_name:
             title = self.book_name
```

### Comparing `miuc-0.1.8/miuc/utils.py` & `miuc-0.1.9/miuc/utils.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.8/miuc/web_parser.py` & `miuc-0.1.9/miuc/web_parser.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.8/README.md` & `miuc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `miuc-0.1.8/PKG-INFO` & `miuc-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

