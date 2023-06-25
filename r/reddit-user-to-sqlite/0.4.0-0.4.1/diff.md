# Comparing `tmp/reddit_user_to_sqlite-0.4.0.tar.gz` & `tmp/reddit_user_to_sqlite-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_user_to_sqlite-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reddit_user_to_sqlite-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reddit_user_to_sqlite-0.4.0.tar` & `reddit_user_to_sqlite-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit_user_to_sqlite-0.4.0/LICENSE
--rw-r--r--   0        0        0     7209 2023-06-15 05:47:17.749668 reddit_user_to_sqlite-0.4.0/README.md
--rw-r--r--   0        0        0     1365 2023-06-15 05:47:08.122458 reddit_user_to_sqlite-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/__init__.py
--rw-r--r--   0        0        0     5914 2023-06-15 05:43:06.259931 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/cli.py
--rw-r--r--   0        0        0     1727 2023-06-15 05:44:28.477049 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/csv_helpers.py
--rw-r--r--   0        0        0     1110 2023-06-15 05:44:28.477262 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/helpers.py
--rw-r--r--   0        0        0     4760 2023-06-15 05:44:28.477491 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/reddit_api.py
--rw-r--r--   0        0        0     6222 2023-06-15 05:44:28.477747 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/sqlite_helpers.py
--rw-r--r--   0        0        0     8587 1970-01-01 00:00:00.000000 reddit_user_to_sqlite-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit_user_to_sqlite-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7209 2023-06-15 05:47:17.749668 reddit_user_to_sqlite-0.4.1/README.md
+-rw-r--r--   0        0        0     1397 2023-06-25 19:00:21.510210 reddit_user_to_sqlite-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     5914 2023-06-19 00:28:14.225335 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/cli.py
+-rw-r--r--   0        0        0     1759 2023-06-25 18:59:52.228184 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/csv_helpers.py
+-rw-r--r--   0        0        0     1110 2023-06-15 05:44:28.477262 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/helpers.py
+-rw-r--r--   0        0        0     4760 2023-06-15 05:44:28.477491 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/reddit_api.py
+-rw-r--r--   0        0        0     6222 2023-06-15 05:44:28.477747 reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/sqlite_helpers.py
+-rw-r--r--   0        0        0     8587 1970-01-01 00:00:00.000000 reddit_user_to_sqlite-0.4.1/PKG-INFO
```

### Comparing `reddit_user_to_sqlite-0.4.0/LICENSE` & `reddit_user_to_sqlite-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/README.md` & `reddit_user_to_sqlite-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/pyproject.toml` & `reddit_user_to_sqlite-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reddit-user-to-sqlite"
-version = "0.4.0"
+version = "0.4.1"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Create a SQLite database containing data pulled from Reddit about a single user."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.9"
@@ -41,7 +41,10 @@
 
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 # needed so the LSP performs typechecking
 [tool.pyright]
+
+[tool.isort]
+profile = "black"
```

### Comparing `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/cli.py` & `reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/csv_helpers.py` & `reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/csv_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     item_type: ItemType,
     prefix: Optional[PrefixType] = None,
 ) -> list[str]:
     filename = build_table_name(item_type, prefix)
     # we save each file into a matching table
     saved_ids = {row["id"] for row in db[filename].rows}
 
-    with open(validate_and_build_path(archive_path, filename)) as archive_rows:
+    with open(
+        validate_and_build_path(archive_path, filename), encoding="utf-8"
+    ) as archive_rows:
         return [
             f'{FULLNAME_PREFIX[item_type]}_{c["id"]}'
             for c in DictReader(archive_rows)
             if c["id"] not in saved_ids
         ]
```

### Comparing `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/helpers.py` & `reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/helpers.py`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/reddit_api.py` & `reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/reddit_api.py`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/sqlite_helpers.py` & `reddit_user_to_sqlite-0.4.1/reddit_user_to_sqlite/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.4.0/PKG-INFO` & `reddit_user_to_sqlite-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-user-to-sqlite
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create a SQLite database containing data pulled from Reddit about a single user.
 Keywords: sqlite,reddit,dogsheep
 Author-email: David Brownman <beamneocube@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

