# Comparing `tmp/heaven-0.0.8.tar.gz` & `tmp/heaven-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.8.tar", max compression
+gzip compressed data, was "heaven-0.0.9.tar", max compression
```

## Comparing `heaven-0.0.8.tar` & `heaven-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.8/LICENSE
--rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.8/README.md
--rw-r--r--   0        0        0      216 2023-06-25 10:39:22.426019 heaven-0.0.8/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.8/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.8/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.8/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.8/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.8/heaven/mocks.py
--rw-r--r--   0        0        0     3693 2023-06-25 10:38:41.771932 heaven-0.0.8/heaven/request.py
--rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.8/heaven/response.py
--rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.8/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.8/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.8/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.8/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-25 10:39:09.312702 heaven-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.9/README.md
+-rw-r--r--   0        0        0      216 2023-06-25 10:40:34.424329 heaven-0.0.9/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.9/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.9/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.9/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.9/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.9/heaven/mocks.py
+-rw-r--r--   0        0        0     3734 2023-06-25 10:40:10.409284 heaven-0.0.9/heaven/request.py
+-rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.9/heaven/response.py
+-rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.9/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.9/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.9/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.9/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-25 10:40:43.222347 heaven-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.9/PKG-INFO
```

### Comparing `heaven-0.0.8/LICENSE` & `heaven-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/README.md` & `heaven-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/constants.py` & `heaven-0.0.9/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/form.py` & `heaven-0.0.9/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/mocks.py` & `heaven-0.0.9/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/request.py` & `heaven-0.0.9/heaven/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,17 @@
             csd = {}
             cookiestring = self.headers.get("cookie")
             if not cookiestring:
                 self._cookies = csd
                 return self._cookies
             cookies = cookiestring.split("; ")
             for cookie in cookies:
-                k, v = cookie.split("=")
-                csd[k] = v
+                try: k, v = cookie.split("=")
+                except: pass
+                else: csd[k] = v
             self._cookies = csd
         return self._cookies
 
     @property
     def form(self) -> "Form":
         if not "multipart/form-data" in self.headers.get("content-type"):
             return None  # currently none
```

### Comparing `heaven-0.0.8/heaven/response.py` & `heaven-0.0.9/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/router.py` & `heaven-0.0.9/heaven/router.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/tutorials.py` & `heaven-0.0.9/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/heaven/utils.py` & `heaven-0.0.9/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.8/PKG-INFO` & `heaven-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

