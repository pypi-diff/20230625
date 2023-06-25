# Comparing `tmp/miao-make-20230622.tar.gz` & `tmp/miao-make-20230624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miao-make-20230622.tar", last modified: Wed Jun 21 23:20:07 2023, max compression
+gzip compressed data, was "miao-make-20230624.tar", last modified: Sun Jun 25 02:25:46 2023, max compression
```

## Comparing `miao-make-20230622.tar` & `miao-make-20230624.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-21 23:20:07.673445 miao-make-20230622/
--rw-r--r--   0 4nji       (501) staff       (20)     2613 2023-06-21 23:20:07.672776 miao-make-20230622/PKG-INFO
--rw-r--r--   0 4nji       (501) staff       (20)     2173 2023-06-21 22:28:54.000000 miao-make-20230622/README.md
--rw-r--r--   0 4nji       (501) staff       (20)      665 2023-06-21 23:18:11.000000 miao-make-20230622/pyproject.toml
--rw-r--r--   0 4nji       (501) staff       (20)       38 2023-06-21 23:20:07.673856 miao-make-20230622/setup.cfg
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-21 23:20:07.668493 miao-make-20230622/src/
--rwxr-xr-x   0 4nji       (501) staff       (20)     9271 2023-06-21 22:35:24.000000 miao-make-20230622/src/miao.py
-drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-21 23:20:07.672169 miao-make-20230622/src/miao_make.egg-info/
--rw-r--r--   0 4nji       (501) staff       (20)     2613 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/PKG-INFO
--rw-r--r--   0 4nji       (501) staff       (20)      260 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/SOURCES.txt
--rw-r--r--   0 4nji       (501) staff       (20)        1 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/dependency_links.txt
--rw-r--r--   0 4nji       (501) staff       (20)       35 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/entry_points.txt
--rw-r--r--   0 4nji       (501) staff       (20)       21 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/requires.txt
--rw-r--r--   0 4nji       (501) staff       (20)        5 2023-06-21 23:20:07.000000 miao-make-20230622/src/miao_make.egg-info/top_level.txt
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 02:25:46.667581 miao-make-20230624/
+-rw-r--r--   0 4nji       (501) staff       (20)     4635 2023-06-25 02:25:46.666987 miao-make-20230624/PKG-INFO
+-rw-r--r--   0 4nji       (501) staff       (20)     4195 2023-06-24 11:10:52.000000 miao-make-20230624/README.md
+-rw-r--r--   0 4nji       (501) staff       (20)      695 2023-06-25 02:25:33.000000 miao-make-20230624/pyproject.toml
+-rw-r--r--   0 4nji       (501) staff       (20)       38 2023-06-25 02:25:46.667748 miao-make-20230624/setup.cfg
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 02:25:46.662407 miao-make-20230624/src/
+-rwxr-xr-x   0 4nji       (501) staff       (20)    14934 2023-06-24 10:55:49.000000 miao-make-20230624/src/miao.py
+drwxr-xr-x   0 4nji       (501) staff       (20)        0 2023-06-25 02:25:46.666234 miao-make-20230624/src/miao_make.egg-info/
+-rw-r--r--   0 4nji       (501) staff       (20)     4635 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/PKG-INFO
+-rw-r--r--   0 4nji       (501) staff       (20)      260 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/SOURCES.txt
+-rw-r--r--   0 4nji       (501) staff       (20)        1 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/dependency_links.txt
+-rw-r--r--   0 4nji       (501) staff       (20)       35 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/entry_points.txt
+-rw-r--r--   0 4nji       (501) staff       (20)       21 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/requires.txt
+-rw-r--r--   0 4nji       (501) staff       (20)       16 2023-06-25 02:25:46.000000 miao-make-20230624/src/miao_make.egg-info/top_level.txt
```

### Comparing `miao-make-20230622/pyproject.toml` & `miao-make-20230624/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools", "wheel", "fire", "jinja2", "colorama"]
 
 [project]
 name = "miao-make"
 authors = [ { name = "Anji Wong", email = "anzhi0708@gmail.com" } ]
 description = "Cargo-like project management tool for working with CMake"
 readme = "README.md"
 dependencies = ["colorama", "fire", "Jinja2"]
@@ -12,14 +12,14 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
-version = { attr = "miao.__version__" }
+version = { attr = "miao.__VERSION__" }
 
 [project.scripts]
 miao = "miao:main"
 
 [project.urls]
 "Homepage" = "https://github.com/anzhi0708/miao"
```

