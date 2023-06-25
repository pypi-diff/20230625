# Comparing `tmp/mythril-0.9.1.tar.gz` & `tmp/mythril-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mythril-0.9.1.tar", last modified: Mon Jan 15 03:44:04 2018, max compression
+gzip compressed data, was "dist/mythril-0.9.2.tar", last modified: Mon Jan 15 06:31:12 2018, max compression
```

## Comparing `mythril-0.9.1.tar` & `mythril-0.9.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)    10207 2018-01-15 03:44:04.000000 mythril-0.9.1/PKG-INFO
--rwxr-xr-x   0 bernhardmueller   (501) staff       (20)    10461 2018-01-09 06:35:08.000000 mythril-0.9.1/myth
--rw-r--r--   0 bernhardmueller   (501) staff       (20)       44 2017-10-04 03:22:08.000000 mythril-0.9.1/MANIFEST.in
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/analysis/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      298 2017-12-09 09:18:02.000000 mythril-0.9.1/mythril/analysis/solver.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     5076 2017-12-06 08:11:41.000000 mythril-0.9.1/mythril/analysis/callgraph.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      742 2018-01-09 06:30:19.000000 mythril-0.9.1/mythril/analysis/security.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/analysis/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     4429 2018-01-08 14:13:46.000000 mythril-0.9.1/mythril/analysis/symbolic.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1188 2018-01-09 06:28:51.000000 mythril-0.9.1/mythril/analysis/ops.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/analysis/modules/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      927 2018-01-09 06:43:01.000000 mythril-0.9.1/mythril/analysis/modules/tx_origin.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     4181 2018-01-04 04:01:24.000000 mythril-0.9.1/mythril/analysis/modules/unchecked_suicide.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/analysis/modules/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1731 2018-01-04 04:02:00.000000 mythril-0.9.1/mythril/analysis/modules/delegatecall_forward.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     2657 2018-01-04 04:00:29.000000 mythril-0.9.1/mythril/analysis/modules/integer_underflow.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     4375 2018-01-08 14:13:46.000000 mythril-0.9.1/mythril/analysis/modules/ether_send.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     2705 2018-01-04 03:59:20.000000 mythril-0.9.1/mythril/analysis/modules/call_to_dynamic_with_gas.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     2785 2018-01-04 03:59:10.000000 mythril-0.9.1/mythril/analysis/modules/delegatecall_to_dynamic.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     2532 2018-01-04 04:01:17.000000 mythril-0.9.1/mythril/analysis/modules/unchecked_retval.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     5263 2018-01-04 04:01:35.000000 mythril-0.9.1/mythril/analysis/modules/weak_random.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1431 2018-01-09 06:28:45.000000 mythril-0.9.1/mythril/analysis/report.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-01 03:55:30.000000 mythril-0.9.1/mythril/__init__.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/ether/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     2639 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ether/ethcontract.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1666 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ether/evm.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1681 2018-01-15 03:25:31.000000 mythril-0.9.1/mythril/ether/util.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-09-18 08:48:57.000000 mythril-0.9.1/mythril/ether/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     3146 2017-12-10 07:13:35.000000 mythril-0.9.1/mythril/ether/asm.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     4002 2018-01-11 07:46:13.000000 mythril-0.9.1/mythril/ether/contractstorage.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/support/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/support/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      863 2017-12-07 10:00:55.000000 mythril-0.9.1/mythril/support/signatures.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1479 2018-01-09 06:18:18.000000 mythril-0.9.1/mythril/support/loader.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/disassembler/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-04 03:13:16.000000 mythril-0.9.1/mythril/disassembler/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1613 2017-12-06 07:53:44.000000 mythril-0.9.1/mythril/disassembler/disassembly.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)       79 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/exceptions.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/ipc/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)    24873 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ipc/client.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      179 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ipc/constants.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ipc/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      687 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ipc/utils.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      228 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/ipc/exceptions.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril/rpc/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)    21211 2017-11-13 09:10:30.000000 mythril-0.9.1/mythril/rpc/client.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      179 2017-09-19 05:59:30.000000 mythril-0.9.1/mythril/rpc/constants.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-09-19 06:52:37.000000 mythril-0.9.1/mythril/rpc/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      687 2017-09-29 04:19:21.000000 mythril-0.9.1/mythril/rpc/utils.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)      248 2017-09-19 05:59:30.000000 mythril-0.9.1/mythril/rpc/exceptions.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     7434 2018-01-04 04:04:17.000000 mythril-0.9.1/README.md
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)    10207 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/PKG-INFO
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1565 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/SOURCES.txt
--rw-r--r--   0 bernhardmueller   (501) staff       (20)       86 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/requires.txt
--rw-r--r--   0 bernhardmueller   (501) staff       (20)       14 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/top_level.txt
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        1 2018-01-15 03:44:04.000000 mythril-0.9.1/mythril.egg-info/dependency_links.txt
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/laser/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:19:50.000000 mythril-0.9.1/laser/__init__.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/laser/ethereum/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1255 2017-10-29 03:20:31.000000 mythril-0.9.1/laser/ethereum/gascost.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:18:43.000000 mythril-0.9.1/laser/ethereum/__init__.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)     1778 2018-01-09 07:34:03.000000 mythril-0.9.1/laser/ethereum/helper.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)    38083 2018-01-12 04:52:36.000000 mythril-0.9.1/laser/ethereum/svm.py
-drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 03:44:04.000000 mythril-0.9.1/laser/ethereum/modules/
--rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:20:53.000000 mythril-0.9.1/laser/ethereum/modules/__init__.py
--rwxr-xr-x   0 bernhardmueller   (501) staff       (20)     8720 2018-01-15 03:43:38.000000 mythril-0.9.1/setup.py
--rw-r--r--   0 bernhardmueller   (501) staff       (20)       59 2018-01-15 03:44:04.000000 mythril-0.9.1/setup.cfg
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)    10207 2018-01-15 06:31:12.000000 mythril-0.9.2/PKG-INFO
+-rwxr-xr-x   0 bernhardmueller   (501) staff       (20)    10461 2018-01-09 06:35:08.000000 mythril-0.9.2/myth
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)       44 2017-10-04 03:22:08.000000 mythril-0.9.2/MANIFEST.in
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/analysis/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      298 2017-12-09 09:18:02.000000 mythril-0.9.2/mythril/analysis/solver.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     5076 2017-12-06 08:11:41.000000 mythril-0.9.2/mythril/analysis/callgraph.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      742 2018-01-09 06:30:19.000000 mythril-0.9.2/mythril/analysis/security.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/analysis/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     4429 2018-01-08 14:13:46.000000 mythril-0.9.2/mythril/analysis/symbolic.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1188 2018-01-09 06:28:51.000000 mythril-0.9.2/mythril/analysis/ops.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/analysis/modules/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      927 2018-01-09 06:43:01.000000 mythril-0.9.2/mythril/analysis/modules/tx_origin.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     4181 2018-01-04 04:01:24.000000 mythril-0.9.2/mythril/analysis/modules/unchecked_suicide.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/analysis/modules/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1731 2018-01-04 04:02:00.000000 mythril-0.9.2/mythril/analysis/modules/delegatecall_forward.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     2657 2018-01-04 04:00:29.000000 mythril-0.9.2/mythril/analysis/modules/integer_underflow.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     4375 2018-01-08 14:13:46.000000 mythril-0.9.2/mythril/analysis/modules/ether_send.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     2705 2018-01-04 03:59:20.000000 mythril-0.9.2/mythril/analysis/modules/call_to_dynamic_with_gas.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     2785 2018-01-04 03:59:10.000000 mythril-0.9.2/mythril/analysis/modules/delegatecall_to_dynamic.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     2532 2018-01-04 04:01:17.000000 mythril-0.9.2/mythril/analysis/modules/unchecked_retval.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     5263 2018-01-04 04:01:35.000000 mythril-0.9.2/mythril/analysis/modules/weak_random.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1431 2018-01-09 06:28:45.000000 mythril-0.9.2/mythril/analysis/report.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-01 03:55:30.000000 mythril-0.9.2/mythril/__init__.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/ether/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     2639 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ether/ethcontract.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1666 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ether/evm.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1681 2018-01-15 03:25:31.000000 mythril-0.9.2/mythril/ether/util.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-09-18 08:48:57.000000 mythril-0.9.2/mythril/ether/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     3146 2017-12-10 07:13:35.000000 mythril-0.9.2/mythril/ether/asm.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     4002 2018-01-11 07:46:13.000000 mythril-0.9.2/mythril/ether/contractstorage.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/support/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/support/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      863 2017-12-07 10:00:55.000000 mythril-0.9.2/mythril/support/signatures.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1479 2018-01-09 06:18:18.000000 mythril-0.9.2/mythril/support/loader.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/disassembler/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-04 03:13:16.000000 mythril-0.9.2/mythril/disassembler/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1613 2017-12-06 07:53:44.000000 mythril-0.9.2/mythril/disassembler/disassembly.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)       79 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/exceptions.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/ipc/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)    24873 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ipc/client.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      179 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ipc/constants.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ipc/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      687 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ipc/utils.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      228 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/ipc/exceptions.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril/rpc/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)    21211 2017-11-13 09:10:30.000000 mythril-0.9.2/mythril/rpc/client.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      179 2017-09-19 05:59:30.000000 mythril-0.9.2/mythril/rpc/constants.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-09-19 06:52:37.000000 mythril-0.9.2/mythril/rpc/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      687 2017-09-29 04:19:21.000000 mythril-0.9.2/mythril/rpc/utils.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)      248 2017-09-19 05:59:30.000000 mythril-0.9.2/mythril/rpc/exceptions.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     7434 2018-01-04 04:04:17.000000 mythril-0.9.2/README.md
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)    10207 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/PKG-INFO
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1565 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)       86 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/requires.txt
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)       14 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/top_level.txt
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        1 2018-01-15 06:31:12.000000 mythril-0.9.2/mythril.egg-info/dependency_links.txt
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/laser/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:19:50.000000 mythril-0.9.2/laser/__init__.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/laser/ethereum/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1255 2017-10-29 03:20:31.000000 mythril-0.9.2/laser/ethereum/gascost.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:18:43.000000 mythril-0.9.2/laser/ethereum/__init__.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)     1778 2018-01-09 07:34:03.000000 mythril-0.9.2/laser/ethereum/helper.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)    38083 2018-01-15 06:27:01.000000 mythril-0.9.2/laser/ethereum/svm.py
+drwxr-xr-x   0 bernhardmueller   (501) staff       (20)        0 2018-01-15 06:31:12.000000 mythril-0.9.2/laser/ethereum/modules/
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)        0 2017-10-17 07:20:53.000000 mythril-0.9.2/laser/ethereum/modules/__init__.py
+-rwxr-xr-x   0 bernhardmueller   (501) staff       (20)     8720 2018-01-15 06:31:05.000000 mythril-0.9.2/setup.py
+-rw-r--r--   0 bernhardmueller   (501) staff       (20)       59 2018-01-15 06:31:12.000000 mythril-0.9.2/setup.cfg
```

### Comparing `mythril-0.9.1/PKG-INFO` & `mythril-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mythril
-Version: 0.9.1
+Version: 0.9.2
 Summary: Security analysis tool for Ethereum smart contracts
 Home-page: https://github.com/b-mueller/mythril
 Author: Bernhard Mueller
 Author-email: bernhard.mueller11@gmail.com
 License: MIT
 Description: 
         Mythril is a security analysis tool for Ethereum smart contracts. It
```

### Comparing `mythril-0.9.1/myth` & `mythril-0.9.2/myth`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/callgraph.py` & `mythril-0.9.2/mythril/analysis/callgraph.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/security.py` & `mythril-0.9.2/mythril/analysis/security.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/symbolic.py` & `mythril-0.9.2/mythril/analysis/symbolic.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/ops.py` & `mythril-0.9.2/mythril/analysis/ops.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/tx_origin.py` & `mythril-0.9.2/mythril/analysis/modules/tx_origin.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/unchecked_suicide.py` & `mythril-0.9.2/mythril/analysis/modules/unchecked_suicide.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/delegatecall_forward.py` & `mythril-0.9.2/mythril/analysis/modules/delegatecall_forward.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/integer_underflow.py` & `mythril-0.9.2/mythril/analysis/modules/integer_underflow.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/ether_send.py` & `mythril-0.9.2/mythril/analysis/modules/ether_send.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/call_to_dynamic_with_gas.py` & `mythril-0.9.2/mythril/analysis/modules/call_to_dynamic_with_gas.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/delegatecall_to_dynamic.py` & `mythril-0.9.2/mythril/analysis/modules/delegatecall_to_dynamic.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/unchecked_retval.py` & `mythril-0.9.2/mythril/analysis/modules/unchecked_retval.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/modules/weak_random.py` & `mythril-0.9.2/mythril/analysis/modules/weak_random.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/analysis/report.py` & `mythril-0.9.2/mythril/analysis/report.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ether/ethcontract.py` & `mythril-0.9.2/mythril/ether/ethcontract.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ether/evm.py` & `mythril-0.9.2/mythril/ether/evm.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ether/util.py` & `mythril-0.9.2/mythril/ether/util.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ether/asm.py` & `mythril-0.9.2/mythril/ether/asm.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ether/contractstorage.py` & `mythril-0.9.2/mythril/ether/contractstorage.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/support/signatures.py` & `mythril-0.9.2/mythril/support/signatures.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/support/loader.py` & `mythril-0.9.2/mythril/support/loader.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/disassembler/disassembly.py` & `mythril-0.9.2/mythril/disassembler/disassembly.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ipc/client.py` & `mythril-0.9.2/mythril/ipc/client.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/ipc/utils.py` & `mythril-0.9.2/mythril/ipc/utils.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/rpc/client.py` & `mythril-0.9.2/mythril/rpc/client.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril/rpc/utils.py` & `mythril-0.9.2/mythril/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/README.md` & `mythril-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/mythril.egg-info/PKG-INFO` & `mythril-0.9.2/mythril.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mythril
-Version: 0.9.1
+Version: 0.9.2
 Summary: Security analysis tool for Ethereum smart contracts
 Home-page: https://github.com/b-mueller/mythril
 Author: Bernhard Mueller
 Author-email: bernhard.mueller11@gmail.com
 License: MIT
 Description: 
         Mythril is a security analysis tool for Ethereum smart contracts. It
```

### Comparing `mythril-0.9.1/mythril.egg-info/SOURCES.txt` & `mythril-0.9.2/mythril.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/laser/ethereum/gascost.py` & `mythril-0.9.2/laser/ethereum/gascost.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/laser/ethereum/helper.py` & `mythril-0.9.2/laser/ethereum/helper.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/laser/ethereum/svm.py` & `mythril-0.9.2/laser/ethereum/svm.py`

 * *Files identical despite different names*

### Comparing `mythril-0.9.1/setup.py` & `mythril-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
    Database <https://www.4byte.directory>`__.
 '''
 
 
 setup(
     name='mythril',
 
-    version='0.9.1',
+    version='0.9.2',
 
     description='Security analysis tool for Ethereum smart contracts',
     long_description=long_description,
 
     url='https://github.com/b-mueller/mythril',
 
     author='Bernhard Mueller',
@@ -287,15 +287,15 @@
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
     install_requires=[
         'ethereum>=2.0.4',
         'web3',
         'ZODB>=5.3.0',
         'z3-solver>=4.5',
-        'laser-ethereum==0.4.0',
+        'laser-ethereum==0.4.1',
         'requests',
         'BTrees'
     ],
 
     python_requires='>=3.5',
 
     extras_require={
```

