# Comparing `tmp/vbtex-0.1.0.tar.gz` & `tmp/vbtex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.0.tar", max compression
+gzip compressed data, was "vbtex-0.1.1.tar", max compression
```

## Comparing `vbtex-0.1.0.tar` & `vbtex-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.0/README.md
--rw-r--r--   0        0        0      270 2023-06-21 16:42:53.864324 vbtex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.0/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.0/vbtex/__main__.py
--rw-r--r--   0        0        0      712 2023-06-25 19:00:06.814542 vbtex-0.1.0/vbtex/framed.py
--rw-r--r--   0        0        0      248 2023-06-25 08:17:44.971030 vbtex-0.1.0/vbtex/main.py
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 vbtex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.1/README.md
+-rw-r--r--   0        0        0      319 2023-06-25 19:01:50.753911 vbtex-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.1/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.1/vbtex/__main__.py
+-rw-r--r--   0        0        0      712 2023-06-25 19:00:06.814542 vbtex-0.1.1/vbtex/framed.py
+-rw-r--r--   0        0        0      248 2023-06-25 08:17:44.971030 vbtex-0.1.1/vbtex/main.py
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 vbtex-0.1.1/PKG-INFO
```

### Comparing `vbtex-0.1.0/vbtex/framed.py` & `vbtex-0.1.1/vbtex/framed.py`

 * *Files identical despite different names*

