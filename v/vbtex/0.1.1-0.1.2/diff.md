# Comparing `tmp/vbtex-0.1.1.tar.gz` & `tmp/vbtex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.1.tar", max compression
+gzip compressed data, was "vbtex-0.1.2.tar", max compression
```

## Comparing `vbtex-0.1.1.tar` & `vbtex-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.1/README.md
--rw-r--r--   0        0        0      319 2023-06-25 19:01:50.753911 vbtex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.1/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.1/vbtex/__main__.py
--rw-r--r--   0        0        0      712 2023-06-25 19:00:06.814542 vbtex-0.1.1/vbtex/framed.py
--rw-r--r--   0        0        0      248 2023-06-25 08:17:44.971030 vbtex-0.1.1/vbtex/main.py
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 vbtex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.2/README.md
+-rw-r--r--   0        0        0      319 2023-06-25 19:03:20.015611 vbtex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.2/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.2/vbtex/__main__.py
+-rw-r--r--   0        0        0      711 2023-06-25 19:03:12.046558 vbtex-0.1.2/vbtex/framed.py
+-rw-r--r--   0        0        0      248 2023-06-25 08:17:44.971030 vbtex-0.1.2/vbtex/main.py
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 vbtex-0.1.2/PKG-INFO
```

### Comparing `vbtex-0.1.1/vbtex/framed.py` & `vbtex-0.1.2/vbtex/framed.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     nargs=2,
     default=([16, 9]),
     type=click.Tuple([int, int]),
     show_default=True,
     help="aspect ratio of the frame"
 )
 @click.pass_context
-def framed(ctx, inputfile, dpi, framed):
+def framed(ctx, inputfile, dpi, ratio):
     tex = click.edit()
     click.echo(tex)
```

