# Comparing `tmp/tikit-1.4.7.230609.tar.gz` & `tmp/tikit-1.5.2.230625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikit-1.4.7.230609.tar", last modified: Fri Jun  9 03:25:22 2023, max compression
+gzip compressed data, was "dist/tikit-1.5.2.230625.tar", last modified: Sun Jun 25 07:16:57 2023, max compression
```

## Comparing `tikit-1.4.7.230609.tar` & `tikit-1.5.2.230625.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.909097 tikit-1.4.7.230609/
--rw-r--r--   0 liuliu     (501) staff       (20)       71 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/MANIFEST.in
--rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-06-09 03:25:22.908507 tikit-1.4.7.230609/PKG-INFO
--rw-r--r--   0 liuliu     (501) staff       (20)      499 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/README.md
--rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/requirements.txt
--rw-r--r--   0 liuliu     (501) staff       (20)       38 2023-06-09 03:25:22.909236 tikit-1.4.7.230609/setup.cfg
--rw-r--r--   0 liuliu     (501) staff       (20)      858 2023-06-09 03:06:25.000000 tikit-1.4.7.230609/setup.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.868266 tikit-1.4.7.230609/tikit/
--rw-r--r--   0 liuliu     (501) staff       (20)      185 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     7896 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/cli.py
--rw-r--r--   0 liuliu     (501) staff       (20)   196762 2023-06-09 03:01:16.000000 tikit-1.4.7.230609/tikit/client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3976 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/default_client.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.877182 tikit-1.4.7.230609/tikit/display_optimize/
--rw-r--r--   0 liuliu     (501) staff       (20)      133 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/display_optimize/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3820 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/display_optimize/dataset.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1628 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/display_optimize/resource_group.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3951 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/display_optimize/training_model.py
--rw-r--r--   0 liuliu     (501) staff       (20)     4973 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/display_optimize/training_task.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1779 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/hdfs.py
--rw-r--r--   0 liuliu     (501) staff       (20)    35625 2023-06-09 02:58:34.000000 tikit-1.4.7.230609/tikit/hive.py
--rw-r--r--   0 liuliu     (501) staff       (20)    20234 2023-06-09 03:01:16.000000 tikit-1.4.7.230609/tikit/models.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.878130 tikit-1.4.7.230609/tikit/templates/
--rw-r--r--   0 liuliu     (501) staff       (20)     7622 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/templates/service_config.yaml
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.879239 tikit-1.4.7.230609/tikit/tencentcloud/
--rw-r--r--   0 liuliu     (501) staff       (20)      630 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.884917 tikit-1.4.7.230609/tikit/tencentcloud/common/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)    16473 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     2337 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 liuliu     (501) staff       (20)     2002 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)    12338 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.886698 tikit-1.4.7.230609/tikit/tencentcloud/common/exception/
--rw-r--r--   0 liuliu     (501) staff       (20)      741 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)      760 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.888354 tikit-1.4.7.230609/tikit/tencentcloud/common/http/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     5071 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.890670 tikit-1.4.7.230609/tikit/tencentcloud/common/profile/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1657 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1857 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1574 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.891518 tikit-1.4.7.230609/tikit/tencentcloud/emr/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.894396 tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     6015 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3465 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)    33848 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.895801 tikit-1.4.7.230609/tikit/tencentcloud/tione/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.902357 tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)    12419 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)   748604 2023-06-09 03:01:16.000000 tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 liuliu     (501) staff       (20)   260703 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.905085 tikit-1.4.7.230609/tikit/tencentcloud/wedata/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.907728 tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)      819 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)    19834 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 liuliu     (501) staff       (20)     4802 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)      893 2023-04-06 06:58:27.000000 tikit-1.4.7.230609/tikit/util.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-06-09 03:25:22.873281 tikit-1.4.7.230609/tikit.egg-info/
--rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/PKG-INFO
--rw-r--r--   0 liuliu     (501) staff       (20)     1883 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 liuliu     (501) staff       (20)        1 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 liuliu     (501) staff       (20)       40 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/entry_points.txt
--rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/requires.txt
--rw-r--r--   0 liuliu     (501) staff       (20)        6 2023-06-09 03:25:22.000000 tikit-1.4.7.230609/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/
+-rw-r--r--   0 root         (0) root         (0)    35625 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/hive.py
+-rw-r--r--   0 root         (0) root         (0)   196654 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/client.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/default_client.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     7896 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/cli.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/templates/
+-rw-r--r--   0 root         (0) root         (0)     7622 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/templates/service_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/display_optimize/
+-rw-r--r--   0 root         (0) root         (0)     3820 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/display_optimize/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/display_optimize/training_model.py
+-rw-r--r--   0 root         (0) root         (0)     4973 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/display_optimize/training_task.py
+-rw-r--r--   0 root         (0) root         (0)      133 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/display_optimize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/display_optimize/resource_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)      819 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)    19834 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)     2337 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/abstract_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)     5071 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)     1857 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/credential.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/common_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      760 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 root         (0) root         (0)      741 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16473 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)     3465 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6015 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    33848 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    12419 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260703 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)   749126 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 02:49:54.000000 tikit-1.5.2.230625/tikit/tencentcloud/tione/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/tikit/models.py
+-rw-r--r--   0 root         (0) root         (0)      858 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/setup.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      413 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 07:16:57.000000 tikit-1.5.2.230625/tikit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      413 2023-06-25 07:16:42.000000 tikit-1.5.2.230625/requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tikit-1.4.7.230609/PKG-INFO` & `tikit-1.5.2.230625/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.7.230609
+Version: 1.5.2.230625
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
+Platform: UNKNOWN
 
 TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
 Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
 
 # 发布
 '''bash
 # 公网
@@ -20,7 +21,8 @@
 '''bash
 yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
 pip install -r requirements.txt
 '''
 # 公网
 pip install tikit -U -i https://pypi.org/simple
 '''
+
```

### Comparing `tikit-1.4.7.230609/setup.py` & `tikit-1.5.2.230625/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.4.7.230609',
+    version='1.5.2.230625',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.4.7.230609/tikit/cli.py` & `tikit-1.5.2.230625/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/client.py` & `tikit-1.5.2.230625/tikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,30 +346,26 @@
         if os.path.isdir(local_path):
             target_path = os.path.join(target_path, os.path.basename(cos_path))
         cos_path_length = len(cos_path)
         pool = SimpleThreadPool()
         for file in file_infos:
             # 文件下载 获取文件到本地
             file_cos_key = file["Key"]
-            local_name = os.path.join(target_path, file_cos_key[cos_path_length:].strip('/'))
+            local_name = os.path.join(target_path, file_cos_key[cos_path_length:].strip('/')).strip("/")
 
             # 如果存在目录类型的object, 则直接跳过不做下载操作
             file_cos_key = str(file_cos_key)
             if file_cos_key.endswith("/") and int(file["Size"]) == 0:
                 continue
 
             # 如果本地目录结构不存在，递归创建
             local_dir = os.path.dirname(local_name)
             if local_dir != "" and not os.path.exists(local_dir):
                 os.makedirs(local_dir)
 
-            # skip dir, no need to download it
-            if str(local_name).endswith("/"):
-                continue
-
             # 使用线程池方式
             if self.__need_download_from_cos(bucket, file_cos_key, local_name):
                 pool.add_task(self._cos_client.download_file, bucket, file_cos_key, local_name)
 
         pool.wait_completion()
         result = pool.get_result()
         if not result['success_all']:
```

### Comparing `tikit-1.4.7.230609/tikit/default_client.py` & `tikit-1.5.2.230625/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/display_optimize/dataset.py` & `tikit-1.5.2.230625/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/display_optimize/resource_group.py` & `tikit-1.5.2.230625/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/display_optimize/training_model.py` & `tikit-1.5.2.230625/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/display_optimize/training_task.py` & `tikit-1.5.2.230625/tikit/display_optimize/training_task.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/hdfs.py` & `tikit-1.5.2.230625/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/hive.py` & `tikit-1.5.2.230625/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/models.py` & `tikit-1.5.2.230625/tikit/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/templates/service_config.yaml` & `tikit-1.5.2.230625/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/__init__.py` & `tikit-1.5.2.230625/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/common_client.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/credential.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/http/request.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/common/sign.py` & `tikit-1.5.2.230625/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.5.2.230625/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,56 +815,63 @@
         self.BillingInfo = params.get("BillingInfo")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
 
 
 class CFSConfig(AbstractModel):
     """CFS存储的配置
 
     """
 
     def __init__(self):
         r"""
         :param Id: cfs的实例的ID
         :type Id: str
         :param Path: 存储的路径
         :type Path: str
+        :param MountType: cfs的挂载类型，可选值为：STORAGE、SOURCE 分别表示存储拓展模式和数据源模式，默认为 STORAGE
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MountType: str
         :param Ip: cfs的ip
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ip: str
         :param VpcId: cfs的vpcid
         :type VpcId: str
         :param SubnetId: cfs的子网id
         :type SubnetId: str
+        :param Protocol: 协议 1: NFS, 2: TURBO
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Protocol: str
         """
         self.Id = None
         self.Path = None
+        self.MountType = None
         self.Ip = None
         self.VpcId = None
         self.SubnetId = None
-
+        self.Protocol = None
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Path = params.get("Path")
+        self.MountType = params.get("MountType")
         self.Ip = params.get("Ip")
         self.VpcId = params.get("VpcId")
         self.SubnetId = params.get("SubnetId")
+        self.Protocol = params.get("Protocol")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
 
 
 class CamTag(AbstractModel):
     """cam详细信息
 
     """
```

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.5.2.230625/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.5.2.230625/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit/util.py` & `tikit-1.5.2.230625/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.7.230609/tikit.egg-info/PKG-INFO` & `tikit-1.5.2.230625/tikit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.7.230609
+Version: 1.5.2.230625
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
+Platform: UNKNOWN
 
 TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
 Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
 
 # 发布
 '''bash
 # 公网
@@ -20,7 +21,8 @@
 '''bash
 yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
 pip install -r requirements.txt
 '''
 # 公网
 pip install tikit -U -i https://pypi.org/simple
 '''
+
```

### Comparing `tikit-1.4.7.230609/tikit.egg-info/SOURCES.txt` & `tikit-1.5.2.230625/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

