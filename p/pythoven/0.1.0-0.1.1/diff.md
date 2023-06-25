# Comparing `tmp/pythoven-0.1.0.tar.gz` & `tmp/pythoven-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoven-0.1.0.tar", max compression
+gzip compressed data, was "pythoven-0.1.1.tar", max compression
```

## Comparing `pythoven-0.1.0.tar` & `pythoven-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-25 14:38:28.663095 pythoven-0.1.0/README.md
--rw-r--r--   0        0        0      294 2023-06-25 14:40:19.144240 pythoven-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-25 14:40:06.550854 pythoven-0.1.0/pythoven/__init__.py
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 pythoven-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 14:38:28.663095 pythoven-0.1.1/README.md
+-rw-r--r--   0        0        0      285 2023-06-25 14:42:23.435114 pythoven-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-25 14:40:06.550854 pythoven-0.1.1/pythoven/__init__.py
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 pythoven-0.1.1/PKG-INFO
```

