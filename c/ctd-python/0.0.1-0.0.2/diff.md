# Comparing `tmp/ctd-python-0.0.1.tar.gz` & `tmp/ctd-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.0.1.tar", last modified: Sun Jun 25 20:30:40 2023, max compression
+gzip compressed data, was "ctd-python-0.0.2.tar", last modified: Sun Jun 25 20:47:45 2023, max compression
```

## Comparing `ctd-python-0.0.1.tar` & `ctd-python-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:30:40.823404 ctd-python-0.0.1/
--rw-r--r--   0 john       (501) staff       (20)      194 2023-06-25 20:30:40.822774 ctd-python-0.0.1/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      133 2023-06-25 20:13:57.000000 ctd-python-0.0.1/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:30:40.817220 ctd-python-0.0.1/ctd/
--rw-r--r--   0 john       (501) staff       (20)     2119 2023-06-25 20:26:06.000000 ctd-python-0.0.1/ctd/__init__.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:30:40.821831 ctd-python-0.0.1/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)      194 2023-06-25 20:30:40.000000 ctd-python-0.0.1/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 20:30:40.000000 ctd-python-0.0.1/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 20:30:40.000000 ctd-python-0.0.1/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 20:30:40.000000 ctd-python-0.0.1/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 20:30:40.000000 ctd-python-0.0.1/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 20:30:40.823579 ctd-python-0.0.1/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      210 2023-06-25 20:30:35.000000 ctd-python-0.0.1/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:47:45.851178 ctd-python-0.0.2/
+-rw-r--r--   0 john       (501) staff       (20)     1064 2023-06-25 20:47:45.850045 ctd-python-0.0.2/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      618 2023-06-25 20:47:22.000000 ctd-python-0.0.2/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:47:45.843692 ctd-python-0.0.2/ctd/
+-rw-r--r--   0 john       (501) staff       (20)     2119 2023-06-25 20:26:06.000000 ctd-python-0.0.2/ctd/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 20:47:45.848955 ctd-python-0.0.2/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1064 2023-06-25 20:47:45.000000 ctd-python-0.0.2/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 20:47:45.000000 ctd-python-0.0.2/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 20:47:45.000000 ctd-python-0.0.2/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 20:47:45.000000 ctd-python-0.0.2/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 20:47:45.000000 ctd-python-0.0.2/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 20:47:45.851333 ctd-python-0.0.2/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      436 2023-06-25 20:47:39.000000 ctd-python-0.0.2/setup.py
```

### Comparing `ctd-python-0.0.1/ctd/__init__.py` & `ctd-python-0.0.2/ctd/__init__.py`

 * *Files identical despite different names*

