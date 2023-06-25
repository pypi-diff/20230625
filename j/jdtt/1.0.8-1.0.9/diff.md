# Comparing `tmp/jdtt-1.0.8.tar.gz` & `tmp/jdtt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtt-1.0.8.tar", last modified: Sun Jun 25 20:18:48 2023, max compression
+gzip compressed data, was "jdtt-1.0.9.tar", last modified: Sun Jun 25 21:29:33 2023, max compression
```

## Comparing `jdtt-1.0.8.tar` & `jdtt-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 20:18:48.919533 jdtt-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 20:18:35.000000 jdtt-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 20:18:35.000000 jdtt-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 20:18:48.919533 jdtt-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.915533 jdtt-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/src/jdtt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-25 20:18:35.000000 jdtt-1.0.8/src/jdtt/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:18:48.919533 jdtt-1.0.8/src/jdtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 20:18:48.000000 jdtt-1.0.8/src/jdtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:29:33.937569 jdtt-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 21:29:33.937569 jdtt-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-25 21:29:24.000000 jdtt-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-25 21:29:24.000000 jdtt-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 21:29:33.937569 jdtt-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:29:33.933569 jdtt-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:29:33.933569 jdtt-1.0.9/src/jdtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 21:29:24.000000 jdtt-1.0.9/src/jdtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 21:29:24.000000 jdtt-1.0.9/src/jdtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-25 21:29:24.000000 jdtt-1.0.9/src/jdtt/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:29:33.937569 jdtt-1.0.9/src/jdtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 21:29:33.000000 jdtt-1.0.9/src/jdtt.egg-info/top_level.txt
```

### Comparing `jdtt-1.0.8/PKG-INFO` & `jdtt-1.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a64 7474  : 2.1.Name: jdtt
-00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 380a  .Version: 1.0.8.
+00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 390a  .Version: 1.0.9.
 00000030: 5375 6d6d 6172 793a 204a 534f 4e20 746f  Summary: JSON to
 00000040: 2070 726f 6772 616d 6d69 6e67 206c 616e   programming lan
 00000050: 6775 6167 6520 7363 6865 6d61 2063 6f6e  guage schema con
 00000060: 7665 7274 6572 0a41 7574 686f 723a 204a  verter.Author: J
 00000070: 6f65 7920 5368 690a 506c 6174 666f 726d  oey Shi.Platform
 00000080: 3a20 756e 6978 0a50 6c61 7466 6f72 6d3a  : unix.Platform:
 00000090: 206c 696e 7578 0a50 6c61 7466 6f72 6d3a   linux.Platform:
@@ -31,8 +31,20 @@
 000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 000001f0: 3a20 332e 390a 5265 7175 6972 6573 2d50  : 3.9.Requires-P
 00000200: 7974 686f 6e3a 203e 3d33 2e36 0a44 6573  ython: >=3.6.Des
 00000210: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 00000220: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
 00000230: 646f 776e 0a0a 2320 6a73 6f6e 2d64 6174  down..# json-dat
 00000240: 612d 7479 7065 2d74 7261 6e73 636f 6d70  a-type-transcomp
-00000250: 696c 6572 0a0a                           iler..
+00000250: 696c 6572 0a0a 496e 7465 7270 7265 7473  iler..Interprets
+00000260: 2064 6174 6120 7479 7065 7320 7363 6865   data types sche
+00000270: 6d61 2066 6f72 2070 726f 6772 616d 6d69  ma for programmi
+00000280: 6e67 206c 616e 6775 6167 6573 2066 726f  ng languages fro
+00000290: 6d20 6120 6769 7665 6e20 4a53 4f4e 206f  m a given JSON o
+000002a0: 626a 6563 742e 0a0a 4120 7765 6220 696e  bject...A web in
+000002b0: 7465 7266 6163 6520 666f 7220 7573 696e  terface for usin
+000002c0: 6720 7468 6973 206c 6962 7261 7279 2069  g this library i
+000002d0: 7320 7072 6f76 6964 6564 2061 7420 3c61  s provided at <a
+000002e0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+000002f0: 6576 746f 6f6c 732e 6a6f 6579 7368 692e  evtools.joeyshi.
+00000300: 7879 7a22 3e64 6576 746f 6f6c 732e 6a6f  xyz">devtools.jo
+00000310: 6579 7368 692e 7879 7a3c 2f61 3e0a       eyshi.xyz</a>.
```

### Comparing `jdtt-1.0.8/setup.cfg` & `jdtt-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.8/src/jdtt/__main__.py` & `jdtt-1.0.9/src/jdtt/__main__.py`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.8/src/jdtt/conversion.py` & `jdtt-1.0.9/src/jdtt/conversion.py`

 * *Files identical despite different names*

### Comparing `jdtt-1.0.8/src/jdtt.egg-info/PKG-INFO` & `jdtt-1.0.9/src/jdtt.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a64 7474  : 2.1.Name: jdtt
-00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 380a  .Version: 1.0.8.
+00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 390a  .Version: 1.0.9.
 00000030: 5375 6d6d 6172 793a 204a 534f 4e20 746f  Summary: JSON to
 00000040: 2070 726f 6772 616d 6d69 6e67 206c 616e   programming lan
 00000050: 6775 6167 6520 7363 6865 6d61 2063 6f6e  guage schema con
 00000060: 7665 7274 6572 0a41 7574 686f 723a 204a  verter.Author: J
 00000070: 6f65 7920 5368 690a 506c 6174 666f 726d  oey Shi.Platform
 00000080: 3a20 756e 6978 0a50 6c61 7466 6f72 6d3a  : unix.Platform:
 00000090: 206c 696e 7578 0a50 6c61 7466 6f72 6d3a   linux.Platform:
@@ -31,8 +31,20 @@
 000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 000001f0: 3a20 332e 390a 5265 7175 6972 6573 2d50  : 3.9.Requires-P
 00000200: 7974 686f 6e3a 203e 3d33 2e36 0a44 6573  ython: >=3.6.Des
 00000210: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 00000220: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
 00000230: 646f 776e 0a0a 2320 6a73 6f6e 2d64 6174  down..# json-dat
 00000240: 612d 7479 7065 2d74 7261 6e73 636f 6d70  a-type-transcomp
-00000250: 696c 6572 0a0a                           iler..
+00000250: 696c 6572 0a0a 496e 7465 7270 7265 7473  iler..Interprets
+00000260: 2064 6174 6120 7479 7065 7320 7363 6865   data types sche
+00000270: 6d61 2066 6f72 2070 726f 6772 616d 6d69  ma for programmi
+00000280: 6e67 206c 616e 6775 6167 6573 2066 726f  ng languages fro
+00000290: 6d20 6120 6769 7665 6e20 4a53 4f4e 206f  m a given JSON o
+000002a0: 626a 6563 742e 0a0a 4120 7765 6220 696e  bject...A web in
+000002b0: 7465 7266 6163 6520 666f 7220 7573 696e  terface for usin
+000002c0: 6720 7468 6973 206c 6962 7261 7279 2069  g this library i
+000002d0: 7320 7072 6f76 6964 6564 2061 7420 3c61  s provided at <a
+000002e0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+000002f0: 6576 746f 6f6c 732e 6a6f 6579 7368 692e  evtools.joeyshi.
+00000300: 7879 7a22 3e64 6576 746f 6f6c 732e 6a6f  xyz">devtools.jo
+00000310: 6579 7368 692e 7879 7a3c 2f61 3e0a       eyshi.xyz</a>.
```

