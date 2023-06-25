# Comparing `tmp/azure-mgmt-graphservices-1.0.0.zip` & `tmp/azure-mgmt-graphservices-1.0.0b1.zip`

## zipinfo {}

```diff
@@ -1,51 +1,53 @@
-Zip file size: 60462 bytes, number of entries: 49
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/LICENSE
--rw-rw-r--  2.0 unx       38 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/setup.cfg
--rw-rw-r--  2.0 unx      644 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/_meta.json
--rw-rw-r--  2.0 unx     2174 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/README.md
--rw-rw-r--  2.0 unx      458 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/CHANGELOG.md
--rw-rw-r--  2.0 unx     3531 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/PKG-INFO
--rw-rw-r--  2.0 unx      219 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/MANIFEST.in
--rw-rw-r--  2.0 unx     2852 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/setup.py
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     1525 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      124 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     3531 b- defN 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_patch.py
--rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_vendor.py
--rw-rw-r--  2.0 unx     3495 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_configuration.py
--rw-rw-r--  2.0 unx      910 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/__init__.py
--rw-rw-r--  2.0 unx     4314 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_graph_services_mgmt_client.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/py.typed
--rw-rw-r--  2.0 unx    78836 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_serialization.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_version.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_patch.py
--rw-rw-r--  2.0 unx     1881 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/__init__.py
--rw-rw-r--  2.0 unx    18485 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_models_py3.py
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_patch.py
--rw-rw-r--  2.0 unx      840 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/__init__.py
--rw-rw-r--  2.0 unx     6467 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_operations.py
--rw-rw-r--  2.0 unx    40630 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_accounts_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-25 04:49 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_patch.py
--rw-rw-r--  2.0 unx     3543 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_configuration.py
--rw-rw-r--  2.0 unx      857 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/__init__.py
--rw-rw-r--  2.0 unx     4454 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      840 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5762 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    32849 b- defN 23-Jun-25 04:48 azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_accounts_operations.py
-49 files, 227093 bytes uncompressed, 50242 bytes compressed:  77.9%
+Zip file size: 64913 bytes, number of entries: 51
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/
+-rw-rw-r--  2.0 unx      642 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/_meta.json
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/LICENSE
+-rw-rw-r--  2.0 unx     3137 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/setup.cfg
+-rw-rw-r--  2.0 unx       62 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2174 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/README.md
+-rw-rw-r--  2.0 unx      219 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     2840 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/setup.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     3137 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      124 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     1667 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/not-zip-safe
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_patch.py
+-rw-rw-r--  2.0 unx     3768 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_configuration.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/py.typed
+-rw-rw-r--  2.0 unx      910 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/__init__.py
+-rw-rw-r--  2.0 unx     4603 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_graph_services_mgmt_client.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_vendor.py
+-rw-rw-r--  2.0 unx    78824 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_serialization.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-23 02:01 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_patch.py
+-rw-rw-r--  2.0 unx     3816 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_configuration.py
+-rw-rw-r--  2.0 unx      857 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/__init__.py
+-rw-rw-r--  2.0 unx     4747 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    25083 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_account_operations.py
+-rw-rw-r--  2.0 unx      944 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     6058 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_operation_operations.py
+-rw-rw-r--  2.0 unx    10504 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_accounts_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_patch.py
+-rw-rw-r--  2.0 unx     1881 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/__init__.py
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx    18485 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_models_py3.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_patch.py
+-rw-rw-r--  2.0 unx    31012 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_account_operations.py
+-rw-rw-r--  2.0 unx      944 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/__init__.py
+-rw-rw-r--  2.0 unx     6801 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_operation_operations.py
+-rw-rw-r--  2.0 unx    12774 b- defN 23-Mar-23 02:00 azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_accounts_operations.py
+51 files, 233887 bytes uncompressed, 53933 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,148 +1,154 @@
-Filename: azure-mgmt-graphservices-1.0.0/
+Filename: azure-mgmt-graphservices-1.0.0b1/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/LICENSE
+Filename: azure-mgmt-graphservices-1.0.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/setup.cfg
+Filename: azure-mgmt-graphservices-1.0.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/_meta.json
+Filename: azure-mgmt-graphservices-1.0.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/README.md
+Filename: azure-mgmt-graphservices-1.0.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/CHANGELOG.md
+Filename: azure-mgmt-graphservices-1.0.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/PKG-INFO
+Filename: azure-mgmt-graphservices-1.0.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/MANIFEST.in
+Filename: azure-mgmt-graphservices-1.0.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/setup.py
+Filename: azure-mgmt-graphservices-1.0.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/not-zip-safe
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/SOURCES.txt
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/top_level.txt
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/requires.txt
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/dependency_links.txt
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/PKG-INFO
+Filename: azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_patch.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_patch.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_vendor.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_configuration.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/py.typed
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_graph_services_mgmt_client.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_graph_services_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/py.typed
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_serialization.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_version.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_version.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_patch.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_models_py3.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_patch.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_operations.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_account_operations.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_accounts_operations.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_operation_operations.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_patch.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_accounts_operations.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_configuration.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_patch.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/__init__.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_operations.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_account_operations.py
 Comment: 
 
-Filename: azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_accounts_operations.py
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_operation_operations.py
+Comment: 
+
+Filename: azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_accounts_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-graphservices-1.0.0/LICENSE` & `azure-mgmt-graphservices-1.0.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/_meta.json` & `azure-mgmt-graphservices-1.0.0b1/_meta.json`

 * *Files 22% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/graphservicesprod/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'d4dfb3388ab40185cf302512268ad1406f666d64'",*

 * * "'use'": […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/graphservicesprod/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.12 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "de54b003aee3524343bef30852213db29f55cccd",
+    "autorest_command": "autorest specification/graphservicesprod/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "d4dfb3388ab40185cf302512268ad1406f666d64",
     "readme": "specification/graphservicesprod/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.4.12",
+        "@autorest/python@6.4.3",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-graphservices-1.0.0/README.md` & `azure-mgmt-graphservices-1.0.0b1/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/PKG-INFO` & `azure-mgmt-graphservices-1.0.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-graphservices
-Version: 1.0.0
+Version: 1.0.0b1
 Summary: Microsoft Azure Graphservices Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,25 +85,10 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-graphservices%2FREADME.png)
 
 
 # Release History
 
-## 1.0.0 (2023-06-25)
-
-### Features Added
-
-  - Added operation AccountsOperations.begin_create_and_update
-  - Added operation AccountsOperations.delete
-  - Added operation AccountsOperations.get
-  - Added operation AccountsOperations.update
-  - Added operation group Operations
-
-### Breaking Changes
-
-  - Removed operation group AccountOperations
-  - Removed operation group OperationOperations
-
 ## 1.0.0b1 (2023-03-22)
 
 * Initial Release
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/SOURCES.txt` & `azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 azure/mgmt/graphservices/_version.py
 azure/mgmt/graphservices/py.typed
 azure/mgmt/graphservices/aio/__init__.py
 azure/mgmt/graphservices/aio/_configuration.py
 azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py
 azure/mgmt/graphservices/aio/_patch.py
 azure/mgmt/graphservices/aio/operations/__init__.py
+azure/mgmt/graphservices/aio/operations/_account_operations.py
 azure/mgmt/graphservices/aio/operations/_accounts_operations.py
-azure/mgmt/graphservices/aio/operations/_operations.py
+azure/mgmt/graphservices/aio/operations/_operation_operations.py
 azure/mgmt/graphservices/aio/operations/_patch.py
 azure/mgmt/graphservices/models/__init__.py
 azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py
 azure/mgmt/graphservices/models/_models_py3.py
 azure/mgmt/graphservices/models/_patch.py
 azure/mgmt/graphservices/operations/__init__.py
+azure/mgmt/graphservices/operations/_account_operations.py
 azure/mgmt/graphservices/operations/_accounts_operations.py
-azure/mgmt/graphservices/operations/_operations.py
+azure/mgmt/graphservices/operations/_operation_operations.py
 azure/mgmt/graphservices/operations/_patch.py
 azure_mgmt_graphservices.egg-info/PKG-INFO
 azure_mgmt_graphservices.egg-info/SOURCES.txt
 azure_mgmt_graphservices.egg-info/dependency_links.txt
 azure_mgmt_graphservices.egg-info/not-zip-safe
 azure_mgmt_graphservices.egg-info/requires.txt
 azure_mgmt_graphservices.egg-info/top_level.txt
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure_mgmt_graphservices.egg-info/PKG-INFO` & `azure-mgmt-graphservices-1.0.0b1/azure_mgmt_graphservices.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-graphservices
-Version: 1.0.0
+Version: 1.0.0b1
 Summary: Microsoft Azure Graphservices Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,25 +85,10 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-graphservices%2FREADME.png)
 
 
 # Release History
 
-## 1.0.0 (2023-06-25)
-
-### Features Added
-
-  - Added operation AccountsOperations.begin_create_and_update
-  - Added operation AccountsOperations.delete
-  - Added operation AccountsOperations.get
-  - Added operation AccountsOperations.update
-  - Added operation group Operations
-
-### Breaking Changes
-
-  - Removed operation group AccountOperations
-  - Removed operation group OperationOperations
-
 ## 1.0.0b1 (2023-03-22)
 
 * Initial Release
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_patch.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_vendor.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_configuration.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class GraphServicesMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for GraphServicesMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-04-13". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-09-22-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(GraphServicesMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-04-13")
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop("api_version", "2022-09-22-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +58,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/__init__.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_graph_services_mgmt_client.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_graph_services_mgmt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from ._configuration import GraphServicesMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
-from .operations import AccountsOperations, Operations
+from .operations import AccountOperations, AccountsOperations, OperationOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class GraphServicesMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """Self service experience for Microsoft Graph metered services.
 
     :ivar accounts: AccountsOperations operations
     :vartype accounts: azure.mgmt.graphservices.operations.AccountsOperations
-    :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.graphservices.operations.Operations
+    :ivar account: AccountOperations operations
+    :vartype account: azure.mgmt.graphservices.operations.AccountOperations
+    :ivar operation: OperationOperations operations
+    :vartype operation: azure.mgmt.graphservices.operations.OperationOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-04-13". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-09-22-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -55,15 +57,16 @@
         self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.accounts = AccountsOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.account = AccountOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.operation = OperationOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/_serialization.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                                xml_name = "{}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -1267,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+        xml_name = "{}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1291,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+        xml_name = "{}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_patch.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/__init__.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_models_py3.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_graph_services_mgmt_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_patch.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/__init__.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._accounts_operations import AccountsOperations
-from ._operations import Operations
+from ._account_operations import AccountOperations
+from ._operation_operations import OperationOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AccountsOperations",
-    "Operations",
+    "AccountOperations",
+    "OperationOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_operations.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_operation_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -25,48 +26,54 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
+    api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-09-22-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.GraphServices/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class Operations:
+class OperationOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.graphservices.GraphServicesMgmtClient`'s
-        :attr:`operations` attribute.
+        :attr:`operation` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -82,15 +89,17 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.graphservices.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/operations/_accounts_operations.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_account_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,106 +2,56 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
-import urllib.parse
+import sys
+from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.GraphServices/accounts")
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
 def build_get_request(resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
+    api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-09-22-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts/{resourceName}",
     )  # pylint: disable=line-too-long
@@ -126,15 +76,17 @@
 
 def build_create_and_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
+    api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-09-22-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts/{resourceName}",
@@ -162,15 +114,17 @@
 
 def build_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
+    api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-09-22-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts/{resourceName}",
@@ -198,15 +152,17 @@
 
 def build_delete_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-13"))
+    api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-09-22-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts/{resourceName}",
     )  # pylint: disable=line-too-long
@@ -225,204 +181,34 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AccountsOperations:
+class AccountOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.graphservices.GraphServicesMgmtClient`'s
-        :attr:`accounts` attribute.
+        :attr:`account` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.AccountResource"]:
-        """Returns list of accounts apps.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AccountResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.graphservices.models.AccountResource]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AccountResourceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("AccountResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
-
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return ItemPaged(get_next, extract_data)
-
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts"
-    }
-
-    @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.AccountResource"]:
-        """Returns list of accounts belonging to a subscription.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AccountResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.graphservices.models.AccountResource]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AccountResourceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("AccountResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
-
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return ItemPaged(get_next, extract_data)
-
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.GraphServices/accounts"
-    }
-
-    @distributed_trace
     def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.AccountResource:
         """Returns account resource for a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
@@ -439,15 +225,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -495,22 +283,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(account_resource, (IOBase, bytes)):
+        if isinstance(account_resource, (IO, bytes)):
             _content = account_resource
         else:
             _json = self._serialize.body(account_resource, "AccountResource")
 
         request = build_create_and_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -658,15 +448,17 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.graphservices.models.AccountResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_and_update_initial(
@@ -798,22 +590,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(account_resource, (IOBase, bytes)):
+        if isinstance(account_resource, (IO, bytes)):
             _content = account_resource
         else:
             _json = self._serialize.body(account_resource, "AccountPatchResource")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -875,15 +669,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_patch.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_configuration.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class GraphServicesMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for GraphServicesMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-04-13". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-09-22-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(GraphServicesMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-04-13")
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop("api_version", "2022-09-22-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +58,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/__init__.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/_graph_services_mgmt_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import GraphServicesMgmtClientConfiguration
-from .operations import AccountsOperations, Operations
+from .operations import AccountOperations, AccountsOperations, OperationOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class GraphServicesMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """Self service experience for Microsoft Graph metered services.
 
     :ivar accounts: AccountsOperations operations
     :vartype accounts: azure.mgmt.graphservices.aio.operations.AccountsOperations
-    :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.graphservices.aio.operations.Operations
+    :ivar account: AccountOperations operations
+    :vartype account: azure.mgmt.graphservices.aio.operations.AccountOperations
+    :ivar operation: OperationOperations operations
+    :vartype operation: azure.mgmt.graphservices.aio.operations.OperationOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-04-13". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-09-22-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -55,15 +57,16 @@
         self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.accounts = AccountsOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.account = AccountOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.operation = OperationOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_patch.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/__init__.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/operations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._accounts_operations import AccountsOperations
-from ._operations import Operations
+from ._account_operations import AccountOperations
+from ._operation_operations import OperationOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AccountsOperations",
-    "Operations",
+    "AccountOperations",
+    "OperationOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_operations.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_operation_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -23,28 +24,32 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
+from ...operations._operation_operations import build_list_request
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class Operations:
+class OperationOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.graphservices.aio.GraphServicesMgmtClient`'s
-        :attr:`operations` attribute.
+        :attr:`operation` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -60,15 +65,17 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.graphservices.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-graphservices-1.0.0/azure/mgmt/graphservices/aio/operations/_accounts_operations.py` & `azure-mgmt-graphservices-1.0.0b1/azure/mgmt/graphservices/aio/operations/_account_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,245 +2,70 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
-import urllib.parse
+import sys
+from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._accounts_operations import (
+from ...operations._account_operations import (
     build_create_and_update_request,
     build_delete_request,
     build_get_request,
-    build_list_by_resource_group_request,
-    build_list_by_subscription_request,
     build_update_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class AccountsOperations:
+class AccountOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.graphservices.aio.GraphServicesMgmtClient`'s
-        :attr:`accounts` attribute.
+        :attr:`account` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def list_by_resource_group(
-        self, resource_group_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.AccountResource"]:
-        """Returns list of accounts apps.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AccountResource or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.graphservices.models.AccountResource]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AccountResourceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("AccountResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.GraphServices/accounts"
-    }
-
-    @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.AccountResource"]:
-        """Returns list of accounts belonging to a subscription.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AccountResource or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.graphservices.models.AccountResource]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AccountResourceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("AccountResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.GraphServices/accounts"
-    }
-
     @distributed_trace_async
     async def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.AccountResource:
         """Returns account resource for a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
@@ -258,15 +83,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -314,22 +141,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(account_resource, (IOBase, bytes)):
+        if isinstance(account_resource, (IO, bytes)):
             _content = account_resource
         else:
             _json = self._serialize.body(account_resource, "AccountResource")
 
         request = build_create_and_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -477,15 +306,17 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.graphservices.models.AccountResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_and_update_initial(
@@ -618,22 +449,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AccountResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(account_resource, (IOBase, bytes)):
+        if isinstance(account_resource, (IO, bytes)):
             _content = account_resource
         else:
             _json = self._serialize.body(account_resource, "AccountPatchResource")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -695,15 +528,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        api_version: Literal["2022-09-22-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

