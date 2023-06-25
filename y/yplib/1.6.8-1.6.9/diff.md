# Comparing `tmp/yplib-1.6.8.tar.gz` & `tmp/yplib-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.8.tar", last modified: Mon Jun 19 09:01:47 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.9.tar", last modified: Sun Jun 25 02:45:47 2023, max compression
```

## Comparing `yplib-1.6.8.tar` & `yplib-1.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.986600 yplib-1.6.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 09:01:47.986115 yplib-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 09:01:47.986791 yplib-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 09:01:42.000000 yplib-1.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.981691 yplib-1.6.8/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    24955 2023-06-19 09:01:29.000000 yplib-1.6.8/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.985538 yplib-1.6.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 02:45:47.007185 yplib-1.6.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 02:45:47.006328 yplib-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 02:45:47.007271 yplib-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 02:45:26.000000 yplib-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:45:47.003599 yplib-1.6.9/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    25626 2023-06-25 02:45:16.000000 yplib-1.6.9/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-25 02:45:47.005849 yplib-1.6.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 02:45:46.000000 yplib-1.6.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-25 02:45:46.000000 yplib-1.6.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 02:45:46.000000 yplib-1.6.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 02:45:46.000000 yplib-1.6.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.8/LICENSE` & `yplib-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.8/setup.py` & `yplib-1.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.8",
+  version="1.6.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.8/yplib/chart.py` & `yplib-1.6.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.8/yplib/chart_html.py` & `yplib-1.6.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.8/yplib/file.py` & `yplib-1.6.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.8/yplib/http_util.py` & `yplib-1.6.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.8/yplib/index.py` & `yplib-1.6.9/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,31 +278,46 @@
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
 # 根据json的key排序,用于签名
-def sort_by_json_key(data_obj):
-    return '&'.join(list(map(
-        lambda x: f'{x}={data_obj[x]}',
-        sorted(data_obj, key=lambda x: x)
-    )))
+# 按照 key 排序, 按照 key=value 然后再 & 连接, 如果数据中有 list, 使用 , 连接 list 中的数据, 然后拼接成 str 返回
+# separator : 分隔符 , 默认 &
+# join      : 连接符 , 默认 =
+# join_list : list 数据 连接符 , 默认 ,
+def sort_by_json_key(data_obj, separator='&', join='=', join_list=','):
+    if isinstance(data_obj, list) or isinstance(data_obj, tuple) or isinstance(data_obj, set):
+        return join_list.join(list(map(lambda x: f'{x}', data_obj)))
+    # 按照 key 排序
+    key_list = sorted(data_obj, key=lambda x: x)
+    r_l = []
+    for key_one in key_list:
+        value_one = data_obj[key_one]
+        if can_use_json(value_one):
+            s = sort_by_json_key(value_one)
+        else:
+            s = str(value_one)
+        r_l.append(f'{key_one}{join}{s}')
+    return separator.join(r_l)
 
 
 # data = {}
 # data['merchantId'] = "merchantId"
 # data['currency'] = "IDR"
-# data['aaccType'] = "payout"
-# data['abccType'] = "payout"
-# data['adcType'] = "payout"
 # data['accType'] = "payout"
-# data['accType1'] = "payout"
-# data['accType2'] = "payout"
 # data['version'] = "1.0"
+# data['b'] = {
+#     'a': 1,
+#     'c': 'c',
+#     'b': 'po',
+# }
+# b = [2, 3, 8, 4, "yp"]
+# data['c'] = b
 # sign = sort_by_json_key(data)
 # print(sign)
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # separator : 是否对每一行进行分割,如果存在这个字段,就分割
```

