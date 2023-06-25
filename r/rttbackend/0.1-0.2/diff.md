# Comparing `tmp/rttbackend-0.1-py3.8-macosx-13.2-arm64.egg` & `tmp/rttbackend-0.2-py3.8-macosx-13.2-arm64.egg`

## zipinfo {}

```diff
@@ -1,12 +1,34 @@
-Zip file size: 57557 bytes, number of entries: 10
--rw-r--r--  2.0 unx      717 b- defN 23-Jun-25 15:10 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      206 b- defN 23-Jun-25 15:10 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 15:10 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-25 15:10 EGG-INFO/native_libs.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 15:10 EGG-INFO/not-zip-safe
--rw-r--r--  2.0 unx      137 b- defN 23-Jun-25 15:10 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-25 15:10 EGG-INFO/top_level.txt
--rwxr-xr-x  2.0 unx   212535 b- defN 23-Jun-25 15:10 rttbackend/types.cpython-38-darwin.so
--rw-r--r--  2.0 unx      420 b- defN 23-Jun-25 15:10 rttbackend/types.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jun-25 15:10 rttbackend/__pycache__/types.cpython-38.pyc
-10 files, 214636 bytes uncompressed, 56269 bytes compressed:  73.8%
+Zip file size: 81667 bytes, number of entries: 32
+-rw-r--r--  2.0 unx      717 b- defN 23-Jun-25 15:14 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      501 b- defN 23-Jun-25 15:14 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 15:14 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-25 15:14 EGG-INFO/native_libs.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 15:14 EGG-INFO/not-zip-safe
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-25 15:14 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-25 15:14 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-25 15:14 rttbackend/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 23-Jun-23 23:02 rttbackend/config.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Jun-23 23:03 rttbackend/connection.py
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-25 14:42 rttbackend/defines.py
+-rw-r--r--  2.0 unx      718 b- defN 23-Jun-25 12:13 rttbackend/exceptions.py
+-rw-r--r--  2.0 unx     6737 b- defN 23-Jun-25 14:34 rttbackend/exchange.py
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-24 12:56 rttbackend/symbols.py
+-rwxr-xr-x  2.0 unx   212535 b- defN 23-Jun-25 15:14 rttbackend/types.cpython-38-darwin.so
+-rw-r--r--  2.0 unx      420 b- defN 23-Jun-25 15:14 rttbackend/types.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--  2.0 unx     3263 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/config.cpython-38.pyc
+-rw-r--r--  2.0 unx     3342 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/connection.cpython-38.pyc
+-rw-r--r--  2.0 unx      319 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/defines.cpython-38.pyc
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/exceptions.cpython-38.pyc
+-rw-r--r--  2.0 unx     6682 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/exchange.cpython-38.pyc
+-rw-r--r--  2.0 unx     2723 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/symbols.cpython-38.pyc
+-rw-r--r--  2.0 unx      570 b- defN 23-Jun-25 15:14 rttbackend/__pycache__/types.cpython-38.pyc
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-24 13:17 rttbackend/backends/__init__.py
+-rw-r--r--  2.0 unx     3398 b- defN 23-Jun-25 14:44 rttbackend/backends/postgres.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-25 15:14 rttbackend/backends/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--  2.0 unx     5250 b- defN 23-Jun-25 15:14 rttbackend/backends/__pycache__/postgres.cpython-38.pyc
+-rw-r--r--  2.0 unx      334 b- defN 23-Jun-24 12:55 rttbackend/exchanges/__init__.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Jun-25 12:35 rttbackend/exchanges/alphavantage.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-25 15:14 rttbackend/exchanges/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--  2.0 unx     3119 b- defN 23-Jun-25 15:14 rttbackend/exchanges/__pycache__/alphavantage.cpython-38.pyc
+32 files, 262740 bytes uncompressed, 77043 bytes compressed:  70.7%
```

## zipnote «TEMP»/diffoscope_nrbaguw2_/tmppo_v9cet_.zip

```diff
@@ -15,17 +15,83 @@
 
 Filename: EGG-INFO/requires.txt
 Comment: 
 
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
+Filename: rttbackend/__init__.py
+Comment: 
+
+Filename: rttbackend/config.py
+Comment: 
+
+Filename: rttbackend/connection.py
+Comment: 
+
+Filename: rttbackend/defines.py
+Comment: 
+
+Filename: rttbackend/exceptions.py
+Comment: 
+
+Filename: rttbackend/exchange.py
+Comment: 
+
+Filename: rttbackend/symbols.py
+Comment: 
+
 Filename: rttbackend/types.cpython-38-darwin.so
 Comment: 
 
 Filename: rttbackend/types.py
 Comment: 
 
+Filename: rttbackend/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/config.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/connection.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/defines.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/exceptions.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/exchange.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/__pycache__/symbols.cpython-38.pyc
+Comment: 
+
 Filename: rttbackend/__pycache__/types.cpython-38.pyc
 Comment: 
 
+Filename: rttbackend/backends/__init__.py
+Comment: 
+
+Filename: rttbackend/backends/postgres.py
+Comment: 
+
+Filename: rttbackend/backends/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/backends/__pycache__/postgres.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/exchanges/__init__.py
+Comment: 
+
+Filename: rttbackend/exchanges/alphavantage.py
+Comment: 
+
+Filename: rttbackend/exchanges/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: rttbackend/exchanges/__pycache__/alphavantage.cpython-38.pyc
+Comment: 
+
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rttbackend
-Version: 0.1
+Version: 0.2
 Summary: realtimetrade backend service
 Home-page: https://github.com/liej6799/realtimetrade
 Author: Joes Lie
 Author-email: liej6799@protonmail.ch
 License: XFree86
 Description:
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,8 +1,19 @@
 README.md
 setup.py
+rttbackend/__init__.py
+rttbackend/config.py
+rttbackend/connection.py
+rttbackend/defines.py
+rttbackend/exceptions.py
+rttbackend/exchange.py
+rttbackend/symbols.py
 rttbackend/types.c
 rttbackend.egg-info/PKG-INFO
 rttbackend.egg-info/SOURCES.txt
 rttbackend.egg-info/dependency_links.txt
 rttbackend.egg-info/requires.txt
-rttbackend.egg-info/top_level.txt
+rttbackend.egg-info/top_level.txt
+rttbackend/backends/__init__.py
+rttbackend/backends/postgres.py
+rttbackend/exchanges/__init__.py
+rttbackend/exchanges/alphavantage.py
```

## rttbackend/types.cpython-38-darwin.so

### llvm-readobj --symbols {}

```diff
@@ -2319,15 +2319,15 @@
   Symbol {
     Name: /Users/joeslie/Development/realtimetrade/rtt-backend/build/temp.macosx-13.2-arm64-3.8/rttbackend/types.o (13523)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6497E876
+    Value: 0x6497E970
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

### aarch64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit arm64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -10713,15 +10713,15 @@
 00029d80: 405b 0200 0000 0000 5334 0000 0e0c 0000  @[......S4......
 00029d90: 605b 0200 0000 0000 6534 0000 0e0c 0000  `[......e4......
 00029da0: 685b 0200 0000 0000 7634 0000 0e0c 0000  h[......v4......
 00029db0: 705b 0200 0000 0000 0100 0000 6401 0000  p[..........d...
 00029dc0: 0000 0000 0000 0000 8a34 0000 6400 0000  .........4..d...
 00029dd0: 0000 0000 0000 0000 cb34 0000 6400 0000  .........4..d...
 00029de0: 0000 0000 0000 0000 d334 0000 6600 0100  .........4..f...
-00029df0: 76e8 9764 0000 0000 0100 0000 2e01 0000  v..d............
+00029df0: 70e9 9764 0000 0000 0100 0000 2e01 0000  p..d............
 00029e00: a03a 0000 0000 0000 3c35 0000 2401 0000  .:......<5..$...
 00029e10: a03a 0000 0000 0000 0100 0000 2400 0000  .:..........$...
 00029e20: 0c00 0000 0000 0000 0100 0000 4e01 0000  ............N...
 00029e30: a03a 0000 0000 0000 0100 0000 2e01 0000  .:..............
 00029e40: ac3a 0000 0000 0000 4a35 0000 2401 0000  .:......J5..$...
 00029e50: ac3a 0000 0000 0000 0100 0000 2400 0000  .:..........$...
 00029e60: 2803 0000 0000 0000 0100 0000 4e01 0000  (...........N...
@@ -13255,17 +13255,17 @@
 00033c60: 32e1 a395 7a08 86d5 2ca1 5c8a 665e ec68  2...z...,.\.f^.h
 00033c70: 7643 db5a 4710 9ead 7fac b258 6fc6 e966  vC.ZG......Xo..f
 00033c80: c004 d7d1 d16b 024f 5805 ff7c b47c 7a85  .....k.OX..|.|z.
 00033c90: dabd 8b48 892c a7ad 7fac b258 6fc6 e966  ...H.,.....Xo..f
 00033ca0: c004 d7d1 d16b 024f 5805 ff7c b47c 7a85  .....k.OX..|.|z.
 00033cb0: dabd 8b48 892c a707 177f 50f6 6d64 b3bd  ...H.,....P.md..
 00033cc0: a5a1 dcf2 7076 6513 f25f ef44 dbc3 8972  ....pve.._.D...r
-00033cd0: 3a49 13f1 d18f a0e8 96ce 00d3 bea7 7e08  :I............~.
-00033ce0: 369c 4a6f 76c9 c2a0 e2de d87e 5ce9 7999  6.Jov......~\.y.
-00033cf0: b7ea 9559 0fcd 0030 bb4c d1bc 7414 7b20  ...Y...0.L..t.{ 
+00033cd0: 3a49 13f1 d18f a0b2 6b9e de2d be38 c751  :I......k..-.8.Q
+00033ce0: cf29 052e 5491 759d f16e 88e0 7c64 2c2a  .)..T.u..n..|d,*
+00033cf0: 6f56 58b4 e833 3230 bb4c d1bc 7414 7b20  oVX..320.L..t.{ 
 00033d00: 4caf 5477 f388 efda 8bc0 ee9a 64f6 4f1e  L.Tw........d.O.
 00033d10: 94c3 8813 e2fc d928 614f bd9f f3fa 5126  .......(aO....Q&
 00033d20: 6f11 3f7c b87f a688 1251 eff1 5992 642b  o.?|.....Q..Y.d+
 00033d30: 8340 b65e 49d5 c46d 13be 3de2 2f6c 5e69  .@.^I..m..=./l^i
 00033d40: af2e 1b6a a199 89f3 b4dc 0de6 bcd6 46a4  ...j..........F.
 00033d50: e772 c32a 6493 fe83 868f 9e1a 7293 870e  .r.*d.......r...
 00033d60: 2870 78c4 2f96 9fb5 1d3d 8da1 0a62 0a68  (px./....=...b.h
```

## rttbackend/__pycache__/types.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jun 25 07:10:46 2023 UTC, .py size: 420 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 76e8 9764 a401 0000  U.......v..d....
+00000000: 550d 0d0a 0000 0000 71e9 9764 a401 0000  U.......q..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1200 0000 6400  .....@...s....d.
 00000030: 6401 8400 6100 7400 8300 0100 6402 5300  d...a.t.....d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0005  ).c.............
 00000050: 0000 0004 0000 0043 0000 0073 5600 0000  .......C...sV...
 00000060: 6401 6400 6c00 7d00 6401 6400 6c01 7d01  d.d.l.}.d.d.l.}.
 00000070: 6401 6400 6c02 7d02 7c01 a003 7404 6402  d.d.l.}.|...t.d.
```

