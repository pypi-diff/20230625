# Comparing `tmp/mareep-0.0.1.tar.gz` & `tmp/mareep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mareep-0.0.1.tar", last modified: Sun Jun 25 10:14:07 2023, max compression
+gzip compressed data, was "mareep-0.0.2.tar", last modified: Sun Jun 25 13:11:55 2023, max compression
```

## Comparing `mareep-0.0.1.tar` & `mareep-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.743499 mareep-0.0.1/
--rw-r--r--   0 datnh      (501) staff       (20)      510 2023-06-25 10:14:07.743298 mareep-0.0.1/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.1/README.md
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.736346 mareep-0.0.1/mareep/
--rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.1/mareep/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.1/mareep/__main__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2380 2023-06-25 08:08:40.000000 mareep-0.0.1/mareep/app.py
--rw-r--r--   0 datnh      (501) staff       (20)     1523 2023-06-25 10:04:13.000000 mareep-0.0.1/mareep/function.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.739338 mareep-0.0.1/mareep/loaders/
--rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.1/mareep/loaders/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.740513 mareep-0.0.1/mareep/loaders/json_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.1/mareep/loaders/json_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.1/mareep/loaders/json_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.1/mareep/loaders/loader.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.742376 mareep-0.0.1/mareep/loaders/yaml_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.1/mareep/loaders/yaml_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.1/mareep/loaders/yaml_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)     2556 2023-06-25 10:04:46.000000 mareep-0.0.1/mareep/renderer.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 10:14:07.738291 mareep-0.0.1/mareep.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)      510 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      494 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)       48 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/entry_points.txt
--rw-r--r--   0 datnh      (501) staff       (20)       55 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/requires.txt
--rw-r--r--   0 datnh      (501) staff       (20)        7 2023-06-25 10:14:07.000000 mareep-0.0.1/mareep.egg-info/top_level.txt
--rw-r--r--   0 datnh      (501) staff       (20)       38 2023-06-25 10:14:07.743546 mareep-0.0.1/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-06-25 08:27:30.000000 mareep-0.0.1/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.911548 mareep-0.0.2/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-25 13:11:55.911398 mareep-0.0.2/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.2/README.md
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.906562 mareep-0.0.2/mareep/
+-rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.2/mareep/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.2/mareep/__main__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2380 2023-06-25 08:08:40.000000 mareep-0.0.2/mareep/app.py
+-rw-r--r--   0 datnh      (501) staff       (20)     1523 2023-06-25 10:04:13.000000 mareep-0.0.2/mareep/function.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.909714 mareep-0.0.2/mareep/loaders/
+-rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.2/mareep/loaders/__init__.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.910326 mareep-0.0.2/mareep/loaders/json_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.2/mareep/loaders/json_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.2/mareep/loaders/json_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.2/mareep/loaders/loader.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.910974 mareep-0.0.2/mareep/loaders/yaml_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.2/mareep/loaders/yaml_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.2/mareep/loaders/yaml_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.2/mareep/renderer.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.909227 mareep-0.0.2/mareep.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      494 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       49 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/entry_points.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       55 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/requires.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        7 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/top_level.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-06-25 13:11:55.911595 mareep-0.0.2/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-06-25 13:05:28.000000 mareep-0.0.2/setup.py
```

### Comparing `mareep-0.0.1/mareep/app.py` & `mareep-0.0.2/mareep/app.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.1/mareep/function.py` & `mareep-0.0.2/mareep/function.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.1/mareep/loaders/__init__.py` & `mareep-0.0.2/mareep/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.1/mareep/renderer.py` & `mareep-0.0.2/mareep/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         env.update(kwargs)
 
         with progressbar(template_files) as progress:
             for template_file in progress:
                 with open(template_file) as fin:
                     template: Template = Template(fin.read())
 
-                if template_file.suffix == ".j2":
+                if template_file.suffix[1:] in self.extensions:
                     output_file: Path = self.output_path / template_file.stem
                 else:
                     output_file: Path = self.output_path / template_file.name
 
                 output_file.parent.mkdir(parents=True, exist_ok=True)
 
                 with open(output_file, "w") as fout:
```

### Comparing `mareep-0.0.1/setup.py` & `mareep-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import *
 
 import setuptools
 
 __PACKAGE__ = "mareep"
-__VERSION__ = "0.0.1"
+__VERSION__ = "0.0.2"
 
 base_dir = Path(__file__).resolve().parent
 
 with open(base_dir / "README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

