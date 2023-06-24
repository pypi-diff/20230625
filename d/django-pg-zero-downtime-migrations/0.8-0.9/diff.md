# Comparing `tmp/django-pg-zero-downtime-migrations-0.8.tar.gz` & `tmp/django-pg-zero-downtime-migrations-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-pg-zero-downtime-migrations-0.8.tar", last modified: Wed Dec 11 07:14:24 2019, max compression
+gzip compressed data, was "dist/django-pg-zero-downtime-migrations-0.9.tar", last modified: Tue Jul 28 18:13:06 2020, max compression
```

## Comparing `django-pg-zero-downtime-migrations-0.8.tar` & `django-pg-zero-downtime-migrations-0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       56 2019-09-25 19:22:59.000000 django-pg-zero-downtime-migrations-0.8/AUTHORS
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     3412 2019-12-11 07:12:19.000000 django-pg-zero-downtime-migrations-0.8/CHANGES.md
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1073 2019-08-24 13:26:50.000000 django-pg-zero-downtime-migrations-0.8/LICENSE
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      121 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/MANIFEST.in
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    34699 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/PKG-INFO
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    27126 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.8/README.md
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    34699 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/PKG-INFO
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1020 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        1 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       12 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/requires.txt
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       32 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/top_level.txt
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       20 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/__init__.py
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/__init__.py
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgis/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgis/__init__.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      242 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgis/base.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      269 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgis/schema.py
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgres/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgres/__init__.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      235 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgres/base.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    27466 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgres/schema.py
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/__init__.py
-drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/commands/
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/commands/__init__.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     6683 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/commands/migrate_isnotnull_check_constraints.py
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      508 2019-12-11 07:14:24.000000 django-pg-zero-downtime-migrations-0.8/setup.cfg
--rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1781 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.8/setup.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       56 2019-09-25 19:22:59.000000 django-pg-zero-downtime-migrations-0.9/AUTHORS
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     3507 2020-07-28 18:12:35.000000 django-pg-zero-downtime-migrations-0.9/CHANGES.md
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1073 2019-08-24 13:26:50.000000 django-pg-zero-downtime-migrations-0.9/LICENSE
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      121 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/MANIFEST.in
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    34865 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/PKG-INFO
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    27126 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.9/README.md
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    34865 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1020 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        1 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       12 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/requires.txt
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       32 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/top_level.txt
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)       20 2020-07-28 18:12:35.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/__init__.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/__init__.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgis/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgis/__init__.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      242 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgis/base.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      269 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgis/schema.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgres/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgres/__init__.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      235 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgres/base.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)    27483 2020-07-28 18:01:42.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgres/schema.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/__init__.py
+drwxrwxr-x   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/commands/
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)        0 2019-09-24 23:43:17.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/commands/__init__.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     6683 2019-12-11 07:10:59.000000 django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/commands/migrate_isnotnull_check_constraints.py
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)      508 2020-07-28 18:13:06.000000 django-pg-zero-downtime-migrations-0.9/setup.cfg
+-rw-rw-r--   0 pavel.tysliatski  (5969) pavel.tysliatski  (1001)     1819 2019-12-11 07:20:42.000000 django-pg-zero-downtime-migrations-0.9/setup.py
```

### Comparing `django-pg-zero-downtime-migrations-0.8/CHANGES.md` & `django-pg-zero-downtime-migrations-0.9/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # django-pg-zero-downtime-migrations changelog
 
+## 0.9
+  - fixed decimal to float migration error
+  - fixed django 3.0.2+ tests
+
 ## 0.8
-- added django 3.0 support
-- added concurrently index creation and removal operations
-- added exclude constraint support as unsafe operation
-- drop postgres 9.4 support
-- drop django 2.0 support
-- drop django 2.1 support
-- drop deprecated `django_zero_downtime_migrations_postgres_backend` module
+  - added django 3.0 support
+  - added concurrently index creation and removal operations
+  - added exclude constraint support as unsafe operation
+  - drop postgres 9.4 support
+  - drop django 2.0 support
+  - drop django 2.1 support
+  - drop deprecated `django_zero_downtime_migrations_postgres_backend` module
 
 ## 0.7
   - added python 3.8 support
   - added postgres specific indexes support
   - improved tests clearness
   - fixed regexp escaping warning for management command
   - fixed style check
```

### Comparing `django-pg-zero-downtime-migrations-0.8/LICENSE` & `django-pg-zero-downtime-migrations-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pg-zero-downtime-migrations-0.8/PKG-INFO` & `django-pg-zero-downtime-migrations-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pg-zero-downtime-migrations
-Version: 0.8
+Version: 0.9
 Summary: Django postgresql backend that apply migrations with respect to database locks
 Home-page: https://github.com/tbicr/django-pg-zero-downtime-migrations
 Author: Paveł Tyślacki
 Author-email: pavel.tyslacki@gmail.com
 License: MIT
 Description: [![PyPI](https://img.shields.io/pypi/v/django-pg-zero-downtime-migrations.svg)](https://pypi.org/project/django-pg-zero-downtime-migrations/)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-pg-zero-downtime-migrations.svg)
@@ -55,23 +55,23 @@
         There ara main rules for zero downtime deployment:
         1. We have one database;
         1. We have several instances with application - application always should be available, even you restart one of instances;
         1. We have balancer before instances;
         1. Our application works fine before, on and after migration - old application works fine with old and new database schema version;
         1. Our application works fine before, on and after instance updating - old and new application versions work fine with new database schema version.
         
-        ![deployment timeline](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/timeline.png "deployment timeline")
+        ![deployment timeline](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/timeline.png "deployment timeline")
         
         Flow:
         1. apply migrations
         1. disconnect instance form balancer, restart it and back to balancer - repeat this operation one by one for all instances
         
         If our deployment don't satisfy zero downtime deployment rules, then we split it to smaller deployments.
         
-        ![deployment flow](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/deployment.gif "deployment flow")
+        ![deployment flow](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/deployment.gif "deployment flow")
         
         ### Settings
         
         #### ZERO_DOWNTIME_MIGRATIONS_LOCK_TIMEOUT
         
         Apply [`lock_timeout`](https://www.postgresql.org/docs/current/static/runtime-config-client.html#GUC-LOCK-TIMEOUT) for SQL statements that require `ACCESS EXCLUSIVE` lock, default `None`:
         
@@ -179,15 +179,15 @@
         
         Main point there is if you have two transactions that update one row, then second transaction will wait until first will be completed. So for business logic and data migrations better to avoid updates for whole table and use batch operations instead.
         
         > *NOTE:* batch operations also can work faster because postgres can use more optimal execution plan with indexes for small data range.
         
         ### Transactions FIFO waiting
         
-        ![postgres FIFO](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/fifo-diagram.png "postgres FIFO")
+        ![postgres FIFO](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/fifo-diagram.png "postgres FIFO")
         
         Found same diagram in interesting article http://pankrat.github.io/2015/django-migrations-without-downtimes/.
         
         In this diagram we can extract several metrics:
         
         1. operation time - time what you spend for schema change, so there is issue for long running operation on many rows tables like `CREATE INDEX` or `ALTER TABLE ADD COLUMN SET DEFAULT`, so you need use more save equivalents instead.
         2. waiting time - your migration will wait until all transactions will be completed, so there is issue for long running operations/transactions like analytic, so you need avoid it or disable on migration time.
@@ -307,22 +307,26 @@
         3. `numeric(LESS, SAME)` to `numeric(MORE, SAME)` where LESS < MORE and SAME == SAME
         
         For other operations propose to create new column and copy data to it. Eg. some types can be also safe, but you should check yourself.
         
         
         # django-pg-zero-downtime-migrations changelog
         
+        ## 0.9
+          - fixed decimal to float migration error
+          - fixed django 3.0.2+ tests
+        
         ## 0.8
-        - added django 3.0 support
-        - added concurrently index creation and removal operations
-        - added exclude constraint support as unsafe operation
-        - drop postgres 9.4 support
-        - drop django 2.0 support
-        - drop django 2.1 support
-        - drop deprecated `django_zero_downtime_migrations_postgres_backend` module
+          - added django 3.0 support
+          - added concurrently index creation and removal operations
+          - added exclude constraint support as unsafe operation
+          - drop postgres 9.4 support
+          - drop django 2.0 support
+          - drop django 2.1 support
+          - drop deprecated `django_zero_downtime_migrations_postgres_backend` module
         
         ## 0.7
           - added python 3.8 support
           - added postgres specific indexes support
           - improved tests clearness
           - fixed regexp escaping warning for management command
           - fixed style check
@@ -387,9 +391,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `django-pg-zero-downtime-migrations-0.8/README.md` & `django-pg-zero-downtime-migrations-0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/PKG-INFO` & `django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pg-zero-downtime-migrations
-Version: 0.8
+Version: 0.9
 Summary: Django postgresql backend that apply migrations with respect to database locks
 Home-page: https://github.com/tbicr/django-pg-zero-downtime-migrations
 Author: Paveł Tyślacki
 Author-email: pavel.tyslacki@gmail.com
 License: MIT
 Description: [![PyPI](https://img.shields.io/pypi/v/django-pg-zero-downtime-migrations.svg)](https://pypi.org/project/django-pg-zero-downtime-migrations/)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-pg-zero-downtime-migrations.svg)
@@ -55,23 +55,23 @@
         There ara main rules for zero downtime deployment:
         1. We have one database;
         1. We have several instances with application - application always should be available, even you restart one of instances;
         1. We have balancer before instances;
         1. Our application works fine before, on and after migration - old application works fine with old and new database schema version;
         1. Our application works fine before, on and after instance updating - old and new application versions work fine with new database schema version.
         
-        ![deployment timeline](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/timeline.png "deployment timeline")
+        ![deployment timeline](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/timeline.png "deployment timeline")
         
         Flow:
         1. apply migrations
         1. disconnect instance form balancer, restart it and back to balancer - repeat this operation one by one for all instances
         
         If our deployment don't satisfy zero downtime deployment rules, then we split it to smaller deployments.
         
-        ![deployment flow](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/deployment.gif "deployment flow")
+        ![deployment flow](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/deployment.gif "deployment flow")
         
         ### Settings
         
         #### ZERO_DOWNTIME_MIGRATIONS_LOCK_TIMEOUT
         
         Apply [`lock_timeout`](https://www.postgresql.org/docs/current/static/runtime-config-client.html#GUC-LOCK-TIMEOUT) for SQL statements that require `ACCESS EXCLUSIVE` lock, default `None`:
         
@@ -179,15 +179,15 @@
         
         Main point there is if you have two transactions that update one row, then second transaction will wait until first will be completed. So for business logic and data migrations better to avoid updates for whole table and use batch operations instead.
         
         > *NOTE:* batch operations also can work faster because postgres can use more optimal execution plan with indexes for small data range.
         
         ### Transactions FIFO waiting
         
-        ![postgres FIFO](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.8/images/fifo-diagram.png "postgres FIFO")
+        ![postgres FIFO](https://raw.githubusercontent.com/tbicr/django-pg-zero-downtime-migrations/0.9/images/fifo-diagram.png "postgres FIFO")
         
         Found same diagram in interesting article http://pankrat.github.io/2015/django-migrations-without-downtimes/.
         
         In this diagram we can extract several metrics:
         
         1. operation time - time what you spend for schema change, so there is issue for long running operation on many rows tables like `CREATE INDEX` or `ALTER TABLE ADD COLUMN SET DEFAULT`, so you need use more save equivalents instead.
         2. waiting time - your migration will wait until all transactions will be completed, so there is issue for long running operations/transactions like analytic, so you need avoid it or disable on migration time.
@@ -307,22 +307,26 @@
         3. `numeric(LESS, SAME)` to `numeric(MORE, SAME)` where LESS < MORE and SAME == SAME
         
         For other operations propose to create new column and copy data to it. Eg. some types can be also safe, but you should check yourself.
         
         
         # django-pg-zero-downtime-migrations changelog
         
+        ## 0.9
+          - fixed decimal to float migration error
+          - fixed django 3.0.2+ tests
+        
         ## 0.8
-        - added django 3.0 support
-        - added concurrently index creation and removal operations
-        - added exclude constraint support as unsafe operation
-        - drop postgres 9.4 support
-        - drop django 2.0 support
-        - drop django 2.1 support
-        - drop deprecated `django_zero_downtime_migrations_postgres_backend` module
+          - added django 3.0 support
+          - added concurrently index creation and removal operations
+          - added exclude constraint support as unsafe operation
+          - drop postgres 9.4 support
+          - drop django 2.0 support
+          - drop django 2.1 support
+          - drop deprecated `django_zero_downtime_migrations_postgres_backend` module
         
         ## 0.7
           - added python 3.8 support
           - added postgres specific indexes support
           - improved tests clearness
           - fixed regexp escaping warning for management command
           - fixed style check
@@ -387,9 +391,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `django-pg-zero-downtime-migrations-0.8/django_pg_zero_downtime_migrations.egg-info/SOURCES.txt` & `django-pg-zero-downtime-migrations-0.9/django_pg_zero_downtime_migrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/backends/postgres/schema.py` & `django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/backends/postgres/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,20 +577,20 @@
                 else:
                     return False
         old_type_numeric_match = self._numeric_type_regexp.match(old_type)
         if old_type_numeric_match:
             new_type_numeric_match = self._numeric_type_regexp.match(new_type)
             old_type_precision = int(old_type_numeric_match.group("precision"))
             old_type_scale = int(old_type_numeric_match.group("scale"))
-            new_type_precision = int(new_type_numeric_match.group("precision"))
-            new_type_scale = int(new_type_numeric_match.group("scale"))
-            if new_type_precision >= old_type_precision and new_type_scale == old_type_scale:
-                return True
-            else:
+            try:
+                new_type_precision = int(new_type_numeric_match.group("precision"))
+                new_type_scale = int(new_type_numeric_match.group("scale"))
+            except AttributeError:
                 return False
+            return new_type_precision >= old_type_precision and new_type_scale == old_type_scale
         return False
 
     def _alter_column_type_sql(self, model, old_field, new_field, new_type):
         old_db_params = old_field.db_parameters(connection=self.connection)
         old_type = old_db_params["type"]
         if not self._immediate_type_cast(old_type, new_type):
             if self.RAISE_FOR_UNSAFE:
```

### Comparing `django-pg-zero-downtime-migrations-0.8/django_zero_downtime_migrations/management/commands/migrate_isnotnull_check_constraints.py` & `django-pg-zero-downtime-migrations-0.9/django_zero_downtime_migrations/management/commands/migrate_isnotnull_check_constraints.py`

 * *Files identical despite different names*

### Comparing `django-pg-zero-downtime-migrations-0.8/setup.py` & `django-pg-zero-downtime-migrations-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.0',
     ],
     keywords='django postgres postgresql migrations',
     packages=find_packages(exclude=['manage*', 'tests*']),
     python_requires='>=3.5',
     install_requires=[
         'django>=2.2',
     ]
```

