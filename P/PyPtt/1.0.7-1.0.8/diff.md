# Comparing `tmp/PyPtt-1.0.7.tar.gz` & `tmp/PyPtt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPtt-1.0.7.tar", last modified: Sun Apr  9 09:46:25 2023, max compression
+gzip compressed data, was "PyPtt-1.0.8.tar", last modified: Sun Jun 25 10:13:23 2023, max compression
```

## Comparing `PyPtt-1.0.7.tar` & `PyPtt-1.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-09 09:46:16.000000 PyPtt-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 09:46:16.000000 PyPtt-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (123)    30780 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    22808 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-09 09:46:16.000000 PyPtt-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:46:25.868772 PyPtt-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-09 09:46:16.000000 PyPtt-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-25 10:13:11.000000 PyPtt-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-25 10:13:11.000000 PyPtt-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (123)    30780 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-25 10:13:11.000000 PyPtt-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 10:13:23.826362 PyPtt-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-25 10:13:11.000000 PyPtt-1.0.8/setup.py
```

### Comparing `PyPtt-1.0.7/LICENSE` & `PyPtt-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PKG-INFO` & `PyPtt-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.0.7/PyPtt/PTT.py` & `PyPtt-1.0.8/PyPtt/PTT.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_bucket.py` & `PyPtt-1.0.8/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_call_status.py` & `PyPtt-1.0.8/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_change_pw.py` & `PyPtt-1.0.8/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_comment.py` & `PyPtt-1.0.8/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_del_post.py` & `PyPtt-1.0.8/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_board_info.py` & `PyPtt-1.0.8/PyPtt/_api_get_board_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,15 @@
     if r is not None:
         moderator_line = r.group(0)[5:].strip()
         if '(無)' in moderator_line:
             moderators = []
         else:
             moderators = moderator_line.split('/')
             for moderator in moderators.copy():
-                check = True
-                for c in moderator:
-                    if len(c.encode('big5')) > 1:
-                        check = False
-                        break
-                if not check:
+                if moderator == '徵求中':
                     moderators.remove(moderator)
     logger.debug('板主名單', moderators)
 
     open_status = ('公開狀態(是否隱形): 公開' in ori_screen)
     logger.debug('公開狀態', open_status)
 
     into_top_ten_when_hide = ('隱板時 可以 進入十大排行榜' in ori_screen)
```

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_board_list.py` & `PyPtt-1.0.8/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_bottom_post_list.py` & `PyPtt-1.0.8/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_favourite_board.py` & `PyPtt-1.0.8/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_newest_index.py` & `PyPtt-1.0.8/PyPtt/_api_get_newest_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_post.py` & `PyPtt-1.0.8/PyPtt/_api_get_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     if search_type is not None and not isinstance(search_type, st):
         raise TypeError(f'search_type must be SearchType, but got {search_type}')
     if search_condition is not None:
         check_value.check_type(search_condition, str, 'SearchCondition')
 
     if search_list is not None:
-        check_value.check_type(search_condition, list, 'search_list')
+        check_value.check_type(search_list, list, 'search_list')
 
     if len(board) == 0:
         raise ValueError(f'board error parameter: {board}')
 
     if post_index != 0 and isinstance(post_aid, str):
         raise ValueError('wrong parameter index and aid can\'t both input')
```

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_post_index.py` & `PyPtt-1.0.8/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_time.py` & `PyPtt-1.0.8/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_get_user.py` & `PyPtt-1.0.8/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_give_money.py` & `PyPtt-1.0.8/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_has_new_mail.py` & `PyPtt-1.0.8/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_loginout.py` & `PyPtt-1.0.8/PyPtt/_api_loginout.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_mail.py` & `PyPtt-1.0.8/PyPtt/_api_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_mark_post.py` & `PyPtt-1.0.8/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_post.py` & `PyPtt-1.0.8/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_reply_post.py` & `PyPtt-1.0.8/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_search_user.py` & `PyPtt-1.0.8/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_set_board_title.py` & `PyPtt-1.0.8/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/_api_util.py` & `PyPtt-1.0.8/PyPtt/_api_util.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/check_value.py` & `PyPtt-1.0.8/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/command.py` & `PyPtt-1.0.8/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/config.py` & `PyPtt-1.0.8/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/connect_core.py` & `PyPtt-1.0.8/PyPtt/connect_core.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/data_type.py` & `PyPtt-1.0.8/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/exceptions.py` & `PyPtt-1.0.8/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/i18n.py` & `PyPtt-1.0.8/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/lib_util.py` & `PyPtt-1.0.8/PyPtt/lib_util.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/screens.py` & `PyPtt-1.0.8/PyPtt/screens.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt/service.py` & `PyPtt-1.0.8/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/PyPtt.egg-info/PKG-INFO` & `PyPtt-1.0.8/PyPtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.7
+Version: 1.0.8
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.0.7/PyPtt.egg-info/SOURCES.txt` & `PyPtt-1.0.8/PyPtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/README.md` & `PyPtt-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.7/setup.py` & `PyPtt-1.0.8/setup.py`

 * *Files identical despite different names*

