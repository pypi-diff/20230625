# Comparing `tmp/atlassian_api_py-0.5.0-py3-none-any.whl.zip` & `tmp/atlassian_api_py-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12293 bytes, number of entries: 12
--rw-r--r--  2.0 unx      194 b- defN 23-Apr-10 13:25 atlassian/__init__.py
--rw-r--r--  2.0 unx    12925 b- defN 23-Apr-10 13:25 atlassian/bitbucket.py
--rw-r--r--  2.0 unx     3349 b- defN 23-Apr-10 13:25 atlassian/client.py
--rw-r--r--  2.0 unx     2124 b- defN 23-Apr-10 13:25 atlassian/confluence.py
--rw-r--r--  2.0 unx     1608 b- defN 23-Apr-10 13:25 atlassian/error.py
--rw-r--r--  2.0 unx    11448 b- defN 23-Apr-10 13:25 atlassian/jira.py
--rw-r--r--  2.0 unx     1162 b- defN 23-Apr-10 13:25 atlassian/logger.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3840 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      970 b- defN 23-Apr-10 13:25 atlassian_api_py-0.5.0.dist-info/RECORD
-12 files, 38796 bytes uncompressed, 10673 bytes compressed:  72.5%
+Zip file size: 12354 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-25 04:27 atlassian/__init__.py
+-rw-r--r--  2.0 unx    12925 b- defN 23-Jun-25 04:27 atlassian/bitbucket.py
+-rw-r--r--  2.0 unx     3349 b- defN 23-Jun-25 04:27 atlassian/client.py
+-rw-r--r--  2.0 unx     2124 b- defN 23-Jun-25 04:27 atlassian/confluence.py
+-rw-r--r--  2.0 unx     1608 b- defN 23-Jun-25 04:27 atlassian/error.py
+-rw-r--r--  2.0 unx    11524 b- defN 23-Jun-25 04:27 atlassian/jira.py
+-rw-r--r--  2.0 unx     1162 b- defN 23-Jun-25 04:27 atlassian/logger.py
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-25 04:27 atlassian_api_py-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3943 b- defN 23-Jun-25 04:27 atlassian_api_py-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 04:27 atlassian_api_py-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-25 04:27 atlassian_api_py-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      970 b- defN 23-Jun-25 04:27 atlassian_api_py-0.5.1.dist-info/RECORD
+12 files, 38975 bytes uncompressed, 10734 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlassian/jira.py
 Comment: 
 
 Filename: atlassian/logger.py
 Comment: 
 
-Filename: atlassian_api_py-0.5.0.dist-info/LICENSE
+Filename: atlassian_api_py-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: atlassian_api_py-0.5.0.dist-info/METADATA
+Filename: atlassian_api_py-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: atlassian_api_py-0.5.0.dist-info/WHEEL
+Filename: atlassian_api_py-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: atlassian_api_py-0.5.0.dist-info/top_level.txt
+Filename: atlassian_api_py-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: atlassian_api_py-0.5.0.dist-info/RECORD
+Filename: atlassian_api_py-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlassian/jira.py

```diff
@@ -254,26 +254,29 @@
         return self.post(url, json=json)
 
     def get_transitions(self, issue_id):
         """Get a list of the transitions possible for this issue by the current user"""
         url = f"/rest/api/2/issue/{issue_id}/transitions"
         return self.get(url) or {}
 
-    def search_issue_with_jql(self, jql, max_result=1000):
+    def search_issue_with_jql(self, jql, max_result=1000) -> list:
         url = "/rest/api/2/search"
         start_at = 0
         issues = []
         json = {
             "jql": jql,
             "startAt": start_at,
             "maxResults": max_result,
             "fields": ["summary", "status", "issuetype", "fixVersions"],
         }
         response = self.post(url, json=json) or {}
-        total = response["total"]
+        try:
+            total = response["total"]
+        except KeyError:
+            return issues
         max_results = response["maxResults"]
         for issue in response["issues"]:
             issues.append(issue)
 
         while total > max_results:
             start_at = start_at + max_results
             json = {
```

## Comparing `atlassian_api_py-0.5.0.dist-info/LICENSE` & `atlassian_api_py-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlassian_api_py-0.5.0.dist-info/METADATA` & `atlassian_api_py-0.5.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassian-api-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Wrapper for Atlassian REST API
 Author: Peter Shen
 Author-email: xianpeng.shen@gmail.com
 License: MIT License
 Project-URL: source, https://github.com/shenxianpeng/atlassian-api-py
 Project-URL: tracker, https://github.com/shenxianpeng/atlassian-api-py/issues
 Project-URL: download, https://pypi.org/project/atlassian-api-py/#files
@@ -27,18 +27,19 @@
 Requires-Dist: requests
 
 # Python Wrapper for Atlassian REST API
 
 [![PyPI](https://img.shields.io/pypi/v/atlassian-api-py)](https://pypi.org/project/atlassian-api-py/)
 [![CodeFactor](https://www.codefactor.io/repository/github/shenxianpeng/atlassian-api-py/badge/main?s=3f5b565625069f5c5ab303a02b120197cd3abdde)](https://www.codefactor.io/repository/github/shenxianpeng/atlassian-api-py/overview/main)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/atlassian-api-py)
+[![commit-check](https://img.shields.io/badge/commit--check-enabled-brightgreen?logo=Git&logoColor=white)](https://github.com/commit-check/commit-check)
 
 ## What is this?
 
-This is a package wrapper of Atlassian REST API written in Python, currently, it only supports JIRA and Bitbucket.
+This is a package wrapper of Atlassian REST API written in Python, currently, it supports JIRA and Bitbucket.
 
 This package was created to simplify the implementation of integration with JIRA and Bitbucket.
 
 ## QuickStart
 
 ## Install from PyPI
 
@@ -132,18 +133,14 @@
 ```bash
 cd tests
 coverage run -m unittest
 coverage report -m              # to report on the results
 coverage html                   # to get annotated HTML
 ```
 
-## Changelog
-
-See [CHANGELOG](CHANGELOG.md)
-
 ## FAQ
 
 ### Q1: Which Jira/BitBucket version I used to develop?
 
 > For Jira I used Jira v8.5.9 and Jira Cloud.
 >
 > For BitBucket I used Bitbucket v5.13.1. not support Bitbucket cloud for now.
```

## Comparing `atlassian_api_py-0.5.0.dist-info/RECORD` & `atlassian_api_py-0.5.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 atlassian/__init__.py,sha256=bOwS4IT5qBytCyNravdUfLdM4SsCAM1qRWCOQPa_j6I,194
 atlassian/bitbucket.py,sha256=0g9SGkTEwkLWET1J2FxaDODGOSeOH4QY-sJUArHVwU8,12925
 atlassian/client.py,sha256=MmJSGT2RPOxgK_0CA4_jDmoAK4nLpoytRlJeUmDkEDE,3349
 atlassian/confluence.py,sha256=Xz_pFdsZrv7Df51dnc-uHCS_p8qGsxdwXN_eWRVuj_0,2124
 atlassian/error.py,sha256=6HnhRu1CQLuHjNEj1OmthP8AJqBliwhalHOL76y49Ec,1608
-atlassian/jira.py,sha256=KweXfpIPdxs2BvdtVhO3HoTV1PPGf3lwpID4HudKiSw,11448
+atlassian/jira.py,sha256=6U-xZSC2XLwAg9HQdPTdW53JiX1WuZTM5J3xOa_Inw4,11524
 atlassian/logger.py,sha256=L31bRNHMMw4YFZS4_sU5YeK4JGDSj6oRCz7khmL4Sjc,1162
-atlassian_api_py-0.5.0.dist-info/LICENSE,sha256=0yknWMrerC-pJulAKg6uiNAywvjwHJICz0BZllIeuD8,1074
-atlassian_api_py-0.5.0.dist-info/METADATA,sha256=JuLKbHbWk48aGE6tU5Ga6pcm0jATL7lIoRx_1Fh-NPE,3840
-atlassian_api_py-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-atlassian_api_py-0.5.0.dist-info/top_level.txt,sha256=84-EDv8LNaZx01TCGjBzglwPU1JSRJ7fPSq9uy55Sv0,10
-atlassian_api_py-0.5.0.dist-info/RECORD,,
+atlassian_api_py-0.5.1.dist-info/LICENSE,sha256=0yknWMrerC-pJulAKg6uiNAywvjwHJICz0BZllIeuD8,1074
+atlassian_api_py-0.5.1.dist-info/METADATA,sha256=ypYbIaXeRjL95phK8uscUhmTlb2CZTo1CCKf0z9hRaA,3943
+atlassian_api_py-0.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+atlassian_api_py-0.5.1.dist-info/top_level.txt,sha256=84-EDv8LNaZx01TCGjBzglwPU1JSRJ7fPSq9uy55Sv0,10
+atlassian_api_py-0.5.1.dist-info/RECORD,,
```

