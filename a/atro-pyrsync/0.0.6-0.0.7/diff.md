# Comparing `tmp/atro-pyrsync-0.0.6.tar.gz` & `tmp/atro-pyrsync-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pyrsync-0.0.6.tar", last modified: Sat Jun 24 20:09:43 2023, max compression
+gzip compressed data, was "atro-pyrsync-0.0.7.tar", last modified: Sun Jun 25 09:33:07 2023, max compression
```

## Comparing `atro-pyrsync-0.0.6.tar` & `atro-pyrsync-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 20:09:43.831833 atro-pyrsync-0.0.6/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 20:09:43.831833 atro-pyrsync-0.0.6/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.6/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 20:09:43.831833 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 20:09:43.000000 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      236 2023-06-24 20:09:43.000000 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 20:09:43.000000 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-24 20:09:43.000000 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-24 20:09:43.000000 atro-pyrsync-0.0.6/atro_pyrsync.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 20:09:43.831833 atro-pyrsync-0.0.6/pyrsync/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1379 2023-06-24 20:09:28.000000 atro-pyrsync-0.0.6/pyrsync/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       80 2023-06-24 19:43:49.000000 atro-pyrsync-0.0.6/pyrsync/helpers.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 20:09:43.831833 atro-pyrsync-0.0.6/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-24 20:09:35.000000 atro-pyrsync-0.0.6/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.7/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      236 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-25 09:33:07.000000 atro-pyrsync-0.0.7/atro_pyrsync.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/pyrsync/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1418 2023-06-25 09:32:47.000000 atro-pyrsync-0.0.7/pyrsync/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       72 2023-06-24 20:11:31.000000 atro-pyrsync-0.0.7/pyrsync/helpers.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 09:33:07.773560 atro-pyrsync-0.0.7/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-25 09:32:28.000000 atro-pyrsync-0.0.7/setup.py
```

### Comparing `atro-pyrsync-0.0.6/PKG-INFO` & `atro-pyrsync-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.6/atro_pyrsync.egg-info/PKG-INFO` & `atro-pyrsync-0.0.7/atro_pyrsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.6/pyrsync/__init__.py` & `atro-pyrsync-0.0.7/pyrsync/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import os
 import subprocess
 from pathlib import Path
+
+from pylog import set_logger
+
 from pyrsync.helpers import wrap_in_double_quotes
-from pylog import get_logger
 
 
-def rsync(source: Path, destination: Path, options: list[str] = [], exclusions: list[str] = [], cwd=os.getcwd(), logger=get_logger()):
+def rsync(source: Path, destination: Path, options: list[str] = [], exclusions: list[str] = [], cwd=os.getcwd(), logger=set_logger()):
     log_msg = f"Running rsync from {source.as_posix()} to {destination.as_posix()}"
     if len(options) == 1:
         log_msg += f" with option {options[0]}"
     elif len(options) > 1:
         log_msg += f" with options {', '.join(options)}"
     exclusion_command = []
     if len(exclusions) > 0:
         if len(exclusions) == 1:
             log_msg += f" excluding {exclusions[0]}"
         else:
             log_msg += f" excluding {', '.join(exclusions)}"
-        
+
         exclusion_command = [f'--exclude="{exclusion}"' for exclusion in exclusions]
 
     logger.info(log_msg)
-    command_list = ["rsync", *options, wrap_in_double_quotes(str(source) + "/"), wrap_in_double_quotes(str(destination) + "/"), *exclusion_command, ]
+    command_list = [
+        "rsync",
+        *options,
+        wrap_in_double_quotes(str(source) + "/"),
+        wrap_in_double_quotes(str(destination) + "/"),
+        *exclusion_command,
+    ]
     command = " ".join(command_list)
     logger.info("Command ran: '" + command + "'")
     output = subprocess.run(command, cwd=cwd, shell=True, capture_output=True)
     logger.debug("Rsync output: " + output.stdout.decode())
     if output.stderr:
         logger.error("Rsync error: " + output.stderr.decode())
     if output.returncode != 0:
```

### Comparing `atro-pyrsync-0.0.6/setup.py` & `atro-pyrsync-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pyrsync",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple rsync.wrapper with atro-pylog logging.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

