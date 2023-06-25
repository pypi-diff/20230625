# Comparing `tmp/RouterExecutor-0.2.0.linux-x86_64.tar.gz` & `tmp/RouterExecutor-1.2.0.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/www/html/Model Package/dist/RouterExecutor-0.2.0.linux-x86_64.tar", last modified: Sun Jun 25 13:27:51 2023, max compression
+gzip compressed data, was "/var/www/html/Model Package/dist/RouterExecutor-1.2.0.linux-x86_64.tar", last modified: Sun Jun 25 13:36:14 2023, max compression
```

## Comparing `RouterExecutor-0.2.0.linux-x86_64.tar` & `RouterExecutor-1.2.0.linux-x86_64.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/bin/
--rwxr-xr-x   0 odai      (1000) odai      (1000)     1032 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/bin/RouterExecutor
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/bin/
+-rwxr-xr-x   0 odai      (1000) odai      (1000)     1032 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/bin/RouterExecutor
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/
 -rw-r--r--   0 odai      (1000) odai      (1000)     1410 2023-06-25 11:56:33.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/__init__.py
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/__pycache__/
--rw-r--r--   0 odai      (1000) odai      (1000)     1619 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/
--rw-r--r--   0 odai      (1000) odai      (1000)      609 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/PKG-INFO
--rw-r--r--   0 odai      (1000) odai      (1000)      275 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/SOURCES.txt
--rw-r--r--   0 odai      (1000) odai      (1000)        1 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/dependency_links.txt
--rw-r--r--   0 odai      (1000) odai      (1000)       74 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/entry_points.txt
--rw-r--r--   0 odai      (1000) odai      (1000)       38 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/requires.txt
--rw-r--r--   0 odai      (1000) odai      (1000)       15 2023-06-25 13:27:51.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/top_level.txt
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/__pycache__/
+-rw-r--r--   0 odai      (1000) odai      (1000)     1619 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 odai      (1000) odai      (1000)        0 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/
+-rw-r--r--   0 odai      (1000) odai      (1000)      609 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/PKG-INFO
+-rw-r--r--   0 odai      (1000) odai      (1000)      275 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/SOURCES.txt
+-rw-r--r--   0 odai      (1000) odai      (1000)        1 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/dependency_links.txt
+-rw-r--r--   0 odai      (1000) odai      (1000)       74 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/entry_points.txt
+-rw-r--r--   0 odai      (1000) odai      (1000)       38 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/requires.txt
+-rw-r--r--   0 odai      (1000) odai      (1000)       15 2023-06-25 13:36:14.000000 ./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/top_level.txt
```

### ./home/odai/anaconda3/envs/connection_channel/bin/RouterExecutor

```diff
@@ -1,14 +1,14 @@
 #!/home/odai/anaconda3/envs/connection_channel/bin/python
-# EASY-INSTALL-ENTRY-SCRIPT: 'RouterExecutor==0.2.0','console_scripts','RouterExecutor'
+# EASY-INSTALL-ENTRY-SCRIPT: 'RouterExecutor==1.2.0','console_scripts','RouterExecutor'
 import re
 import sys
 
 # for compatibility with easy_install; see #2198
-__requires__ = 'RouterExecutor==0.2.0'
+__requires__ = 'RouterExecutor==1.2.0'
 
 try:
     from importlib.metadata import distribution
 except ImportError:
     try:
         from importlib_metadata import distribution
     except ImportError:
@@ -26,8 +26,8 @@
 
 
 globals().setdefault('load_entry_point', importlib_load_entry_point)
 
 
 if __name__ == '__main__':
     sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
-    sys.exit(load_entry_point('RouterExecutor==0.2.0', 'console_scripts', 'RouterExecutor')())
+    sys.exit(load_entry_point('RouterExecutor==1.2.0', 'console_scripts', 'RouterExecutor')())
```

### Comparing `./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-0.2.0-py3.7.egg-info/PKG-INFO` & `./home/odai/anaconda3/envs/connection_channel/lib/python3.7/site-packages/RouterExecutor-1.2.0-py3.7.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RouterExecutor
-Version: 0.2.0
+Version: 1.2.0
 Summary: Route message through Queues
 Home-page: https://github.com/Odai-Atef/RouterExecutor
 Author: Odai
 Author-email: o.3odai@gmail.com
 License: OpenSource
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

