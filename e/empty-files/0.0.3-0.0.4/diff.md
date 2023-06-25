# Comparing `tmp/empty-files-0.0.3.tar.gz` & `tmp/empty-files-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empty-files-0.0.3.tar", last modified: Sun Oct 31 17:24:17 2021, max compression
+gzip compressed data, was "empty-files-0.0.4.tar", last modified: Sun Jun 25 18:25:22 2023, max compression
```

## Comparing `empty-files-0.0.3.tar` & `empty-files-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 17:24:17.222044 empty-files-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    10273 2021-10-31 17:24:04.000000 empty-files-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-31 17:24:04.000000 empty-files-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-10-31 17:24:17.222044 empty-files-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-10-31 17:24:04.000000 empty-files-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 17:24:17.218043 empty-files-0.0.3/empty_files/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-31 17:24:04.000000 empty-files-0.0.3/empty_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-10-31 17:24:04.000000 empty-files-0.0.3/empty_files/empty_files.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-10-31 17:24:04.000000 empty-files-0.0.3/empty_files/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 17:24:17.222044 empty-files-0.0.3/empty_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-10-31 17:24:16.000000 empty-files-0.0.3/empty_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-10-31 17:24:17.000000 empty-files-0.0.3/empty_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-31 17:24:16.000000 empty-files-0.0.3/empty_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-31 17:24:16.000000 empty-files-0.0.3/empty_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-31 17:24:16.000000 empty-files-0.0.3/empty_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-31 17:24:17.222044 empty-files-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2021-10-31 17:24:04.000000 empty-files-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-25 18:25:08.000000 empty-files-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:08.000000 empty-files-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 18:25:22.122274 empty-files-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-25 18:25:08.000000 empty-files-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/empty_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/empty_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/empty_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 18:25:22.122274 empty-files-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 18:25:08.000000 empty-files-0.0.4/setup.py
```

### Comparing `empty-files-0.0.3/LICENSE` & `empty-files-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `empty-files-0.0.3/PKG-INFO` & `empty-files-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: empty-files
-Version: 0.0.3
+Version: 0.0.4
 Summary: Serves empty files of many types
 Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.1
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EmptyFiles.Python
 
 [![PyPI version](https://img.shields.io/pypi/v/empty-files.svg)](https://pypi.org/project/empty-files)
+[![Test](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml)
 
 **TL;DR** Null Object pattern for files. 
 
 <!-- toc -->
 ## Contents
 
   * [Setup](#setup)
@@ -81,9 +81,7 @@
 name_length = 0
 if (person.last_name())
  name_length = len(person.last_name()) 
 ```
 
 ## Attributions
 The empty files are taken from [Simon Cropp's Empty Files](https://github.com/VerifyTests/EmptyFiles/tree/main/index).
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: empty-files Version: 0.0.3 Summary: Serves empty
+Metadata-Version: 2.1 Name: empty-files Version: 0.0.4 Summary: Serves empty
 files of many types Home-page: https://github.com/approvals/EmptyFiles.Python
-Author: empty_files Contributors License: UNKNOWN Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: POSIX Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Utilities Requires-Python:
->=3.6.1 Description-Content-Type: text/markdown License-File: LICENSE #
-EmptyFiles.Python [![PyPI version](https://img.shields.io/pypi/v/empty-
-files.svg)](https://pypi.org/project/empty-files) **TL;DR** Null Object pattern
-for files.  ## Contents * [Setup](#setup) * [Usage](#usage) * [Null Object
-Pattern](#null-object-pattern) * [Attributions](#attributions) This project
-will create an empty file of a type requested. If possible, that file will be
-the smallest valid file for that type. For example, an empty jpg will be a 1x1
-pixel jpg. ## Setup From [pypi](https://pypi.org/project/empty-files/): pip
-install empty-files ## Usage This code:   ```py from empty_files.empty_files
-import create_empty_file create_empty_file("temp/empty.jpg") ``` snippet_source
-| anchor  will create the following [image](tests/
-test_empty_files.test_sample.approved.jpg) ## Null Object Pattern **Issue:**
-null/None causes extra checks in order to avoid errors. **Solution:** return an
-empty version of the object, so methods can be used normally. **Example:** if
-`last_name` returns `""` instead of `None`, we can write: ```python name_length
-= len(person.last_name()) ``` instead of : ```python name_length = 0 if
-(person.last_name()) name_length = len(person.last_name()) ``` ## Attributions
-The empty files are taken from [Simon Cropp's Empty Files](https://github.com/
-VerifyTests/EmptyFiles/tree/main/index).
+Author: empty_files Contributors Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: POSIX Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+:: MacOS X Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Utilities
+Requires-Python: >=3.7.1 Description-Content-Type: text/markdown License-File:
+LICENSE # EmptyFiles.Python [![PyPI version](https://img.shields.io/pypi/v/
+empty-files.svg)](https://pypi.org/project/empty-files) [![Test](https://
+github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)]
+(https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml)
+**TL;DR** Null Object pattern for files.  ## Contents * [Setup](#setup) *
+[Usage](#usage) * [Null Object Pattern](#null-object-pattern) * [Attributions]
+(#attributions) This project will create an empty file of a type requested. If
+possible, that file will be the smallest valid file for that type. For example,
+an empty jpg will be a 1x1 pixel jpg. ## Setup From [pypi](https://pypi.org/
+project/empty-files/): pip install empty-files ## Usage This code:   ```py from
+empty_files.empty_files import create_empty_file create_empty_file("temp/
+empty.jpg") ``` snippet_source | anchor  will create the following [image]
+(tests/test_empty_files.test_sample.approved.jpg) ## Null Object Pattern
+**Issue:** null/None causes extra checks in order to avoid errors. **Solution:
+** return an empty version of the object, so methods can be used normally.
+**Example:** if `last_name` returns `""` instead of `None`, we can write:
+```python name_length = len(person.last_name()) ``` instead of : ```python
+name_length = 0 if (person.last_name()) name_length = len(person.last_name())
+``` ## Attributions The empty files are taken from [Simon Cropp's Empty Files]
+(https://github.com/VerifyTests/EmptyFiles/tree/main/index).
```

### Comparing `empty-files-0.0.3/README.md` & `empty-files-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # EmptyFiles.Python
 
 [![PyPI version](https://img.shields.io/pypi/v/empty-files.svg)](https://pypi.org/project/empty-files)
+[![Test](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml)
 
 **TL;DR** Null Object pattern for files. 
 
 <!-- toc -->
 ## Contents
 
   * [Setup](#setup)
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
 # EmptyFiles.Python [![PyPI version](https://img.shields.io/pypi/v/empty-
-files.svg)](https://pypi.org/project/empty-files) **TL;DR** Null Object pattern
-for files.  ## Contents * [Setup](#setup) * [Usage](#usage) * [Null Object
-Pattern](#null-object-pattern) * [Attributions](#attributions) This project
-will create an empty file of a type requested. If possible, that file will be
-the smallest valid file for that type. For example, an empty jpg will be a 1x1
-pixel jpg. ## Setup From [pypi](https://pypi.org/project/empty-files/): pip
-install empty-files ## Usage This code:   ```py from empty_files.empty_files
-import create_empty_file create_empty_file("temp/empty.jpg") ``` snippet_source
-| anchor  will create the following [image](tests/
-test_empty_files.test_sample.approved.jpg) ## Null Object Pattern **Issue:**
-null/None causes extra checks in order to avoid errors. **Solution:** return an
-empty version of the object, so methods can be used normally. **Example:** if
-`last_name` returns `""` instead of `None`, we can write: ```python name_length
-= len(person.last_name()) ``` instead of : ```python name_length = 0 if
-(person.last_name()) name_length = len(person.last_name()) ``` ## Attributions
-The empty files are taken from [Simon Cropp's Empty Files](https://github.com/
-VerifyTests/EmptyFiles/tree/main/index).
+files.svg)](https://pypi.org/project/empty-files) [![Test](https://github.com/
+approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)](https://
+github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml) **TL;DR**
+Null Object pattern for files.  ## Contents * [Setup](#setup) * [Usage](#usage)
+* [Null Object Pattern](#null-object-pattern) * [Attributions](#attributions)
+This project will create an empty file of a type requested. If possible, that
+file will be the smallest valid file for that type. For example, an empty jpg
+will be a 1x1 pixel jpg. ## Setup From [pypi](https://pypi.org/project/empty-
+files/): pip install empty-files ## Usage This code:   ```py from
+empty_files.empty_files import create_empty_file create_empty_file("temp/
+empty.jpg") ``` snippet_source | anchor  will create the following [image]
+(tests/test_empty_files.test_sample.approved.jpg) ## Null Object Pattern
+**Issue:** null/None causes extra checks in order to avoid errors. **Solution:
+** return an empty version of the object, so methods can be used normally.
+**Example:** if `last_name` returns `""` instead of `None`, we can write:
+```python name_length = len(person.last_name()) ``` instead of : ```python
+name_length = 0 if (person.last_name()) name_length = len(person.last_name())
+``` ## Attributions The empty files are taken from [Simon Cropp's Empty Files]
+(https://github.com/VerifyTests/EmptyFiles/tree/main/index).
```

### Comparing `empty-files-0.0.3/empty_files/empty_files.py` & `empty-files-0.0.4/empty_files/empty_files.py`

 * *Files identical despite different names*

### Comparing `empty-files-0.0.3/empty_files.egg-info/PKG-INFO` & `empty-files-0.0.4/empty_files.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: empty-files
-Version: 0.0.3
+Version: 0.0.4
 Summary: Serves empty files of many types
 Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.1
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EmptyFiles.Python
 
 [![PyPI version](https://img.shields.io/pypi/v/empty-files.svg)](https://pypi.org/project/empty-files)
+[![Test](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)](https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml)
 
 **TL;DR** Null Object pattern for files. 
 
 <!-- toc -->
 ## Contents
 
   * [Setup](#setup)
@@ -81,9 +81,7 @@
 name_length = 0
 if (person.last_name())
  name_length = len(person.last_name()) 
 ```
 
 ## Attributions
 The empty files are taken from [Simon Cropp's Empty Files](https://github.com/VerifyTests/EmptyFiles/tree/main/index).
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: empty-files Version: 0.0.3 Summary: Serves empty
+Metadata-Version: 2.1 Name: empty-files Version: 0.0.4 Summary: Serves empty
 files of many types Home-page: https://github.com/approvals/EmptyFiles.Python
-Author: empty_files Contributors License: UNKNOWN Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: POSIX Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Utilities Requires-Python:
->=3.6.1 Description-Content-Type: text/markdown License-File: LICENSE #
-EmptyFiles.Python [![PyPI version](https://img.shields.io/pypi/v/empty-
-files.svg)](https://pypi.org/project/empty-files) **TL;DR** Null Object pattern
-for files.  ## Contents * [Setup](#setup) * [Usage](#usage) * [Null Object
-Pattern](#null-object-pattern) * [Attributions](#attributions) This project
-will create an empty file of a type requested. If possible, that file will be
-the smallest valid file for that type. For example, an empty jpg will be a 1x1
-pixel jpg. ## Setup From [pypi](https://pypi.org/project/empty-files/): pip
-install empty-files ## Usage This code:   ```py from empty_files.empty_files
-import create_empty_file create_empty_file("temp/empty.jpg") ``` snippet_source
-| anchor  will create the following [image](tests/
-test_empty_files.test_sample.approved.jpg) ## Null Object Pattern **Issue:**
-null/None causes extra checks in order to avoid errors. **Solution:** return an
-empty version of the object, so methods can be used normally. **Example:** if
-`last_name` returns `""` instead of `None`, we can write: ```python name_length
-= len(person.last_name()) ``` instead of : ```python name_length = 0 if
-(person.last_name()) name_length = len(person.last_name()) ``` ## Attributions
-The empty files are taken from [Simon Cropp's Empty Files](https://github.com/
-VerifyTests/EmptyFiles/tree/main/index).
+Author: empty_files Contributors Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: POSIX Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+:: MacOS X Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Utilities
+Requires-Python: >=3.7.1 Description-Content-Type: text/markdown License-File:
+LICENSE # EmptyFiles.Python [![PyPI version](https://img.shields.io/pypi/v/
+empty-files.svg)](https://pypi.org/project/empty-files) [![Test](https://
+github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml/badge.svg)]
+(https://github.com/approvals/EmptyFiles.Python/actions/workflows/test.yml)
+**TL;DR** Null Object pattern for files.  ## Contents * [Setup](#setup) *
+[Usage](#usage) * [Null Object Pattern](#null-object-pattern) * [Attributions]
+(#attributions) This project will create an empty file of a type requested. If
+possible, that file will be the smallest valid file for that type. For example,
+an empty jpg will be a 1x1 pixel jpg. ## Setup From [pypi](https://pypi.org/
+project/empty-files/): pip install empty-files ## Usage This code:   ```py from
+empty_files.empty_files import create_empty_file create_empty_file("temp/
+empty.jpg") ``` snippet_source | anchor  will create the following [image]
+(tests/test_empty_files.test_sample.approved.jpg) ## Null Object Pattern
+**Issue:** null/None causes extra checks in order to avoid errors. **Solution:
+** return an empty version of the object, so methods can be used normally.
+**Example:** if `last_name` returns `""` instead of `None`, we can write:
+```python name_length = len(person.last_name()) ``` instead of : ```python
+name_length = 0 if (person.last_name()) name_length = len(person.last_name())
+``` ## Attributions The empty files are taken from [Simon Cropp's Empty Files]
+(https://github.com/VerifyTests/EmptyFiles/tree/main/index).
```

### Comparing `empty-files-0.0.3/setup.py` & `empty-files-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 setup(
     name="empty-files",
     version=VERSION,
     description="Serves empty files of many types",
     author="empty_files Contributors",
     url="https://github.com/approvals/EmptyFiles.Python",
-    python_requires=">=3.6.1",
+    python_requires=">=3.7.1",
     install_requires=["requests"],
     packages=find_packages(exclude=["tests*"]),
     long_description=(HERE / "README.md").read_text(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
 )
```

