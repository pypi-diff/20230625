# Comparing `tmp/c-custom-code-checker-1.0.0.tar.gz` & `tmp/c-custom-code-checker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c-custom-code-checker-1.0.0.tar", last modified: Sun Jun 25 18:09:25 2023, max compression
+gzip compressed data, was "c-custom-code-checker-1.0.1.tar", last modified: Sun Jun 25 20:43:42 2023, max compression
```

## Comparing `c-custom-code-checker-1.0.0.tar` & `c-custom-code-checker-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.484277 c-custom-code-checker-1.0.0/
--rw-rw-rw-   0        0        0      205 2023-06-25 18:09:25.483287 c-custom-code-checker-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4371 2023-06-25 16:35:13.000000 c-custom-code-checker-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.359281 c-custom-code-checker-1.0.0/c_custom_code_checker/
--rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.382282 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/
--rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/__init__.py
--rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/criterion_keys.py
--rw-rw-rw-   0        0        0      767 2023-06-24 23:57:10.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/rules_reserved_keys.py
--rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/strings.py
--rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/constants/target_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.388284 c-custom-code-checker-1.0.0/c_custom_code_checker/enums/
--rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/enums/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/enums/criterion_enum.py
--rw-rw-rw-   0        0        0     1728 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/enums/target_enum.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.456285 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/
--rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
--rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
--rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/invalid_criterion_exception.py
--rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/invalid_target_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
--rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/exceptions/rule_missing_target_exception.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.461284 c-custom-code-checker-1.0.0/c_custom_code_checker/handlers/
--rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/handlers/__init__.py
--rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/handlers/criterion_handlers.py
--rw-rw-rw-   0        0        0     3721 2023-06-25 18:09:20.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.468276 c-custom-code-checker-1.0.0/c_custom_code_checker/models/
--rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/models/__init__.py
--rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/models/rule_model.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.474276 c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/
--rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-06-25 18:05:46.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/code_parser.py
--rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/rule_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.481279 c-custom-code-checker-1.0.0/c_custom_code_checker/utlis/
--rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/utlis/__init__.py
--rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/utlis/console_utils.py
--rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c-custom-code-checker-1.0.0/c_custom_code_checker/utlis/files_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:09:25.371282 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/
--rw-rw-rw-   0        0        0      205 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1673 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-25 18:09:25.000000 c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 18:09:25.484277 c-custom-code-checker-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      387 2023-06-25 16:44:28.000000 c-custom-code-checker-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.675145 c-custom-code-checker-1.0.1/
+-rw-rw-rw-   0        0        0      205 2023-06-25 20:43:42.675145 c-custom-code-checker-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4577 2023-06-25 20:41:57.000000 c-custom-code-checker-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.417142 c-custom-code-checker-1.0.1/c_custom_code_checker/
+-rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.483304 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/
+-rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/criterion_keys.py
+-rw-rw-rw-   0        0        0      767 2023-06-24 23:57:10.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/rules_reserved_keys.py
+-rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/strings.py
+-rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/constants/target_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.543145 c-custom-code-checker-1.0.1/c_custom_code_checker/enums/
+-rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/enums/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/enums/criterion_enum.py
+-rw-rw-rw-   0        0        0     1728 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/enums/target_enum.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.636155 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/
+-rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
+-rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
+-rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/invalid_criterion_exception.py
+-rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/invalid_target_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
+-rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/exceptions/rule_missing_target_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.640148 c-custom-code-checker-1.0.1/c_custom_code_checker/handlers/
+-rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/handlers/criterion_handlers.py
+-rw-rw-rw-   0        0        0     3721 2023-06-25 18:09:20.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/main.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.645150 c-custom-code-checker-1.0.1/c_custom_code_checker/models/
+-rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/models/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/models/rule_model.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.658203 c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/
+-rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/__init__.py
+-rw-rw-rw-   0        0        0     4044 2023-06-25 18:05:46.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/code_parser.py
+-rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/rule_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.673151 c-custom-code-checker-1.0.1/c_custom_code_checker/utlis/
+-rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/utlis/__init__.py
+-rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/utlis/console_utils.py
+-rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c-custom-code-checker-1.0.1/c_custom_code_checker/utlis/files_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:43:42.456144 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1688 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-25 20:43:42.000000 c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-06-25 20:42:27.000000 c-custom-code-checker-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 20:43:42.676150 c-custom-code-checker-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-06-25 20:39:07.000000 c-custom-code-checker-1.0.1/setup.py
```

### Comparing `c-custom-code-checker-1.0.0/README.md` & `c-custom-code-checker-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,37 @@
 - [Installation](#installation)
 - [Usage](#usage)
 - [How it works](#how-it-works)
 - [Contributing](#contributing)
 
 ## Installation
 
+### Requirements
+
+#### Clang
+
 This project use [libclang](https://github.com/llvm/llvm-project/releases/) tools to handle with C files and to create the AST. You need to install it, and set libclang installation path on PATH environment variable 
 
 
 ### Installing required python modules
 
 ```bash
 pip install -r requirements.txt
+
+```
+
+### Installing by pip
+
+This project is available on pip repository, you just have to write the follow command
+
 ```
+    pip install c-custom-code-checker
+
+```
+
 
 ## Usage
 
 A typical use of this tool is shown below.
 
 ```
      c-validator --input {files or directory to check} -r {folder where rules are declared}
```

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/constants/rules_reserved_keys.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/constants/rules_reserved_keys.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/enums/criterion_enum.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/enums/criterion_enum.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/enums/target_enum.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/enums/target_enum.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/handlers/criterion_handlers.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/handlers/criterion_handlers.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/main.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/main.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/models/rule_model.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/models/rule_model.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/code_parser.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/code_parser.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/parsers/rule_parser.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/parsers/rule_parser.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker/utlis/console_utils.py` & `c-custom-code-checker-1.0.1/c_custom_code_checker/utlis/console_utils.py`

 * *Files identical despite different names*

### Comparing `c-custom-code-checker-1.0.0/c_custom_code_checker.egg-info/SOURCES.txt` & `c-custom-code-checker-1.0.1/c_custom_code_checker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+pyproject.toml
 setup.py
 c_custom_code_checker/__init__.py
 c_custom_code_checker/main.py
 c_custom_code_checker.egg-info/PKG-INFO
 c_custom_code_checker.egg-info/SOURCES.txt
 c_custom_code_checker.egg-info/dependency_links.txt
 c_custom_code_checker.egg-info/entry_points.txt
```

