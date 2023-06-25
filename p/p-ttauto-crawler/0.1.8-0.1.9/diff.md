# Comparing `tmp/p-ttauto-crawler-0.1.8.tar.gz` & `tmp/p-ttauto-crawler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.1.8.tar", last modified: Wed Jun 21 11:23:59 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.9.tar", last modified: Wed Jun 21 11:28:13 2023, max compression
```

## Comparing `p-ttauto-crawler-0.1.8.tar` & `p-ttauto-crawler-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:23:59.087402 p-ttauto-crawler-0.1.8/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      397 2023-06-21 11:23:59.086403 p-ttauto-crawler-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:23:59.066402 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 11:23:58.000000 p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:23:59.087402 p-ttauto-crawler-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-06-21 11:23:56.000000 p-ttauto-crawler-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:23:59.083401 p-ttauto-crawler-0.1.8/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/__init__.py
--rw-rw-rw-   0        0        0     9460 2023-06-21 11:15:15.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/auto_crawler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:23:59.084401 p-ttauto-crawler-0.1.8/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/bin/print_md5.py
--rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/binary.py
--rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/downloader.py
--rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/mecord_downloader.py
--rw-rw-rw-   0        0        0     9074 2023-06-21 11:23:39.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/processing.py
--rw-rw-rw-   0        0        0     3934 2023-06-21 11:15:21.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/task.py
--rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/ttsUtils.py
--rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/txt2proj.py
--rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/uploading.py
--rw-rw-rw-   0        0        0    10914 2023-06-21 11:06:41.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/utils.py
--rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/video_merge.py
--rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/video_random_cutter.py
--rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.8/ttauto_crawler/ytdlp_downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:28:13.209024 p-ttauto-crawler-0.1.9/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:28:13.209024 p-ttauto-crawler-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 11:28:13.183793 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 11:28:13.000000 p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:28:13.210023 p-ttauto-crawler-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-21 11:28:09.000000 p-ttauto-crawler-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:28:13.206024 p-ttauto-crawler-0.1.9/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-06-21 11:15:15.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:28:13.208022 p-ttauto-crawler-0.1.9/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4093 2023-06-21 07:12:34.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-21 10:59:45.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9074 2023-06-21 11:23:39.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-21 11:15:21.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2256 2023-06-21 05:25:26.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-21 11:06:41.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.9/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.1.8/LICENSE` & `p-ttauto-crawler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/p_ttauto_crawler.egg-info/SOURCES.txt` & `p-ttauto-crawler-0.1.9/p_ttauto_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/setup.py` & `p-ttauto-crawler-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.1.8",
+    version="0.1.9",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -18,15 +18,15 @@
     ],
     py_modules=[],
     install_requires=[
         'requests',
         'oss2',
         'Image',
         'Pillow',
-        'p-template-generator>=0.1.87',
+        'p-template-generator>=0.1.67',
         'fake_useragent',
         'mutagen',
         'yt-dlp==2023.3.4',
         'moviepy',
         'urlparser'
     ],
     dependency_links=[],
```

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/auto_crawler.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/auto_crawler.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/bin/print_md5.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/binary.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/binary.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/downloader.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/main.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/mecord_downloader.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/mecord_downloader.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/processing.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/processing.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/task.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/task.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/ttsUtils.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/ttsUtils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/txt2proj.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/txt2proj.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/uploading.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/uploading.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/video_merge.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/video_merge.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/video_random_cutter.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/video_random_cutter.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.1.8/ttauto_crawler/ytdlp_downloader.py` & `p-ttauto-crawler-0.1.9/ttauto_crawler/ytdlp_downloader.py`

 * *Files identical despite different names*

