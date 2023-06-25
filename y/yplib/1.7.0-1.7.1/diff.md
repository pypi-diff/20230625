# Comparing `tmp/yplib-1.7.0.tar.gz` & `tmp/yplib-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.0.tar", last modified: Sun Jun 25 06:25:32 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.1.tar", last modified: Sun Jun 25 07:46:56 2023, max compression
```

## Comparing `yplib-1.7.0.tar` & `yplib-1.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:25:32.715018 yplib-1.7.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 06:25:32.714837 yplib-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 06:25:32.715487 yplib-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 06:25:13.000000 yplib-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:25:32.711196 yplib-1.7.0/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.7.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.7.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.0/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    25687 2023-06-25 06:24:20.000000 yplib-1.7.0/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:25:32.714307 yplib-1.7.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 06:25:32.000000 yplib-1.7.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-25 06:25:32.000000 yplib-1.7.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:25:32.000000 yplib-1.7.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 06:25:32.000000 yplib-1.7.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.383916 yplib-1.7.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 07:46:56.383857 yplib-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:46:56.383916 yplib-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 07:46:07.000000 yplib-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.380982 yplib-1.7.1/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.7.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.1/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.1/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:46:56.382890 yplib-1.7.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 07:46:56.000000 yplib-1.7.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.0/LICENSE` & `yplib-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.0/setup.py` & `yplib-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.0",
+  version="1.7.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.0/yplib/chart.py` & `yplib-1.7.1/yplib/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,31 +77,31 @@
 #         ]
 #  name : 文件名称,折线图的名称
 #  name_raw : 用原始的名字,不用带上属性 line_stack
 def to_chart(x_list,
              y_list=None,
              name=None,
              name_raw=False):
+    # 当 y_list 没有的话, 需要整理出 y_list 的数据
     if y_list is None:
         data_list = x_list
         x_list = []
         y_list = []
-        index = 0
-        for line_one in data_list:
+        for index in range(len(data_list)):
+            line_one = data_list[index]
             if index > 0:
                 x_list.append(line_one[0])
             # 第一行数据
             if index == 0:
                 for y in range(1, len(line_one)):
                     y_list.append({'name': line_one[y], 'data': []})
             # 第二行开始的数据
             if index > 0:
                 for y in range(1, len(line_one)):
                     y_list[y - 1]['data'].append(line_one[y])
-            index += 1
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
         if 'hide' in y_one and y_one['hide']:
             legend_selected[y_one['name']] = 0
         else:
@@ -121,15 +121,15 @@
         y_one['stack'] = 'Total'
         if 'smooth' in y_one and y_one['smooth']:
             y_one['smooth'] = 1
         else:
             y_one['smooth'] = 0
         series.append(y_one)
 
-    if name_raw is False:
+    if not name_raw:
         name = 'line_stack' if name is None else name + '_line_stack'
     insert_data_to_chart(html_data=line_stack_html(),
                          name=name,
                          x_list=x_list,
                          legend=legend,
                          series=series)
 
@@ -336,9 +336,11 @@
 #
 # data_list =
 #
 # to_chart(data_list)
 
 # to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls'))
 
+to_chart(to_list(r'C:\Users\yangpu\Desktop\study\12.xls', column_date=1), name='yp')
+
 #
 # print('end')
```

### Comparing `yplib-1.7.0/yplib/chart_html.py` & `yplib-1.7.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.0/yplib/file.py` & `yplib-1.7.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.0/yplib/http_util.py` & `yplib-1.7.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.0/yplib/index.py` & `yplib-1.7.1/yplib/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,30 +105,37 @@
     if isinstance(data, dict) or isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set):
         return True
     return False
 
 
 # 检查文件夹是否存在,不存在,就创建新的
 def check_file(file_name):
-    if file_name != '' and os.path.exists(file_name) is False:
-        os.mkdir(file_name)
+    if file_name is None or file_name == '':
+        return
+    for sep in ['\\', '/']:
+        f_n = file_name.split(sep)
+        for i in range(1, len(f_n) + 1):
+            # C:\Users\yangpu\Desktop\study\p.t
+            p_n = sep.join(f_n[0:i])
+            if not os.path.exists(p_n):
+                os.mkdir(p_n)
 
 
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
-    t = datetime.today().strftime('%d%H%M_%S_%f').split('_')
+    [day, hour, minute, second, ss] = datetime.today().strftime('%d_%H_%M_%S_%f').split('_')
     return str(file_name) \
-        + '_' + t[0] \
-        + '_' + t[1] + t[2][0] + random_int(1) \
+        + '_' + day + hour + minute \
+        + '_' + second + ss[0] + random_int(1) \
         + suffix
 
 
 # 获得文件名称
 def file_is_empty(file_name=None):
-    return file_name is None or file_name == '' or os.path.exists(file_name) is False
+    return file_name is None or file_name == '' or not os.path.exists(file_name)
 
 
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
 
 
 def do_sha256(data='do_sha256'):
@@ -236,34 +243,45 @@
 def to_date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return str(to_datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds,
                                milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # data_list : 数组数据, 也可以不是数组
-# file_name : 文件名
+# file_name : 文件名 , 当文件名是 C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt 这种类型的时候, 可以直接创建文件夹,
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def to_txt(data_list, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
+    for sep in ['\\', '/']:
+        f_n = file_name.split(sep)
+        if len(f_n) > 1:
+            file_name = f_n[-1]
+            file_path = sep.join(f_n[0:-1])
+            if '.' in file_name:
+                suffix = '.' + file_name.split('.')[-1]
+                file_name = file_name[0:file_name.find('.')]
+                fixed_name = True
+
     # 检查路径 file_path
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     # 生成 file_name
     if fixed_name:
         file_name = file_name + suffix
     else:
         file_name = get_file_name(file_name, suffix)
     # 文件路径
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
+    # 写入文件
     text_file = open(file_name_path, 'a', encoding='utf-8')
-    if isinstance(data_list, list) is False:
+    if not isinstance(data_list, list):
         text_file.write(to_str(data_list) + '\n')
     else:
         for one in data_list:
             text_file.write(to_str(one) + '\n')
     text_file.close()
     return file_name_path
 
@@ -285,15 +303,15 @@
 # 按照 key 排序, 按照 key=value 然后再 & 连接, 如果数据中有 list, 使用 , 连接 list 中的数据, 然后拼接成 str 返回
 # separator : 分隔符 , 默认 &
 # join      : 连接符 , 默认 =
 # join_list : list 数据 连接符 , 默认 ,
 def sort_by_json_key(data_obj, separator='&', join='=', join_list=','):
     if isinstance(data_obj, list) or isinstance(data_obj, tuple) or isinstance(data_obj, set):
         return join_list.join(list(map(lambda x: f'{x}', data_obj)))
-    if isinstance(data_obj, dict) is False:
+    if not isinstance(data_obj, dict):
         return str(data_obj)
     data_list = sorted(data_obj.items(), key=lambda x: x[0])
     r_l = []
     for one in data_list:
         value_one = one[1]
         if can_use_json(value_one):
             s = sort_by_json_key(value_one)
@@ -421,22 +439,22 @@
             if list_index[1] is not None and j + 1 in list_index[1]:
                 cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
                 is_date = True
                 row_data.append(cell_data)
                 if list_only_one:
                     row_data = cell_data
             # 日期时间格式的列
-            if is_date is False and list_index[2] is not None and j + 1 in list_index[2]:
+            if not is_date and list_index[2] is not None and j + 1 in list_index[2]:
                 cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
                 is_datetime = True
                 row_data.append(cell_data)
                 if list_only_one:
                     row_data = cell_data
             # 指定需要的列
-            if is_date is False and is_datetime is False:
+            if not is_date and not is_datetime:
                 if list_index[0] is None:
                     row_data.append(cell_data)
                 else:
                     # 指定需要的列
                     if j + 1 in list_index[0]:
                         row_data.append(cell_data)
                         if list_only_one:
@@ -482,20 +500,20 @@
         # 判断结束位置
         if end_index is not None and i + 1 >= to_int(end_index):
             continue
         # 判断数量
         if count is not None and c >= to_int(count):
             continue
         # 开始标记位
-        if start_flag is False and line.find(start_line) > -1:
+        if not start_flag and line.find(start_line) > -1:
             start_flag = True
         # 开始标记位
-        if end_flag is False and line.find(end_line) > -1:
+        if not end_flag and line.find(end_line) > -1:
             end_flag = True
-        if start_flag is False:
+        if not start_flag:
             continue
         elif end_flag:
             continue
         c += 1
         if separator is not None:
             data_list.append(line.split(str(separator)))
         else:
@@ -568,15 +586,18 @@
             sh.write(m, n, s)  # 写入A3，数值等于1
         m += 1
     # 5. 保存
     # myWorkbook.save('5002200.xls')
     w_b.save(file_path + '/' + get_file_name(file_name, '.xls'))
 
 # print('start')
-# to_txt([1,2,3], 'p')
+# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt')
+# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\abc\d\e\f')
+# to_txt([1, 2, 3], r'C:\Users\yangpu\Desktop\study\p.t')
+# to_txt([1, 2, 3], 'C:/Users/yangpu/Desktop/study/p.t')
 # to_txt_file_name([1,2,3], 'p')
 #
 #
 # li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
 #
 # to_log()
 #
@@ -709,14 +730,16 @@
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, end_index=1288))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_index=1285, count=3))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', count=1))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
 # print(to_list(r'D:\notepad_file\202306\asfdf.html', start_line='<h2>Unicode 字符串</h2>', end_line='所有的字符串都是Unicode字符串'))
 
 #
+# print(not False)
+# print(not True)
 # print(datetime.now())
 # print(datetime.today())
 # print(datetime.today().strftime('%m%d%H%M_%S_%f'))
 # print(get_file_name('1'))
 #
 # for i in range(100):
 #     print(get_file_name('a'))
```

