# Comparing `tmp/cns-1.0.31-py3-none-any.whl.zip` & `tmp/cns-1.0.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 514373 bytes, number of entries: 19
+Zip file size: 527425 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat   173056 b- defN 23-Jun-15 05:40 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   156672 b- defN 23-Jun-15 05:40 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    71168 b- defN 23-Jun-23 11:03 cns/PathX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    59392 b- defN 23-Jun-23 11:02 cns/PathX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-23 11:03 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      490 b- defN 23-Jun-25 05:39 cns/__init__.py
--rw-rw-rw-  2.0 fat    64512 b- defN 23-Jun-25 05:37 cns/cmdX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    52736 b- defN 23-Jun-25 05:39 cns/cmdX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-25 05:41 cns-1.0.31.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1990 b- defN 23-Jun-25 05:41 cns-1.0.31.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-25 05:41 cns-1.0.31.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-25 05:41 cns-1.0.31.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1570 b- defN 23-Jun-25 05:41 cns-1.0.31.dist-info/RECORD
-19 files, 1155600 bytes uncompressed, 511841 bytes compressed:  55.7%
+-rw-rw-rw-  2.0 fat    81920 b- defN 23-Jun-25 10:18 cns/cmdX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    68096 b- defN 23-Jun-25 10:18 cns/cmdX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-25 10:22 cns-1.0.32.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1990 b- defN 23-Jun-25 10:22 cns-1.0.32.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-25 10:22 cns-1.0.32.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-25 10:22 cns-1.0.32.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1570 b- defN 23-Jun-25 10:22 cns-1.0.32.dist-info/RECORD
+19 files, 1188368 bytes uncompressed, 524893 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: cns/cmdX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/cmdX.cp39-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.0.31.dist-info/LICENSE
+Filename: cns-1.0.32.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.31.dist-info/METADATA
+Filename: cns-1.0.32.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.31.dist-info/WHEEL
+Filename: cns-1.0.32.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.31.dist-info/top_level.txt
+Filename: cns-1.0.32.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.31.dist-info/RECORD
+Filename: cns-1.0.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cns-1.0.31.dist-info/METADATA` & `cns-1.0.32.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.31
+Version: 1.0.32
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: Rambo
 Author-email: 6566666@qq.com
 License: Copyright (C) 2023 CNS. All Rights Reserved. See LICENSE for license.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.31.dist-info/RECORD` & `cns-1.0.32.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 cns/PathX.cp36-win_amd64.pyd,sha256=mrBJ9wWP59j6keB9rc1RdS2KJ04NtOVYwh-l0JCTwFw,71168
 cns/PathX.cp39-win_amd64.pyd,sha256=lH0XLNMSHPme0sNiUiMbpiEecqFu4mntnq1zeRNnHz4,59392
 cns/SQLstrX.cp36-win_amd64.pyd,sha256=3NLRKJa7q2Dl1sKlzVBbScgYjcgoSgMOClS2BuxDIzI,84992
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
 cns/TextX.cp36-win_amd64.pyd,sha256=cbQwr_FGkhhWoyyq3i43Tj11YSa-8r_3ZSN5JpXTcWk,77312
 cns/TextX.cp39-win_amd64.pyd,sha256=tJkutc00Vya2KBtXFWGcCm0wOSt9vvAm_7cZBsB1DgE,65536
 cns/__init__.py,sha256=mZnBTIBbDMPYkk9m5MH9PtQIi84iPQf9Tc-9TGIzMQQ,490
-cns/cmdX.cp36-win_amd64.pyd,sha256=777EXQbTKDoZCrIJxbrz8QaF9O82y6D1zDj8GXsJnVs,64512
-cns/cmdX.cp39-win_amd64.pyd,sha256=MTIgBA-_zq69zIy2Du6xoStAtOFZKcCaZSQkjzR9Nas,52736
-cns-1.0.31.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.31.dist-info/METADATA,sha256=ZT3SFI80T2W4KIg7dNlnpZuvyu0Ywmwj9-fkPzOUJjI,1990
-cns-1.0.31.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.31.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.31.dist-info/RECORD,,
+cns/cmdX.cp36-win_amd64.pyd,sha256=FAfnl1fc_Fr-fXauALU7Bd-B9sjWwq7nR8Rylo8ib5M,81920
+cns/cmdX.cp39-win_amd64.pyd,sha256=6YUg31N-MCntRXkBZGfpIaoaY6XLq7kEeSTp6ejtSHQ,68096
+cns-1.0.32.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.32.dist-info/METADATA,sha256=IfhCbCITwNu3VcNdJOdU8cZymrjq7J_mVARdtjz4jZI,1990
+cns-1.0.32.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.32.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.32.dist-info/RECORD,,
```

