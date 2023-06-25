# Comparing `tmp/aliyun-python-sdk-ddosbgp-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-ddosbgp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ddosbgp-1.0.0.tar", last modified: Sun Jun 25 09:43:31 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ddosbgp-1.0.1.tar", last modified: Sun Jun 25 09:50:02 2023, max compression
```

## Comparing `aliyun-python-sdk-ddosbgp-1.0.0.tar` & `aliyun-python-sdk-ddosbgp-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/
--rw-r--r--   0 root         (0) root         (0)     1833 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/AddIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CheckAccessLogAuthRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CheckGrantRequest.py
--rw-r--r--   0 root         (0) root         (0)     3571 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ConfigSchedruleOnDemandRequest.py
--rw-r--r--   0 root         (0) root         (0)     3571 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CreateSchedruleOnDemandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteBlackholeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteSchedruleOnDemandRequest.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeDdosEventRequest.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeExcpetionCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeInstanceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeInstanceSpecsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandDdosEventRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOpEntitiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribePackIpListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeTrafficRequest.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/GetSlsOpenStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListOpenedAccessLogInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ModifyRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/QuerySchedruleOnDemandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/SetInstanceModeOnDemandRequest.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2472 2023-06-25 09:43:31.000000 aliyun-python-sdk-ddosbgp-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/AddIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CheckAccessLogAuthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CheckGrantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ConfigSchedruleOnDemandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CreateSchedruleOnDemandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteBlackholeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteSchedruleOnDemandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeDdosEventRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeExcpetionCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeInstanceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeInstanceSpecsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandDdosEventRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOpEntitiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribePackIpListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeTrafficRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/GetSlsOpenStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListOpenedAccessLogInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ModifyRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/QuerySchedruleOnDemandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/SetInstanceModeOnDemandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-06-25 09:50:02.000000 aliyun-python-sdk-ddosbgp-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/LICENSE` & `aliyun-python-sdk-ddosbgp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/PKG-INFO` & `aliyun-python-sdk-ddosbgp-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ddosbgp
-Version: 1.0.0
+Version: 1.0.1
 Summary: The ddosbgp module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ddosbgp
```

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/README.rst` & `aliyun-python-sdk-ddosbgp-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/PKG-INFO` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ddosbgp
-Version: 1.0.0
+Version: 1.0.1
 Summary: The ddosbgp module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ddosbgp
```

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyun_python_sdk_ddosbgp.egg-info/SOURCES.txt` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyun_python_sdk_ddosbgp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/endpoint.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/AddIpRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/AddIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CheckAccessLogAuthRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CheckAccessLogAuthRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CheckGrantRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CheckGrantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ConfigSchedruleOnDemandRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ConfigSchedruleOnDemandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/CreateSchedruleOnDemandRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/CreateSchedruleOnDemandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteBlackholeRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteBlackholeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteIpRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DeleteSchedruleOnDemandRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DeleteSchedruleOnDemandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeDdosEventRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeDdosEventRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeExcpetionCountRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeExcpetionCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeInstanceListRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeInstanceListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeInstanceSpecsRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeInstanceSpecsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandDdosEventRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandDdosEventRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandInstanceStatusRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOnDemandInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeOpEntitiesRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeOpEntitiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribePackIpListRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribePackIpListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeRegionsRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/DescribeTrafficRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/DescribeTrafficRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/GetSlsOpenStatusRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/GetSlsOpenStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListOpenedAccessLogInstancesRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListOpenedAccessLogInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListTagKeysRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ListTagResourcesRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/ModifyRemarkRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/ModifyRemarkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/QuerySchedruleOnDemandRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/QuerySchedruleOnDemandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/SetInstanceModeOnDemandRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/SetInstanceModeOnDemandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/TagResourcesRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/aliyunsdkddosbgp/request/v20180720/UntagResourcesRequest.py` & `aliyun-python-sdk-ddosbgp-1.0.1/aliyunsdkddosbgp/request/v20180720/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ddosbgp-1.0.0/setup.py` & `aliyun-python-sdk-ddosbgp-1.0.1/setup.py`

 * *Files identical despite different names*

