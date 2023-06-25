# Comparing `tmp/ilds-2023.5.16.tar.gz` & `tmp/ilds-2023.6.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2023.5.16.tar", last modified: Tue May 16 08:29:59 2023, max compression
+gzip compressed data, was "dist\ilds-2023.6.25.tar", last modified: Sun Jun 25 11:31:10 2023, max compression
```

## Comparing `ilds-2023.5.16.tar` & `ilds-2023.6.25.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.5.16/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.5.16/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.5.16/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.5.16/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.5.16/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.5.16/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.5.16/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.5.16/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.5.16/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2023.5.16/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    27734 2023-05-16 08:23:40.000000 ilds-2023.5.16/ilds/file.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.5.16/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.5.16/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.5.16/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    17951 2023-04-27 08:50:24.000000 ilds-2023.5.16/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.5.16/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.5.16/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.5.16/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.5.16/ilds/net.py
--rw-rw-rw-   0        0        0     8384 2023-05-16 07:09:24.000000 ilds-2023.5.16/ilds/pd.py
--rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.5.16/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.5.16/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.5.16/ilds/util.py
--rw-rw-rw-   0        0        0       23 2023-05-16 08:29:14.000000 ilds-2023.5.16/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.5.16/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1317 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      695 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1317 2023-05-16 08:29:59.000000 ilds-2023.5.16/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.5.16/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-16 08:29:59.000000 ilds-2023.5.16/setup.cfg
--rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.5.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.6.25/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.6.25/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.6.25/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.6.25/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.6.25/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.6.25/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.6.25/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.6.25/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.6.25/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2023.6.25/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    27734 2023-05-16 08:23:40.000000 ilds-2023.6.25/ilds/file.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.6.25/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.6.25/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.6.25/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.6.25/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.6.25/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.6.25/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    18007 2023-06-25 11:27:17.000000 ilds-2023.6.25/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.6.25/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.6.25/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.6.25/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.6.25/ilds/net.py
+-rw-rw-rw-   0        0        0     8384 2023-05-16 07:09:24.000000 ilds-2023.6.25/ilds/pd.py
+-rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.6.25/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.6.25/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.6.25/ilds/util.py
+-rw-rw-rw-   0        0        0       23 2023-06-25 11:31:07.000000 ilds-2023.6.25/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.6.25/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-25 11:31:09.000000 ilds-2023.6.25/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1317 2023-06-25 11:31:09.000000 ilds-2023.6.25/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-06-25 11:31:09.000000 ilds-2023.6.25/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      695 2023-06-25 11:31:10.000000 ilds-2023.6.25/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 11:31:09.000000 ilds-2023.6.25/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1317 2023-06-25 11:31:10.000000 ilds-2023.6.25/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.6.25/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-25 11:31:10.000000 ilds-2023.6.25/setup.cfg
+-rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.6.25/setup.py
```

### Comparing `ilds-2023.5.16/ilds/cmd.py` & `ilds-2023.6.25/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/django/admin.py` & `ilds-2023.6.25/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/django/import_export.py` & `ilds-2023.6.25/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/django/model.py` & `ilds-2023.6.25/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/django/user.py` & `ilds-2023.6.25/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/django/util.py` & `ilds-2023.6.25/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/everything.py` & `ilds-2023.6.25/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/excel_xlrd.py` & `ilds-2023.6.25/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/excel_xlsx.py` & `ilds-2023.6.25/ilds/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/file.py` & `ilds-2023.6.25/ilds/file.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/lib/browsercookie.py` & `ilds-2023.6.25/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/lib/configobj/validate.py` & `ilds-2023.6.25/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/lib/configobj/__init__.py` & `ilds-2023.6.25/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/lib/hexdump.py` & `ilds-2023.6.25/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/match_data.py` & `ilds-2023.6.25/ilds/match_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 
     # print('cleaning_data', is_digital, dropna_subset, exists_subset, astype_str_list, multiple_results, replace_columns)
 
     # 清理需要检查数据中的空白内容
     if dropna_subset is not None:
         old_count = len(df)
         df = df.dropna(how='all', subset=dropna_subset)
-        infos.append(f'{dropna_subset} 删除空白内容：{old_count - len(df)} 行')
+        info = f'cleaning_data {dropna_subset} 删除空白内容：{old_count - len(df)} 行'
+        print(info)
+        infos.append(info)
 
     # print('填充数据表中空值')
     df = df.fillna(value='')
 
     if is_digital:
         if exists_subset is not None:
             df['检查重复'] = df.apply(get_digital_dup, axis=1, args=exists_subset)
```

### Comparing `ilds-2023.5.16/ilds/md.py` & `ilds-2023.6.25/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/md5summer.py` & `ilds-2023.6.25/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/mycsv.py` & `ilds-2023.6.25/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/net.py` & `ilds-2023.6.25/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/pd.py` & `ilds-2023.6.25/ilds/pd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/spider.py` & `ilds-2023.6.25/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/time.py` & `ilds-2023.6.25/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds/util.py` & `ilds-2023.6.25/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/ilds.egg-info/PKG-INFO` & `ilds-2023.6.25/ilds.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.5.16
+Version: 2023.6.25
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.5.16/ilds.egg-info/SOURCES.txt` & `ilds-2023.6.25/ilds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilds-2023.5.16/PKG-INFO` & `ilds-2023.6.25/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.5.16
+Version: 2023.6.25
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.5.16/setup.py` & `ilds-2023.6.25/setup.py`

 * *Files identical despite different names*

