# Comparing `tmp/flask-migratepg-0.0.1.tar.gz` & `tmp/flask-migratepg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-migratepg-0.0.1.tar", last modified: Sun Jun 25 17:01:35 2023, max compression
+gzip compressed data, was "flask-migratepg-0.0.3.tar", last modified: Sun Jun 25 17:23:11 2023, max compression
```

## Comparing `flask-migratepg-0.0.1.tar` & `flask-migratepg-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:01:35.955215 flask-migratepg-0.0.1/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.1/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:01:35.955215 flask-migratepg-0.0.1/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 16:49:01.000000 flask-migratepg-0.0.1/README.md
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      540 2023-06-25 16:49:04.000000 flask-migratepg-0.0.1/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-25 17:01:35.955215 flask-migratepg-0.0.1/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:01:35.954215 flask-migratepg-0.0.1/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:01:35.954215 flask-migratepg-0.0.1/src/flask_migratepg/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2576 2023-06-25 16:36:49.000000 flask-migratepg-0.0.1/src/flask_migratepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:01:35.955215 flask-migratepg-0.0.1/src/flask_migratepg.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:01:35.000000 flask-migratepg-0.0.1/src/flask_migratepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-25 17:01:35.000000 flask-migratepg-0.0.1/src/flask_migratepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-25 17:01:35.000000 flask-migratepg-0.0.1/src/flask_migratepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-25 17:01:35.000000 flask-migratepg-0.0.1/src/flask_migratepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.3/LICENSE
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 16:49:01.000000 flask-migratepg-0.0.3/README.md
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      540 2023-06-25 17:22:38.000000 flask-migratepg-0.0.3/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.831378 flask-migratepg-0.0.3/src/
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.832378 flask-migratepg-0.0.3/src/flask_migratepg/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2682 2023-06-25 17:21:23.000000 flask-migratepg-0.0.3/src/flask_migratepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/top_level.txt
```

### Comparing `flask-migratepg-0.0.1/LICENSE` & `flask-migratepg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-migratepg-0.0.1/PKG-INFO` & `flask-migratepg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-migratepg
-Version: 0.0.1
+Version: 0.0.3
 Summary: Simple migration command for Flask and Psycopg 3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-migratepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-migratepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask-migratepg-0.0.1/pyproject.toml` & `flask-migratepg-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flask-migratepg"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Damien Bezborodov", email="dbezborodov@gmail.com" },
 ]
 description = "Simple migration command for Flask and Psycopg 3."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flask-migratepg-0.0.1/src/flask_migratepg/__init__.py` & `flask-migratepg-0.0.3/src/flask_migratepg/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,22 +66,23 @@
 
     def init(self, app):
         bp = Blueprint('migrate', __name__)
 
         @bp.cli.command('execute')
         def execute():
             conninfo = current_app.config.get('PSYCOPG_CONNINFO')
+            default_migrations_path = os.path.join(current_app.root_path, 'database/migrations')
+            migrations_path = current_app.config.get('MIGRATIONS_PATH', default_migrations_path)
             with psycopg.connect(conninfo) as conn:
                 init(conn)
 
-                migrations = os.path.join(os.path.dirname(__file__), '../database/migrations/')
-                with os.scandir(migrations) as d:
-                    l = list(d)
-                    l.sort(key = lambda e: e.name)
-                    for e in l:
+                with os.scandir(migrations_path) as d:
+                    ls = list(d)
+                    ls.sort(key = lambda e: e.name)
+                    for e in ls:
                         if not e.is_file():
                             continue
                         if e.name.startswith('.'):
                             continue
                         if e.name.endswith('.sql'):
                             migrate_sql(conn, e)
                         if e.name.endswith('.py'):
```

### Comparing `flask-migratepg-0.0.1/src/flask_migratepg.egg-info/PKG-INFO` & `flask-migratepg-0.0.3/src/flask_migratepg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-migratepg
-Version: 0.0.1
+Version: 0.0.3
 Summary: Simple migration command for Flask and Psycopg 3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-migratepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-migratepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

