# Comparing `tmp/xia_git_gitlab-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_git_gitlab-0.1.5-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 1890 bytes, number of entries: 6
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-25 12:47 xia_git_gitlab/__init__.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 12:47 xia_git_gitlab-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Jun-25 12:47 xia_git_gitlab-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 12:47 xia_git_gitlab-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-25 12:47 xia_git_gitlab-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      504 b- defN 23-Jun-25 12:47 xia_git_gitlab-0.1.4.dist-info/RECORD
-6 files, 1564 bytes uncompressed, 964 bytes compressed:  38.4%
+Zip file size: 164624 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-25 13:57 xia_git_gitlab/__init__.py
+-rw-r--r--  2.0 unx   455712 b- defN 23-Jun-25 13:57 xia_git_gitlab/git.cpython-39-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-25 13:57 xia_git_gitlab-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      700 b- defN 23-Jun-25 13:57 xia_git_gitlab-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-25 13:57 xia_git_gitlab-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-25 13:57 xia_git_gitlab-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      603 b- defN 23-Jun-25 13:57 xia_git_gitlab-0.1.5.dist-info/RECORD
+7 files, 457384 bytes uncompressed, 163544 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: xia_git_gitlab/__init__.py
 Comment: 
 
-Filename: xia_git_gitlab-0.1.4.dist-info/LICENSE.txt
+Filename: xia_git_gitlab/git.cpython-39-darwin.so
 Comment: 
 
-Filename: xia_git_gitlab-0.1.4.dist-info/METADATA
+Filename: xia_git_gitlab-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.1.4.dist-info/WHEEL
+Filename: xia_git_gitlab-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_git_gitlab-0.1.4.dist-info/top_level.txt
+Filename: xia_git_gitlab-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git_gitlab-0.1.4.dist-info/RECORD
+Filename: xia_git_gitlab-0.1.5.dist-info/top_level.txt
+Comment: 
+
+Filename: xia_git_gitlab-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git_gitlab/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git_gitlab.git import GitlabGit
 
 __all__ = [
     "GitlabGit"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## Comparing `xia_git_gitlab-0.1.4.dist-info/METADATA` & `xia_git_gitlab-0.1.5.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git-gitlab
-Version: 0.1.4
+Version: 0.1.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.1.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.1.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

