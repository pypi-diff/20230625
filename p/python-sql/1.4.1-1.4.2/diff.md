# Comparing `tmp/python-sql-1.4.1.tar.gz` & `tmp/python-sql-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sql-1.4.1.tar", last modified: Fri Jun 16 15:15:02 2023, max compression
+gzip compressed data, was "python-sql-1.4.2.tar", last modified: Sun Jun 25 09:04:49 2023, max compression
```

## Comparing `python-sql-1.4.1.tar` & `python-sql-1.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-16 15:15:02.546451 python-sql-1.4.1/
--rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python-sql-1.4.1/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1455 2023-05-01 16:05:42.000000 python-sql-1.4.1/.gitlab-ci.yml
--rw-r--r--   0 ced       (1000) ced       (1000)      781 2023-06-16 15:14:07.000000 python-sql-1.4.1/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python-sql-1.4.1/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2724 2023-06-16 15:12:55.000000 python-sql-1.4.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-16 15:13:18.000000 python-sql-1.4.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python-sql-1.4.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     8463 2023-06-16 15:15:02.546451 python-sql-1.4.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python-sql-1.4.1/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-16 15:15:02.526450 python-sql-1.4.1/python_sql.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     8463 2023-06-16 15:15:01.000000 python-sql-1.4.1/python_sql.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      932 2023-06-16 15:15:02.000000 python-sql-1.4.1/python_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-16 15:15:01.000000 python-sql-1.4.1/python_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        4 2023-06-16 15:15:01.000000 python-sql-1.4.1/python_sql.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-16 15:15:02.546451 python-sql-1.4.1/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1872 2023-05-01 16:05:42.000000 python-sql-1.4.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-16 15:15:02.529784 python-sql-1.4.1/sql/
--rw-r--r--   0 ced       (1000) ced       (1000)    47133 2023-05-25 15:35:05.000000 python-sql-1.4.1/sql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5241 2022-01-29 01:09:33.000000 python-sql-1.4.1/sql/aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12307 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10782 2022-04-27 16:39:13.000000 python-sql-1.4.1/sql/operators.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-16 15:15:02.546451 python-sql-1.4.1/sql/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python-sql-1.4.1/sql/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python-sql-1.4.1/sql/tests/test_aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_alias.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_as.py
--rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python-sql-1.4.1/sql/tests/test_cast.py
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python-sql-1.4.1/sql/tests/test_collate.py
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python-sql-1.4.1/sql/tests/test_column.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1809 2021-09-14 07:32:34.000000 python-sql-1.4.1/sql/tests/test_combining_query.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python-sql-1.4.1/sql/tests/test_delete.py
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python-sql-1.4.1/sql/tests/test_for.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3960 2023-05-25 15:32:13.000000 python-sql-1.4.1/sql/tests/test_insert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_join.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_lateral.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_literal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15639 2022-04-27 16:39:13.000000 python-sql-1.4.1/sql/tests/test_operators.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18053 2021-12-18 00:49:44.000000 python-sql-1.4.1/sql/tests/test_select.py
--rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python-sql-1.4.1/sql/tests/test_table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3486 2023-05-25 15:40:48.000000 python-sql-1.4.1/sql/tests/test_update.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python-sql-1.4.1/sql/tests/test_values.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_window.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python-sql-1.4.1/sql/tests/test_with.py
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-01-09 18:27:57.000000 python-sql-1.4.1/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-25 09:04:49.931034 python-sql-1.4.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python-sql-1.4.2/.flake8
+-rw-r--r--   0 ced       (1000) ced       (1000)     1455 2023-05-01 16:05:42.000000 python-sql-1.4.2/.gitlab-ci.yml
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2023-06-25 09:04:06.000000 python-sql-1.4.2/.hgtags
+-rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python-sql-1.4.2/.isort.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     2801 2023-06-25 09:03:30.000000 python-sql-1.4.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-25 09:03:37.000000 python-sql-1.4.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python-sql-1.4.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     8463 2023-06-25 09:04:49.931034 python-sql-1.4.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python-sql-1.4.2/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-25 09:04:49.917700 python-sql-1.4.2/python_sql.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8463 2023-06-25 09:04:49.000000 python-sql-1.4.2/python_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      932 2023-06-25 09:04:49.000000 python-sql-1.4.2/python_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-25 09:04:49.000000 python-sql-1.4.2/python_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        4 2023-06-25 09:04:49.000000 python-sql-1.4.2/python_sql.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-25 09:04:49.931034 python-sql-1.4.2/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1872 2023-05-01 16:05:42.000000 python-sql-1.4.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-25 09:04:49.921033 python-sql-1.4.2/sql/
+-rw-r--r--   0 ced       (1000) ced       (1000)    47369 2023-06-18 08:34:57.000000 python-sql-1.4.2/sql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5241 2022-01-29 01:09:33.000000 python-sql-1.4.2/sql/aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12307 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10782 2022-04-27 16:39:13.000000 python-sql-1.4.2/sql/operators.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-25 09:04:49.931034 python-sql-1.4.2/sql/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python-sql-1.4.2/sql/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python-sql-1.4.2/sql/tests/test_aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_alias.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_as.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python-sql-1.4.2/sql/tests/test_cast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python-sql-1.4.2/sql/tests/test_collate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python-sql-1.4.2/sql/tests/test_column.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2021-09-14 07:32:34.000000 python-sql-1.4.2/sql/tests/test_combining_query.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python-sql-1.4.2/sql/tests/test_delete.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python-sql-1.4.2/sql/tests/test_for.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3972 2023-06-18 08:11:33.000000 python-sql-1.4.2/sql/tests/test_insert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_join.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_lateral.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_literal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15639 2022-04-27 16:39:13.000000 python-sql-1.4.2/sql/tests/test_operators.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18053 2021-12-18 00:49:44.000000 python-sql-1.4.2/sql/tests/test_select.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python-sql-1.4.2/sql/tests/test_table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3490 2023-06-18 08:11:33.000000 python-sql-1.4.2/sql/tests/test_update.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python-sql-1.4.2/sql/tests/test_values.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python-sql-1.4.2/sql/tests/test_with.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-01-09 18:27:57.000000 python-sql-1.4.2/tox.ini
```

### Comparing `python-sql-1.4.1/.gitlab-ci.yml` & `python-sql-1.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/.hgtags` & `python-sql-1.4.2/.hgtags`

 * *Files 5% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 194182e5b0e2dc6486a32778860f29c80c0672f9 1.1.0
 de68c850bc6a809b0c88ddbe2fa99b02df07bee3 1.2.0
 b2bcc0f71f6881316c11330c07de34113f088888 1.2.1
 1c38ffeacbb82a9ff6ae3568cdc017dbbeddff5d 1.2.2
 edc03ee84f0ac96d403d8f984d59fffa3274cd2f 1.3.0
 a317c40a4d60089ba9e465fbd64b78df24f9e890 1.4.0
 e71bbae3398cb6a0e72f97a0cada9fcdee2bddea 1.4.1
+fcb64787b51db2068061eb4aa13825abc1134916 1.4.2
```

### Comparing `python-sql-1.4.1/CHANGELOG` & `python-sql-1.4.2/CHANGELOG`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Version 1.4.2 - 2023-06-25
+* Restore usage of alias in returning expression
+
 Version 1.4.1 - 2023-06-16
 * Do not use alias in returning expression
 
 Version 1.4.0 - 2022-05-02
 * Use unittest discover
 * Use only column name for INSERT and UPDATE
 * Add escape to Like operators
```

### Comparing `python-sql-1.4.1/COPYRIGHT` & `python-sql-1.4.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/PKG-INFO` & `python-sql-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.4.1
+Version: 1.4.2
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python-sql-1.4.1/README.rst` & `python-sql-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/python_sql.egg-info/PKG-INFO` & `python-sql-1.4.2/python_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.4.1
+Version: 1.4.2
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python-sql-1.4.1/python_sql.egg-info/SOURCES.txt` & `python-sql-1.4.2/python_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/setup.py` & `python-sql-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/__init__.py` & `python-sql-1.4.2/sql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numbers
 import string
 import warnings
 from collections import defaultdict
 from itertools import chain
 from threading import current_thread, local
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 __all__ = ['Flavor', 'Table', 'Values', 'Literal', 'Column', 'Join',
     'Asc', 'Desc', 'NullsFirst', 'NullsLast', 'format2numeric']
 
 
 def _escape_identifier(name):
     return '"%s"' % name.replace('"', '""')
 
@@ -715,44 +715,42 @@
 
     @returning.setter
     def returning(self, value):
         if value is not None:
             assert isinstance(value, list)
         self._returning = value
 
-    def _format(self, value, param=None):
+    @staticmethod
+    def _format(value, param=None):
         if param is None:
             param = Flavor.get().param
-        if isinstance(value, Column) and value.table == self.table:
-            return value.column_name
-        elif isinstance(value, Expression):
+        if isinstance(value, Expression):
             return str(value)
         elif isinstance(value, Select):
-            with AliasManager():
-                return '(%s)' % value
+            return '(%s)' % value
         else:
             return param
 
     def __str__(self):
         columns = ''
         if self.columns:
             assert all(col.table == self.table for col in self.columns)
             # Get columns without alias
             columns = ', '.join(c.column_name for c in self.columns)
             columns = ' (' + columns + ')'
-        returning = ''
-        if self.returning:
-            returning = ' RETURNING ' + ', '.join(
-                map(self._format, self.returning))
         with AliasManager():
             if isinstance(self.values, Query):
                 values = ' %s' % str(self.values)
                 # TODO manage DEFAULT
             elif self.values is None:
                 values = ' DEFAULT VALUES'
+            returning = ''
+            if self.returning:
+                returning = ' RETURNING ' + ', '.join(
+                    map(self._format, self.returning))
             return (self._with_str()
                 + 'INSERT INTO %s AS "%s"' % (self.table, self.table.alias)
                 + columns + values + returning)
 
     @property
     def params(self):
         p = []
@@ -798,27 +796,28 @@
             assert isinstance(value, (Expression, And, Or))
         self._where = value
 
     def __str__(self):
         assert all(col.table == self.table for col in self.columns)
         # Get columns without alias
         columns = [c.column_name for c in self.columns]
-        returning = ''
-        if self.returning:
-            returning = ' RETURNING ' + ', '.join(
-                map(self._format, self.returning))
+
         with AliasManager():
             from_ = ''
             if self.from_:
                 from_ = ' FROM %s' % str(self.from_)
             values = ', '.join('%s = %s' % (c, self._format(v))
                 for c, v in zip(columns, self.values))
             where = ''
             if self.where:
                 where = ' WHERE ' + str(self.where)
+            returning = ''
+            if self.returning:
+                returning = ' RETURNING ' + ', '.join(
+                    map(self._format, self.returning))
             return (self._with_str()
                 + 'UPDATE %s AS "%s" SET ' % (self.table, self.table.alias)
                 + values + from_ + where + returning)
 
     @property
     def params(self):
         p = []
@@ -879,23 +878,35 @@
 
     @returning.setter
     def returning(self, value):
         if value is not None:
             assert isinstance(value, list)
         self._returning = value
 
+    @staticmethod
+    def _format(value, param=None):
+        if param is None:
+            param = Flavor.get().param
+        if isinstance(value, Expression):
+            return str(value)
+        elif isinstance(value, Select):
+            return '(%s)' % value
+        else:
+            return param
+
     def __str__(self):
         with AliasManager(exclude=[self.table]):
             only = ' ONLY' if self.only else ''
             where = ''
             if self.where:
                 where = ' WHERE ' + str(self.where)
             returning = ''
             if self.returning:
-                returning = ' RETURNING ' + ', '.join(map(str, self.returning))
+                returning = ' RETURNING ' + ', '.join(
+                    map(self._format, self.returning))
             return (self._with_str()
                 + 'DELETE FROM%s %s' % (only, self.table)
                 + where + returning)
 
     @property
     def params(self):
         p = []
```

### Comparing `python-sql-1.4.1/sql/aggregate.py` & `python-sql-1.4.2/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/conditionals.py` & `python-sql-1.4.2/sql/conditionals.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/functions.py` & `python-sql-1.4.2/sql/functions.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/operators.py` & `python-sql-1.4.2/sql/operators.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/__init__.py` & `python-sql-1.4.2/sql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_aggregate.py` & `python-sql-1.4.2/sql/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_alias.py` & `python-sql-1.4.2/sql/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_as.py` & `python-sql-1.4.2/sql/tests/test_as.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_cast.py` & `python-sql-1.4.2/sql/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_collate.py` & `python-sql-1.4.2/sql/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_column.py` & `python-sql-1.4.2/sql/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_combining_query.py` & `python-sql-1.4.2/sql/tests/test_combining_query.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_conditionals.py` & `python-sql-1.4.2/sql/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_delete.py` & `python-sql-1.4.2/sql/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_for.py` & `python-sql-1.4.2/sql/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_functions.py` & `python-sql-1.4.2/sql/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_insert.py` & `python-sql-1.4.2/sql/tests/test_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,25 +45,25 @@
         self.assertEqual(tuple(query.params), (-1,))
 
     def test_insert_returning(self):
         query = self.table.insert([self.table.c1, self.table.c2],
             [['foo', 'bar']], returning=[self.table.c1, self.table.c2])
         self.assertEqual(str(query),
             'INSERT INTO "t" AS "a" ("c1", "c2") VALUES (%s, %s) '
-            'RETURNING "c1", "c2"')
+            'RETURNING "a"."c1", "a"."c2"')
         self.assertEqual(tuple(query.params), ('foo', 'bar'))
 
     def test_insert_returning_select(self):
         t1 = Table('t1')
         t2 = Table('t2')
         query = t1.insert([t1.c], [['foo']],
             returning=[
                 t2.select(t2.c, where=(t2.c1 == t1.c) & (t2.c2 == 'bar'))])
         self.assertEqual(str(query),
-            'INSERT INTO "t1" AS "a" ("c") VALUES (%s) '
+            'INSERT INTO "t1" AS "b" ("c") VALUES (%s) '
             'RETURNING (SELECT "a"."c" FROM "t2" AS "a" '
             'WHERE (("a"."c1" = "b"."c") AND ("a"."c2" = %s)))')
         self.assertEqual(tuple(query.params), ('foo', 'bar'))
 
     def test_with(self):
         t1 = Table('t1')
         w = With(query=t1.select())
@@ -88,15 +88,15 @@
             [t1.c],
             [w.id],
             from_=[w],
             with_=[w])
         self.assertEqual(str(query),
             'WITH "a" AS ('
                 'INSERT INTO "t" AS "b" ("c1") VALUES (%s) '
-                'RETURNING "id") '
+                'RETURNING "b"."id") '
             'UPDATE "t1" AS "c" SET "c" = "a"."id" FROM "a" AS "a"')
         self.assertEqual(tuple(query.params), ('foo',))
 
     def test_schema(self):
         t1 = Table('t1', 'default')
         query = t1.insert([t1.c1], [['foo']])
```

### Comparing `python-sql-1.4.1/sql/tests/test_join.py` & `python-sql-1.4.2/sql/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_lateral.py` & `python-sql-1.4.2/sql/tests/test_lateral.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_literal.py` & `python-sql-1.4.2/sql/tests/test_literal.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_operators.py` & `python-sql-1.4.2/sql/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_order.py` & `python-sql-1.4.2/sql/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_select.py` & `python-sql-1.4.2/sql/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_table.py` & `python-sql-1.4.2/sql/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_update.py` & `python-sql-1.4.2/sql/tests/test_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,25 @@
                 'SELECT "a"."c" FROM "t2" AS "a" WHERE ("a"."i" = "b"."i"))')
             self.assertEqual(query.params, ())
 
     def test_update_returning(self):
         query = self.table.update([self.table.c], ['foo'],
             returning=[self.table.c])
         self.assertEqual(str(query),
-            'UPDATE "t" AS "a" SET "c" = %s RETURNING "c"')
+            'UPDATE "t" AS "a" SET "c" = %s RETURNING "a"."c"')
         self.assertEqual(query.params, ('foo',))
 
     def test_update_returning_select(self):
         t1 = Table('t1')
         t2 = Table('t2')
         query = t1.update([t1.c], ['foo'],
             returning=[
                 t2.select(t2.c, where=(t2.c1 == t1.c) & (t2.c2 == 'bar'))])
         self.assertEqual(str(query),
-            'UPDATE "t1" AS "a" SET "c" = %s '
+            'UPDATE "t1" AS "b" SET "c" = %s '
             'RETURNING (SELECT "a"."c" FROM "t2" AS "a" '
             'WHERE (("a"."c1" = "b"."c") AND ("a"."c2" = %s)))')
         self.assertEqual(query.params, ('foo', 'bar'))
 
     def test_with(self):
         t1 = Table('t1')
         w = With(query=t1.select(t1.c1))
```

### Comparing `python-sql-1.4.1/sql/tests/test_values.py` & `python-sql-1.4.2/sql/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_window.py` & `python-sql-1.4.2/sql/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/sql/tests/test_with.py` & `python-sql-1.4.2/sql/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.1/tox.ini` & `python-sql-1.4.2/tox.ini`

 * *Files identical despite different names*

