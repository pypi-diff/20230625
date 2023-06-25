# Comparing `tmp/miuc-0.1.7.tar.gz` & `tmp/miuc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.7.tar", max compression
+gzip compressed data, was "miuc-0.1.8.tar", max compression
```

## Comparing `miuc-0.1.7.tar` & `miuc-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.7/LICENSE
--rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.7/miuc/__init__.py
--rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.7/miuc/main.py
--rw-r--r--   0        0        0    26107 2023-06-25 01:17:31.758549 miuc-0.1.7/miuc/site_processor.py
--rw-r--r--   0        0        0     2258 2023-06-25 01:14:57.116556 miuc-0.1.7/miuc/utils.py
--rw-r--r--   0        0        0     2179 2023-06-25 01:17:49.848313 miuc-0.1.7/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-25 01:19:57.490194 miuc-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1543 2023-06-24 17:29:12.273734 miuc-0.1.7/README.md
--rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 miuc-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.8/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.8/miuc/__init__.py
+-rw-r--r--   0        0        0     1091 2023-06-25 03:33:01.484702 miuc-0.1.8/miuc/main.py
+-rw-r--r--   0        0        0    26107 2023-06-25 01:17:31.758549 miuc-0.1.8/miuc/site_processor.py
+-rw-r--r--   0        0        0     2258 2023-06-25 01:14:57.116556 miuc-0.1.8/miuc/utils.py
+-rw-r--r--   0        0        0     2179 2023-06-25 01:17:49.848313 miuc-0.1.8/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-25 03:33:14.927747 miuc-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1543 2023-06-24 17:29:12.273734 miuc-0.1.8/README.md
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 miuc-0.1.8/PKG-INFO
```

### Comparing `miuc-0.1.7/LICENSE` & `miuc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `miuc-0.1.7/miuc/main.py` & `miuc-0.1.8/miuc/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,29 @@
 """
 
 import argparse
 from .web_parser import parse_url
 import io
 import sys
 
+VERSION = (0,1,0)
 
 def main():
     
     parser = argparse.ArgumentParser("Markdown Intelligence Url Complete")
     parser.add_argument("-s", "--site", action="store_true", help="add site info")
     parser.add_argument("-t", "--max-time-limit", type=int, default=5, help="max time limit")
+    parser.add_argument('-v','--version',action='store_true',help='show version')
     parser.add_argument("url", type=str, help="website url")
     args = parser.parse_args()
 
+    if args.version:
+        print(VERSION)
+        return
+
     if not args.url:
         print("miuc <url>")
         exit(1)
 
     markdown_url = parse_url(args.url, max_time_limit=args.max_time_limit)
     sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8')
     print(markdown_url)
```

### Comparing `miuc-0.1.7/miuc/site_processor.py` & `miuc-0.1.8/miuc/site_processor.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.7/miuc/utils.py` & `miuc-0.1.8/miuc/utils.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.7/miuc/web_parser.py` & `miuc-0.1.8/miuc/web_parser.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.7/README.md` & `miuc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `miuc-0.1.7/PKG-INFO` & `miuc-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

