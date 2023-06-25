# Comparing `tmp/msaf-0.1.70.tar.gz` & `tmp/msaf-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/msaf-0.1.70.tar", last modified: Sat Jun 16 00:40:31 2018, max compression
+gzip compressed data, was "msaf-0.1.80.tar", last modified: Sun Jun 25 10:46:38 2023, max compression
```

## Comparing `msaf-0.1.70.tar` & `msaf-0.1.80.tar`

### file list

```diff
@@ -1,101 +1,111 @@
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/
--rw-r--r--   0 onieto    (5306)     5306     1001 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/__init__.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/
--rw-r--r--   0 onieto    (5306)     5306      900 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/__init__.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/cnmf/
--rw-r--r--   0 onieto    (5306)     5306      194 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/cnmf/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      348 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/cnmf/config.py
--rw-r--r--   0 onieto    (5306)     5306     7147 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/cnmf/segmenter.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/example/
--rw-r--r--   0 onieto    (5306)     5306       47 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/example/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      318 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/example/config.py
--rw-r--r--   0 onieto    (5306)     5306     1095 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/example/segmenter.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/fmc2d/
--rw-r--r--   0 onieto    (5306)     5306      180 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/fmc2d/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      490 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/fmc2d/config.py
--rw-r--r--   0 onieto    (5306)     5306     6919 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/fmc2d/segmenter.py
--rw-r--r--   0 onieto    (5306)     5306     4219 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/fmc2d/utils_2dfmc.py
--rwxr-xr-x   0 onieto    (5306)     5306     7344 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/fmc2d/xmeans.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/foote/
--rw-r--r--   0 onieto    (5306)     5306      152 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/foote/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      522 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/foote/config.py
--rw-r--r--   0 onieto    (5306)     5306     4176 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/foote/segmenter.py
--rw-r--r--   0 onieto    (5306)     5306     5024 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/interface.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/olda/
--rw-r--r--   0 onieto    (5306)     5306      186 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      567 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/config.py
--rwxr-xr-x   0 onieto    (5306)     5306     3844 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/fit_olda_model.py
--rwxr-xr-x   0 onieto    (5306)     5306     6210 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/make_train.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/olda/models/
--rw-r--r--   0 onieto    (5306)     5306    70768 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_BeatlesIso.npy
--rw-r--r--   0 onieto    (5306)     5306    70768 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_BeatlesTUT.npy
--rw-r--r--   0 onieto    (5306)     5306    70768 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_SALAMI-i.npy
--rw-r--r--   0 onieto    (5306)     5306     4026 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/OLDA.py
--rw-r--r--   0 onieto    (5306)     5306    10238 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/olda/segmenter.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/scluster/
--rw-r--r--   0 onieto    (5306)     5306      158 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/scluster/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      410 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/scluster/config.py
--rw-r--r--   0 onieto    (5306)     5306     4321 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/algorithms/scluster/main2.py
--rw-r--r--   0 onieto    (5306)     5306     3235 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/scluster/segmenter.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/sf/
--rw-r--r--   0 onieto    (5306)     5306      152 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/sf/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      568 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/sf/config.py
--rw-r--r--   0 onieto    (5306)     5306     6939 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/algorithms/sf/segmenter.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/algorithms/vmo/
--rw-r--r--   0 onieto    (5306)     5306      177 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/algorithms/vmo/__init__.py
--rw-r--r--   0 onieto    (5306)     5306      480 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/algorithms/vmo/config.py
--rw-r--r--   0 onieto    (5306)     5306     3076 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/algorithms/vmo/main.py
--rw-r--r--   0 onieto    (5306)     5306     2496 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/algorithms/vmo/segmenter.py
--rw-r--r--   0 onieto    (5306)     5306    20079 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/base.py
--rw-r--r--   0 onieto    (5306)     5306     3889 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/configdefaults.py
--rw-r--r--   0 onieto    (5306)     5306    13382 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/configparser.py
--rw-r--r--   0 onieto    (5306)     5306    14967 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/eval.py
--rw-r--r--   0 onieto    (5306)     5306     1169 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/exceptions.py
--rw-r--r--   0 onieto    (5306)     5306    11937 2018-05-21 02:56:55.000000 msaf-0.1.70/msaf/features.py
--rw-r--r--   0 onieto    (5306)     5306    15248 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/input_output.py
--rw-r--r--   0 onieto    (5306)     5306     8511 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/plotting.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf/pymf/
--rw-r--r--   0 onieto    (5306)     5306      891 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/__init__.py
--rw-r--r--   0 onieto    (5306)     5306     4634 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/aa.py
--rw-r--r--   0 onieto    (5306)     5306     4326 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/bnmf.py
--rw-r--r--   0 onieto    (5306)     5306     7383 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/chnmf.py
--rw-r--r--   0 onieto    (5306)     5306     2509 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/cmd.py
--rw-r--r--   0 onieto    (5306)     5306     2732 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/cmeans.py
--rw-r--r--   0 onieto    (5306)     5306     5996 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/cnmf.py
--rw-r--r--   0 onieto    (5306)     5306     4365 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/cur.py
--rw-r--r--   0 onieto    (5306)     5306     2900 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/cursl.py
--rw-r--r--   0 onieto    (5306)     5306     4056 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/dist.py
--rw-r--r--   0 onieto    (5306)     5306     7238 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/gmap.py
--rw-r--r--   0 onieto    (5306)     5306     5697 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/greedy.py
--rw-r--r--   0 onieto    (5306)     5306     2649 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/greedycur.py
--rw-r--r--   0 onieto    (5306)     5306     2658 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/kmeans.py
--rw-r--r--   0 onieto    (5306)     5306     2603 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/laesa.py
--rw-r--r--   0 onieto    (5306)     5306     6329 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/nmf.py
--rw-r--r--   0 onieto    (5306)     5306     3188 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/nmfals.py
--rw-r--r--   0 onieto    (5306)     5306     2461 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/nmfnnls.py
--rw-r--r--   0 onieto    (5306)     5306     3887 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/nndsvd.py
--rw-r--r--   0 onieto    (5306)     5306     4037 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/pca.py
--rw-r--r--   0 onieto    (5306)     5306     3736 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/rnmf.py
--rw-r--r--   0 onieto    (5306)     5306     7669 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sivm.py
--rw-r--r--   0 onieto    (5306)     5306     3017 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sivm_cur.py
--rw-r--r--   0 onieto    (5306)     5306     6147 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sivm_gsat.py
--rw-r--r--   0 onieto    (5306)     5306     5400 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sivm_search.py
--rw-r--r--   0 onieto    (5306)     5306     4666 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sivm_sgreedy.py
--rw-r--r--   0 onieto    (5306)     5306     2661 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/snmf.py
--rw-r--r--   0 onieto    (5306)     5306     6821 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/sub.py
--rw-r--r--   0 onieto    (5306)     5306     8152 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/svd.py
--rw-r--r--   0 onieto    (5306)     5306     1024 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/pymf/vol.py
--rw-r--r--   0 onieto    (5306)     5306    13774 2018-06-16 00:07:07.000000 msaf-0.1.70/msaf/run.py
--rw-r--r--   0 onieto    (5306)     5306     7800 2018-05-21 02:43:25.000000 msaf-0.1.70/msaf/utils.py
--rw-r--r--   0 onieto    (5306)     5306       60 2018-06-16 00:37:08.000000 msaf-0.1.70/msaf/version.py
-drwxr-xr-x   0 onieto    (5306)     5306        0 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/
--rw-r--r--   0 onieto    (5306)     5306        1 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/dependency_links.txt
--rw-r--r--   0 onieto    (5306)     5306     1021 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/PKG-INFO
--rw-r--r--   0 onieto    (5306)     5306      210 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/requires.txt
--rw-r--r--   0 onieto    (5306)     5306     2187 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/SOURCES.txt
--rw-r--r--   0 onieto    (5306)     5306        5 2018-06-16 00:40:31.000000 msaf-0.1.70/msaf.egg-info/top_level.txt
--rw-r--r--   0 onieto    (5306)     5306     1021 2018-06-16 00:40:31.000000 msaf-0.1.70/PKG-INFO
--rw-r--r--   0 onieto    (5306)     5306     1617 2018-05-21 02:43:25.000000 msaf-0.1.70/README.md
--rw-r--r--   0 onieto    (5306)     5306       38 2018-06-16 00:40:31.000000 msaf-0.1.70/setup.cfg
--rw-r--r--   0 onieto    (5306)     5306     2059 2018-06-16 00:07:07.000000 msaf-0.1.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.254147 msaf-0.1.80/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-25 10:46:27.000000 msaf-0.1.80/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-25 10:46:27.000000 msaf-0.1.80/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 10:46:38.254147 msaf-0.1.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-25 10:46:27.000000 msaf-0.1.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.230147 msaf-0.1.80/msaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.230147 msaf-0.1.80/msaf/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.234147 msaf-0.1.80/msaf/algorithms/cnmf/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/cnmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/cnmf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/cnmf/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.234147 msaf-0.1.80/msaf/algorithms/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/example/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/example/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.234147 msaf-0.1.80/msaf/algorithms/fmc2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/fmc2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/fmc2d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/fmc2d/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/fmc2d/utils_2dfmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7344 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/fmc2d/xmeans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.238147 msaf-0.1.80/msaf/algorithms/foote/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/foote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/foote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/foote/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.238147 msaf-0.1.80/msaf/algorithms/olda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/OLDA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3844 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/fit_olda_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6210 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/make_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.238147 msaf-0.1.80/msaf/algorithms/olda/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_BeatlesIso.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_BeatlesTUT.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_SALAMI-i.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/olda/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.242147 msaf-0.1.80/msaf/algorithms/scluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/scluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/scluster/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/scluster/main2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/scluster/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.242147 msaf-0.1.80/msaf/algorithms/sf/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/sf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/sf/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.242147 msaf-0.1.80/msaf/algorithms/vmo/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/vmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/vmo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/vmo/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/algorithms/vmo/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20211 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/configdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14890 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.254147 msaf-0.1.80/msaf/pymf/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/aa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/bnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/chnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/cmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/cur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/cursl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/gmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/greedycur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/laesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/nmfals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/nmfnnls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/nndsvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/rnmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sivm_cur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sivm_gsat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sivm_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sivm_sgreedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/snmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/pymf/vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-25 10:46:27.000000 msaf-0.1.80/msaf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.230147 msaf-0.1.80/msaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 10:46:38.000000 msaf-0.1.80/msaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-25 10:46:38.000000 msaf-0.1.80/msaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:46:38.000000 msaf-0.1.80/msaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 10:46:38.000000 msaf-0.1.80/msaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 10:46:38.000000 msaf-0.1.80/msaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 10:46:38.258148 msaf-0.1.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-25 10:46:27.000000 msaf-0.1.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:46:38.254147 msaf-0.1.80/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_fmc2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-25 10:46:27.000000 msaf-0.1.80/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `msaf-0.1.70/msaf/__init__.py` & `msaf-0.1.80/msaf/__init__.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/__init__.py` & `msaf-0.1.80/msaf/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/cnmf/segmenter.py` & `msaf-0.1.80/msaf/algorithms/cnmf/segmenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # coding: utf-8
 import numpy as np
-from scipy.ndimage import filters
+from scipy import ndimage
 
 import msaf.utils as U
 from msaf.algorithms.interface import SegmenterInterface
 from msaf import pymf
 
 
 def median_filter(X, M=8):
     """Median filter along the first axis of the feature matrix X."""
     for i in range(X.shape[1]):
-        X[:, i] = filters.median_filter(X[:, i], size=M)
+        X[:, i] = ndimage.median_filter(X[:, i], size=M)
     return X
 
 
 def cnmf(S, rank, niter=500, hull=False):
     """(Convex) Non-Negative Matrix Factorization.
 
     Parameters
```

### Comparing `msaf-0.1.70/msaf/algorithms/example/segmenter.py` & `msaf-0.1.80/msaf/algorithms/example/segmenter.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/fmc2d/segmenter.py` & `msaf-0.1.80/msaf/algorithms/fmc2d/segmenter.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/fmc2d/utils_2dfmc.py` & `msaf-0.1.80/msaf/algorithms/fmc2d/utils_2dfmc.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/fmc2d/xmeans.py` & `msaf-0.1.80/msaf/algorithms/fmc2d/xmeans.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/foote/config.py` & `msaf-0.1.80/msaf/algorithms/foote/config.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/foote/segmenter.py` & `msaf-0.1.80/msaf/algorithms/foote/segmenter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
 # coding: utf-8
 import librosa
 import logging
 import numpy as np
 from scipy.spatial import distance
-from scipy import signal
-from scipy.ndimage import filters
+from scipy import signal, ndimage
 import pylab as plt
 
 import msaf
 from msaf.algorithms.interface import SegmenterInterface
 
 
 def median_filter(X, M=8):
     """Median filter along the first axis of the feature matrix X."""
     for i in range(X.shape[1]):
-        X[:, i] = filters.median_filter(X[:, i], size=M)
+        X[:, i] = ndimage.median_filter(X[:, i], size=M)
     return X
 
 
 def compute_gaussian_krnl(M):
     """Creates a gaussian kernel following Foote's paper."""
     g = signal.gaussian(M, M // 3., sym=True)
     G = np.dot(g.reshape(-1, 1), g.reshape(1, -1))
@@ -52,18 +51,18 @@
     return nc
 
 
 def pick_peaks(nc, L=16):
     """Obtain peaks from a novelty curve using an adaptive threshold."""
     offset = nc.mean() / 20.
 
-    nc = filters.gaussian_filter1d(nc, sigma=4)  # Smooth out nc
+    nc = ndimage.gaussian_filter1d(nc, sigma=4)  # Smooth out nc
 
-    th = filters.median_filter(nc, size=L) + offset
-    #th = filters.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
+    th = ndimage.median_filter(nc, size=L) + offset
+    #th = ndimage.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
 
     peaks = []
     for i in range(1, nc.shape[0] - 1):
         # is it a peak?
         if nc[i - 1] < nc[i] and nc[i] > nc[i + 1]:
             # is it above the threshold?
             if nc[i] > th[i]:
```

### Comparing `msaf-0.1.70/msaf/algorithms/interface.py` & `msaf-0.1.80/msaf/algorithms/interface.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/config.py` & `msaf-0.1.80/msaf/algorithms/olda/config.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/fit_olda_model.py` & `msaf-0.1.80/msaf/algorithms/olda/fit_olda_model.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/make_train.py` & `msaf-0.1.80/msaf/algorithms/olda/make_train.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_BeatlesIso.npy` & `msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_BeatlesIso.npy`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_BeatlesTUT.npy` & `msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_BeatlesTUT.npy`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/models/EstBeats_SALAMI-i.npy` & `msaf-0.1.80/msaf/algorithms/olda/models/EstBeats_SALAMI-i.npy`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/OLDA.py` & `msaf-0.1.80/msaf/algorithms/olda/OLDA.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/olda/segmenter.py` & `msaf-0.1.80/msaf/algorithms/olda/segmenter.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/scluster/main2.py` & `msaf-0.1.80/msaf/algorithms/scluster/main2.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,14 @@
 
     if config["hier"]:
         est_idxs = []
         est_labels = []
         for k in range(1, config["num_layers"] + 1):
             est_idx, est_label = cluster(embedding, Cnorm, k)
             est_idxs.append(est_idx)
-            est_labels.append(np.asarray(est_label, dtype=np.int))
+            est_labels.append(np.asarray(est_label, dtype=np.int64))
 
     else:
         est_idxs, est_labels = cluster(embedding, Cnorm, config["scluster_k"], in_bound_idxs)
-        est_labels = np.asarray(est_labels, dtype=np.int)
+        est_labels = np.asarray(est_labels, dtype=np.int64)
 
     return est_idxs, est_labels, Cnorm
```

### Comparing `msaf-0.1.70/msaf/algorithms/scluster/segmenter.py` & `msaf-0.1.80/msaf/algorithms/scluster/segmenter.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/sf/config.py` & `msaf-0.1.80/msaf/algorithms/sf/config.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/algorithms/sf/segmenter.py` & `msaf-0.1.80/msaf/algorithms/sf/segmenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #!/usr/bin/env python
 # coding: utf-8
 import librosa
 import logging
 import numpy as np
 from scipy.spatial import distance
-from scipy import signal
-from scipy.ndimage import filters
+from scipy import signal, ndimage
 
 from msaf.algorithms.interface import SegmenterInterface
 import msaf.utils as U
 
 
 def median_filter(X, M=8):
     """Median filter along the first axis of the feature matrix X."""
     for i in range(X.shape[1]):
-        X[:, i] = filters.median_filter(X[:, i], size=M)
+        X[:, i] = ndimage.median_filter(X[:, i], size=M)
     return X
 
 
 def gaussian_filter(X, M=8, axis=0):
     """Gaussian filter along the first axis of the feature matrix X."""
     for i in range(X.shape[axis]):
         if axis == 1:
-            X[:, i] = filters.gaussian_filter(X[:, i], sigma=M / 2.)
+            X[:, i] = ndimage.gaussian_filter(X[:, i], sigma=M / 2.)
         elif axis == 0:
-            X[i, :] = filters.gaussian_filter(X[i, :], sigma=M / 2.)
+            X[i, :] = ndimage.gaussian_filter(X[i, :], sigma=M / 2.)
     return X
 
 
 def compute_gaussian_krnl(M):
     """Creates a gaussian kernel following Serra's paper."""
     g = signal.gaussian(M, M / 3., sym=True)
     G = np.dot(g.reshape(-1, 1), g.reshape(1, -1))
@@ -59,16 +58,16 @@
     nc /= float(nc.max())
     return nc
 
 
 def pick_peaks(nc, L=16, offset_denom=0.1):
     """Obtain peaks from a novelty curve using an adaptive threshold."""
     offset = nc.mean() * float(offset_denom)
-    th = filters.median_filter(nc, size=L) + offset
-    #th = filters.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
+    th = ndimage.median_filter(nc, size=L) + offset
+    #th = ndimage.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
     #import pylab as plt
     #plt.plot(nc)
     #plt.plot(th)
     #plt.show()
     # th = np.ones(nc.shape[0]) * nc.mean() - 0.08
     peaks = []
     for i in range(1, nc.shape[0] - 1):
@@ -142,16 +141,16 @@
         # Check size in case the track is too short
         if F.shape[0] > 20:
 
             if self.framesync:
                 red = 0.1
                 F_copy = np.copy(F)
                 F = librosa.util.utils.sync(
-                    F.T, np.linspace(0, F.shape[0], num=F.shape[0] * red),
-                    pad=False).T
+                         F.T, np.linspace(0, F.shape[0], num=int(F.shape[0] * red), dtype= np.int64),
+                         pad=False).T
 
             # Emedding the feature space (i.e. shingle)
             E = embedded_space(F, m)
             # plt.imshow(E.T, interpolation="nearest", aspect="auto"); plt.show()
 
             # Recurrence matrix
             R = librosa.segment.recurrence_matrix(
@@ -178,15 +177,15 @@
             # Find peaks in the novelty curve
             est_bounds = pick_peaks(nc, L=Mp, offset_denom=od)
 
             # Re-align embedded space
             est_bounds = np.asarray(est_bounds) + int(np.ceil(m / 2.))
 
             if self.framesync:
-                est_bounds /= red
+                est_bounds = np.asarray(est_bounds // red, dtype=np.int64)
                 F = F_copy
         else:
             est_bounds = []
 
         # Add first and last frames
         est_idxs = np.concatenate(([0], est_bounds, [F.shape[0] - 1]))
         est_idxs = np.unique(est_idxs)
```

### Comparing `msaf-0.1.70/msaf/algorithms/vmo/main.py` & `msaf-0.1.80/msaf/algorithms/vmo/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,14 @@
 
     if config["hier"]:
         est_idxs = []
         est_labels = []
         for k in range(1, config["hier_num_layers"] + 1):
             est_idx, est_label = cluster(embedding, Cnorm, k)
             est_idxs.append(est_idx)
-            est_labels.append(np.asarray(est_label, dtype=np.int))
+            est_labels.append(np.asarray(est_label, dtype=np.int64))
 
     else:
         est_idxs, est_labels = cluster(embedding, Cnorm, config["vmo_k"], in_bound_idxs)
-        est_labels = np.asarray(est_labels, dtype=np.int)
+        est_labels = np.asarray(est_labels, dtype=np.int64)
 
     return est_idxs, est_labels, Cnorm
```

### Comparing `msaf-0.1.70/msaf/algorithms/vmo/segmenter.py` & `msaf-0.1.80/msaf/algorithms/vmo/segmenter.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/base.py` & `msaf-0.1.80/msaf/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,28 +347,31 @@
         the global parameters."""
         return [name for name in vars(self) if not name.startswith('_') and
                 name not in self._global_param_names]
 
     def _compute_framesync_times(self):
         """Computes the framesync times based on the framesync features."""
         self._framesync_times = librosa.core.frames_to_time(
-            np.arange(self._framesync_features.shape[0]), self.sr,
-            self.hop_length)
+            np.arange(self._framesync_features.shape[0]), sr=self.sr,
+            hop_length=self.hop_length)
 
     def _compute_all_features(self):
         """Computes all the features (beatsync, framesync) from the audio."""
         # Read actual audio waveform
         self._audio, _ = librosa.load(self.file_struct.audio_file,
                                       sr=self.sr)
 
         # Get duration of audio file
         self.dur = len(self._audio) / float(self.sr)
 
         # Compute actual features
+        feat_type = self.feat_type
+        self.feat_type = FeatureTypes.framesync
         self._framesync_features = self.compute_features()
+        self.feat_type = feat_type
 
         # Compute framesync times
         self._compute_framesync_times()
 
         # Compute/Read beats
         self._est_beats_times, self._est_beats_frames = self.estimate_beats()
         self._ann_beats_times, self._ann_beats_frames = self.read_ann_beats()
```

### Comparing `msaf-0.1.70/msaf/configdefaults.py` & `msaf-0.1.80/msaf/configdefaults.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/configparser.py` & `msaf-0.1.80/msaf/configparser.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/eval.py` & `msaf-0.1.80/msaf/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ----------
     results: pd.DataFrame
         Dataframe with all the results
     """
     if len(results) == 0:
         logging.warning("No results to print!")
         return
-    res = results.mean()
+    res = results.mean(numeric_only=True)
     logging.info("Results:\n%s" % res)
 
 
 def compute_results(ann_inter, est_inter, ann_labels, est_labels, bins,
                     est_file, weight=0.58):
     """Compute the results using all the available evaluations.
 
@@ -379,18 +379,15 @@
         # Evaluate in parallel
         logging.info("Evaluating %d tracks..." % len(file_structs))
         evals = Parallel(n_jobs=n_jobs)(delayed(process_track)(
             file_struct, boundaries_id, labels_id, config,
             annotator_id=annotator_id) for file_struct in file_structs[:])
 
     # Aggregate evaluations in pandas format
-    results = pd.DataFrame()
-    for e in evals:
-        if e != []:
-            results = results.append(e, ignore_index=True)
+    results = pd.DataFrame(evals)
     logging.info("%d tracks analyzed" % len(results))
 
     # Print results
     print_results(results)
 
     # Save all results
     if save:
```

### Comparing `msaf-0.1.70/msaf/exceptions.py` & `msaf-0.1.80/msaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/features.py` & `msaf-0.1.80/msaf/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         Returns
         -------
         mfcc: np.array(N, F)
             The features, each row representing a feature vector for a give
             time frame/beat.
         """
-        S = librosa.feature.melspectrogram(self._audio,
+        S = librosa.feature.melspectrogram(y=self._audio,
                                            sr=self.sr,
                                            n_fft=self.n_fft,
                                            hop_length=self.hop_length,
                                            n_mels=self.n_mels)
         log_S = librosa.amplitude_to_db(S, ref=self.ref_power)
         mfcc = librosa.feature.mfcc(S=log_S, n_mfcc=self.n_mfcc).T
         return mfcc
@@ -338,10 +338,10 @@
 
         Returns
         -------
         tempogram: np.array(N, F)
             The features, each row representing a feature vector for a give
             time frame/beat.
         """
-        return librosa.feature.tempogram(self._audio, sr=self.sr,
+        return librosa.feature.tempogram(y=self._audio, sr=self.sr,
                                          hop_length=self.hop_length,
                                          win_length=self.win_length).T
```

### Comparing `msaf-0.1.70/msaf/input_output.py` & `msaf-0.1.80/msaf/input_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,16 @@
     # Use handy JAMS search interface
     namespace = "multi_segment" if params["hier"] else "segment_open"
     # TODO: This is a workaround to issue in JAMS. Should be
     # resolved in JAMS 0.2.3, but for now, this works too.
     ann = jam.search(namespace=namespace).\
         search(**{"Sandbox.boundaries_id": boundaries_id}).\
         search(**{"Sandbox.labels_id": lambda x:
-                  (isinstance(x, six.string_types) and
+                  (isinstance(labels_id, six.string_types) and
+                   isinstance(x, six.string_types) and
                    re.match(labels_id, x) is not None) or x is None})
     for key, val in zip(params.keys(), params.values()):
         if isinstance(val, six.string_types):
             ann = ann.search(**{"Sandbox.%s" % key: val})
         else:
             ann = ann.search(**{"Sandbox.%s" % key: lambda x: x == val})
```

### Comparing `msaf-0.1.70/msaf/plotting.py` & `msaf-0.1.80/msaf/plotting.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/__init__.py` & `msaf-0.1.80/msaf/pymf/__init__.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/aa.py` & `msaf-0.1.80/msaf/pymf/aa.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/bnmf.py` & `msaf-0.1.80/msaf/pymf/bnmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/chnmf.py` & `msaf-0.1.80/msaf/pymf/chnmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/cmd.py` & `msaf-0.1.80/msaf/pymf/cmd.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/cmeans.py` & `msaf-0.1.80/msaf/pymf/cmeans.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/cnmf.py` & `msaf-0.1.80/msaf/pymf/cnmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/cur.py` & `msaf-0.1.80/msaf/pymf/cur.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/cursl.py` & `msaf-0.1.80/msaf/pymf/cursl.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/dist.py` & `msaf-0.1.80/msaf/pymf/dist.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/gmap.py` & `msaf-0.1.80/msaf/pymf/gmap.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/greedy.py` & `msaf-0.1.80/msaf/pymf/greedy.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/greedycur.py` & `msaf-0.1.80/msaf/pymf/greedycur.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/kmeans.py` & `msaf-0.1.80/msaf/pymf/kmeans.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/laesa.py` & `msaf-0.1.80/msaf/pymf/laesa.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/nmf.py` & `msaf-0.1.80/msaf/pymf/nmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/nmfals.py` & `msaf-0.1.80/msaf/pymf/nmfals.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/nmfnnls.py` & `msaf-0.1.80/msaf/pymf/nmfnnls.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/nndsvd.py` & `msaf-0.1.80/msaf/pymf/nndsvd.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/pca.py` & `msaf-0.1.80/msaf/pymf/pca.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/rnmf.py` & `msaf-0.1.80/msaf/pymf/rnmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/sivm.py` & `msaf-0.1.80/msaf/pymf/sivm.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/sivm_cur.py` & `msaf-0.1.80/msaf/pymf/sivm_cur.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/sivm_gsat.py` & `msaf-0.1.80/msaf/pymf/sivm_gsat.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
             self._logger.info('Volume increased:' + str(self.V))
             return True, s
 
         return False,-1
 
     def update_w(self):
-        n = np.int(np.floor(np.random.random() * self._num_samples))
+        n = np.int64(np.floor(np.random.random() * self._num_samples))
         if n not in self.select:
             updated, s = self.online_update_w(self.data[:,n])
             if updated:
                 self.select[s] = n
                 self._logger.info('Current selection:' + str(self.select))
```

### Comparing `msaf-0.1.70/msaf/pymf/sivm_search.py` & `msaf-0.1.80/msaf/pymf/sivm_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 """
 
 
 import scipy.sparse
 import numpy as np
 from scipy import inf
 try:
-    from scipy.misc.common import factorial
-except:
     from scipy.misc import factorial
+except:
+    from scipy.special import factorial # scipy > 1.3
 
 from .dist import *
 from .vol import *
 from .sivm import SIVM
 
 __all__ = ["SIVM_SEARCH"]
```

### Comparing `msaf-0.1.70/msaf/pymf/sivm_sgreedy.py` & `msaf-0.1.80/msaf/pymf/sivm_sgreedy.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/snmf.py` & `msaf-0.1.80/msaf/pymf/snmf.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/sub.py` & `msaf-0.1.80/msaf/pymf/sub.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/svd.py` & `msaf-0.1.80/msaf/pymf/svd.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/pymf/vol.py` & `msaf-0.1.80/msaf/pymf/vol.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 	simplex_volume(): Ordinary simplex volume
 		
 """
 
 
 import numpy as np
 try:
-	from scipy.misc.common import factorial
-except:
 	from scipy.misc import factorial
+except:
+	from scipy.special import factorial # scipy > 1.3
 
 __all__ = ["cmdet", "simplex"]
 
 def cmdet(d):
 	# compute the CMD determinant of the euclidean distance matrix d
 	# -> d should not be squared!
 	D = np.ones((d.shape[0]+1,d.shape[0]+1))
```

### Comparing `msaf-0.1.70/msaf/run.py` & `msaf-0.1.80/msaf/run.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf/utils.py` & `msaf-0.1.80/msaf/utils.py`

 * *Files identical despite different names*

### Comparing `msaf-0.1.70/msaf.egg-info/PKG-INFO` & `msaf-0.1.80/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: msaf
-Version: 0.1.70
+Version: 0.1.80
 Summary: Python module to discover the structure of music files
 Home-page: https://github.com/urinieto/msaf
+Download-URL: https://github.com/urinieto/msaf/releases
 Author: Oriol Nieto
 Author-email: oriol@nyu.edu
 License: MIT
-Download-URL: https://github.com/urinieto/msaf/releases
-Description: A python module to segment audio into all its different large-scale sections and label them based on their acoustic similarity
 Keywords: audio music sound
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Provides-Extra: resample
+Provides-Extra: tests
+License-File: LICENSE.md
+License-File: AUTHORS.md
+
+A python module to segment audio into all its different large-scale sections and label them based on their acoustic similarity
```

### Comparing `msaf-0.1.70/msaf.egg-info/SOURCES.txt` & `msaf-0.1.80/msaf.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+AUTHORS.md
+LICENSE.md
 README.md
+setup.cfg
 setup.py
 msaf/__init__.py
 msaf/base.py
 msaf/configdefaults.py
 msaf/configparser.py
 msaf/eval.py
 msaf/exceptions.py
@@ -78,8 +81,15 @@
 msaf/pymf/sivm_cur.py
 msaf/pymf/sivm_gsat.py
 msaf/pymf/sivm_search.py
 msaf/pymf/sivm_sgreedy.py
 msaf/pymf/snmf.py
 msaf/pymf/sub.py
 msaf/pymf/svd.py
-msaf/pymf/vol.py
+msaf/pymf/vol.py
+tests/test_config.py
+tests/test_eval.py
+tests/test_features.py
+tests/test_fmc2d.py
+tests/test_input_output.py
+tests/test_run.py
+tests/test_utils.py
```

### Comparing `msaf-0.1.70/PKG-INFO` & `msaf-0.1.80/msaf.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: msaf
-Version: 0.1.70
+Version: 0.1.80
 Summary: Python module to discover the structure of music files
 Home-page: https://github.com/urinieto/msaf
+Download-URL: https://github.com/urinieto/msaf/releases
 Author: Oriol Nieto
 Author-email: oriol@nyu.edu
 License: MIT
-Download-URL: https://github.com/urinieto/msaf/releases
-Description: A python module to segment audio into all its different large-scale sections and label them based on their acoustic similarity
 Keywords: audio music sound
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Provides-Extra: resample
+Provides-Extra: tests
+License-File: LICENSE.md
+License-File: AUTHORS.md
+
+A python module to segment audio into all its different large-scale sections and label them based on their acoustic similarity
```

### Comparing `msaf-0.1.70/README.md` & `msaf-0.1.80/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # Music Structure Analysis Framework #
 
 A Python framework to analyze music structure.
 
-[![PyPI version](https://badge.fury.io/py/msaf.svg)](https://badge.fury.io/py/msaf) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/urinieto/msaf/master/LICENSE.md) [![Code Health](https://landscape.io/github/urinieto/msaf/master/landscape.svg?style=flat)](https://landscape.io/github/urinieto/msaf/master) [![Build Status](https://travis-ci.org/urinieto/msaf.svg?branch=master)](https://travis-ci.org/urinieto/msaf) [![Coverage Status](https://coveralls.io/repos/github/urinieto/msaf/badge.svg?branch=master)](https://coveralls.io/github/urinieto/msaf?branch=master)
+[![PyPI version](https://badge.fury.io/py/msaf.svg)](https://badge.fury.io/py/msaf)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/urinieto/msaf/master/LICENSE.md)
+[![Build Status](https://github.com/urinieto/msaf/actions/workflows/test.yaml/badge.svg)](https://github.com/urinieto/msaf/actions/workflows/test.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/urinieto/msaf/badge.svg?branch=master)](https://coveralls.io/github/urinieto/msaf?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/msaf/badge/?version=latest)](https://msaf.readthedocs.io/en/latest/?badge=latest)
 
 ## Documentation ##
 
-See http://pythonhosted.org/msaf/ for a complete reference manual and introductory tutorials.
+See https://msaf.readthedocs.io for a complete reference manual and introductory tutorials.
 
 ## Installation ##
 
 From the root folder, type:
     
-    pip install msaf
+    pip install .
 
-(Note: you may need to prefix the previous line with `sudo`, depending on your system configuration).
+(Note: you may need to create and activate a Python virtual environment with `python -m venv .venv` and `source .venv/bin/activate` first, depending on your system configuration).
 
 ## Demonstration Notebook ##
 
 You can follow a thorough example on this titanic [Jupyter Notebook](https://github.com/urinieto/msaf/blob/master/examples/Run%20MSAF.ipynb).
 
 ## Citing MSAF ##
 
-Nieto, O., Bello, J. P., Systematic Exploration Of Computational Music Structure Research. Proc. of the 17th International Society for Music Information Retrieval Conference (ISMIR). New York City, NY, USA, 2016 ([PDF](http://marl.smusic.nyu.edu/nieto/publications/ISMIR2016-NietoBello.pdf)).
+Nieto, O., Bello, J. P., Systematic Exploration Of Computational Music Structure Research. Proc. of the 17th International Society for Music Information Retrieval Conference (ISMIR). New York City, NY, USA, 2016 ([PDF](https://ccrma.stanford.edu/~urinieto/MARL/publications/ISMIR2016-NietoBello.pdf)).
 
 ## Credits ##
 
 Created by [Oriol Nieto](http://marl.smusic.nyu.edu/nieto/) (<oriol@nyu.edu>).
```

### Comparing `msaf-0.1.70/setup.py` & `msaf-0.1.80/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from setuptools import setup, find_packages
 import glob
 import imp
-import numpy.distutils.misc_util
 
 version = imp.load_source('msaf.version', 'msaf/version.py')
 
 # MSAF configuration
 setup(
     name='msaf',
     version=version.version,
@@ -34,28 +33,28 @@
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6"
     ],
     keywords='audio music sound',
     license='MIT',
     install_requires=[
         'audioread',
+        'cvxopt',
+        'decorator',
         'enum34',
         'future',
         'jams >= 0.3.0',
-        'numpy >= 1.8.0',
-        'scipy >= 0.13.0',
-        'scikit-learn >= 0.17.0',
-        'seaborn',  # For notebook example (but everyone should have this :-))
-        'matplotlib >= 1.5',
         'joblib',
-        'decorator',
-        'cvxopt',
         'librosa >= 0.6.0',
         'mir_eval',
+        'matplotlib >= 1.5',
+        'numpy >= 1.8.0',
         'pandas',
+        'scikit-learn >= 0.17.0',
+        'scipy >= 0.13.0',
+        'seaborn',  # For notebook example (but everyone should have this :-))
         'vmo >= 0.3.3'
     ],
     extras_require={
-        'resample': 'scikits.samplerate>=0.3'
-    },
-    include_dirs=numpy.distutils.misc_util.get_numpy_include_dirs()
+        'resample': 'scikits.samplerate>=0.3',
+        'tests': ['pytest', 'pytest-cov']
+    }
 )
```

