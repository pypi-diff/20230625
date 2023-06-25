# Comparing `tmp/miley-0.1.1.tar.gz` & `tmp/miley-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miley-0.1.1.tar", max compression
+gzip compressed data, was "miley-0.1.2.tar", max compression
```

## Comparing `miley-0.1.1.tar` & `miley-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-0.1.1/LICENSE
--rw-r--r--   0        0        0       12 2023-06-25 18:10:39.386980 miley-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-0.1.1/miley/__init__.py
--rw-r--r--   0        0        0       65 2023-06-25 18:24:54.654208 miley-0.1.1/miley/client.py
--rwxr-xr-x   0        0        0      140 2023-06-25 18:36:41.645209 miley-0.1.1/miley/main.py
--rw-r--r--   0        0        0      391 2023-06-25 18:36:55.401352 miley-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 miley-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-0.1.2/LICENSE
+-rw-r--r--   0        0        0       12 2023-06-25 18:10:39.386980 miley-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-0.1.2/miley/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-25 18:24:54.654208 miley-0.1.2/miley/client.py
+-rwxr-xr-x   0        0        0      155 2023-06-25 18:46:54.312903 miley-0.1.2/miley/main.py
+-rw-r--r--   0        0        0      391 2023-06-25 18:47:29.856962 miley-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 miley-0.1.2/PKG-INFO
```

### Comparing `miley-0.1.1/LICENSE` & `miley-0.1.2/LICENSE`

 * *Files identical despite different names*

