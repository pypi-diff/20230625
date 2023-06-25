# Comparing `tmp/meo-0.1.1.tar.gz` & `tmp/meo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.1.tar", last modified: Sat Jun 24 12:07:38 2023, max compression
+gzip compressed data, was "meo-0.1.2.tar", last modified: Sun Jun 25 14:11:38 2023, max compression
```

## Comparing `meo-0.1.1.tar` & `meo-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.089032 meo-0.1.1/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.1/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 12:07:38.089032 meo-0.1.1/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.1/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      125 2023-06-24 12:03:20.000000 meo-0.1.1/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-24 12:05:02.000000 meo-0.1.1/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)     4164 2023-06-24 11:27:45.000000 meo-0.1.1/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)        0 2023-06-24 11:23:59.000000 meo-0.1.1/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.1/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2220 2023-06-24 11:57:52.000000 meo-0.1.1/meo/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)      814 2023-06-24 09:52:08.000000 meo-0.1.1/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.1/meo/screen.py
--rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.1/meo/utils.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      326 2023-06-24 12:07:38.000000 meo-0.1.1/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       11 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-24 12:07:38.089032 meo-0.1.1/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1314 2023-06-24 12:07:31.000000 meo-0.1.1/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/test/
--rw-r--r--   0 meo       (1000) meo       (1000)       56 2023-06-24 10:34:35.000000 meo-0.1.1/test/test-read.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.1/test/test.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.2/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 14:11:38.034730 meo-0.1.2/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.2/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.031396 meo-0.1.2/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      114 2023-06-24 12:18:03.000000 meo-0.1.2/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-25 14:11:34.000000 meo-0.1.2/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)      253 2023-06-24 12:22:10.000000 meo-0.1.2/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      459 2023-06-24 12:43:12.000000 meo-0.1.2/meo/crack/pdf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     4881 2023-06-24 14:53:11.000000 meo-0.1.2/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.2/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2212 2023-06-24 12:29:18.000000 meo-0.1.2/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.2/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.2/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.2/meo/utils.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.031396 meo-0.1.2/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      343 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-25 14:11:37.000000 meo-0.1.2/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-25 14:11:38.034730 meo-0.1.2/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1341 2023-06-25 14:06:12.000000 meo-0.1.2/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 14:11:38.034730 meo-0.1.2/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)      101 2023-06-24 13:02:17.000000 meo-0.1.2/test/test-read.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.2/test/test.py
```

### Comparing `meo-0.1.1/LICENSE` & `meo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.1/PKG-INFO` & `meo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.1
+Version: 0.1.2
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.1/meo/crack/__init__.py` & `meo-0.1.2/meo/crack/zip.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import zipfile
+from pyzipper import ZipFile
 import asyncio
 from tqdm.asyncio import tqdm
 from itertools import permutations
 import multiprocessing
 import itertools
+import gc
+import weakref
+from tqdm import tqdm
 
 PWD_SEED = b"1234567890qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM!@#$%^&*()_+-=[{}]\|;:,<.>/?'\" "
+PWD_SEED_SIMPLE = b'1234567890qwertyuiopasdfghjklzxcvbnm'
 
-def try_open_zip(zfile: zipfile.ZipFile, pwd: bytes):
-    assert isinstance(zfile, zipfile.ZipFile) and isinstance(pwd, bytes)
+def try_open_zip(zfile: ZipFile, pwd: bytes):
+    assert isinstance(zfile, ZipFile) and isinstance(pwd, bytes)
     try:
         mem = zfile.filelist[0].filename
         with zfile.open(mem, pwd=pwd) as f:
             if f.seek(1):
                 return True
     except ValueError as e:
         raise e
     except:
         return False
     
 def guess_number_pwd(path, start=0, end=1e99, step=1):
-    zfile = zipfile.ZipFile(path)
+    zfile = ZipFile(path)
     for number in tqdm(range(start, end, step)):
         pwd = str(number).encode("utf8")
         if try_open_zip(zfile, pwd):
             return pwd
     return None
             
 def key_permution(seed, size):
@@ -43,15 +47,15 @@
         while True:
             n_size += 1
             if n_size <= end:
                 for k in key_permution(seed, n_size):
                     yield k, n_size
 
 async def guess_async(path, min_length=None, max_length=None, seed=PWD_SEED):
-    zfile = zipfile.ZipFile(path)
+    zfile = ZipFile(path)
 
     async def block(pwd):
         if try_open_zip(zfile, pwd):
             return pwd
         return False
     
     with tqdm(key_generator(min_length, max_length, seed=seed)) as bar:
@@ -63,46 +67,64 @@
 def guess_pwd_normal(path, min_length=None, max_length=None, seed=PWD_SEED):
     loop = asyncio.get_event_loop()
     future = asyncio.ensure_future(guess_async(path, min_length, max_length, seed))
     loop.run_until_complete(future)
     pwd = future.result()
     return pwd
 
-def __guess_step(path, pwds: list[tuple[bytes, int]]):
-    zfile = zipfile.ZipFile(path)
-    for pwd, _ in pwds:
+def __guess_step(path, *pwds: bytes):
+    zfile = ZipFile(path)
+    for pwd in pwds:
         if try_open_zip(zfile, pwd):
             return pwd
+    del pwds
     return False
 
-def guess_in_multiprocess(path, min_length=None, max_length=None, n_processes=8, slice_size=500, seed=PWD_SEED):
+def guess_in_multiprocess(path, min_length=None, max_length=None, n_processes=8, slice_size=500, seed=PWD_SEED, progressbar=False):
     pool = multiprocessing.Pool(n_processes)
     it = key_generator(min_length, max_length, seed=seed)
     manager = multiprocessing.Manager()
     info = manager.dict()
     info['key'] = None
+    if progressbar:
+        bar = tqdm(mininterval=0.25)
     def cb(re):
+        if progressbar:
+            bar.update(slice_size)
         if re:
             info['key'] = re
             pool.terminate()
+    char_size_display = 0
     while True:
         for _ in range(n_processes):
             try:
                 pwds = itertools.islice(it, 0, slice_size)
-                pool.apply_async(__guess_step, (path, list(pwds)), callback=cb, error_callback=print)
+                pwds, char_sizes = list(zip(*pwds))
+                char_size = char_sizes[-1]
+                pool.apply_async(__guess_step, (path, *pwds), callback=cb, error_callback=print)
+                del pwds
+                del char_sizes
             except StopIteration:
                 pool.terminate()
                 return None
             except Exception as e:
                 if e.args[0] == 'Pool not running':
                     return info['key']
                 else:
                     raise e
+        if progressbar:
+            if char_size_display != char_size:
+                char_size_display = char_size
+                bar.reset()
+            bar.set_postfix({
+                "char": char_size_display
+            }, refresh=False)
+        gc.collect()
 
-class ZipPasswordGuesser:
+class ZipCracker:
 
     def __init__(self, path, seed=PWD_SEED) -> None:
         assert isinstance(seed, bytes)
         self.seed = seed
         self.path = path
 
     def only_number(self):
@@ -110,21 +132,15 @@
     
     async def by_seed_async(self, min_length=None, max_length=None):
         return await guess_async(self.path, min_length, max_length, seed=self.seed)
     
     def by_seed(self, min_length=None, max_length=None):
         return guess_pwd_normal(self.path, min_length, max_length, seed=self.seed)
     
-    def by_seed_mp(self, min_length=None, max_length=None, n_processes=8, slice_size=500):
-        return guess_in_multiprocess(self.path, min_length, max_length, n_processes, slice_size, seed=self.seed)
-
-
-class Crack:
-    @staticmethod
-    def zip(path: str, seed=PWD_SEED):
-        return ZipPasswordGuesser(path, seed)
-    
+    def by_seed_mp(self, min_length=None, max_length=None, n_processes=8, slice_size=500, progressbar=False):
+        return guess_in_multiprocess(self.path, min_length, max_length, n_processes, slice_size, seed=self.seed, progressbar=progressbar)
 
 if __name__ == '__main__':
-    zg = Crack.zip("./examples/flag.zip")
-    k = zg.by_seed_mp()
-    print(k)
+    zguess = ZipCracker("./examples/data/flag.zip", seed=PWD_SEED_SIMPLE)
+    # zguess = ZipCracker("./test/flag.zip", seed=PWD_SEED_SIMPLE)
+    pwd = zguess.by_seed_mp(n_processes=13, slice_size=1000, progressbar=True)
+    print(pwd)
```

### Comparing `meo-0.1.1/meo/flask.py` & `meo-0.1.2/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.1/meo/io.py` & `meo-0.1.2/meo/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 import os
 
 def checkout_dir(dir_path):
     """Create if the folder does not exist"""
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
 
-def __checkout_file_path(path):
+def checkout_file_path(path):
     fdir, _ = os.path.split(path)
     checkout_dir(fdir)
 
 def to_json5(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
     if auto_mkdirs:
-        __checkout_file_path(path)
+        checkout_file_path(path)
     with open(path, 'w+', encoding=encoding) as _f:
         json5.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
 
 def load_json5(path: str):
     with open(path, 'rb') as _f:
         return json5.load(_f)
 
 def to_json(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
     """ Serialize obj as a JSON formatted stream to ```path```` """
     if auto_mkdirs:
-        __checkout_file_path(path)
+        checkout_file_path(path)
     with open(path, 'w+', encoding=encoding) as _f:
         json.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
 
 def load_json(path: str):
     """ load json file from ```path``` """
     with open(path, 'rb') as _f:
         return json.load(_f)
 
 def to_file(path, data, mode='w+', encoding=..., auto_mkdirs=True):
     """write file and auto create dir not existed """
     if auto_mkdirs:
-        __checkout_file_path(path)
+        checkout_file_path(path)
     if 'b' in mode:
         if encoding is ...:
             encoding = None
     elif encoding is ...:
         encoding = 'utf8'
     with open(path, mode, encoding=encoding) as _f:
         return _f.write(data)
```

### Comparing `meo-0.1.1/meo/screen.py` & `meo-0.1.2/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.1/meo.egg-info/PKG-INFO` & `meo-0.1.2/meo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.1
+Version: 0.1.2
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.1/setup.py` & `meo-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,10 +34,11 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'json5>=0.9'
+        'json5>=0.9',
+        'pyzipper>=0.3.6'
     ],
 )
```

