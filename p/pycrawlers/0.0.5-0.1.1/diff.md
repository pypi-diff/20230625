# Comparing `tmp/pycrawlers-0.0.5.tar.gz` & `tmp/pycrawlers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-0.0.5.tar", last modified: Thu Feb 16 07:13:52 2023, max compression
+gzip compressed data, was "pycrawlers-0.1.1.tar", last modified: Sun Jun 25 05:57:50 2023, max compression
```

## Comparing `pycrawlers-0.0.5.tar` & `pycrawlers-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.490272 pycrawlers-0.0.5/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.0.5/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     1362 2023-02-16 07:13:52.490141 pycrawlers-0.0.5/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      905 2023-02-16 07:10:01.000000 pycrawlers-0.0.5/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.487887 pycrawlers-0.0.5/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.0.5/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.0.5/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.488086 pycrawlers-0.0.5/pycrawlers/
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.489079 pycrawlers-0.0.5/pycrawlers/Hugging_Face/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.0.5/pycrawlers/Hugging_Face/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.0.5/pycrawlers/Hugging_Face/download.py
--rw-r--r--   0 bo         (501) staff       (20)      205 2022-08-17 09:04:51.000000 pycrawlers-0.0.5/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.489822 pycrawlers-0.0.5/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.0.5/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      247 2022-09-13 06:34:23.000000 pycrawlers-0.0.5/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     1963 2022-09-13 11:29:26.000000 pycrawlers-0.0.5/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-02-16 07:13:52.488721 pycrawlers-0.0.5/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     1362 2023-02-16 07:13:52.000000 pycrawlers-0.0.5/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      414 2023-02-16 07:13:52.000000 pycrawlers-0.0.5/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-02-16 07:13:52.000000 pycrawlers-0.0.5/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       42 2023-02-16 07:13:52.000000 pycrawlers-0.0.5/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-02-16 07:13:52.000000 pycrawlers-0.0.5/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-02-16 07:13:52.490313 pycrawlers-0.0.5/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      825 2022-11-07 05:14:05.000000 pycrawlers-0.0.5/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.429322 pycrawlers-0.1.1/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.1/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     1746 2023-06-25 05:57:50.429196 pycrawlers-0.1.1/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     1289 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.426503 pycrawlers-0.1.1/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.1/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.1/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.426708 pycrawlers-0.1.1/pycrawlers/
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.427702 pycrawlers-0.1.1/pycrawlers/Hugging_Face/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.1/pycrawlers/Hugging_Face/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.1/pycrawlers/Hugging_Face/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.428320 pycrawlers-0.1.1/pycrawlers/Web_Site/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3228 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)     1006 2023-06-25 03:48:03.000000 pycrawlers-0.1.1/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.428918 pycrawlers-0.1.1/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.1/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.1/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.1/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.427374 pycrawlers-0.1.1/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     1746 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      521 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-25 05:57:50.429361 pycrawlers-0.1.1/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-25 04:15:50.000000 pycrawlers-0.1.1/setup.py
```

### Comparing `pycrawlers-0.0.5/LICENSE` & `pycrawlers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.0.5/PKG-INFO` & `pycrawlers-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.0.5
+Version: 0.1.1
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -52,8 +52,24 @@
     # 2.批量获取
     # 2.1 使用默认保存位置（'./'）
     hg.get_batch_data(urls)
     
     # 2.2 自定义保存地址
     # hg.get_batch_data(urls, paths)
 
+#### 2.  通用抓取网页
+可以抓取那些反爬不厉害的网站
+
+
+    from pycrawlers import website
+
+    mongo_host = ''
+    mongo_port = '27017'
+    db_name = 'huxiu'
+    id_collection_name = 'huxiu_id'
+    collection_name = 'huxiu'
+    base_url = 'https://www.huxiu.com'
+    
+    
+    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
+
```

### Comparing `pycrawlers-0.0.5/README.md` & `pycrawlers-0.1.1/other/dw_hg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-# crawlers
+# -*- coding: UTF-8 -*-
+# @Time : 2022/8/17 15:16 
+# @Author : 刘洪波
 
-### 介绍
-爬虫集合
 
-### 可获取的项目
+from pycrawlers import huggingface
 
-1.  hugging face 上的模型文件
+urls = ['https://huggingface.co/albert-base-v2/tree/main',
+        'https://huggingface.co/dmis-lab/biosyn-sapbert-bc5cdr-disease/tree/main']
 
+paths = ['./model_1/albert-base-v2', './model_2/']
+# 实例化类
+# 使用默认 base_url (https://huggingface.co)
+hg = huggingface()
+# 自定义 base_uel
+# hg = huggingface('https://huggingface.co')
 
-### 项目示例
-
-#### 1.  hugging face
+# 1. 单个获取
+# 1.1 使用默认保存位置（'./'）
+hg.get_data(urls[0])
+
+# 1.2 自定义保存地址
+# hg.get_data(urls[0], paths[0])
+
+# 2.批量获取
+# 2.1 使用默认保存位置（'./'）
+hg.get_batch_data(urls)
+
+# 2.2 自定义保存地址
+# hg.get_batch_data(urls, paths)
 
 
 
-    from pycrawlers import huggingface
-
-    urls = ['https://huggingface.co/albert-base-v2/tree/main',
-            'https://huggingface.co/dmis-lab/biosyn-sapbert-bc5cdr-disease/tree/main']
-    
-    paths = ['./model_1/albert-base-v2', './model_2/']
-    # 实例化类
-    # 使用默认 base_url (https://huggingface.co)
-    hg = huggingface()
-    # 自定义 base_uel
-    # hg = huggingface('https://huggingface.co')
-    
-    # 1. 单个获取
-    # 1.1 使用默认保存位置（'./'）
-    hg.get_data(urls[0])
-    
-    # 1.2 自定义保存地址
-    # hg.get_data(urls[0], paths[0])
-    
-    # 2.批量获取
-    # 2.1 使用默认保存位置（'./'）
-    hg.get_batch_data(urls)
-    
-    # 2.2 自定义保存地址
-    # hg.get_batch_data(urls, paths)
```

### Comparing `pycrawlers-0.0.5/pycrawlers/Hugging_Face/download.py` & `pycrawlers-0.1.1/pycrawlers/Hugging_Face/download.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.0.5/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-0.1.1/pycrawlers.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.0.5
+Version: 0.1.1
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -52,8 +52,24 @@
     # 2.批量获取
     # 2.1 使用默认保存位置（'./'）
     hg.get_batch_data(urls)
     
     # 2.2 自定义保存地址
     # hg.get_batch_data(urls, paths)
 
+#### 2.  通用抓取网页
+可以抓取那些反爬不厉害的网站
+
+
+    from pycrawlers import website
+
+    mongo_host = ''
+    mongo_port = '27017'
+    db_name = 'huxiu'
+    id_collection_name = 'huxiu_id'
+    collection_name = 'huxiu'
+    base_url = 'https://www.huxiu.com'
+    
+    
+    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
+
```

### Comparing `pycrawlers-0.0.5/setup.py` & `pycrawlers-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='0.0.5',
+    version='0.1.1',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['requests>=2.27.1', 'tqdm>=4.64.0', 'lxml>=4.8.0'],
+    install_requires=[
+        'requests>=2.27.1',
+        'tqdm>=4.64.0',
+        'lxml>=4.8.0',
+        'pymongo>=3.12.0',
+        'pytz>=2021.3',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

