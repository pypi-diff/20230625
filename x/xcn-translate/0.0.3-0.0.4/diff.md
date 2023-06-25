# Comparing `tmp/xcn_translate-0.0.3.tar.gz` & `tmp/xcn_translate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcn_translate-0.0.3.tar", last modified: Sat Mar 18 07:05:09 2023, max compression
+gzip compressed data, was "xcn_translate-0.0.4.tar", last modified: Sun Jun 25 07:10:47 2023, max compression
```

## Comparing `xcn_translate-0.0.3.tar` & `xcn_translate-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.398499 xcn_translate-0.0.3/
--rw-r--r--   0 sqa        (501) staff       (20)     1074 2023-03-16 04:02:18.000000 xcn_translate-0.0.3/LICENSE
--rw-r--r--   0 sqa        (501) staff       (20)      668 2023-03-18 07:05:09.398610 xcn_translate-0.0.3/PKG-INFO
--rw-r--r--   0 sqa        (501) staff       (20)      171 2023-03-16 04:13:20.000000 xcn_translate-0.0.3/README.md
--rw-r--r--   0 sqa        (501) staff       (20)      104 2023-03-16 04:09:08.000000 xcn_translate-0.0.3/pyproject.toml
--rw-r--r--   0 sqa        (501) staff       (20)      622 2023-03-18 07:05:09.399104 xcn_translate-0.0.3/setup.cfg
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.394326 xcn_translate-0.0.3/src/
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.395958 xcn_translate-0.0.3/src/xcn_translate/
--rw-r--r--   0 sqa        (501) staff       (20)        0 2023-03-16 04:15:27.000000 xcn_translate-0.0.3/src/xcn_translate/__init__.py
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.397766 xcn_translate-0.0.3/src/xcn_translate/conf/
--rw-r--r--   0 sqa        (501) staff       (20)        0 2023-03-18 05:15:02.000000 xcn_translate-0.0.3/src/xcn_translate/conf/__init__.py
--rw-r--r--   0 sqa        (501) staff       (20)     4260 2023-03-18 06:42:00.000000 xcn_translate-0.0.3/src/xcn_translate/conf/ini_file.py
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.398290 xcn_translate-0.0.3/src/xcn_translate/date/
--rw-r--r--   0 sqa        (501) staff       (20)       20 2023-03-16 04:17:12.000000 xcn_translate-0.0.3/src/xcn_translate/date/__init__.py
--rw-r--r--   0 sqa        (501) staff       (20)      760 2023-03-16 06:44:10.000000 xcn_translate-0.0.3/src/xcn_translate/date/str.py
-drwxr-xr-x   0 sqa        (501) staff       (20)        0 2023-03-18 07:05:09.397131 xcn_translate-0.0.3/src/xcn_translate.egg-info/
--rw-r--r--   0 sqa        (501) staff       (20)      668 2023-03-18 07:05:09.000000 xcn_translate-0.0.3/src/xcn_translate.egg-info/PKG-INFO
--rw-r--r--   0 sqa        (501) staff       (20)      371 2023-03-18 07:05:09.000000 xcn_translate-0.0.3/src/xcn_translate.egg-info/SOURCES.txt
--rw-r--r--   0 sqa        (501) staff       (20)        1 2023-03-18 07:05:09.000000 xcn_translate-0.0.3/src/xcn_translate.egg-info/dependency_links.txt
--rw-r--r--   0 sqa        (501) staff       (20)       14 2023-03-18 07:05:09.000000 xcn_translate-0.0.3/src/xcn_translate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.736284 xcn_translate-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      688 2023-06-25 07:10:47.736284 xcn_translate-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/README.md
+-rw-rw-rw-   0        0        0      110 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      651 2023-06-25 07:10:47.736284 xcn_translate-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.716441 xcn_translate-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.723744 xcn_translate-0.0.4/src/xcn_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/src/xcn_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.735280 xcn_translate-0.0.4/src/xcn_translate/conf/
+-rw-rw-rw-   0        0        0        0 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/src/xcn_translate/conf/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-25 06:58:42.000000 xcn_translate-0.0.4/src/xcn_translate/conf/folder.py
+-rw-rw-rw-   0        0        0     4387 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/src/xcn_translate/conf/ini_file.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.736284 xcn_translate-0.0.4/src/xcn_translate/date/
+-rw-rw-rw-   0        0        0       22 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/src/xcn_translate/date/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-06-25 06:14:46.000000 xcn_translate-0.0.4/src/xcn_translate/date/str.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:10:47.732911 xcn_translate-0.0.4/src/xcn_translate.egg-info/
+-rw-rw-rw-   0        0        0      688 2023-06-25 07:10:47.000000 xcn_translate-0.0.4/src/xcn_translate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-06-25 07:10:47.000000 xcn_translate-0.0.4/src/xcn_translate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:10:47.000000 xcn_translate-0.0.4/src/xcn_translate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 07:10:47.000000 xcn_translate-0.0.4/src/xcn_translate.egg-info/top_level.txt
```

### Comparing `xcn_translate-0.0.3/LICENSE` & `xcn_translate-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

