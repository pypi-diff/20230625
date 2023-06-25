# Comparing `tmp/splunk_kvstore_cli-1.0.0.tar.gz` & `tmp/splunk_kvstore_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunk_kvstore_cli-1.0.0.tar", last modified: Wed Dec 21 22:05:22 2022, max compression
+gzip compressed data, was "splunk_kvstore_cli-1.0.1.tar", last modified: Sun Jun 25 11:19:31 2023, max compression
```

## Comparing `splunk_kvstore_cli-1.0.0.tar` & `splunk_kvstore_cli-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 22:05:22.549744 splunk_kvstore_cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-21 22:05:11.000000 splunk_kvstore_cli-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-21 22:05:22.549744 splunk_kvstore_cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2022-12-21 22:05:11.000000 splunk_kvstore_cli-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-21 22:05:22.549744 splunk_kvstore_cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 22:05:11.000000 splunk_kvstore_cli-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 22:05:22.549744 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-21 22:05:22.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-21 22:05:22.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 22:05:22.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-21 22:05:22.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-21 22:05:22.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2022-12-21 22:05:11.000000 splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:19:31.874992 splunk_kvstore_cli-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 11:19:23.000000 splunk_kvstore_cli-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-25 11:19:31.878991 splunk_kvstore_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-25 11:19:23.000000 splunk_kvstore_cli-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-25 11:19:31.878991 splunk_kvstore_cli-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:19:23.000000 splunk_kvstore_cli-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:19:31.874992 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-25 11:19:31.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-25 11:19:31.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:19:31.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 11:19:31.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 11:19:31.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-25 11:19:23.000000 splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.py
```

### Comparing `splunk_kvstore_cli-1.0.0/LICENSE` & `splunk_kvstore_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splunk_kvstore_cli-1.0.0/PKG-INFO` & `splunk_kvstore_cli-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splunk_kvstore_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Splunk KVStore CLI
 Home-page: https://github.com/artemrys/splunk-kvstore-cli
 Author: Artem Rys
 Author-email: rysartem@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +19,22 @@
 
 This is a small utility that helps to query Splunk KV Store (intended to use with [`jq`](https://stedolan.github.io/jq/)).  
 
 This tool is intended for local development, when developing something for Splunk which interacts with KVStore.
 
 ## Installation
 
-`pip install git+https://github.com/artemrys/splunk-kvstore-cli`
+`pip install splunk-kvstore-cli`
 
 ## Examples
 
 > All the examples below can be suffixed with `| jq .` for better output
 
 All the examples below use default value of `--host` parameter which is `https://localhost:8089`, but you can provide your own.
 
 * `kv get -a addon_name -u user:password` - prints data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -u user:password -m full` - prints **ALL** data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -c collection_name -u user:password` - prints data from the particular collection `collection_name`
+
+### Disclaimer
+
+This is not an official Splunk product.
```

### Comparing `splunk_kvstore_cli-1.0.0/README.md` & `splunk_kvstore_cli-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 This is a small utility that helps to query Splunk KV Store (intended to use with [`jq`](https://stedolan.github.io/jq/)).  
 
 This tool is intended for local development, when developing something for Splunk which interacts with KVStore.
 
 ## Installation
 
-`pip install git+https://github.com/artemrys/splunk-kvstore-cli`
+`pip install splunk-kvstore-cli`
 
 ## Examples
 
 > All the examples below can be suffixed with `| jq .` for better output
 
 All the examples below use default value of `--host` parameter which is `https://localhost:8089`, but you can provide your own.
 
 * `kv get -a addon_name -u user:password` - prints data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -u user:password -m full` - prints **ALL** data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -c collection_name -u user:password` - prints data from the particular collection `collection_name`
+
+### Disclaimer
+
+This is not an official Splunk product.
```

### Comparing `splunk_kvstore_cli-1.0.0/setup.cfg` & `splunk_kvstore_cli-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = splunk_kvstore_cli
-version = 1.0.0
+version = 1.0.1
 description = Splunk KVStore CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/artemrys/splunk-kvstore-cli
 author = Artem Rys
 author_email = rysartem@gmail.com
 license = Apache-2.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.egg-info/PKG-INFO` & `splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splunk-kvstore-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Splunk KVStore CLI
 Home-page: https://github.com/artemrys/splunk-kvstore-cli
 Author: Artem Rys
 Author-email: rysartem@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +19,22 @@
 
 This is a small utility that helps to query Splunk KV Store (intended to use with [`jq`](https://stedolan.github.io/jq/)).  
 
 This tool is intended for local development, when developing something for Splunk which interacts with KVStore.
 
 ## Installation
 
-`pip install git+https://github.com/artemrys/splunk-kvstore-cli`
+`pip install splunk-kvstore-cli`
 
 ## Examples
 
 > All the examples below can be suffixed with `| jq .` for better output
 
 All the examples below use default value of `--host` parameter which is `https://localhost:8089`, but you can provide your own.
 
 * `kv get -a addon_name -u user:password` - prints data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -u user:password -m full` - prints **ALL** data about all the collections associated with the add-on `addon_name`
 * `kv get -a addon_name -c collection_name -u user:password` - prints data from the particular collection `collection_name`
+
+### Disclaimer
+
+This is not an official Splunk product.
```

### Comparing `splunk_kvstore_cli-1.0.0/splunk_kvstore_cli.py` & `splunk_kvstore_cli-1.0.1/splunk_kvstore_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         ),
         context=ctx,
     )
     response_json = json.load(response)
     return json.dumps(response_json, indent=2)
 
 
-def main(argv: Optional[Sequence[str]] = None):
+def main(argv: Optional[Sequence[str]] = None) -> None:
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="command")
     get_parser = subparsers.add_parser("get")
     get_parser.add_argument(
         "-a",
         "--addon",
         required=True,
```

