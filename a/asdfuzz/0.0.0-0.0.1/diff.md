# Comparing `tmp/asdfuzz-0.0.0.tar.gz` & `tmp/asdfuzz-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\git\asdfuzz\dist\.tmp-0r4tao_y\asdfuzz-0.0.0.tar", last modified: Sun Jun 25 18:55:39 2023, max compression
+gzip compressed data, was "C:\git\asdfuzz\dist\.tmp-s2fpf861\asdfuzz-0.0.1.tar", last modified: Sun Jun 25 19:28:49 2023, max compression
```

## Comparing `asdfuzz-0.0.0.tar` & `asdfuzz-0.0.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:39.000000 asdfuzz-0.0.0/
--rw-rw-rw-   0        0        0     1093 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      101 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4063 2023-06-25 18:55:39.000000 asdfuzz-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3559 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/README.md
--rw-rw-rw-   0        0        0      108 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      678 2023-06-25 18:55:39.000000 asdfuzz-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz/
--rw-rw-rw-   0        0        0        0 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/__init__.py
--rw-rw-rw-   0        0        0       63 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/__main__.py
--rw-rw-rw-   0        0        0     3002 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/_utils.py
--rw-rw-rw-   0        0        0     9425 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/app.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz/fuzzing/
--rw-rw-rw-   0        0        0        0 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/fuzzing/__init__.py
--rw-rw-rw-   0        0        0     4329 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/fuzzing/fuzz_result.py
--rw-rw-rw-   0        0        0    23011 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/fuzzing/fuzzer.py
--rw-rw-rw-   0        0        0     1144 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/fuzzing/hex_replacements.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:39.000000 asdfuzz-0.0.0/src/asdfuzz/http/
--rw-rw-rw-   0        0        0        0 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/__init__.py
--rw-rw-rw-   0        0        0     1283 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/cookie.py
--rw-rw-rw-   0        0        0      122 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/directory.py
--rw-rw-rw-   0        0        0      392 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/form_data.py
--rw-rw-rw-   0        0        0     5980 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/json_data.py
--rw-rw-rw-   0        0        0     1285 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/parameter.py
--rw-rw-rw-   0        0        0    10179 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/request.py
--rw-rw-rw-   0        0        0     2741 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/response.py
--rw-rw-rw-   0        0        0     3495 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/http/url.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:39.000000 asdfuzz-0.0.0/src/asdfuzz/wordlists/
--rw-rw-rw-   0        0        0      762 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/wordlists/default.txt
--rw-rw-rw-   0        0        0      275 2023-06-25 18:52:35.000000 asdfuzz-0.0.0/src/asdfuzz/wordlists/small.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/
--rw-rw-rw-   0        0        0     4063 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 18:55:38.000000 asdfuzz-0.0.0/src/asdfuzz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4068 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       95 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz/
+-rw-rw-rw-   0        0        0        0 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/__main__.py
+-rw-rw-rw-   0        0        0     3002 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/_utils.py
+-rw-rw-rw-   0        0        0     9425 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/app.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/src/asdfuzz/fuzzing/
+-rw-rw-rw-   0        0        0        0 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/fuzzing/__init__.py
+-rw-rw-rw-   0        0        0     4329 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/fuzzing/fuzz_result.py
+-rw-rw-rw-   0        0        0    23011 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/fuzzing/fuzzer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/fuzzing/hex_replacements.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/
+-rw-rw-rw-   0        0        0        0 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/__init__.py
+-rw-rw-rw-   0        0        0     1283 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/cookie.py
+-rw-rw-rw-   0        0        0      122 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/directory.py
+-rw-rw-rw-   0        0        0      392 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/form_data.py
+-rw-rw-rw-   0        0        0     5980 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/json_data.py
+-rw-rw-rw-   0        0        0     1285 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/parameter.py
+-rw-rw-rw-   0        0        0    10179 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/request.py
+-rw-rw-rw-   0        0        0     2741 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/response.py
+-rw-rw-rw-   0        0        0     3495 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/http/url.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:49.000000 asdfuzz-0.0.1/src/asdfuzz/wordlists/
+-rw-rw-rw-   0        0        0        0 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/wordlists/__init__.py
+-rw-rw-rw-   0        0        0      762 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/wordlists/default.txt
+-rw-rw-rw-   0        0        0      275 2023-06-25 19:27:49.000000 asdfuzz-0.0.1/src/asdfuzz/wordlists/small.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/
+-rw-rw-rw-   0        0        0     4068 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 19:28:48.000000 asdfuzz-0.0.1/src/asdfuzz.egg-info/top_level.txt
```

### Comparing `asdfuzz-0.0.0/LICENSE` & `asdfuzz-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/PKG-INFO` & `asdfuzz-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdfuzz
-Version: 0.0.0
+Version: 0.0.1
 Summary: Web application fuzzer that automatically detects and fuzzes data in HTTP requests
 Home-page: https://github.com/spmvg/asdfuzz
 Author: Steven van Gemert
 Author-email: steven@vangemert.dev
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 The starting point of fuzzing can be a raw HTTP request or OWASP ZAP message export.
 Every individual field will be fuzzed in a separate section and the results are shown on screen.
 The performed requests and received responses are stored by default in a folder called `asdfuzz_output/` for later reference.
 To skip a section while the fuzzer is already running, press `[control]`+`[spacebar]`.
 
 Individual fields in JSON data will be fuzzed recursively.
-If base64-urlencoded JSON is present in parameters or cookies, this data will be fuzzed recursively as well.
+If base64-urlencoded JSON data is present in parameters or cookies, this data will be fuzzed recursively as well.
 
 ## Usage
 ```text
 Usage: python -m asdfuzz [OPTIONS]
 
 Options:
   --filename PATH                 File containing a single HTTP request to
```

### Comparing `asdfuzz-0.0.0/README.md` & `asdfuzz-0.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 The starting point of fuzzing can be a raw HTTP request or OWASP ZAP message export.
 Every individual field will be fuzzed in a separate section and the results are shown on screen.
 The performed requests and received responses are stored by default in a folder called `asdfuzz_output/` for later reference.
 To skip a section while the fuzzer is already running, press `[control]`+`[spacebar]`.
 
 Individual fields in JSON data will be fuzzed recursively.
-If base64-urlencoded JSON is present in parameters or cookies, this data will be fuzzed recursively as well.
+If base64-urlencoded JSON data is present in parameters or cookies, this data will be fuzzed recursively as well.
 
 ## Usage
 ```text
 Usage: python -m asdfuzz [OPTIONS]
 
 Options:
   --filename PATH                 File containing a single HTTP request to
```

### Comparing `asdfuzz-0.0.0/setup.cfg` & `asdfuzz-0.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7364 6675 7a7a 0d0a 7665 7273   = asdfuzz..vers
-00000020: 696f 6e20 3d20 302e 302e 300d 0a61 7574  ion = 0.0.0..aut
+00000020: 696f 6e20 3d20 302e 302e 310d 0a61 7574  ion = 0.0.1..aut
 00000030: 686f 7220 3d20 5374 6576 656e 2076 616e  hor = Steven van
 00000040: 2047 656d 6572 740d 0a61 7574 686f 725f   Gemert..author_
 00000050: 656d 6169 6c20 3d20 7374 6576 656e 4076  email = steven@v
 00000060: 616e 6765 6d65 7274 2e64 6576 0d0a 6465  angemert.dev..de
 00000070: 7363 7269 7074 696f 6e20 3d20 5765 6220  scription = Web 
 00000080: 6170 706c 6963 6174 696f 6e20 6675 7a7a  application fuzz
 00000090: 6572 2074 6861 7420 6175 746f 6d61 7469  er that automati
```

### Comparing `asdfuzz-0.0.0/src/asdfuzz/_utils.py` & `asdfuzz-0.0.1/src/asdfuzz/_utils.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/app.py` & `asdfuzz-0.0.1/src/asdfuzz/app.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/fuzzing/fuzz_result.py` & `asdfuzz-0.0.1/src/asdfuzz/fuzzing/fuzz_result.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/fuzzing/fuzzer.py` & `asdfuzz-0.0.1/src/asdfuzz/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/fuzzing/hex_replacements.py` & `asdfuzz-0.0.1/src/asdfuzz/fuzzing/hex_replacements.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/cookie.py` & `asdfuzz-0.0.1/src/asdfuzz/http/cookie.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/json_data.py` & `asdfuzz-0.0.1/src/asdfuzz/http/json_data.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/parameter.py` & `asdfuzz-0.0.1/src/asdfuzz/http/parameter.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/request.py` & `asdfuzz-0.0.1/src/asdfuzz/http/request.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/response.py` & `asdfuzz-0.0.1/src/asdfuzz/http/response.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/http/url.py` & `asdfuzz-0.0.1/src/asdfuzz/http/url.py`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz/wordlists/default.txt` & `asdfuzz-0.0.1/src/asdfuzz/wordlists/default.txt`

 * *Files identical despite different names*

### Comparing `asdfuzz-0.0.0/src/asdfuzz.egg-info/PKG-INFO` & `asdfuzz-0.0.1/src/asdfuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdfuzz
-Version: 0.0.0
+Version: 0.0.1
 Summary: Web application fuzzer that automatically detects and fuzzes data in HTTP requests
 Home-page: https://github.com/spmvg/asdfuzz
 Author: Steven van Gemert
 Author-email: steven@vangemert.dev
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 The starting point of fuzzing can be a raw HTTP request or OWASP ZAP message export.
 Every individual field will be fuzzed in a separate section and the results are shown on screen.
 The performed requests and received responses are stored by default in a folder called `asdfuzz_output/` for later reference.
 To skip a section while the fuzzer is already running, press `[control]`+`[spacebar]`.
 
 Individual fields in JSON data will be fuzzed recursively.
-If base64-urlencoded JSON is present in parameters or cookies, this data will be fuzzed recursively as well.
+If base64-urlencoded JSON data is present in parameters or cookies, this data will be fuzzed recursively as well.
 
 ## Usage
 ```text
 Usage: python -m asdfuzz [OPTIONS]
 
 Options:
   --filename PATH                 File containing a single HTTP request to
```

### Comparing `asdfuzz-0.0.0/src/asdfuzz.egg-info/SOURCES.txt` & `asdfuzz-0.0.1/src/asdfuzz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 src/asdfuzz/http/directory.py
 src/asdfuzz/http/form_data.py
 src/asdfuzz/http/json_data.py
 src/asdfuzz/http/parameter.py
 src/asdfuzz/http/request.py
 src/asdfuzz/http/response.py
 src/asdfuzz/http/url.py
+src/asdfuzz/wordlists/__init__.py
 src/asdfuzz/wordlists/default.txt
 src/asdfuzz/wordlists/small.txt
```

