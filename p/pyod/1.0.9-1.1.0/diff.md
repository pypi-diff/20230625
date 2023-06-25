# Comparing `tmp/pyod-1.0.9.tar.gz` & `tmp/pyod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyod-1.0.9.tar", last modified: Mon Mar 20 01:13:23 2023, max compression
+gzip compressed data, was "pyod-1.1.0.tar", last modified: Sun Jun 25 06:00:23 2023, max compression
```

## Comparing `pyod-1.0.9.tar` & `pyod-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 01:13:23.212607 pyod-1.0.9/
--rw-rw-rw-   0        0        0     1313 2023-03-20 01:12:56.000000 pyod-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      106 2023-03-20 01:12:56.000000 pyod-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0    42880 2023-03-20 01:13:23.213607 pyod-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    41057 2023-03-20 01:12:56.000000 pyod-1.0.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-20 01:13:23.154094 pyod-1.0.9/pyod/
--rw-rw-rw-   0        0        0      134 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 01:13:23.205608 pyod-1.0.9/pyod/models/
--rw-rw-rw-   0        0        0      701 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/__init__.py
--rw-rw-rw-   0        0        0     9918 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/abod.py
--rw-rw-rw-   0        0        0    24031 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/alad.py
--rw-rw-rw-   0        0        0    16485 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/anogan.py
--rw-rw-rw-   0        0        0    11087 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/auto_encoder.py
--rw-rw-rw-   0        0        0    15366 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/auto_encoder_torch.py
--rw-rw-rw-   0        0        0    20759 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/base.py
--rw-rw-rw-   0        0        0      720 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/base_dl.py
--rw-rw-rw-   0        0        0    13423 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/cblof.py
--rw-rw-rw-   0        0        0     5860 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/cd.py
--rw-rw-rw-   0        0        0     8614 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/cof.py
--rw-rw-rw-   0        0        0     5717 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/combination.py
--rw-rw-rw-   0        0        0    10364 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/copod.py
--rw-rw-rw-   0        0        0    12159 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/deep_svdd.py
--rw-rw-rw-   0        0        0    10493 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/ecod.py
--rw-rw-rw-   0        0        0    15681 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/feature_bagging.py
--rw-rw-rw-   0        0        0     2574 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/gaal_base.py
--rw-rw-rw-   0        0        0     9512 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/gmm.py
--rw-rw-rw-   0        0        0    13758 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/hbos.py
--rw-rw-rw-   0        0        0    13303 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/iforest.py
--rw-rw-rw-   0        0        0     9494 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/inne.py
--rw-rw-rw-   0        0        0     6322 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/kde.py
--rw-rw-rw-   0        0        0    10540 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/knn.py
--rw-rw-rw-   0        0        0    14856 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/kpca.py
--rw-rw-rw-   0        0        0     8285 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/lmdd.py
--rw-rw-rw-   0        0        0     8167 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/loci.py
--rw-rw-rw-   0        0        0     7918 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/loda.py
--rw-rw-rw-   0        0        0     9250 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/lof.py
--rw-rw-rw-   0        0        0    15690 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/lscp.py
--rw-rw-rw-   0        0        0    12581 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/lunar.py
--rw-rw-rw-   0        0        0     5298 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/mad.py
--rw-rw-rw-   0        0        0     8595 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/mcd.py
--rw-rw-rw-   0        0        0    10785 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/mo_gaal.py
--rw-rw-rw-   0        0        0     8352 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/ocsvm.py
--rw-rw-rw-   0        0        0    14866 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/pca.py
--rw-rw-rw-   0        0        0     5191 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/qmcd.py
--rw-rw-rw-   0        0        0    23604 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/rgraph.py
--rw-rw-rw-   0        0        0    16659 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/rod.py
--rw-rw-rw-   0        0        0     6624 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/sampling.py
--rw-rw-rw-   0        0        0     3621 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/sklearn_base.py
--rw-rw-rw-   0        0        0     7670 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/so_gaal.py
--rw-rw-rw-   0        0        0     7024 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/sod.py
--rw-rw-rw-   0        0        0    10383 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/sos.py
--rw-rw-rw-   0        0        0    10517 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/suod.py
--rw-rw-rw-   0        0        0    22599 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/thresholds.py
--rw-rw-rw-   0        0        0    14081 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/vae.py
--rw-rw-rw-   0        0        0    16394 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/models/xgbod.py
-drwxrwxrwx   0        0        0        0 2023-03-20 01:13:23.211608 pyod-1.0.9/pyod/utils/
--rw-rw-rw-   0        0        0      884 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/__init__.py
--rw-rw-rw-   0        0        0    23674 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/data.py
--rw-rw-rw-   0        0        0     6685 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/example.py
--rw-rw-rw-   0        0        0     7630 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/stat_models.py
--rw-rw-rw-   0        0        0      319 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/torch_utility.py
--rw-rw-rw-   0        0        0    17061 2023-03-20 01:12:59.000000 pyod-1.0.9/pyod/utils/utility.py
--rw-rw-rw-   0        0        0      579 2023-03-20 01:12:58.000000 pyod-1.0.9/pyod/version.py
-drwxrwxrwx   0        0        0        0 2023-03-20 01:13:23.159094 pyod-1.0.9/pyod.egg-info/
--rw-rw-rw-   0        0        0    42880 2023-03-20 01:13:23.000000 pyod-1.0.9/pyod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1397 2023-03-20 01:13:23.000000 pyod-1.0.9/pyod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 01:13:23.000000 pyod-1.0.9/pyod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-03-20 01:13:23.000000 pyod-1.0.9/pyod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-20 01:13:23.000000 pyod-1.0.9/pyod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       79 2023-03-20 01:12:56.000000 pyod-1.0.9/requirements.txt
--rw-rw-rw-   0        0        0       87 2023-03-20 01:13:23.213607 pyod-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2030 2023-03-20 01:12:56.000000 pyod-1.0.9/setup.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-06-25 06:00:23.069427 pyod-1.1.0/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     1313 2023-06-25 05:56:54.000000 pyod-1.1.0/LICENSE
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      106 2023-06-25 05:56:54.000000 pyod-1.1.0/MANIFEST.in
+-rw-r--r--   0 yuezhao    (501) staff       (20)    49916 2023-06-25 06:00:23.069540 pyod-1.1.0/PKG-INFO
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    48763 2023-06-25 05:56:54.000000 pyod-1.1.0/README.rst
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-06-25 06:00:23.058949 pyod-1.1.0/pyod/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      134 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/__init__.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-06-25 06:00:23.067642 pyod-1.1.0/pyod/models/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      701 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/__init__.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     9918 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/abod.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    24031 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/alad.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    16485 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/anogan.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    11087 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/auto_encoder.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    15366 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/auto_encoder_torch.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    20721 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/base.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      720 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/base_dl.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    13423 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/cblof.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     5879 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/cd.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     8614 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/cof.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     5717 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/combination.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10364 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/copod.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    12159 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/deep_svdd.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10493 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/ecod.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    15681 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/feature_bagging.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     2574 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/gaal_base.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     9512 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/gmm.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    13758 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/hbos.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    13303 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/iforest.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     9494 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/inne.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     6322 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/kde.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10540 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/knn.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    14856 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/kpca.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     8285 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/lmdd.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     8167 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/loci.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     7918 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/loda.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     9250 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/lof.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    15690 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/lscp.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    12581 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/lunar.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     5298 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/mad.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     8595 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/mcd.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10785 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/mo_gaal.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     8352 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/ocsvm.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    14866 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/pca.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     5191 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/qmcd.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    23604 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/rgraph.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    16659 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/rod.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     6624 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/sampling.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     3621 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/sklearn_base.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     7670 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/so_gaal.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     7024 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/sod.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10383 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/sos.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    10517 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/suod.py
+-rwxr-xr-x   0 yuezhao    (501) staff       (20)    24352 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/thresholds.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    14081 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/vae.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    16394 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/models/xgbod.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-06-25 06:00:23.069161 pyod-1.1.0/pyod/utils/
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      884 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/__init__.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    23674 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/data.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     6685 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/example.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     7630 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/stat_models.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      319 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/torch_utility.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)    17061 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/utils/utility.py
+-rw-rw-r--   0 yuezhao    (501) staff       (20)      579 2023-06-25 05:56:54.000000 pyod-1.1.0/pyod/version.py
+drwxr-xr-x   0 yuezhao    (501) staff       (20)        0 2023-06-25 06:00:23.059595 pyod-1.1.0/pyod.egg-info/
+-rw-r--r--   0 yuezhao    (501) staff       (20)    49916 2023-06-25 06:00:22.000000 pyod-1.1.0/pyod.egg-info/PKG-INFO
+-rw-r--r--   0 yuezhao    (501) staff       (20)     1397 2023-06-25 06:00:22.000000 pyod-1.1.0/pyod.egg-info/SOURCES.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)        1 2023-06-25 06:00:22.000000 pyod-1.1.0/pyod.egg-info/dependency_links.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)       80 2023-06-25 06:00:22.000000 pyod-1.1.0/pyod.egg-info/requires.txt
+-rw-r--r--   0 yuezhao    (501) staff       (20)       14 2023-06-25 06:00:22.000000 pyod-1.1.0/pyod.egg-info/top_level.txt
+-rw-rw-r--   0 yuezhao    (501) staff       (20)       79 2023-06-25 05:56:54.000000 pyod-1.1.0/requirements.txt
+-rw-rw-r--   0 yuezhao    (501) staff       (20)       80 2023-06-25 06:00:23.069787 pyod-1.1.0/setup.cfg
+-rw-rw-r--   0 yuezhao    (501) staff       (20)     2030 2023-06-25 05:56:54.000000 pyod-1.1.0/setup.py
```

### Comparing `pyod-1.0.9/LICENSE` & `pyod-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/PKG-INFO` & `pyod-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,670 +1,724 @@
-Metadata-Version: 2.1
-Name: pyod
-Version: 1.0.9
-Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
-Home-page: https://github.com/yzhao062/pyod
-Author: Yue Zhao
-Author-email: zhaoy@cmu.edu
-License: UNKNOWN
-Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
-Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Python Outlier Detection (PyOD)
-===============================
-
-**Deployment & Documentation & Stats & License**
-
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
-   :target: https://pypi.org/project/pyod/
-   :alt: PyPI version
-
-
-.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
-   :target: https://anaconda.org/conda-forge/pyod
-   :alt: Anaconda version
-
-
-.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
-   :target: https://pyod.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation status
-
-
-.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
-   :target: https://github.com/yzhao062/pyod/stargazers
-   :alt: GitHub stars
-
-
-.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
-   :target: https://github.com/yzhao062/pyod/network
-   :alt: GitHub forks
-
-
-.. image:: https://pepy.tech/badge/pyod
-   :target: https://pepy.tech/project/pyod
-   :alt: Downloads
-
-.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
-   :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
-   :alt: testing
-
-
-.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
-   :target: https://coveralls.io/github/yzhao062/pyod
-   :alt: Coverage Status
-
-
-.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
-   :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
-   :alt: Maintainability
-
-
-.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
-   :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
-   :alt: License
-
-.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
-   :target: https://github.com/Minqi824/ADBench
-   :alt: Benchmark
-
-
------
-
-**News**: We just released a 45-page, the most comprehensive `anomaly detection benchmark paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_.
-The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
-
-**For time-series outlier detection**, please use `TODS <https://github.com/datamllab/tods>`_.
-**For graph outlier detection**, please use `PyGOD <https://pygod.org/>`_.
-
-PyOD is the most comprehensive and scalable **Python library** for **detecting outlying objects** in
-multivariate data. This exciting yet challenging field is commonly referred as 
-`Outlier Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_
-or `Anomaly Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_.
-
-PyOD includes more than 40 detection algorithms, from classical LOF (SIGMOD 2000) to
-the latest ECOD (TKDE 2022). Since 2017, PyOD has been successfully used in numerous academic researches and
-commercial products with more than `10 million downloads <https://pepy.tech/project/pyod>`_.
-It is also well acknowledged by the machine learning community with various dedicated posts/tutorials, including
-`Analytics Vidhya <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_,
-`KDnuggets <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, and
-`Towards Data Science <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_.
-
-
-**PyOD is featured for**:
-
-* **Unified APIs, detailed documentation, and interactive examples** across various algorithms.
-* **Advanced models**\, including **classical distance and density estimation**, **latest deep learning methods**, and **emerging algorithms like ECOD**.
-* **Optimized performance with JIT and parallelization** using `numba <https://github.com/numba/numba>`_ and `joblib <https://github.com/joblib/joblib>`_.
-* **Fast training & prediction with SUOD** [#Zhao2021SUOD]_.
-
-
-**Outlier Detection with 5 Lines of Code**\ :
-
-
-.. code-block:: python
-
-
-    # train an ECOD detector
-    from pyod.models.ecod import ECOD
-    clf = ECOD()
-    clf.fit(X_train)
-
-    # get outlier scores
-    y_train_scores = clf.decision_scores_  # raw outlier scores on the train data
-    y_test_scores = clf.decision_function(X_test)  # predict raw outlier scores on test
-
-
-**Personal suggestion on selecting an OD algorithm**. If you do not know which algorithm to try, go with:
-
-- `ECOD <https://github.com/yzhao062/pyod/blob/master/examples/ecod_example.py>`_: Example of using ECOD for outlier detection
-- `Isolation Forest <https://github.com/yzhao062/pyod/blob/master/examples/iforest_example.py>`_: Example of using Isolation Forest for outlier detection
-
-They are both fast and interpretable. Or, you could try more data-driven approach `MetaOD <https://github.com/yzhao062/MetaOD>`_.
-
-**Citing PyOD**\ :
-
-`PyOD paper <http://www.jmlr.org/papers/volume20/19-011/19-011.pdf>`_ is published in
-`Journal of Machine Learning Research (JMLR) <http://www.jmlr.org/>`_ (MLOSS track).
-If you use PyOD in a scientific publication, we would appreciate
-citations to the following paper::
-
-    @article{zhao2019pyod,
-        author  = {Zhao, Yue and Nasrullah, Zain and Li, Zheng},
-        title   = {PyOD: A Python Toolbox for Scalable Outlier Detection},
-        journal = {Journal of Machine Learning Research},
-        year    = {2019},
-        volume  = {20},
-        number  = {96},
-        pages   = {1-7},
-        url     = {http://jmlr.org/papers/v20/19-011.html}
-    }
-
-or::
-
-    Zhao, Y., Nasrullah, Z. and Li, Z., 2019. PyOD: A Python Toolbox for Scalable Outlier Detection. Journal of machine learning research (JMLR), 20(96), pp.1-7.
-
-If you want more general insights of anomaly detection and/or algorithm performance comparison, please see our
-NeurIPS 2022 paper `ADBench: Anomaly Detection Benchmark Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_::
-
-    @inproceedings{han2022adbench,
-        title={ADBench: Anomaly Detection Benchmark},
-        author={Songqiao Han and Xiyang Hu and Hailiang Huang and Mingqi Jiang and Yue Zhao},
-        booktitle={Neural Information Processing Systems (NeurIPS)}
-        year={2022},
-    }
-
-**Key Links and Resources**\ :
-
-
-* `View the latest codes on Github <https://github.com/yzhao062/pyod>`_
-* `Anomaly Detection Resources <https://github.com/yzhao062/anomaly-detection-resources>`_
-
-
-**Table of Contents**\ :
-
-
-* `Installation <#installation>`_
-* `API Cheatsheet & Reference <#api-cheatsheet--reference>`_
-* `ADBench Benchmark <#adbench-benchmark>`_
-* `Model Save & Load <#model-save--load>`_
-* `Fast Train with SUOD <#fast-train-with-suod>`_
-* `Implemented Algorithms <#implemented-algorithms>`_
-* `Quick Start for Outlier Detection <#quick-start-for-outlier-detection>`_
-* `How to Contribute <#how-to-contribute>`_
-* `Inclusion Criteria <#inclusion-criteria>`_
-
-
-----
-
-
-Installation
-^^^^^^^^^^^^
-
-It is recommended to use **pip** or **conda** for installation. Please make sure
-**the latest version** is installed, as PyOD is updated frequently:
-
-.. code-block:: bash
-
-   pip install pyod            # normal install
-   pip install --upgrade pyod  # or update if needed
-
-.. code-block:: bash
-
-   conda install -c conda-forge pyod
-
-Alternatively, you could clone and run setup.py file:
-
-.. code-block:: bash
-
-   git clone https://github.com/yzhao062/pyod.git
-   cd pyod
-   pip install .
-
-
-**Required Dependencies**\ :
-
-
-* Python 3.6+
-* joblib
-* matplotlib
-* numpy>=1.19
-* numba>=0.51
-* scipy>=1.5.1
-* scikit_learn>=0.20.0
-* six
-
-**Optional Dependencies (see details below)**\ :
-
-* combo (optional, required for models/combination.py and FeatureBagging)
-* keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
-* pandas (optional, required for running benchmark)
-* suod (optional, required for running SUOD model)
-* xgboost (optional, required for XGBOD)
-* pythresh to use thresholding
-
-**Warning**\ :
-PyOD has multiple neural network based models, e.g., AutoEncoders, which are
-implemented in both Tensorflow and PyTorch. However, PyOD does **NOT** install these deep learning libraries for you.
-This reduces the risk of interfering with your local copies.
-If you want to use neural-net based models, please make sure these deep learning libraries are installed.
-Instructions are provided: `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_.
-Similarly, models depending on **xgboost**, e.g., XGBOD, would **NOT** enforce xgboost installation by default.
-
-
-
-----
-
-
-API Cheatsheet & Reference
-^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Full API Reference: (https://pyod.readthedocs.io/en/latest/pyod.html). API cheatsheet for all detectors:
-
-
-* **fit(X)**\ : Fit detector. y is ignored in unsupervised methods.
-* **decision_function(X)**\ : Predict raw anomaly score of X using the fitted detector.
-* **predict(X)**\ : Predict if a particular sample is an outlier or not using the fitted detector.
-* **predict_proba(X)**\ : Predict the probability of a sample being outlier using the fitted detector.
-* **predict_confidence(X)**\ : Predict the model's sample-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
-
-
-Key Attributes of a fitted model:
-
-
-* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
-  Outliers tend to have higher scores.
-* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
-
-
-----
-
-
-ADBench Benchmark
-^^^^^^^^^^^^^^^^^
-
-We just released a 45-page, the most comprehensive `ADBench: Anomaly Detection Benchmark <https://arxiv.org/abs/2206.09426>`_ [#Han2022ADBench]_.
-The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
-
-The organization of **ADBench** is provided below:
-
-.. image:: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
-   :target: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
-   :alt: benchmark-fig
-
-
-**The comparison of selected models** is made available below
-(\ `Figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png>`_\ ,
-`compare_all_models.py <https://github.com/yzhao062/pyod/blob/master/examples/compare_all_models.py>`_\ ,
-`Interactive Jupyter Notebooks <https://mybinder.org/v2/gh/yzhao062/pyod/master>`_\ ).
-For Jupyter Notebooks, please navigate to **"/notebooks/Compare All Models.ipynb"**.
-
-
-.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
-   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
-   :alt: Comparision_of_All
-
-
-
-----
-
-Model Save & Load
-^^^^^^^^^^^^^^^^^
-
-PyOD takes a similar approach of sklearn regarding model persistence.
-See `model persistence <https://scikit-learn.org/stable/modules/model_persistence.html>`_ for clarification.
-
-In short, we recommend to use joblib or pickle for saving and loading PyOD models.
-See `"examples/save_load_model_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/save_load_model_example.py>`_ for an example.
-In short, it is simple as below:
-
-.. code-block:: python
-
-    from joblib import dump, load
-
-    # save the model
-    dump(clf, 'clf.joblib')
-    # load the model
-    clf = load('clf.joblib')
-
-It is known that there are challenges in saving neural network models.
-Check `#328 <https://github.com/yzhao062/pyod/issues/328#issuecomment-917192704>`_
-and `#88 <https://github.com/yzhao062/pyod/issues/88#issuecomment-615343139>`_
-for temporary workaround.
-
-
-----
-
-
-Fast Train with SUOD
-^^^^^^^^^^^^^^^^^^^^
-
-**Fast training and prediction**: it is possible to train and predict with
-a large number of detection models in PyOD by leveraging SUOD framework [#Zhao2021SUOD]_.
-See  `SUOD Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/21-mlsys-suod.pdf>`_
-and  `SUOD example <https://github.com/yzhao062/pyod/blob/master/examples/suod_example.py>`_.
-
-
-.. code-block:: python
-
-    from pyod.models.suod import SUOD
-
-    # initialized a group of outlier detectors for acceleration
-    detector_list = [LOF(n_neighbors=15), LOF(n_neighbors=20),
-                     LOF(n_neighbors=25), LOF(n_neighbors=35),
-                     COPOD(), IForest(n_estimators=100),
-                     IForest(n_estimators=200)]
-
-    # decide the number of parallel process, and the combination method
-    # then clf can be used as any outlier detection model
-    clf = SUOD(base_estimators=detector_list, n_jobs=2, combination='average',
-               verbose=False)
-
-
-
-
-----
-
-
-
-Implemented Algorithms
-^^^^^^^^^^^^^^^^^^^^^^
-
-PyOD toolkit consists of three major functional groups:
-
-**(i) Individual Detection Algorithms** :
-
-===================  ==================  ======================================================================================================  =====  ========================================
-Type                 Abbr                Algorithm                                                                                               Year   Ref
-===================  ==================  ======================================================================================================  =====  ========================================
-Probabilistic        ECOD                Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions                        2022   [#Li2021ECOD]_
-Probabilistic        ABOD                Angle-Based Outlier Detection                                                                           2008   [#Kriegel2008Angle]_
-Probabilistic        FastABOD            Fast Angle-Based Outlier Detection using approximation                                                  2008   [#Kriegel2008Angle]_
-Probabilistic        COPOD               COPOD: Copula-Based Outlier Detection                                                                   2020   [#Li2020COPOD]_
-Probabilistic        MAD                 Median Absolute Deviation (MAD)                                                                         1993   [#Iglewicz1993How]_
-Probabilistic        SOS                 Stochastic Outlier Selection                                                                            2012   [#Janssens2012Stochastic]_
-Probabilistic        QMCD                Quasi-Monte Carlo Discrepancy outlier detection                                                         2001   [#Fang2001Wrap]_
-Probabilistic        KDE                 Outlier Detection with Kernel Density Functions                                                         2007   [#Latecki2007Outlier]_
-Probabilistic        Sampling            Rapid distance-based outlier detection via sampling                                                     2013   [#Sugiyama2013Rapid]_
-Probabilistic        GMM                 Probabilistic Mixture Modeling for Outlier Analysis                                                            [#Aggarwal2015Outlier]_ [Ch.2]
-Linear Model         PCA                 Principal Component Analysis (the sum of weighted projected distances to the eigenvector hyperplanes)   2003   [#Shyu2003A]_
-Linear Model         KPCA                Kernel Principal Component Analysis                                                                     2007   [#Hoffmann2007Kernel]_
-Linear Model         MCD                 Minimum Covariance Determinant (use the mahalanobis distances as the outlier scores)                    1999   [#Hardin2004Outlier]_ [#Rousseeuw1999A]_
-Linear Model         CD                  Use Cook's distance for outlier detection                                                               1977   [#Cook1977Detection]_
-Linear Model         OCSVM               One-Class Support Vector Machines                                                                       2001   [#Scholkopf2001Estimating]_
-Linear Model         LMDD                Deviation-based Outlier Detection (LMDD)                                                                1996   [#Arning1996A]_
-Proximity-Based      LOF                 Local Outlier Factor                                                                                    2000   [#Breunig2000LOF]_
-Proximity-Based      COF                 Connectivity-Based Outlier Factor                                                                       2002   [#Tang2002Enhancing]_
-Proximity-Based      (Incremental) COF   Memory Efficient Connectivity-Based Outlier Factor (slower but reduce storage complexity)               2002   [#Tang2002Enhancing]_
-Proximity-Based      CBLOF               Clustering-Based Local Outlier Factor                                                                   2003   [#He2003Discovering]_
-Proximity-Based      LOCI                LOCI: Fast outlier detection using the local correlation integral                                       2003   [#Papadimitriou2003LOCI]_
-Proximity-Based      HBOS                Histogram-based Outlier Score                                                                           2012   [#Goldstein2012Histogram]_
-Proximity-Based      kNN                 k Nearest Neighbors (use the distance to the kth nearest neighbor as the outlier score)                 2000   [#Ramaswamy2000Efficient]_
-Proximity-Based      AvgKNN              Average kNN (use the average distance to k nearest neighbors as the outlier score)                      2002   [#Angiulli2002Fast]_
-Proximity-Based      MedKNN              Median kNN (use the median distance to k nearest neighbors as the outlier score)                        2002   [#Angiulli2002Fast]_
-Proximity-Based      SOD                 Subspace Outlier Detection                                                                              2009   [#Kriegel2009Outlier]_
-Proximity-Based      ROD                 Rotation-based Outlier Detection                                                                        2020   [#Almardeny2020A]_
-Outlier Ensembles    IForest             Isolation Forest                                                                                        2008   [#Liu2008Isolation]_
-Outlier Ensembles    INNE                Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                      2018   [#Bandaragoda2018Isolation]_
-Outlier Ensembles    FB                  Feature Bagging                                                                                         2005   [#Lazarevic2005Feature]_
-Outlier Ensembles    LSCP                LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                       2019   [#Zhao2019LSCP]_
-Outlier Ensembles    XGBOD               Extreme Boosting Based Outlier Detection **(Supervised)**                                               2018   [#Zhao2018XGBOD]_
-Outlier Ensembles    LODA                Lightweight On-line Detector of Anomalies                                                               2016   [#Pevny2016Loda]_
-Outlier Ensembles    SUOD                SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**          2021   [#Zhao2021SUOD]_
-Neural Networks      AutoEncoder         Fully connected AutoEncoder (use reconstruction error as the outlier score)                                    [#Aggarwal2015Outlier]_ [Ch.3]
-Neural Networks      VAE                 Variational AutoEncoder (use reconstruction error as the outlier score)                                 2013   [#Kingma2013Auto]_
-Neural Networks      Beta-VAE            Variational AutoEncoder (all customized loss term by varying gamma and capacity)                        2018   [#Burgess2018Understanding]_
-Neural Networks      SO_GAAL             Single-Objective Generative Adversarial Active Learning                                                 2019   [#Liu2019Generative]_
-Neural Networks      MO_GAAL             Multiple-Objective Generative Adversarial Active Learning                                               2019   [#Liu2019Generative]_
-Neural Networks      DeepSVDD            Deep One-Class Classification                                                                           2018   [#Ruff2018Deep]_
-Neural Networks      AnoGAN              Anomaly Detection with Generative Adversarial Networks                                                  2017   [#Schlegl2017Unsupervised]_
-Neural Networks      ALAD                Adversarially learned anomaly detection                                                                 2018   [#Zenati2018Adversarially]_
-Graph-based          R-Graph             Outlier detection by R-graph                                                                            2017   [#You2017Provable]_
-Graph-based          LUNAR               LUNAR: Unifying Local Outlier Detection Methods via Graph Neural Networks                               2022   [#Goodge2022Lunar]_
-===================  ==================  ======================================================================================================  =====  ========================================
-
-
-**(ii) Outlier Ensembles & Outlier Detector Combination Frameworks**:
-
-===================  ================  =====================================================================================================  =====  ========================================
-Type                 Abbr              Algorithm                                                                                              Year   Ref
-===================  ================  =====================================================================================================  =====  ========================================
-Outlier Ensembles    FB                Feature Bagging                                                                                        2005   [#Lazarevic2005Feature]_
-Outlier Ensembles    LSCP              LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                      2019   [#Zhao2019LSCP]_
-Outlier Ensembles    XGBOD             Extreme Boosting Based Outlier Detection **(Supervised)**                                              2018   [#Zhao2018XGBOD]_
-Outlier Ensembles    LODA              Lightweight On-line Detector of Anomalies                                                              2016   [#Pevny2016Loda]_
-Outlier Ensembles    SUOD              SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**         2021   [#Zhao2021SUOD]_
-Outlier Ensembles    INNE              Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                     2018   [#Bandaragoda2018Isolation]_
-Combination          Average           Simple combination by averaging the scores                                                             2015   [#Aggarwal2015Theoretical]_
-Combination          Weighted Average  Simple combination by averaging the scores with detector weights                                       2015   [#Aggarwal2015Theoretical]_
-Combination          Maximization      Simple combination by taking the maximum scores                                                        2015   [#Aggarwal2015Theoretical]_
-Combination          AOM               Average of Maximum                                                                                     2015   [#Aggarwal2015Theoretical]_
-Combination          MOA               Maximization of Average                                                                                2015   [#Aggarwal2015Theoretical]_
-Combination          Median            Simple combination by taking the median of the scores                                                  2015   [#Aggarwal2015Theoretical]_
-Combination          majority Vote     Simple combination by taking the majority vote of the labels (weights can be used)                     2015   [#Aggarwal2015Theoretical]_
-===================  ================  =====================================================================================================  =====  ========================================
-
-
-**(iii) Utility Functions**:
-
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-Type                 Name                    Function                                                                                                                                               Documentation
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-Data                 generate_data           Synthesized data generation; normal data is generated by a multivariate Gaussian and outliers are generated by a uniform distribution                  `generate_data <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.data.generate_data>`_
-Data                 generate_data_clusters  Synthesized data generation in clusters; more complex data patterns can be created with multiple clusters                                              `generate_data_clusters <https://pyod.readthedocs.io/en/latest/pyod.utils.html#pyod.utils.data.generate_data_clusters>`_
-Stat                 wpearsonr               Calculate the weighted Pearson correlation of two samples                                                                                              `wpearsonr <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.stat_models.wpearsonr>`_
-Utility              get_label_n             Turn raw outlier scores into binary labels by assign 1 to top n outlier scores                                                                         `get_label_n <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.get_label_n>`_
-Utility              precision_n_scores      calculate precision @ rank n                                                                                                                           `precision_n_scores <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.precision_n_scores>`_
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-
-----
-
-Quick Start for Outlier Detection
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-PyOD has been well acknowledged by the machine learning community with a few featured posts and tutorials.
-
-**Analytics Vidhya**: `An Awesome Tutorial to Learn Outlier Detection in Python using PyOD Library <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_
-
-**KDnuggets**: `Intuitive Visualization of Outlier Detection Methods <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, `An Overview of Outlier Detection Methods from PyOD <https://www.kdnuggets.com/2019/06/overview-outlier-detection-methods-pyod.html>`_
-
-**Towards Data Science**: `Anomaly Detection for Dummies <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_
-
-**Computer Vision News (March 2019)**: `Python Open Source Toolbox for Outlier Detection <https://rsipvision.com/ComputerVisionNews-2019March/18/>`_
-
-`"examples/knn_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/knn_example.py>`_
-demonstrates the basic API of using kNN detector. **It is noted that the API across all other algorithms are consistent/similar**.
-
-More detailed instructions for running examples can be found in `examples directory <https://github.com/yzhao062/pyod/blob/master/examples>`_.
-
-
-#. Initialize a kNN detector, fit the model, and make the prediction.
-
-   .. code-block:: python
-
-
-       from pyod.models.knn import KNN   # kNN detector
-
-       # train kNN detector
-       clf_name = 'KNN'
-       clf = KNN()
-       clf.fit(X_train)
-
-       # get the prediction label and outlier scores of the training data
-       y_train_pred = clf.labels_  # binary labels (0: inliers, 1: outliers)
-       y_train_scores = clf.decision_scores_  # raw outlier scores
-
-       # get the prediction on the test data
-       y_test_pred = clf.predict(X_test)  # outlier labels (0 or 1)
-       y_test_scores = clf.decision_function(X_test)  # outlier scores
-
-       # it is possible to get the prediction confidence as well
-       y_test_pred, y_test_pred_confidence = clf.predict(X_test, return_confidence=True)  # outlier labels (0 or 1) and confidence in the range of [0,1]
-
-#. Evaluate the prediction by ROC and Precision @ Rank n (p@n).
-
-   .. code-block:: python
-
-       from pyod.utils.data import evaluate_print
-       
-       # evaluate and print the results
-       print("\nOn Training Data:")
-       evaluate_print(clf_name, y_train, y_train_scores)
-       print("\nOn Test Data:")
-       evaluate_print(clf_name, y_test, y_test_scores)
-
-
-#. See a sample output & visualization.
-
-
-   .. code-block:: python
-
-
-       On Training Data:
-       KNN ROC:1.0, precision @ rank n:1.0
-
-       On Test Data:
-       KNN ROC:0.9989, precision @ rank n:0.9
-
-   .. code-block:: python
-
-
-       visualize(clf_name, X_train, y_train, X_test, y_test, y_train_pred,
-           y_test_pred, show_figure=True, save_figure=False)
-
-Visualization (\ `knn_figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png>`_\ ):
-
-.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
-   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
-   :alt: kNN example figure
-
-----
-
-How to Contribute
-^^^^^^^^^^^^^^^^^
-
-You are welcome to contribute to this exciting project:
-
-
-* Please first check Issue lists for "help wanted" tag and comment the one
-  you are interested. We will assign the issue to you.
-
-* Fork the master branch and add your improvement/modification/fix.
-
-* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-
-* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
-
-
-To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
-
-You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
-
-
-Inclusion Criteria
-^^^^^^^^^^^^^^^^^^
-
-Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
-We mainly consider well-established algorithms for inclusion.
-A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
-
-However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
-for boosting ML accessibility and reproducibility.
-This exception only applies if you could commit to the maintenance of your model for at least two year period.
-
-
-----
-
-Reference
-^^^^^^^^^
-
-
-.. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
-
-.. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
-
-.. [#Aggarwal2017Outlier] Aggarwal, C.C. and Sathe, S., 2017. Outlier ensembles: An introduction. Springer.
-
-.. [#Almardeny2020A] Almardeny, Y., Boujnah, N. and Cleary, F., 2020. A Novel Outlier Detection Method for Multivariate Data. *IEEE Transactions on Knowledge and Data Engineering*.
-
-.. [#Angiulli2002Fast] Angiulli, F. and Pizzuti, C., 2002, August. Fast outlier detection in high dimensional spaces. In *European Conference on Principles of Data Mining and Knowledge Discovery* pp. 15-27.
-
-.. [#Arning1996A] Arning, A., Agrawal, R. and Raghavan, P., 1996, August. A Linear Method for Deviation Detection in Large Databases. In *KDD* (Vol. 1141, No. 50, pp. 972-981).
-
-.. [#Bandaragoda2018Isolation] Bandaragoda, T. R., Ting, K. M., Albrecht, D., Liu, F. T., Zhu, Y., and Wells, J. R., 2018, Isolation-based anomaly detection using nearest-neighbor ensembles. *Computational Intelligence*\ , 34(4), pp. 968-998.
-
-.. [#Breunig2000LOF] Breunig, M.M., Kriegel, H.P., Ng, R.T. and Sander, J., 2000, May. LOF: identifying density-based local outliers. *ACM Sigmod Record*\ , 29(2), pp. 93-104.
-
-.. [#Burgess2018Understanding] Burgess, Christopher P., et al. "Understanding disentangling in beta-VAE." arXiv preprint arXiv:1804.03599 (2018).
-
-.. [#Cook1977Detection] Cook, R.D., 1977. Detection of influential observation in linear regression. Technometrics, 19(1), pp.15-18.
-
-.. [#Fang2001Wrap] Fang, K.T. and Ma, C.X., 2001. Wrap-around L2-discrepancy of random sampling, Latin hypercube and uniform designs. Journal of complexity, 17(4), pp.608-624.
-
-.. [#Goldstein2012Histogram] Goldstein, M. and Dengel, A., 2012. Histogram-based outlier score (hbos): A fast unsupervised anomaly detection algorithm. In *KI-2012: Poster and Demo Track*\ , pp.59-63.
-
-.. [#Goodge2022Lunar] Goodge, A., Hooi, B., Ng, S.K. and Ng, W.S., 2022, June. Lunar: Unifying local outlier detection methods via graph neural networks. In Proceedings of the AAAI Conference on Artificial Intelligence.
-
-.. [#Gopalan2019PIDForest] Gopalan, P., Sharan, V. and Wieder, U., 2019. PIDForest: Anomaly Detection via Partial Identification. In Advances in Neural Information Processing Systems, pp. 15783-15793.
-
-.. [#Han2022ADBench] Han, S., Hu, X., Huang, H., Jiang, M. and Zhao, Y., 2022. ADBench: Anomaly Detection Benchmark. arXiv preprint arXiv:2206.09426.
-
-.. [#Hardin2004Outlier] Hardin, J. and Rocke, D.M., 2004. Outlier detection in the multiple cluster setting using the minimum covariance determinant estimator. *Computational Statistics & Data Analysis*\ , 44(4), pp.625-638.
-
-.. [#He2003Discovering] He, Z., Xu, X. and Deng, S., 2003. Discovering cluster-based local outliers. *Pattern Recognition Letters*\ , 24(9-10), pp.1641-1650.
-
-.. [#Hoffmann2007Kernel] Hoffmann, H., 2007. Kernel PCA for novelty detection. Pattern recognition, 40(3), pp.863-874.
-
-.. [#Iglewicz1993How] Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
-
-.. [#Janssens2012Stochastic] Janssens, J.H.M., Huszár, F., Postma, E.O. and van den Herik, H.J., 2012. Stochastic outlier selection. Technical report TiCC TR 2012-001, Tilburg University, Tilburg Center for Cognition and Communication, Tilburg, The Netherlands.
-
-.. [#Kingma2013Auto] Kingma, D.P. and Welling, M., 2013. Auto-encoding variational bayes. arXiv preprint arXiv:1312.6114.
-
-.. [#Kriegel2008Angle] Kriegel, H.P. and Zimek, A., 2008, August. Angle-based outlier detection in high-dimensional data. In *KDD '08*\ , pp. 444-452. ACM.
-
-.. [#Kriegel2009Outlier] Kriegel, H.P., Kröger, P., Schubert, E. and Zimek, A., 2009, April. Outlier detection in axis-parallel subspaces of high dimensional data. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*\ , pp. 831-838. Springer, Berlin, Heidelberg.
-
-.. [#Latecki2007Outlier] Latecki, L.J., Lazarevic, A. and Pokrajac, D., 2007, July. Outlier detection with kernel density functions. In International Workshop on Machine Learning and Data Mining in Pattern Recognition (pp. 61-75). Springer, Berlin, Heidelberg.
-
-.. [#Lazarevic2005Feature] Lazarevic, A. and Kumar, V., 2005, August. Feature bagging for outlier detection. In *KDD '05*. 2005.
-
-.. [#Li2019MADGAN] Li, D., Chen, D., Jin, B., Shi, L., Goh, J. and Ng, S.K., 2019, September. MAD-GAN: Multivariate anomaly detection for time series data with generative adversarial networks. In *International Conference on Artificial Neural Networks* (pp. 703-716). Springer, Cham.
-
-.. [#Li2020COPOD] Li, Z., Zhao, Y., Botta, N., Ionescu, C. and Hu, X. COPOD: Copula-Based Outlier Detection. *IEEE International Conference on Data Mining (ICDM)*, 2020.
-
-.. [#Li2021ECOD] Li, Z., Zhao, Y., Hu, X., Botta, N., Ionescu, C. and Chen, H. G. ECOD: Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions. *IEEE Transactions on Knowledge and Data Engineering (TKDE)*, 2022.
-
-.. [#Liu2008Isolation] Liu, F.T., Ting, K.M. and Zhou, Z.H., 2008, December. Isolation forest. In *International Conference on Data Mining*\ , pp. 413-422. IEEE.
-
-.. [#Liu2019Generative] Liu, Y., Li, Z., Zhou, C., Jiang, Y., Sun, J., Wang, M. and He, X., 2019. Generative adversarial active learning for unsupervised outlier detection. *IEEE Transactions on Knowledge and Data Engineering*.
-
-.. [#Papadimitriou2003LOCI] Papadimitriou, S., Kitagawa, H., Gibbons, P.B. and Faloutsos, C., 2003, March. LOCI: Fast outlier detection using the local correlation integral. In *ICDE '03*, pp. 315-326. IEEE.
-
-.. [#Pevny2016Loda] Pevný, T., 2016. Loda: Lightweight on-line detector of anomalies. *Machine Learning*, 102(2), pp.275-304.
-
-.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
-
-.. [#Ramaswamy2000Efficient] Ramaswamy, S., Rastogi, R. and Shim, K., 2000, May. Efficient algorithms for mining outliers from large data sets. *ACM Sigmod Record*\ , 29(2), pp. 427-438.
-
-.. [#Rousseeuw1999A] Rousseeuw, P.J. and Driessen, K.V., 1999. A fast algorithm for the minimum covariance determinant estimator. *Technometrics*\ , 41(3), pp.212-223.
-
-.. [#Ruff2018Deep] Ruff, L., Vandermeulen, R., Goernitz, N., Deecke, L., Siddiqui, S.A., Binder, A., Müller, E. and Kloft, M., 2018, July. Deep one-class classification. In *International conference on machine learning* (pp. 4393-4402). PMLR.
-
-.. [#Schlegl2017Unsupervised] Schlegl, T., Seeböck, P., Waldstein, S.M., Schmidt-Erfurth, U. and Langs, G., 2017, June. Unsupervised anomaly detection with generative adversarial networks to guide marker discovery. In International conference on information processing in medical imaging (pp. 146-157). Springer, Cham.
-
-.. [#Scholkopf2001Estimating] Scholkopf, B., Platt, J.C., Shawe-Taylor, J., Smola, A.J. and Williamson, R.C., 2001. Estimating the support of a high-dimensional distribution. *Neural Computation*, 13(7), pp.1443-1471.
-
-.. [#Shyu2003A] Shyu, M.L., Chen, S.C., Sarinnapakorn, K. and Chang, L., 2003. A novel anomaly detection scheme based on principal component classifier. *MIAMI UNIV CORAL GABLES FL DEPT OF ELECTRICAL AND COMPUTER ENGINEERING*.
-
-.. [#Sugiyama2013Rapid] Sugiyama, M. and Borgwardt, K., 2013. Rapid distance-based outlier detection via sampling. Advances in neural information processing systems, 26.
-
-.. [#Tang2002Enhancing] Tang, J., Chen, Z., Fu, A.W.C. and Cheung, D.W., 2002, May. Enhancing effectiveness of outlier detections for low density patterns. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*, pp. 535-548. Springer, Berlin, Heidelberg.
-
-.. [#Wang2020adVAE] Wang, X., Du, Y., Lin, S., Cui, P., Shen, Y. and Yang, Y., 2019. adVAE: A self-adversarial variational autoencoder with Gaussian anomaly prior knowledge for anomaly detection. *Knowledge-Based Systems*.
-
-.. [#You2017Provable] You, C., Robinson, D.P. and Vidal, R., 2017. Provable self-representation based outlier detection in a union of subspaces. In Proceedings of the IEEE conference on computer vision and pattern recognition.
-
-.. [#Zenati2018Adversarially] Zenati, H., Romain, M., Foo, C.S., Lecouat, B. and Chandrasekhar, V., 2018, November. Adversarially learned anomaly detection. In 2018 IEEE International conference on data mining (ICDM) (pp. 727-736). IEEE.
-
-.. [#Zhao2018XGBOD] Zhao, Y. and Hryniewicki, M.K. XGBOD: Improving Supervised Outlier Detection with Unsupervised Representation Learning. *IEEE International Joint Conference on Neural Networks*\ , 2018.
-
-.. [#Zhao2019LSCP] Zhao, Y., Nasrullah, Z., Hryniewicki, M.K. and Li, Z., 2019, May. LSCP: Locally selective combination in parallel outlier ensembles. In *Proceedings of the 2019 SIAM International Conference on Data Mining (SDM)*, pp. 585-593. Society for Industrial and Applied Mathematics.
-
-.. [#Zhao2021SUOD] Zhao, Y., Hu, X., Cheng, C., Wang, C., Wan, C., Wang, W., Yang, J., Bai, H., Li, Z., Xiao, C., Wang, Y., Qiao, Z., Sun, J. and Akoglu, L. (2021). SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection. *Conference on Machine Learning and Systems (MLSys)*.
-
-
+Metadata-Version: 2.1
+Name: pyod
+Version: 1.1.0
+Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
+Home-page: https://github.com/yzhao062/pyod
+Author: Yue Zhao
+Author-email: zhaoy@cmu.edu
+License: UNKNOWN
+Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
+Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Python Outlier Detection (PyOD)
+===============================
+
+**Deployment & Documentation & Stats & License**
+
+.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
+   :target: https://pypi.org/project/pyod/
+   :alt: PyPI version
+
+
+.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
+   :target: https://anaconda.org/conda-forge/pyod
+   :alt: Anaconda version
+
+
+.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
+   :target: https://pyod.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation status
+
+
+.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
+   :target: https://github.com/yzhao062/pyod/stargazers
+   :alt: GitHub stars
+
+
+.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
+   :target: https://github.com/yzhao062/pyod/network
+   :alt: GitHub forks
+
+
+.. image:: https://pepy.tech/badge/pyod
+   :target: https://pepy.tech/project/pyod
+   :alt: Downloads
+
+.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
+   :alt: testing
+
+
+.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
+   :target: https://coveralls.io/github/yzhao062/pyod
+   :alt: Coverage Status
+
+
+.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
+   :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
+   :alt: Maintainability
+
+
+.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
+   :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
+   :alt: License
+
+.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
+   :target: https://github.com/Minqi824/ADBench
+   :alt: Benchmark
+
+
+-----
+
+**News**: We just released a 45-page, the most comprehensive `anomaly detection benchmark paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_.
+The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
+
+**For time-series outlier detection**, please use `TODS <https://github.com/datamllab/tods>`_.
+**For graph outlier detection**, please use `PyGOD <https://pygod.org/>`_.
+
+PyOD is the most comprehensive and scalable **Python library** for **detecting outlying objects** in
+multivariate data. This exciting yet challenging field is commonly referred as 
+`Outlier Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_
+or `Anomaly Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_.
+
+PyOD includes more than 40 detection algorithms, from classical LOF (SIGMOD 2000) to
+the latest ECOD (TKDE 2022). Since 2017, PyOD has been successfully used in numerous academic researches and
+commercial products with more than `10 million downloads <https://pepy.tech/project/pyod>`_.
+It is also well acknowledged by the machine learning community with various dedicated posts/tutorials, including
+`Analytics Vidhya <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_,
+`KDnuggets <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, and
+`Towards Data Science <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_.
+
+
+**PyOD is featured for**:
+
+* **Unified APIs, detailed documentation, and interactive examples** across various algorithms.
+* **Advanced models**\, including **classical distance and density estimation**, **latest deep learning methods**, and **emerging algorithms like ECOD**.
+* **Optimized performance with JIT and parallelization** using `numba <https://github.com/numba/numba>`_ and `joblib <https://github.com/joblib/joblib>`_.
+* **Fast training & prediction with SUOD** [#Zhao2021SUOD]_.
+
+
+**Outlier Detection with 5 Lines of Code**\ :
+
+
+.. code-block:: python
+
+
+    # train an ECOD detector
+    from pyod.models.ecod import ECOD
+    clf = ECOD()
+    clf.fit(X_train)
+
+    # get outlier scores
+    y_train_scores = clf.decision_scores_  # raw outlier scores on the train data
+    y_test_scores = clf.decision_function(X_test)  # predict raw outlier scores on test
+
+
+**Personal suggestion on selecting an OD algorithm**. If you do not know which algorithm to try, go with:
+
+- `ECOD <https://github.com/yzhao062/pyod/blob/master/examples/ecod_example.py>`_: Example of using ECOD for outlier detection
+- `Isolation Forest <https://github.com/yzhao062/pyod/blob/master/examples/iforest_example.py>`_: Example of using Isolation Forest for outlier detection
+
+They are both fast and interpretable. Or, you could try more data-driven approach `MetaOD <https://github.com/yzhao062/MetaOD>`_.
+
+**Citing PyOD**\ :
+
+`PyOD paper <http://www.jmlr.org/papers/volume20/19-011/19-011.pdf>`_ is published in
+`Journal of Machine Learning Research (JMLR) <http://www.jmlr.org/>`_ (MLOSS track).
+If you use PyOD in a scientific publication, we would appreciate
+citations to the following paper::
+
+    @article{zhao2019pyod,
+        author  = {Zhao, Yue and Nasrullah, Zain and Li, Zheng},
+        title   = {PyOD: A Python Toolbox for Scalable Outlier Detection},
+        journal = {Journal of Machine Learning Research},
+        year    = {2019},
+        volume  = {20},
+        number  = {96},
+        pages   = {1-7},
+        url     = {http://jmlr.org/papers/v20/19-011.html}
+    }
+
+or::
+
+    Zhao, Y., Nasrullah, Z. and Li, Z., 2019. PyOD: A Python Toolbox for Scalable Outlier Detection. Journal of machine learning research (JMLR), 20(96), pp.1-7.
+
+If you want more general insights of anomaly detection and/or algorithm performance comparison, please see our
+NeurIPS 2022 paper `ADBench: Anomaly Detection Benchmark Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_::
+
+    @inproceedings{han2022adbench,
+        title={ADBench: Anomaly Detection Benchmark},
+        author={Songqiao Han and Xiyang Hu and Hailiang Huang and Mingqi Jiang and Yue Zhao},
+        booktitle={Neural Information Processing Systems (NeurIPS)}
+        year={2022},
+    }
+
+**Key Links and Resources**\ :
+
+
+* `View the latest codes on Github <https://github.com/yzhao062/pyod>`_
+* `Anomaly Detection Resources <https://github.com/yzhao062/anomaly-detection-resources>`_
+
+
+**Table of Contents**\ :
+
+
+* `Installation <#installation>`_
+* `API Cheatsheet & Reference <#api-cheatsheet--reference>`_
+* `ADBench Benchmark <#adbench-benchmark>`_
+* `Model Save & Load <#model-save--load>`_
+* `Fast Train with SUOD <#fast-train-with-suod>`_
+* `Thresholding Outlier Scores <#thresholding-outlier-scores>`_
+* `Implemented Algorithms <#implemented-algorithms>`_
+* `Quick Start for Outlier Detection <#quick-start-for-outlier-detection>`_
+* `How to Contribute <#how-to-contribute>`_
+* `Inclusion Criteria <#inclusion-criteria>`_
+
+
+----
+
+
+Installation
+^^^^^^^^^^^^
+
+It is recommended to use **pip** or **conda** for installation. Please make sure
+**the latest version** is installed, as PyOD is updated frequently:
+
+.. code-block:: bash
+
+   pip install pyod            # normal install
+   pip install --upgrade pyod  # or update if needed
+
+.. code-block:: bash
+
+   conda install -c conda-forge pyod
+
+Alternatively, you could clone and run setup.py file:
+
+.. code-block:: bash
+
+   git clone https://github.com/yzhao062/pyod.git
+   cd pyod
+   pip install .
+
+
+**Required Dependencies**\ :
+
+
+* Python 3.6+
+* joblib
+* matplotlib
+* numpy>=1.19
+* numba>=0.51
+* scipy>=1.5.1
+* scikit_learn>=0.20.0
+* six
+
+**Optional Dependencies (see details below)**\ :
+
+* combo (optional, required for models/combination.py and FeatureBagging)
+* keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
+* pandas (optional, required for running benchmark)
+* suod (optional, required for running SUOD model)
+* xgboost (optional, required for XGBOD)
+* pythresh to use thresholding
+
+**Warning**\ :
+PyOD has multiple neural network based models, e.g., AutoEncoders, which are
+implemented in both Tensorflow and PyTorch. However, PyOD does **NOT** install these deep learning libraries for you.
+This reduces the risk of interfering with your local copies.
+If you want to use neural-net based models, please make sure these deep learning libraries are installed.
+Instructions are provided: `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_.
+Similarly, models depending on **xgboost**, e.g., XGBOD, would **NOT** enforce xgboost installation by default.
+
+
+
+----
+
+
+API Cheatsheet & Reference
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Full API Reference: (https://pyod.readthedocs.io/en/latest/pyod.html). API cheatsheet for all detectors:
+
+
+* **fit(X)**\ : Fit detector. y is ignored in unsupervised methods.
+* **decision_function(X)**\ : Predict raw anomaly score of X using the fitted detector.
+* **predict(X)**\ : Predict if a particular sample is an outlier or not using the fitted detector.
+* **predict_proba(X)**\ : Predict the probability of a sample being outlier using the fitted detector.
+* **predict_confidence(X)**\ : Predict the model's sample-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
+
+
+Key Attributes of a fitted model:
+
+
+* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
+  Outliers tend to have higher scores.
+* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
+
+
+----
+
+
+ADBench Benchmark
+^^^^^^^^^^^^^^^^^
+
+We just released a 45-page, the most comprehensive `ADBench: Anomaly Detection Benchmark <https://arxiv.org/abs/2206.09426>`_ [#Han2022ADBench]_.
+The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
+
+The organization of **ADBench** is provided below:
+
+.. image:: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
+   :target: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
+   :alt: benchmark-fig
+
+
+**The comparison of selected models** is made available below
+(\ `Figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png>`_\ ,
+`compare_all_models.py <https://github.com/yzhao062/pyod/blob/master/examples/compare_all_models.py>`_\ ,
+`Interactive Jupyter Notebooks <https://mybinder.org/v2/gh/yzhao062/pyod/master>`_\ ).
+For Jupyter Notebooks, please navigate to **"/notebooks/Compare All Models.ipynb"**.
+
+
+.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
+   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
+   :alt: Comparision_of_All
+
+
+
+----
+
+Model Save & Load
+^^^^^^^^^^^^^^^^^
+
+PyOD takes a similar approach of sklearn regarding model persistence.
+See `model persistence <https://scikit-learn.org/stable/modules/model_persistence.html>`_ for clarification.
+
+In short, we recommend to use joblib or pickle for saving and loading PyOD models.
+See `"examples/save_load_model_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/save_load_model_example.py>`_ for an example.
+In short, it is simple as below:
+
+.. code-block:: python
+
+    from joblib import dump, load
+
+    # save the model
+    dump(clf, 'clf.joblib')
+    # load the model
+    clf = load('clf.joblib')
+
+It is known that there are challenges in saving neural network models.
+Check `#328 <https://github.com/yzhao062/pyod/issues/328#issuecomment-917192704>`_
+and `#88 <https://github.com/yzhao062/pyod/issues/88#issuecomment-615343139>`_
+for temporary workaround.
+
+
+----
+
+
+Fast Train with SUOD
+^^^^^^^^^^^^^^^^^^^^
+
+**Fast training and prediction**: it is possible to train and predict with
+a large number of detection models in PyOD by leveraging SUOD framework [#Zhao2021SUOD]_.
+See  `SUOD Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/21-mlsys-suod.pdf>`_
+and  `SUOD example <https://github.com/yzhao062/pyod/blob/master/examples/suod_example.py>`_.
+
+
+.. code-block:: python
+
+    from pyod.models.suod import SUOD
+
+    # initialized a group of outlier detectors for acceleration
+    detector_list = [LOF(n_neighbors=15), LOF(n_neighbors=20),
+                     LOF(n_neighbors=25), LOF(n_neighbors=35),
+                     COPOD(), IForest(n_estimators=100),
+                     IForest(n_estimators=200)]
+
+    # decide the number of parallel process, and the combination method
+    # then clf can be used as any outlier detection model
+    clf = SUOD(base_estimators=detector_list, n_jobs=2, combination='average',
+               verbose=False)
+
+----
+
+Thresholding Outlier Scores
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+A more data based approach can be taken when setting the contamination level.
+By using a thresholding method, guessing an abritrary value can be replaced
+with tested techniques for seperating inliers and outliers. Refer to 
+`PyThresh <https://github.com/KulikDM/pythresh>`_ for
+a more in depth look at thresholding.
+
+
+.. code-block:: python
+
+    from pyod.models.knn import KNN
+    from pyod.models.thresholds import FILTER
+
+    # Set the outlier detection and thresholding methods
+    clf = KNN(contamination=FILTER())
+
+
+----
+
+
+
+Implemented Algorithms
+^^^^^^^^^^^^^^^^^^^^^^
+
+PyOD toolkit consists of four major functional groups:
+
+**(i) Individual Detection Algorithms** :
+
+===================  ==================  ======================================================================================================  =====  ========================================
+Type                 Abbr                Algorithm                                                                                               Year   Ref
+===================  ==================  ======================================================================================================  =====  ========================================
+Probabilistic        ECOD                Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions                        2022   [#Li2021ECOD]_
+Probabilistic        ABOD                Angle-Based Outlier Detection                                                                           2008   [#Kriegel2008Angle]_
+Probabilistic        FastABOD            Fast Angle-Based Outlier Detection using approximation                                                  2008   [#Kriegel2008Angle]_
+Probabilistic        COPOD               COPOD: Copula-Based Outlier Detection                                                                   2020   [#Li2020COPOD]_
+Probabilistic        MAD                 Median Absolute Deviation (MAD)                                                                         1993   [#Iglewicz1993How]_
+Probabilistic        SOS                 Stochastic Outlier Selection                                                                            2012   [#Janssens2012Stochastic]_
+Probabilistic        QMCD                Quasi-Monte Carlo Discrepancy outlier detection                                                         2001   [#Fang2001Wrap]_
+Probabilistic        KDE                 Outlier Detection with Kernel Density Functions                                                         2007   [#Latecki2007Outlier]_
+Probabilistic        Sampling            Rapid distance-based outlier detection via sampling                                                     2013   [#Sugiyama2013Rapid]_
+Probabilistic        GMM                 Probabilistic Mixture Modeling for Outlier Analysis                                                            [#Aggarwal2015Outlier]_ [Ch.2]
+Linear Model         PCA                 Principal Component Analysis (the sum of weighted projected distances to the eigenvector hyperplanes)   2003   [#Shyu2003A]_
+Linear Model         KPCA                Kernel Principal Component Analysis                                                                     2007   [#Hoffmann2007Kernel]_
+Linear Model         MCD                 Minimum Covariance Determinant (use the mahalanobis distances as the outlier scores)                    1999   [#Hardin2004Outlier]_ [#Rousseeuw1999A]_
+Linear Model         CD                  Use Cook's distance for outlier detection                                                               1977   [#Cook1977Detection]_
+Linear Model         OCSVM               One-Class Support Vector Machines                                                                       2001   [#Scholkopf2001Estimating]_
+Linear Model         LMDD                Deviation-based Outlier Detection (LMDD)                                                                1996   [#Arning1996A]_
+Proximity-Based      LOF                 Local Outlier Factor                                                                                    2000   [#Breunig2000LOF]_
+Proximity-Based      COF                 Connectivity-Based Outlier Factor                                                                       2002   [#Tang2002Enhancing]_
+Proximity-Based      (Incremental) COF   Memory Efficient Connectivity-Based Outlier Factor (slower but reduce storage complexity)               2002   [#Tang2002Enhancing]_
+Proximity-Based      CBLOF               Clustering-Based Local Outlier Factor                                                                   2003   [#He2003Discovering]_
+Proximity-Based      LOCI                LOCI: Fast outlier detection using the local correlation integral                                       2003   [#Papadimitriou2003LOCI]_
+Proximity-Based      HBOS                Histogram-based Outlier Score                                                                           2012   [#Goldstein2012Histogram]_
+Proximity-Based      kNN                 k Nearest Neighbors (use the distance to the kth nearest neighbor as the outlier score)                 2000   [#Ramaswamy2000Efficient]_
+Proximity-Based      AvgKNN              Average kNN (use the average distance to k nearest neighbors as the outlier score)                      2002   [#Angiulli2002Fast]_
+Proximity-Based      MedKNN              Median kNN (use the median distance to k nearest neighbors as the outlier score)                        2002   [#Angiulli2002Fast]_
+Proximity-Based      SOD                 Subspace Outlier Detection                                                                              2009   [#Kriegel2009Outlier]_
+Proximity-Based      ROD                 Rotation-based Outlier Detection                                                                        2020   [#Almardeny2020A]_
+Outlier Ensembles    IForest             Isolation Forest                                                                                        2008   [#Liu2008Isolation]_
+Outlier Ensembles    INNE                Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                      2018   [#Bandaragoda2018Isolation]_
+Outlier Ensembles    FB                  Feature Bagging                                                                                         2005   [#Lazarevic2005Feature]_
+Outlier Ensembles    LSCP                LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                       2019   [#Zhao2019LSCP]_
+Outlier Ensembles    XGBOD               Extreme Boosting Based Outlier Detection **(Supervised)**                                               2018   [#Zhao2018XGBOD]_
+Outlier Ensembles    LODA                Lightweight On-line Detector of Anomalies                                                               2016   [#Pevny2016Loda]_
+Outlier Ensembles    SUOD                SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**          2021   [#Zhao2021SUOD]_
+Neural Networks      AutoEncoder         Fully connected AutoEncoder (use reconstruction error as the outlier score)                                    [#Aggarwal2015Outlier]_ [Ch.3]
+Neural Networks      VAE                 Variational AutoEncoder (use reconstruction error as the outlier score)                                 2013   [#Kingma2013Auto]_
+Neural Networks      Beta-VAE            Variational AutoEncoder (all customized loss term by varying gamma and capacity)                        2018   [#Burgess2018Understanding]_
+Neural Networks      SO_GAAL             Single-Objective Generative Adversarial Active Learning                                                 2019   [#Liu2019Generative]_
+Neural Networks      MO_GAAL             Multiple-Objective Generative Adversarial Active Learning                                               2019   [#Liu2019Generative]_
+Neural Networks      DeepSVDD            Deep One-Class Classification                                                                           2018   [#Ruff2018Deep]_
+Neural Networks      AnoGAN              Anomaly Detection with Generative Adversarial Networks                                                  2017   [#Schlegl2017Unsupervised]_
+Neural Networks      ALAD                Adversarially learned anomaly detection                                                                 2018   [#Zenati2018Adversarially]_
+Graph-based          R-Graph             Outlier detection by R-graph                                                                            2017   [#You2017Provable]_
+Graph-based          LUNAR               LUNAR: Unifying Local Outlier Detection Methods via Graph Neural Networks                               2022   [#Goodge2022Lunar]_
+===================  ==================  ======================================================================================================  =====  ========================================
+
+
+**(ii) Outlier Ensembles & Outlier Detector Combination Frameworks**:
+
+===================  ================  =====================================================================================================  =====  ========================================
+Type                 Abbr              Algorithm                                                                                              Year   Ref
+===================  ================  =====================================================================================================  =====  ========================================
+Outlier Ensembles    FB                Feature Bagging                                                                                        2005   [#Lazarevic2005Feature]_
+Outlier Ensembles    LSCP              LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                      2019   [#Zhao2019LSCP]_
+Outlier Ensembles    XGBOD             Extreme Boosting Based Outlier Detection **(Supervised)**                                              2018   [#Zhao2018XGBOD]_
+Outlier Ensembles    LODA              Lightweight On-line Detector of Anomalies                                                              2016   [#Pevny2016Loda]_
+Outlier Ensembles    SUOD              SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**         2021   [#Zhao2021SUOD]_
+Outlier Ensembles    INNE              Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                     2018   [#Bandaragoda2018Isolation]_
+Combination          Average           Simple combination by averaging the scores                                                             2015   [#Aggarwal2015Theoretical]_
+Combination          Weighted Average  Simple combination by averaging the scores with detector weights                                       2015   [#Aggarwal2015Theoretical]_
+Combination          Maximization      Simple combination by taking the maximum scores                                                        2015   [#Aggarwal2015Theoretical]_
+Combination          AOM               Average of Maximum                                                                                     2015   [#Aggarwal2015Theoretical]_
+Combination          MOA               Maximization of Average                                                                                2015   [#Aggarwal2015Theoretical]_
+Combination          Median            Simple combination by taking the median of the scores                                                  2015   [#Aggarwal2015Theoretical]_
+Combination          majority Vote     Simple combination by taking the majority vote of the labels (weights can be used)                     2015   [#Aggarwal2015Theoretical]_
+===================  ================  =====================================================================================================  =====  ========================================
+
+**(iii) Outlier Detection Score Thresholding Methods**:
+
+==================================  ================  ================================================================ ====================================================================================================================
+Type                                Abbr              Algorithm                                                        Documentation                                    
+==================================  ================  ================================================================ ====================================================================================================================
+Kernel-Based                        AUCP              Area Under Curve Percentage                                      `AUCP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.AUCP>`_
+Statistical Moment-Based            BOOT              Bootstrapping                                                    `BOOT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.BOOT>`_ 
+Normality-Based                     CHAU              Chauvenet's Criterion                                            `CHAU <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CHAU>`_
+Linear Model                        CLF               Trained Linear Classifier                                        `CLF <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLF>`_
+cluster-Based                       CLUST             Clustering Based                                                 `CLUST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLUST>`_
+Kernel-Based                        CPD               Change Point Detection                                           `CPD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CPD>`_
+Transformation-Based                DECOMP            Decomposition                                                    `DECOMP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DECOMP>`_
+Normality-Based                     DSN               Distance Shift from Normal                                       `DSN <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DSN>`_
+Curve-Based                         EB                Elliptical Boundary                                              `EB <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.EB>`_
+Kernel-Based                        FGD               Fixed Gradient Descent                                           `FGD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FGD>`_
+Filter-Based                        FILTER            Filtering Based                                                  `FILTER <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FILTER>`_
+Curve-Based                         FWFM              Full Width at Full Minimum                                       `FWFM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FWFM>`_
+Statistical Test-Based              GESD              Generalized Extreme Studentized Deviate                          `GESD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.GESD>`_
+Filter-Based                        HIST              Histogram Based                                                  `HIST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.HIST>`_
+Quantile-Based                      IQR               Inter-Quartile Region                                            `IQR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.IQR>`_
+Statistical Moment-Based            KARCH             Karcher mean (Riemannian Center of Mass)                         `KARCH <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.KARCH>`_
+Statistical Moment-Based            MAD               Median Absolute Deviation                                        `MAD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MAD>`_
+Statistical Test-Based              MCST              Monte Carlo Shapiro Tests                                        `MCST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MCST>`_
+Ensembles-Based                     META              Meta-model Trained Classifier                                    `META <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.META>`_
+Transformation-Based                MOLL              Friedrichs' Mollifier                                            `MOLL <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MOLL>`_
+Statistical Test-Based              MTT               Modified Thompson Tau Test                                       `MTT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MTT>`_
+Linear Model                        OCSVM             One-Class Support Vector Machine                                 `OCSVM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.OCSVM>`_
+Quantile-Based                      QMCD              Quasi-Monte Carlo Discrepancy                                    `QMCD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.QMCD>`_
+Linear Model                        REGR              Regression Based                                                 `REGR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.REGR>`_
+Neural Networks                     VAE               Variational Autoencoder                                          `VAE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.VAE>`_
+Curve-Based                         WIND              Topological Winding Number                                       `WIND <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.WIND>`_
+Transformation-Based                YJ                Yeo-Johnson Transformation                                       `YJ <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.YJ>`_
+Normality-Based                     ZSCORE            Z-score                                                          `ZSCORE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.ZSCORE>`_
+==================================  ================  ================================================================ ====================================================================================================================
+
+
+**(iV) Utility Functions**:
+
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+Type                 Name                    Function                                                                                                                                               Documentation
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+Data                 generate_data           Synthesized data generation; normal data is generated by a multivariate Gaussian and outliers are generated by a uniform distribution                  `generate_data <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.data.generate_data>`_
+Data                 generate_data_clusters  Synthesized data generation in clusters; more complex data patterns can be created with multiple clusters                                              `generate_data_clusters <https://pyod.readthedocs.io/en/latest/pyod.utils.html#pyod.utils.data.generate_data_clusters>`_
+Stat                 wpearsonr               Calculate the weighted Pearson correlation of two samples                                                                                              `wpearsonr <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.stat_models.wpearsonr>`_
+Utility              get_label_n             Turn raw outlier scores into binary labels by assign 1 to top n outlier scores                                                                         `get_label_n <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.get_label_n>`_
+Utility              precision_n_scores      calculate precision @ rank n                                                                                                                           `precision_n_scores <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.precision_n_scores>`_
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+
+----
+
+Quick Start for Outlier Detection
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+PyOD has been well acknowledged by the machine learning community with a few featured posts and tutorials.
+
+**Analytics Vidhya**: `An Awesome Tutorial to Learn Outlier Detection in Python using PyOD Library <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_
+
+**KDnuggets**: `Intuitive Visualization of Outlier Detection Methods <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, `An Overview of Outlier Detection Methods from PyOD <https://www.kdnuggets.com/2019/06/overview-outlier-detection-methods-pyod.html>`_
+
+**Towards Data Science**: `Anomaly Detection for Dummies <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_
+
+**Computer Vision News (March 2019)**: `Python Open Source Toolbox for Outlier Detection <https://rsipvision.com/ComputerVisionNews-2019March/18/>`_
+
+`"examples/knn_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/knn_example.py>`_
+demonstrates the basic API of using kNN detector. **It is noted that the API across all other algorithms are consistent/similar**.
+
+More detailed instructions for running examples can be found in `examples directory <https://github.com/yzhao062/pyod/blob/master/examples>`_.
+
+
+#. Initialize a kNN detector, fit the model, and make the prediction.
+
+   .. code-block:: python
+
+
+       from pyod.models.knn import KNN   # kNN detector
+
+       # train kNN detector
+       clf_name = 'KNN'
+       clf = KNN()
+       clf.fit(X_train)
+
+       # get the prediction label and outlier scores of the training data
+       y_train_pred = clf.labels_  # binary labels (0: inliers, 1: outliers)
+       y_train_scores = clf.decision_scores_  # raw outlier scores
+
+       # get the prediction on the test data
+       y_test_pred = clf.predict(X_test)  # outlier labels (0 or 1)
+       y_test_scores = clf.decision_function(X_test)  # outlier scores
+
+       # it is possible to get the prediction confidence as well
+       y_test_pred, y_test_pred_confidence = clf.predict(X_test, return_confidence=True)  # outlier labels (0 or 1) and confidence in the range of [0,1]
+
+#. Evaluate the prediction by ROC and Precision @ Rank n (p@n).
+
+   .. code-block:: python
+
+       from pyod.utils.data import evaluate_print
+       
+       # evaluate and print the results
+       print("\nOn Training Data:")
+       evaluate_print(clf_name, y_train, y_train_scores)
+       print("\nOn Test Data:")
+       evaluate_print(clf_name, y_test, y_test_scores)
+
+
+#. See a sample output & visualization.
+
+
+   .. code-block:: python
+
+
+       On Training Data:
+       KNN ROC:1.0, precision @ rank n:1.0
+
+       On Test Data:
+       KNN ROC:0.9989, precision @ rank n:0.9
+
+   .. code-block:: python
+
+
+       visualize(clf_name, X_train, y_train, X_test, y_test, y_train_pred,
+           y_test_pred, show_figure=True, save_figure=False)
+
+Visualization (\ `knn_figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png>`_\ ):
+
+.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
+   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
+   :alt: kNN example figure
+
+----
+
+How to Contribute
+^^^^^^^^^^^^^^^^^
+
+You are welcome to contribute to this exciting project:
+
+
+* Please first check Issue lists for "help wanted" tag and comment the one
+  you are interested. We will assign the issue to you.
+
+* Fork the master branch and add your improvement/modification/fix.
+
+* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
+
+* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
+
+
+To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
+
+You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
+
+
+Inclusion Criteria
+^^^^^^^^^^^^^^^^^^
+
+Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
+We mainly consider well-established algorithms for inclusion.
+A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
+
+However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
+for boosting ML accessibility and reproducibility.
+This exception only applies if you could commit to the maintenance of your model for at least two year period.
+
+
+----
+
+Reference
+^^^^^^^^^
+
+
+.. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
+
+.. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
+
+.. [#Aggarwal2017Outlier] Aggarwal, C.C. and Sathe, S., 2017. Outlier ensembles: An introduction. Springer.
+
+.. [#Almardeny2020A] Almardeny, Y., Boujnah, N. and Cleary, F., 2020. A Novel Outlier Detection Method for Multivariate Data. *IEEE Transactions on Knowledge and Data Engineering*.
+
+.. [#Angiulli2002Fast] Angiulli, F. and Pizzuti, C., 2002, August. Fast outlier detection in high dimensional spaces. In *European Conference on Principles of Data Mining and Knowledge Discovery* pp. 15-27.
+
+.. [#Arning1996A] Arning, A., Agrawal, R. and Raghavan, P., 1996, August. A Linear Method for Deviation Detection in Large Databases. In *KDD* (Vol. 1141, No. 50, pp. 972-981).
+
+.. [#Bandaragoda2018Isolation] Bandaragoda, T. R., Ting, K. M., Albrecht, D., Liu, F. T., Zhu, Y., and Wells, J. R., 2018, Isolation-based anomaly detection using nearest-neighbor ensembles. *Computational Intelligence*\ , 34(4), pp. 968-998.
+
+.. [#Breunig2000LOF] Breunig, M.M., Kriegel, H.P., Ng, R.T. and Sander, J., 2000, May. LOF: identifying density-based local outliers. *ACM Sigmod Record*\ , 29(2), pp. 93-104.
+
+.. [#Burgess2018Understanding] Burgess, Christopher P., et al. "Understanding disentangling in beta-VAE." arXiv preprint arXiv:1804.03599 (2018).
+
+.. [#Cook1977Detection] Cook, R.D., 1977. Detection of influential observation in linear regression. Technometrics, 19(1), pp.15-18.
+
+.. [#Fang2001Wrap] Fang, K.T. and Ma, C.X., 2001. Wrap-around L2-discrepancy of random sampling, Latin hypercube and uniform designs. Journal of complexity, 17(4), pp.608-624.
+
+.. [#Goldstein2012Histogram] Goldstein, M. and Dengel, A., 2012. Histogram-based outlier score (hbos): A fast unsupervised anomaly detection algorithm. In *KI-2012: Poster and Demo Track*\ , pp.59-63.
+
+.. [#Goodge2022Lunar] Goodge, A., Hooi, B., Ng, S.K. and Ng, W.S., 2022, June. Lunar: Unifying local outlier detection methods via graph neural networks. In Proceedings of the AAAI Conference on Artificial Intelligence.
+
+.. [#Gopalan2019PIDForest] Gopalan, P., Sharan, V. and Wieder, U., 2019. PIDForest: Anomaly Detection via Partial Identification. In Advances in Neural Information Processing Systems, pp. 15783-15793.
+
+.. [#Han2022ADBench] Han, S., Hu, X., Huang, H., Jiang, M. and Zhao, Y., 2022. ADBench: Anomaly Detection Benchmark. arXiv preprint arXiv:2206.09426.
+
+.. [#Hardin2004Outlier] Hardin, J. and Rocke, D.M., 2004. Outlier detection in the multiple cluster setting using the minimum covariance determinant estimator. *Computational Statistics & Data Analysis*\ , 44(4), pp.625-638.
+
+.. [#He2003Discovering] He, Z., Xu, X. and Deng, S., 2003. Discovering cluster-based local outliers. *Pattern Recognition Letters*\ , 24(9-10), pp.1641-1650.
+
+.. [#Hoffmann2007Kernel] Hoffmann, H., 2007. Kernel PCA for novelty detection. Pattern recognition, 40(3), pp.863-874.
+
+.. [#Iglewicz1993How] Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
+
+.. [#Janssens2012Stochastic] Janssens, J.H.M., Huszár, F., Postma, E.O. and van den Herik, H.J., 2012. Stochastic outlier selection. Technical report TiCC TR 2012-001, Tilburg University, Tilburg Center for Cognition and Communication, Tilburg, The Netherlands.
+
+.. [#Kingma2013Auto] Kingma, D.P. and Welling, M., 2013. Auto-encoding variational bayes. arXiv preprint arXiv:1312.6114.
+
+.. [#Kriegel2008Angle] Kriegel, H.P. and Zimek, A., 2008, August. Angle-based outlier detection in high-dimensional data. In *KDD '08*\ , pp. 444-452. ACM.
+
+.. [#Kriegel2009Outlier] Kriegel, H.P., Kröger, P., Schubert, E. and Zimek, A., 2009, April. Outlier detection in axis-parallel subspaces of high dimensional data. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*\ , pp. 831-838. Springer, Berlin, Heidelberg.
+
+.. [#Latecki2007Outlier] Latecki, L.J., Lazarevic, A. and Pokrajac, D., 2007, July. Outlier detection with kernel density functions. In International Workshop on Machine Learning and Data Mining in Pattern Recognition (pp. 61-75). Springer, Berlin, Heidelberg.
+
+.. [#Lazarevic2005Feature] Lazarevic, A. and Kumar, V., 2005, August. Feature bagging for outlier detection. In *KDD '05*. 2005.
+
+.. [#Li2019MADGAN] Li, D., Chen, D., Jin, B., Shi, L., Goh, J. and Ng, S.K., 2019, September. MAD-GAN: Multivariate anomaly detection for time series data with generative adversarial networks. In *International Conference on Artificial Neural Networks* (pp. 703-716). Springer, Cham.
+
+.. [#Li2020COPOD] Li, Z., Zhao, Y., Botta, N., Ionescu, C. and Hu, X. COPOD: Copula-Based Outlier Detection. *IEEE International Conference on Data Mining (ICDM)*, 2020.
+
+.. [#Li2021ECOD] Li, Z., Zhao, Y., Hu, X., Botta, N., Ionescu, C. and Chen, H. G. ECOD: Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions. *IEEE Transactions on Knowledge and Data Engineering (TKDE)*, 2022.
+
+.. [#Liu2008Isolation] Liu, F.T., Ting, K.M. and Zhou, Z.H., 2008, December. Isolation forest. In *International Conference on Data Mining*\ , pp. 413-422. IEEE.
+
+.. [#Liu2019Generative] Liu, Y., Li, Z., Zhou, C., Jiang, Y., Sun, J., Wang, M. and He, X., 2019. Generative adversarial active learning for unsupervised outlier detection. *IEEE Transactions on Knowledge and Data Engineering*.
+
+.. [#Papadimitriou2003LOCI] Papadimitriou, S., Kitagawa, H., Gibbons, P.B. and Faloutsos, C., 2003, March. LOCI: Fast outlier detection using the local correlation integral. In *ICDE '03*, pp. 315-326. IEEE.
+
+.. [#Pevny2016Loda] Pevný, T., 2016. Loda: Lightweight on-line detector of anomalies. *Machine Learning*, 102(2), pp.275-304.
+
+.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
+
+.. [#Ramaswamy2000Efficient] Ramaswamy, S., Rastogi, R. and Shim, K., 2000, May. Efficient algorithms for mining outliers from large data sets. *ACM Sigmod Record*\ , 29(2), pp. 427-438.
+
+.. [#Rousseeuw1999A] Rousseeuw, P.J. and Driessen, K.V., 1999. A fast algorithm for the minimum covariance determinant estimator. *Technometrics*\ , 41(3), pp.212-223.
+
+.. [#Ruff2018Deep] Ruff, L., Vandermeulen, R., Goernitz, N., Deecke, L., Siddiqui, S.A., Binder, A., Müller, E. and Kloft, M., 2018, July. Deep one-class classification. In *International conference on machine learning* (pp. 4393-4402). PMLR.
+
+.. [#Schlegl2017Unsupervised] Schlegl, T., Seeböck, P., Waldstein, S.M., Schmidt-Erfurth, U. and Langs, G., 2017, June. Unsupervised anomaly detection with generative adversarial networks to guide marker discovery. In International conference on information processing in medical imaging (pp. 146-157). Springer, Cham.
+
+.. [#Scholkopf2001Estimating] Scholkopf, B., Platt, J.C., Shawe-Taylor, J., Smola, A.J. and Williamson, R.C., 2001. Estimating the support of a high-dimensional distribution. *Neural Computation*, 13(7), pp.1443-1471.
+
+.. [#Shyu2003A] Shyu, M.L., Chen, S.C., Sarinnapakorn, K. and Chang, L., 2003. A novel anomaly detection scheme based on principal component classifier. *MIAMI UNIV CORAL GABLES FL DEPT OF ELECTRICAL AND COMPUTER ENGINEERING*.
+
+.. [#Sugiyama2013Rapid] Sugiyama, M. and Borgwardt, K., 2013. Rapid distance-based outlier detection via sampling. Advances in neural information processing systems, 26.
+
+.. [#Tang2002Enhancing] Tang, J., Chen, Z., Fu, A.W.C. and Cheung, D.W., 2002, May. Enhancing effectiveness of outlier detections for low density patterns. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*, pp. 535-548. Springer, Berlin, Heidelberg.
+
+.. [#Wang2020adVAE] Wang, X., Du, Y., Lin, S., Cui, P., Shen, Y. and Yang, Y., 2019. adVAE: A self-adversarial variational autoencoder with Gaussian anomaly prior knowledge for anomaly detection. *Knowledge-Based Systems*.
+
+.. [#You2017Provable] You, C., Robinson, D.P. and Vidal, R., 2017. Provable self-representation based outlier detection in a union of subspaces. In Proceedings of the IEEE conference on computer vision and pattern recognition.
+
+.. [#Zenati2018Adversarially] Zenati, H., Romain, M., Foo, C.S., Lecouat, B. and Chandrasekhar, V., 2018, November. Adversarially learned anomaly detection. In 2018 IEEE International conference on data mining (ICDM) (pp. 727-736). IEEE.
+
+.. [#Zhao2018XGBOD] Zhao, Y. and Hryniewicki, M.K. XGBOD: Improving Supervised Outlier Detection with Unsupervised Representation Learning. *IEEE International Joint Conference on Neural Networks*\ , 2018.
+
+.. [#Zhao2019LSCP] Zhao, Y., Nasrullah, Z., Hryniewicki, M.K. and Li, Z., 2019, May. LSCP: Locally selective combination in parallel outlier ensembles. In *Proceedings of the 2019 SIAM International Conference on Data Mining (SDM)*, pp. 585-593. Society for Industrial and Applied Mathematics.
+
+.. [#Zhao2021SUOD] Zhao, Y., Hu, X., Cheng, C., Wang, C., Wan, C., Wang, W., Yang, J., Bai, H., Li, Z., Xiao, C., Wang, Y., Qiao, Z., Sun, J. and Akoglu, L. (2021). SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection. *Conference on Machine Learning and Systems (MLSys)*.
+
+
```

### Comparing `pyod-1.0.9/README.rst` & `pyod-1.1.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 
 
 * `Installation <#installation>`_
 * `API Cheatsheet & Reference <#api-cheatsheet--reference>`_
 * `ADBench Benchmark <#adbench-benchmark>`_
 * `Model Save & Load <#model-save--load>`_
 * `Fast Train with SUOD <#fast-train-with-suod>`_
+* `Thresholding Outlier Scores <#thresholding-outlier-scores>`_
 * `Implemented Algorithms <#implemented-algorithms>`_
 * `Quick Start for Outlier Detection <#quick-start-for-outlier-detection>`_
 * `How to Contribute <#how-to-contribute>`_
 * `Inclusion Criteria <#inclusion-criteria>`_
 
 
 ----
@@ -323,25 +324,43 @@
                      IForest(n_estimators=200)]
 
     # decide the number of parallel process, and the combination method
     # then clf can be used as any outlier detection model
     clf = SUOD(base_estimators=detector_list, n_jobs=2, combination='average',
                verbose=False)
 
+----
+
+Thresholding Outlier Scores
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+A more data based approach can be taken when setting the contamination level.
+By using a thresholding method, guessing an abritrary value can be replaced
+with tested techniques for seperating inliers and outliers. Refer to 
+`PyThresh <https://github.com/KulikDM/pythresh>`_ for
+a more in depth look at thresholding.
 
 
+.. code-block:: python
+
+    from pyod.models.knn import KNN
+    from pyod.models.thresholds import FILTER
+
+    # Set the outlier detection and thresholding methods
+    clf = KNN(contamination=FILTER())
+
 
 ----
 
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
-PyOD toolkit consists of three major functional groups:
+PyOD toolkit consists of four major functional groups:
 
 **(i) Individual Detection Algorithms** :
 
 ===================  ==================  ======================================================================================================  =====  ========================================
 Type                 Abbr                Algorithm                                                                                               Year   Ref
 ===================  ==================  ======================================================================================================  =====  ========================================
 Probabilistic        ECOD                Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions                        2022   [#Li2021ECOD]_
@@ -407,16 +426,51 @@
 Combination          Maximization      Simple combination by taking the maximum scores                                                        2015   [#Aggarwal2015Theoretical]_
 Combination          AOM               Average of Maximum                                                                                     2015   [#Aggarwal2015Theoretical]_
 Combination          MOA               Maximization of Average                                                                                2015   [#Aggarwal2015Theoretical]_
 Combination          Median            Simple combination by taking the median of the scores                                                  2015   [#Aggarwal2015Theoretical]_
 Combination          majority Vote     Simple combination by taking the majority vote of the labels (weights can be used)                     2015   [#Aggarwal2015Theoretical]_
 ===================  ================  =====================================================================================================  =====  ========================================
 
+**(iii) Outlier Detection Score Thresholding Methods**:
+
+==================================  ================  ================================================================ ====================================================================================================================
+Type                                Abbr              Algorithm                                                        Documentation                                    
+==================================  ================  ================================================================ ====================================================================================================================
+Kernel-Based                        AUCP              Area Under Curve Percentage                                      `AUCP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.AUCP>`_
+Statistical Moment-Based            BOOT              Bootstrapping                                                    `BOOT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.BOOT>`_ 
+Normality-Based                     CHAU              Chauvenet's Criterion                                            `CHAU <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CHAU>`_
+Linear Model                        CLF               Trained Linear Classifier                                        `CLF <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLF>`_
+cluster-Based                       CLUST             Clustering Based                                                 `CLUST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLUST>`_
+Kernel-Based                        CPD               Change Point Detection                                           `CPD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CPD>`_
+Transformation-Based                DECOMP            Decomposition                                                    `DECOMP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DECOMP>`_
+Normality-Based                     DSN               Distance Shift from Normal                                       `DSN <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DSN>`_
+Curve-Based                         EB                Elliptical Boundary                                              `EB <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.EB>`_
+Kernel-Based                        FGD               Fixed Gradient Descent                                           `FGD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FGD>`_
+Filter-Based                        FILTER            Filtering Based                                                  `FILTER <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FILTER>`_
+Curve-Based                         FWFM              Full Width at Full Minimum                                       `FWFM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FWFM>`_
+Statistical Test-Based              GESD              Generalized Extreme Studentized Deviate                          `GESD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.GESD>`_
+Filter-Based                        HIST              Histogram Based                                                  `HIST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.HIST>`_
+Quantile-Based                      IQR               Inter-Quartile Region                                            `IQR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.IQR>`_
+Statistical Moment-Based            KARCH             Karcher mean (Riemannian Center of Mass)                         `KARCH <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.KARCH>`_
+Statistical Moment-Based            MAD               Median Absolute Deviation                                        `MAD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MAD>`_
+Statistical Test-Based              MCST              Monte Carlo Shapiro Tests                                        `MCST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MCST>`_
+Ensembles-Based                     META              Meta-model Trained Classifier                                    `META <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.META>`_
+Transformation-Based                MOLL              Friedrichs' Mollifier                                            `MOLL <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MOLL>`_
+Statistical Test-Based              MTT               Modified Thompson Tau Test                                       `MTT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MTT>`_
+Linear Model                        OCSVM             One-Class Support Vector Machine                                 `OCSVM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.OCSVM>`_
+Quantile-Based                      QMCD              Quasi-Monte Carlo Discrepancy                                    `QMCD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.QMCD>`_
+Linear Model                        REGR              Regression Based                                                 `REGR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.REGR>`_
+Neural Networks                     VAE               Variational Autoencoder                                          `VAE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.VAE>`_
+Curve-Based                         WIND              Topological Winding Number                                       `WIND <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.WIND>`_
+Transformation-Based                YJ                Yeo-Johnson Transformation                                       `YJ <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.YJ>`_
+Normality-Based                     ZSCORE            Z-score                                                          `ZSCORE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.ZSCORE>`_
+==================================  ================  ================================================================ ====================================================================================================================
+
 
-**(iii) Utility Functions**:
+**(iV) Utility Functions**:
 
 ===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
 Type                 Name                    Function                                                                                                                                               Documentation
 ===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
 Data                 generate_data           Synthesized data generation; normal data is generated by a multivariate Gaussian and outliers are generated by a uniform distribution                  `generate_data <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.data.generate_data>`_
 Data                 generate_data_clusters  Synthesized data generation in clusters; more complex data patterns can be created with multiple clusters                                              `generate_data_clusters <https://pyod.readthedocs.io/en/latest/pyod.utils.html#pyod.utils.data.generate_data_clusters>`_
 Stat                 wpearsonr               Calculate the weighted Pearson correlation of two samples                                                                                              `wpearsonr <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.stat_models.wpearsonr>`_
```

### Comparing `pyod-1.0.9/pyod/models/__init__.py` & `pyod-1.1.0/pyod/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/abod.py` & `pyod-1.1.0/pyod/models/abod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/alad.py` & `pyod-1.1.0/pyod/models/alad.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/anogan.py` & `pyod-1.1.0/pyod/models/anogan.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/auto_encoder.py` & `pyod-1.1.0/pyod/models/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/auto_encoder_torch.py` & `pyod-1.1.0/pyod/models/auto_encoder_torch.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/base.py` & `pyod-1.1.0/pyod/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
 
         if isinstance(self.contamination, (float, int)):
             prediction = (pred_score > self.threshold_).astype('int').ravel()
 
         # if this is a PyThresh object
         else:
             prediction = self.contamination.eval(pred_score)
-            print(self.contamination)
 
         if return_confidence:
             confidence = self.predict_confidence(X)
             return prediction, confidence
 
         return prediction
```

### Comparing `pyod-1.0.9/pyod/models/base_dl.py` & `pyod-1.1.0/pyod/models/base_dl.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/cblof.py` & `pyod-1.1.0/pyod/models/cblof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/cd.py` & `pyod-1.1.0/pyod/models/cd.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,72 +5,126 @@
 # Author: D Kulik
 # License: BSD 2 clause
 
 from __future__ import division
 from __future__ import print_function
 
 import numpy as np
-from sklearn.decomposition import PCA
 from sklearn.linear_model import LinearRegression
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
 from .base import BaseDetector
 
 
-def whiten_data(X, pca):
-    X = pca.transform(X)
+def _Cooks_dist(X, y, model):
+    """Calculated the Cook's distance
 
-    return X
+    Parameters
+    ----------
+    X : numpy array of shape (n_samples, n_features)
+        The training dataset.
+
+    y : numpy array of shape (n_samples)
+        The training datset
+
+    model : object
+        Regression model used to calculate the Cook's distance
 
+    Returns
+    -------
+    distances_ : numpy array of shape (n_samples)
+        Cook's distance
+    """
 
-def Cooks_dist(X, y, model):
     # Leverage is computed as the diagonal of the projection matrix of X
     leverage = (X * np.linalg.pinv(X).T).sum(1)
 
     # Compute the rank and the degrees of freedom of the model
     rank = np.linalg.matrix_rank(X)
     df = X.shape[0] - rank
 
     # Compute the MSE from the residuals
     residuals = y - model.predict(X)
     mse = np.dot(residuals, residuals) / df
 
     # Compute Cook's distance
-    residuals_studentized = residuals / np.sqrt(mse) / np.sqrt(1 - leverage)
-    distance_ = residuals_studentized ** 2 / X.shape[1]
-    distance_ *= leverage / (1 - leverage)
+    if (mse != 0) or (mse != np.nan):
+        residuals_studentized = residuals / np.sqrt(mse) / np.sqrt(
+            1 - leverage)
+        distance_ = residuals_studentized ** 2 / X.shape[1]
+        distance_ *= leverage / (1 - leverage)
+        distance_ = ((distance_ - distance_.min())
+                     / (distance_.max() - distance_.min()))
+
+    else:
+        distance_ = np.ones(len(y)) * np.nan
 
     return distance_
 
 
+def _process_distances(X, model):
+    """Calculated the mean Cook's distances for
+    each feature
+
+    Parameters
+    ----------
+    X : numpy array of shape (n_samples, n_features)
+        The training dataset.
+
+    model : object
+        Regression model used to calculate the Cook's distance
+
+    Returns
+    -------
+    distances_ : numpy array of shape (n_samples)
+        mean Cook's distance
+    """
+
+    distances_ = []
+    for i in range(X.shape[1]):
+        mod = model
+
+        # Extract new X and y inputs
+        exp = np.delete(X.copy(), i, axis=1)
+        resp = X[:, i]
+
+        exp = exp.reshape(-1, 1) if exp.ndim == 1 else exp
+
+        # Fit the model
+        mod.fit(exp, resp)
+
+        # Get Cook's Distance
+        distance_ = _Cooks_dist(exp, resp, mod)
+
+        distances_.append(distance_)
+
+    distances_ = np.nanmean(distances_, axis=0)
+
+    return distances_
+
+
 class CD(BaseDetector):
     """Cook's distance can be used to identify points that negatively
        affect a regression model. A combination of each observation’s
        leverage and residual values are used in the measurement. Higher
-       leverage and residuals relate to  higher Cook’s distances.
-       Read more in the :cite:`cook1977detection`.
+       leverage and residuals relate to  higher Cook’s distances. Note
+       that this method is unsupervised and requires at least two 
+       features for X with which to calculate the mean Cook's distance
+       for each datapoint. Read more in the :cite:`cook1977detection`.
 
     Parameters
     ----------
     contamination : float in (0., 0.5), optional (default=0.1)
         The amount of contamination of the data set, i.e.
         the proportion of outliers in the data set. Used when fitting to
         define the threshold on the decision function.
         
-    whiten : bool, optional (default=True)
-        transform X to have a covariance matrix that is the identity matrix
-        of 1 in the diagonal and 0 for the other cells using PCA
-
-    rule_of_thumb : bool, optional (default=False)
-        to apply the rule of thumb prediction (4 / n) as the influence
-        threshold; where n is the number of samples. This has been know to
-        be a good estimate for values over this point as being outliers.
-        ** Note the contamination level is reset when rule_of_thumb is
-           set to True
+    model : object, optional (default=LinearRegression())
+        Regression model used to calculate the Cook's distance
           
 
     Attributes
     ----------
     decision_scores_ : numpy array of shape (n_samples,)
         The outlier scores of the training data.
         The higher, the more abnormal. Outliers tend to have higher
@@ -84,100 +138,67 @@
 
     labels_ : int, either 0 or 1
         The binary labels of the training data. 0 stands for inliers
         and 1 for outliers/anomalies. It is generated by applying
         ``threshold_`` on ``decision_scores_``.
         """
 
-    def __init__(self, whitening=True, contamination=0.1, rule_of_thumb=False):
-
+    def __init__(self, contamination=0.1, model=LinearRegression()):
         super(CD, self).__init__(contamination=contamination)
-        self.whitening = whitening
-        self.rule_of_thumb = rule_of_thumb
+        self.model = model
 
-    def fit(self, X, y):
-        """Fit detector. y is necessary for supervised method.
+    def fit(self, X, y=None):
+        """"Fit detector. y is ignored in unsupervised methods.
 
         Parameters
         ----------
         X : numpy array of shape (n_samples, n_features)
             The input samples.
 
-        y : numpy array of shape (n_samples,), optional (default=None)
-            The ground truth of the input samples (labels).
-        """
+        y : Ignored
+            Not used, present for API consistency by convention.
 
-        # Define OLS model 
-        self.model = LinearRegression()
+        Returns
+        -------
+        self : object
+            Fitted estimator.
+        """
 
         # Validate inputs X and y
-        try:
-            X = check_array(X)
-        except ValueError:
-            X = X.reshape(-1, 1)
+        X = check_array(X)
 
-        y = np.squeeze(check_array(y, ensure_2d=False))
         self._set_n_classes(y)
 
-        # Apply whitening
-        if self.whitening:
-            self.pca = PCA(whiten=True)
-            self.pca.fit(X)
-            X = whiten_data(X, self.pca)
+        # Get Cook's distance
+        distances_ = _process_distances(X, self.model)
 
-        # Fit a linear model to X and y
-        self.model.fit(X, y)
-
-        # Get Cook's Distance
-        distance_ = Cooks_dist(X, y, self.model)
-
-        # Compute the influence threshold
-        if self.rule_of_thumb:
-            influence_threshold_ = 4 / X.shape[0]
-            self.contamination = sum(distance_ > influence_threshold_) / \
-                                 X.shape[0]
-
-        self.decision_scores_ = distance_
+        self.decision_scores_ = distances_
 
         self._process_decision_scores()
 
         return self
 
     def decision_function(self, X):
         """Predict raw anomaly score of X using the fitted detector.
-
-        The anomaly score of an input sample is computed based on different
-        detector algorithms. For consistency, outliers are assigned with
-        larger anomaly scores.
+        For consistency, outliers are assigned with larger anomaly scores.
 
         Parameters
         ----------
         X : numpy array of shape (n_samples, n_features)
-            The independent and dependent/target samples with the target 
-            samples being the last column of the numpy array such that
-            eg: X = np.append(x, y.reshape(-1,1), axis=1). Sparse matrices are 
-            accepted only if they are supported by the base estimator.
+            The training input samples. Sparse matrices are accepted only
+            if they are supported by the base estimator.
 
         Returns
         -------
         anomaly_scores : numpy array of shape (n_samples,)
             The anomaly score of the input samples.
         """
 
         check_is_fitted(self, ['decision_scores_', 'threshold_', 'labels_'])
 
-        try:
-            X = check_array(X)
-        except ValueError:
-            X = X.reshape(-1, 1)
-
-        y = X[:, -1]
-        X = X[:, :-1]
-
-        # Apply whitening
-        if self.whitening:
-            X = whiten_data(X, self.pca)
+        # Validate input X
+        X = check_array(X)
 
-            # Get Cook's Distance
-        distance_ = Cooks_dist(X, y, self.model)
+        # Get Cook's distance
+        distances_ = _process_distances(X, self.model)
 
-        return distance_
+        return distances_
```

### Comparing `pyod-1.0.9/pyod/models/cof.py` & `pyod-1.1.0/pyod/models/cof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/combination.py` & `pyod-1.1.0/pyod/models/combination.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/copod.py` & `pyod-1.1.0/pyod/models/copod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/deep_svdd.py` & `pyod-1.1.0/pyod/models/deep_svdd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/ecod.py` & `pyod-1.1.0/pyod/models/ecod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/feature_bagging.py` & `pyod-1.1.0/pyod/models/feature_bagging.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/gaal_base.py` & `pyod-1.1.0/pyod/models/gaal_base.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/gmm.py` & `pyod-1.1.0/pyod/models/gmm.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/hbos.py` & `pyod-1.1.0/pyod/models/hbos.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/iforest.py` & `pyod-1.1.0/pyod/models/iforest.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/inne.py` & `pyod-1.1.0/pyod/models/inne.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/kde.py` & `pyod-1.1.0/pyod/models/kde.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/knn.py` & `pyod-1.1.0/pyod/models/knn.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/kpca.py` & `pyod-1.1.0/pyod/models/kpca.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/lmdd.py` & `pyod-1.1.0/pyod/models/lmdd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/loci.py` & `pyod-1.1.0/pyod/models/loci.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/loda.py` & `pyod-1.1.0/pyod/models/loda.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/lof.py` & `pyod-1.1.0/pyod/models/lof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/lscp.py` & `pyod-1.1.0/pyod/models/lscp.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/lunar.py` & `pyod-1.1.0/pyod/models/lunar.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/mad.py` & `pyod-1.1.0/pyod/models/mad.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/mcd.py` & `pyod-1.1.0/pyod/models/mcd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/mo_gaal.py` & `pyod-1.1.0/pyod/models/mo_gaal.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/ocsvm.py` & `pyod-1.1.0/pyod/models/ocsvm.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/pca.py` & `pyod-1.1.0/pyod/models/pca.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/qmcd.py` & `pyod-1.1.0/pyod/models/qmcd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/rgraph.py` & `pyod-1.1.0/pyod/models/rgraph.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/rod.py` & `pyod-1.1.0/pyod/models/rod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/sampling.py` & `pyod-1.1.0/pyod/models/sampling.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/sklearn_base.py` & `pyod-1.1.0/pyod/models/sklearn_base.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/so_gaal.py` & `pyod-1.1.0/pyod/models/so_gaal.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/sod.py` & `pyod-1.1.0/pyod/models/sod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/sos.py` & `pyod-1.1.0/pyod/models/sos.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/suod.py` & `pyod-1.1.0/pyod/models/suod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/thresholds.py` & `pyod-1.1.0/pyod/models/thresholds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-def ALL(**kwargs):
-    """ALL class for Combined thresholder.
-
-       Use the multiple thresholders as a non-parametric means
-       to threshold scores generated by the decision_scores where outliers
-       are set to any value beyond the (mean, median, or mode) of the
-       contamination from all the combined thresholders.
-       
-       Parameters
-       ----------
-
-       thresholders : list, optional (default='all')
-            List of instantiated thresholders, e.g. [DSN()]
-       
-       max_contam : float, optional (default=0.5)
-            Maximum contamination allowed for each threshold output. Thresholded scores
-            above the maximum contamination will not be included in the final combined
-            threshold
-
-       method : {'mean', 'median', 'mode'}, optional (default='mean')
-           statistic to apply to contamination levels
-           
-           - 'mean':   calculate the mean combined threshold
-           - 'median': calculate the median combined threshold
-           - 'mode':  calculate the majority vote or mode of the thresholded labels
-           
-    """
-
-    from pythresh.thresholds.all import ALL as ALL_thres
-    return ALL_thres(**kwargs)
-
-
 def AUCP(**kwargs):
     """AUCP class for Area Under Curve Precentage thresholder.
 
        Use the area under the curve to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond where the auc of the kde is less
        than the (mean + abs(mean-median)) percent of the total kde auc.
@@ -45,14 +13,21 @@
 
 def BOOT(**kwargs):
     """BOOT class for Bootstrapping thresholder.
 
        Use a boostrapping based method to find a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond the mean of the confidence intervals.
+   
+       Parameters
+       ----------
+       
+       random_state : int, optional (default=1234)
+            Random seed for bootstrapping a confidence interval. Can also be set to None.
+
     """
 
     from pythresh.thresholds.boot import BOOT as BOOT_thres
     return BOOT_thres(**kwargs)
 
 
 def CHAU(**kwargs):
@@ -80,14 +55,23 @@
 
 def CLF(**kwargs):
     """CLF class for Trained Classifier thresholder.
 
        Use the trained linear classifier to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond 0.
+
+       Parameters
+       ----------
+
+       method : {'simple', 'complex'}, optional (default='complex')
+            Type of linear model
+
+            - 'simple':  Uses only the scores
+            - 'complex': Uses the scores, log of the scores, and the scores' PDF
     """
 
     from pythresh.thresholds.clf import CLF as CLF_thres
     return CLF_thres(**kwargs)
 
 
 def CLUST(**kwargs):
@@ -96,15 +80,15 @@
        Use the clustering methods to evaluate a non-parametric means to
        threshold scores generated by the decision_scores where outliers
        are set to any value not labelled as part of the main cluster.
 
        Parameters
        ----------
         
-       method : {'agg', 'birch', 'bang', 'bgm', 'bsas', 'dbscan', 'ema', 'kmeans', 'mbsas', 'mshift', 'optics', 'somsc', 'spec', 'xmeans'}, optional (default='dbscan')
+       method : {'agg', 'birch', 'bang', 'bgm', 'bsas', 'dbscan', 'ema', 'kmeans', 'mbsas', 'mshift', 'optics', 'somsc', 'spec', 'xmeans'}, optional (default='spec')
             Clustering method
         
             - 'agg':    Agglomerative
             - 'birch':  Balanced Iterative Reducing and Clustering using Hierarchies
             - 'bang':   BANG
             - 'bgm':    Bayesian Gaussian Mixture
             - 'bsas':   Basic Sequential Algorithmic Scheme
@@ -113,37 +97,77 @@
             - 'kmeans': K-means
             - 'mbsas':  Modified Basic Sequential Algorithmic Scheme
             - 'mshift': Mean shift
             - 'optics': Ordering Points To Identify Clustering Structure
             - 'somsc':  Self-organized feature map 
             - 'spec':   Clustering to a projection of the normalized Laplacian 
             - 'xmeans': X-means
+            
+       random_state : int, optional (default=1234)
+            Random seed for the BayesianGaussianMixture clustering (method='bgm'). Can
+            also be set to None.
     """
 
     from pythresh.thresholds.clust import CLUST as CLUST_thres
     return CLUST_thres(**kwargs)
 
 
+def CPD(**kwargs):
+    """CPD class for Change Point Detection thresholder.
+
+       Use change point detection to find a non-parametric means
+       to threshold scores generated by the decision_scores where outliers
+       are set to any value beyond the detected change point.
+
+       Parameters
+       ----------
+
+       method : {'Dynp', 'KernelCPD', 'Binseg', 'BottomUp'}, optional (default='Dynp')
+            Method for change point detection
+
+            - 'Dynp':      Dynamic programming (optimal minimum sum of errors per partition)
+            - 'KernelCPD': RBF kernel function (optimal minimum sum of errors per partition)
+            - 'Binseg':    Binary segmentation
+            - 'BottomUp':  Bottom-up segmentation
+
+       transform : {'cdf', 'kde'}, optional (default='cdf')
+            Data transformation method prior to fit
+
+            - 'cdf': Use the cumulative distribution function
+            - 'kde': Use the kernel density estimation
+            
+    """
+
+    from pythresh.thresholds.cpd import CPD as CPD_thres
+    return CPD_thres(**kwargs)
+
+
 def DECOMP(**kwargs):
     """DECOMP class for Decomposition based thresholders.
 
        Use decomposition to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond the maximum of the decomposed
        matrix that results from decomposing the cumulative distribution
        function of the decision scores.
        
        Parameters
        ----------
-       
-       method: {'NMF', 'PCA'}, optional (default='PCA')
+
+       method : {'NMF', 'PCA', 'GRP', 'SRP'}, optional (default='PCA')
             Method to use for decomposition
-        
+
             - 'NMF':  Non-Negative Matrix Factorization
-            - 'PCA':  Principal component analysis
+            - 'PCA':  Principal Component Analysis
+            - 'GRP':  Gaussian Random Projection
+            - 'SRP':  Sparse Random Projection
+            
+       random_state : int, optional (default=1234)
+            Random seed for the decomposition algorithm. Can also be set to None.
+
     """
 
     from pythresh.thresholds.decomp import DECOMP as DECOMP_thres
     return DECOMP_thres(**kwargs)
 
 
 def DSN(**kwargs):
@@ -153,15 +177,15 @@
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond the distance calculated by the selected
        metric.
        
        Parameters
        ----------
 
-       metric : {'JS', 'WS', 'ENG', 'BHT', 'HLL', 'HI', 'LK', 'LP', 'MAH', 'TMT', 'RES', 'KS', 'INT', 'MMD'}, optional (default='JS')
+       metric : {'JS', 'WS', 'ENG', 'BHT', 'HLL', 'HI', 'LK', 'LP', 'MAH', 'TMT', 'RES', 'KS', 'INT', 'MMD'}, optional (default='MAH')
             Metric to use for distance computation
         
             - 'JS':  Jensen-Shannon distance
             - 'WS':  Wasserstein or Earth Movers distance
             - 'ENG': Energy distance
             - 'BHT': Bhattacharyya distance
             - 'HLL': Hellinger distance
@@ -170,14 +194,18 @@
             - 'LP':  Levy-Prokhorov metric
             - 'MAH': Mahalanobis distance
             - 'TMT': Tanimoto distance
             - 'RES': Studentized residual distance
             - 'KS':  Kolmogorov-Smirnov distance
             - 'INT': Weighted spline interpolated distance
             - 'MMD': Maximum Mean Discrepancy distance
+            
+       random_state : int, optional (default=1234)
+            Random seed for the normal distribution. Can also be set to None.
+
     """
 
     from pythresh.thresholds.dsn import DSN as DSN_thres
     return DSN_thres(**kwargs)
 
 
 def EB(**kwargs):
@@ -214,15 +242,15 @@
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond the maximum filter value.
        See :cite:`hashemi2019filter` for details.
        
        Parameters
        ----------
 
-       method : {'gaussian', 'savgol', 'hilbert', 'wiener', 'medfilt', 'decimate','detrend', 'resample'}, optional (default='wiener')
+       method : {'gaussian', 'savgol', 'hilbert', 'wiener', 'medfilt', 'decimate','detrend', 'resample'}, optional (default='savgol')
             Method to filter the scores
        
             - 'gaussian': use a gaussian based filter
             - 'savgol':   use the savgol based filter
             - 'hilbert':  use the hilbert based filter
             - 'wiener':   use the wiener based filter
             - 'medfilt:   use a median based filter
@@ -292,15 +320,15 @@
        
        Parameters
        ----------
        
        nbins : int, optional (default='auto')
             Number of bins to use in the hostogram, default set to int(len(scores)**0.7)
                
-       method : {'otsu', 'yen', 'isodata', 'li', 'minimum', 'triangle'}, optional (default='otsu')
+       method : {'otsu', 'yen', 'isodata', 'li', 'minimum', 'triangle'}, optional (default='triangle')
             Histogram filtering based method
             
             - 'otsu':     OTSU's method for filtering
             - 'yen':      Yen's method for filtering
             - 'isodata':  Ridler-Calvard or inter-means method for filtering
             - 'li':       Li's iterative Minimum Cross Entropy method for filtering
             - 'minimum':  Minimum between two maxima via smoothing method for filtering
@@ -367,14 +395,21 @@
 
        Use uniform random sampling and statstical testing to evaluate a
        non-parametric means to threshold scores generated by the decision_scores
        where outliers are set to any value beyond the minimum value left after
        iterative Shapiro-Wilk tests have occured. Note** accuracy decreases with
        array size. For good results the should be array<1000. However still this
        threshold method may fail at any array size.
+       
+       Parameters
+       ----------
+
+       random_state : int, optional (default=1234)
+            Random seed for the uniform distribution. Can also be set to None.
+
     """
 
     from pythresh.thresholds.mcst import MCST as MCST_thres
     return MCST_thres(**kwargs)
 
 
 def META(**kwargs):
@@ -382,20 +417,23 @@
 
        Use a trained meta-model to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set based on the trained meta-model classifier. 
        
        Parameters
        ----------
-       
-       method : {'LIN', 'GNB'}, optional (default='LIN')
-           select 
-           
-           - 'LIN': RidgeCV trained linear classifier meta-model
-           - 'GNB': Gaussian Naive Bayes trained classifier meta-model
+
+       method : {'LIN', 'GNB', 'GNBC', 'GNBM'}, optional (default='GNBM')
+           select
+
+           - 'LIN':  RidgeCV trained linear classifier meta-model on true labels
+           - 'GNB':  Gaussian Naive Bayes trained classifier meta-model on true labels
+           - 'GNBC': Gaussian Naive Bayes trained classifier meta-model on best contamination
+           - 'GNBM': Gaussian Naive Bayes multivariate trained classifier meta-model
+
     """
 
     from pythresh.thresholds.meta import META as META_thres
     return META_thres(**kwargs)
 
 
 def MOLL(**kwargs):
@@ -436,15 +474,15 @@
        are determined by the one-class svm using a polynomial kernel
        with the polynomial degree either set or determined by regression
        internally.
        
        Parameters
        ----------
        
-       model : {'poly', 'sgd'}, optional (default='poly')
+       model : {'poly', 'sgd'}, optional (default='sgd')
            OCSVM model to apply
 
            - 'poly':  Use a polynomial kernel with a regular OCSVM
            - 'sgd':   Used the Additive Chi2 kernel approximation with a SGDOneClassSVM
 
        degree : int, optional (default='auto')
            Polynomial degree to use for the one-class svm.
@@ -464,14 +502,18 @@
            of the fraction of support vectors. Default 'auto' sets nu as the ratio
            between the any point that is less than or equal to the median plus
            the absolute difference between the mean and geometric mean over the
            the number of points in the entire dataset 
 
        tol : float, optional (default=1e-3)
            The stopping criterion for the one-class svm
+           
+       random_state : int, optional (default=1234)
+           Random seed for the SVM's data sampling. Can also be set to None.
+
     """
 
     from pythresh.thresholds.ocsvm import OCSVM as OCSVM_thres
     return OCSVM_thres(**kwargs)
 
 
 def QMCD(**kwargs):
@@ -517,14 +559,18 @@
        ----------
 
        method : {'siegel', 'theil'}, optional (default='siegel')
             Regression based method to calculate the y-intercept
             
             - 'siegel': implements a method for robust linear regression using repeated medians
             - 'theil':  implements a method for robust linear regression using paired values
+            
+       random_state : int, optional (default=1234)
+            random seed for the normal distribution. Can also be set to None
+
     """
 
     from pythresh.thresholds.regr import REGR as REGR_thres
     return REGR_thres(**kwargs)
 
 
 def VAE(**kwargs):
@@ -577,14 +623,21 @@
 def WIND(**kwargs):
     """WIND class for topological Winding number thresholder.
 
        Use the topological winding number (with respect to the origin) to
        evaluate a non-parametric means to threshold scores generated by
        the decision_scores where outliers are set to any value beyond the
        mean intersection point calculated from the winding number.
+       
+       Parameters
+       ----------
+
+       random_state : int, optional (default=1234)
+            Random seed for the normal distribution. Can also be set to None.
+
     """
 
     from pythresh.thresholds.wind import WIND as WIND_thres
     return WIND_thres(**kwargs)
 
 
 def YJ(**kwargs):
```

### Comparing `pyod-1.0.9/pyod/models/vae.py` & `pyod-1.1.0/pyod/models/vae.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/models/xgbod.py` & `pyod-1.1.0/pyod/models/xgbod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/utils/__init__.py` & `pyod-1.1.0/pyod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/utils/data.py` & `pyod-1.1.0/pyod/utils/data.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/utils/example.py` & `pyod-1.1.0/pyod/utils/example.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/utils/stat_models.py` & `pyod-1.1.0/pyod/utils/stat_models.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/utils/utility.py` & `pyod-1.1.0/pyod/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/pyod/version.py` & `pyod-1.1.0/pyod/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '1.0.9'  # pragma: no cover
+__version__ = '1.1.0'  # pragma: no cover
```

### Comparing `pyod-1.0.9/pyod.egg-info/PKG-INFO` & `pyod-1.1.0/pyod.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,670 +1,724 @@
-Metadata-Version: 2.1
-Name: pyod
-Version: 1.0.9
-Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
-Home-page: https://github.com/yzhao062/pyod
-Author: Yue Zhao
-Author-email: zhaoy@cmu.edu
-License: UNKNOWN
-Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
-Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Python Outlier Detection (PyOD)
-===============================
-
-**Deployment & Documentation & Stats & License**
-
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
-   :target: https://pypi.org/project/pyod/
-   :alt: PyPI version
-
-
-.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
-   :target: https://anaconda.org/conda-forge/pyod
-   :alt: Anaconda version
-
-
-.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
-   :target: https://pyod.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation status
-
-
-.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
-   :target: https://github.com/yzhao062/pyod/stargazers
-   :alt: GitHub stars
-
-
-.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
-   :target: https://github.com/yzhao062/pyod/network
-   :alt: GitHub forks
-
-
-.. image:: https://pepy.tech/badge/pyod
-   :target: https://pepy.tech/project/pyod
-   :alt: Downloads
-
-.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
-   :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
-   :alt: testing
-
-
-.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
-   :target: https://coveralls.io/github/yzhao062/pyod
-   :alt: Coverage Status
-
-
-.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
-   :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
-   :alt: Maintainability
-
-
-.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
-   :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
-   :alt: License
-
-.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
-   :target: https://github.com/Minqi824/ADBench
-   :alt: Benchmark
-
-
------
-
-**News**: We just released a 45-page, the most comprehensive `anomaly detection benchmark paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_.
-The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
-
-**For time-series outlier detection**, please use `TODS <https://github.com/datamllab/tods>`_.
-**For graph outlier detection**, please use `PyGOD <https://pygod.org/>`_.
-
-PyOD is the most comprehensive and scalable **Python library** for **detecting outlying objects** in
-multivariate data. This exciting yet challenging field is commonly referred as 
-`Outlier Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_
-or `Anomaly Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_.
-
-PyOD includes more than 40 detection algorithms, from classical LOF (SIGMOD 2000) to
-the latest ECOD (TKDE 2022). Since 2017, PyOD has been successfully used in numerous academic researches and
-commercial products with more than `10 million downloads <https://pepy.tech/project/pyod>`_.
-It is also well acknowledged by the machine learning community with various dedicated posts/tutorials, including
-`Analytics Vidhya <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_,
-`KDnuggets <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, and
-`Towards Data Science <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_.
-
-
-**PyOD is featured for**:
-
-* **Unified APIs, detailed documentation, and interactive examples** across various algorithms.
-* **Advanced models**\, including **classical distance and density estimation**, **latest deep learning methods**, and **emerging algorithms like ECOD**.
-* **Optimized performance with JIT and parallelization** using `numba <https://github.com/numba/numba>`_ and `joblib <https://github.com/joblib/joblib>`_.
-* **Fast training & prediction with SUOD** [#Zhao2021SUOD]_.
-
-
-**Outlier Detection with 5 Lines of Code**\ :
-
-
-.. code-block:: python
-
-
-    # train an ECOD detector
-    from pyod.models.ecod import ECOD
-    clf = ECOD()
-    clf.fit(X_train)
-
-    # get outlier scores
-    y_train_scores = clf.decision_scores_  # raw outlier scores on the train data
-    y_test_scores = clf.decision_function(X_test)  # predict raw outlier scores on test
-
-
-**Personal suggestion on selecting an OD algorithm**. If you do not know which algorithm to try, go with:
-
-- `ECOD <https://github.com/yzhao062/pyod/blob/master/examples/ecod_example.py>`_: Example of using ECOD for outlier detection
-- `Isolation Forest <https://github.com/yzhao062/pyod/blob/master/examples/iforest_example.py>`_: Example of using Isolation Forest for outlier detection
-
-They are both fast and interpretable. Or, you could try more data-driven approach `MetaOD <https://github.com/yzhao062/MetaOD>`_.
-
-**Citing PyOD**\ :
-
-`PyOD paper <http://www.jmlr.org/papers/volume20/19-011/19-011.pdf>`_ is published in
-`Journal of Machine Learning Research (JMLR) <http://www.jmlr.org/>`_ (MLOSS track).
-If you use PyOD in a scientific publication, we would appreciate
-citations to the following paper::
-
-    @article{zhao2019pyod,
-        author  = {Zhao, Yue and Nasrullah, Zain and Li, Zheng},
-        title   = {PyOD: A Python Toolbox for Scalable Outlier Detection},
-        journal = {Journal of Machine Learning Research},
-        year    = {2019},
-        volume  = {20},
-        number  = {96},
-        pages   = {1-7},
-        url     = {http://jmlr.org/papers/v20/19-011.html}
-    }
-
-or::
-
-    Zhao, Y., Nasrullah, Z. and Li, Z., 2019. PyOD: A Python Toolbox for Scalable Outlier Detection. Journal of machine learning research (JMLR), 20(96), pp.1-7.
-
-If you want more general insights of anomaly detection and/or algorithm performance comparison, please see our
-NeurIPS 2022 paper `ADBench: Anomaly Detection Benchmark Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_::
-
-    @inproceedings{han2022adbench,
-        title={ADBench: Anomaly Detection Benchmark},
-        author={Songqiao Han and Xiyang Hu and Hailiang Huang and Mingqi Jiang and Yue Zhao},
-        booktitle={Neural Information Processing Systems (NeurIPS)}
-        year={2022},
-    }
-
-**Key Links and Resources**\ :
-
-
-* `View the latest codes on Github <https://github.com/yzhao062/pyod>`_
-* `Anomaly Detection Resources <https://github.com/yzhao062/anomaly-detection-resources>`_
-
-
-**Table of Contents**\ :
-
-
-* `Installation <#installation>`_
-* `API Cheatsheet & Reference <#api-cheatsheet--reference>`_
-* `ADBench Benchmark <#adbench-benchmark>`_
-* `Model Save & Load <#model-save--load>`_
-* `Fast Train with SUOD <#fast-train-with-suod>`_
-* `Implemented Algorithms <#implemented-algorithms>`_
-* `Quick Start for Outlier Detection <#quick-start-for-outlier-detection>`_
-* `How to Contribute <#how-to-contribute>`_
-* `Inclusion Criteria <#inclusion-criteria>`_
-
-
-----
-
-
-Installation
-^^^^^^^^^^^^
-
-It is recommended to use **pip** or **conda** for installation. Please make sure
-**the latest version** is installed, as PyOD is updated frequently:
-
-.. code-block:: bash
-
-   pip install pyod            # normal install
-   pip install --upgrade pyod  # or update if needed
-
-.. code-block:: bash
-
-   conda install -c conda-forge pyod
-
-Alternatively, you could clone and run setup.py file:
-
-.. code-block:: bash
-
-   git clone https://github.com/yzhao062/pyod.git
-   cd pyod
-   pip install .
-
-
-**Required Dependencies**\ :
-
-
-* Python 3.6+
-* joblib
-* matplotlib
-* numpy>=1.19
-* numba>=0.51
-* scipy>=1.5.1
-* scikit_learn>=0.20.0
-* six
-
-**Optional Dependencies (see details below)**\ :
-
-* combo (optional, required for models/combination.py and FeatureBagging)
-* keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
-* pandas (optional, required for running benchmark)
-* suod (optional, required for running SUOD model)
-* xgboost (optional, required for XGBOD)
-* pythresh to use thresholding
-
-**Warning**\ :
-PyOD has multiple neural network based models, e.g., AutoEncoders, which are
-implemented in both Tensorflow and PyTorch. However, PyOD does **NOT** install these deep learning libraries for you.
-This reduces the risk of interfering with your local copies.
-If you want to use neural-net based models, please make sure these deep learning libraries are installed.
-Instructions are provided: `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_.
-Similarly, models depending on **xgboost**, e.g., XGBOD, would **NOT** enforce xgboost installation by default.
-
-
-
-----
-
-
-API Cheatsheet & Reference
-^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Full API Reference: (https://pyod.readthedocs.io/en/latest/pyod.html). API cheatsheet for all detectors:
-
-
-* **fit(X)**\ : Fit detector. y is ignored in unsupervised methods.
-* **decision_function(X)**\ : Predict raw anomaly score of X using the fitted detector.
-* **predict(X)**\ : Predict if a particular sample is an outlier or not using the fitted detector.
-* **predict_proba(X)**\ : Predict the probability of a sample being outlier using the fitted detector.
-* **predict_confidence(X)**\ : Predict the model's sample-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
-
-
-Key Attributes of a fitted model:
-
-
-* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
-  Outliers tend to have higher scores.
-* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
-
-
-----
-
-
-ADBench Benchmark
-^^^^^^^^^^^^^^^^^
-
-We just released a 45-page, the most comprehensive `ADBench: Anomaly Detection Benchmark <https://arxiv.org/abs/2206.09426>`_ [#Han2022ADBench]_.
-The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
-
-The organization of **ADBench** is provided below:
-
-.. image:: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
-   :target: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
-   :alt: benchmark-fig
-
-
-**The comparison of selected models** is made available below
-(\ `Figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png>`_\ ,
-`compare_all_models.py <https://github.com/yzhao062/pyod/blob/master/examples/compare_all_models.py>`_\ ,
-`Interactive Jupyter Notebooks <https://mybinder.org/v2/gh/yzhao062/pyod/master>`_\ ).
-For Jupyter Notebooks, please navigate to **"/notebooks/Compare All Models.ipynb"**.
-
-
-.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
-   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
-   :alt: Comparision_of_All
-
-
-
-----
-
-Model Save & Load
-^^^^^^^^^^^^^^^^^
-
-PyOD takes a similar approach of sklearn regarding model persistence.
-See `model persistence <https://scikit-learn.org/stable/modules/model_persistence.html>`_ for clarification.
-
-In short, we recommend to use joblib or pickle for saving and loading PyOD models.
-See `"examples/save_load_model_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/save_load_model_example.py>`_ for an example.
-In short, it is simple as below:
-
-.. code-block:: python
-
-    from joblib import dump, load
-
-    # save the model
-    dump(clf, 'clf.joblib')
-    # load the model
-    clf = load('clf.joblib')
-
-It is known that there are challenges in saving neural network models.
-Check `#328 <https://github.com/yzhao062/pyod/issues/328#issuecomment-917192704>`_
-and `#88 <https://github.com/yzhao062/pyod/issues/88#issuecomment-615343139>`_
-for temporary workaround.
-
-
-----
-
-
-Fast Train with SUOD
-^^^^^^^^^^^^^^^^^^^^
-
-**Fast training and prediction**: it is possible to train and predict with
-a large number of detection models in PyOD by leveraging SUOD framework [#Zhao2021SUOD]_.
-See  `SUOD Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/21-mlsys-suod.pdf>`_
-and  `SUOD example <https://github.com/yzhao062/pyod/blob/master/examples/suod_example.py>`_.
-
-
-.. code-block:: python
-
-    from pyod.models.suod import SUOD
-
-    # initialized a group of outlier detectors for acceleration
-    detector_list = [LOF(n_neighbors=15), LOF(n_neighbors=20),
-                     LOF(n_neighbors=25), LOF(n_neighbors=35),
-                     COPOD(), IForest(n_estimators=100),
-                     IForest(n_estimators=200)]
-
-    # decide the number of parallel process, and the combination method
-    # then clf can be used as any outlier detection model
-    clf = SUOD(base_estimators=detector_list, n_jobs=2, combination='average',
-               verbose=False)
-
-
-
-
-----
-
-
-
-Implemented Algorithms
-^^^^^^^^^^^^^^^^^^^^^^
-
-PyOD toolkit consists of three major functional groups:
-
-**(i) Individual Detection Algorithms** :
-
-===================  ==================  ======================================================================================================  =====  ========================================
-Type                 Abbr                Algorithm                                                                                               Year   Ref
-===================  ==================  ======================================================================================================  =====  ========================================
-Probabilistic        ECOD                Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions                        2022   [#Li2021ECOD]_
-Probabilistic        ABOD                Angle-Based Outlier Detection                                                                           2008   [#Kriegel2008Angle]_
-Probabilistic        FastABOD            Fast Angle-Based Outlier Detection using approximation                                                  2008   [#Kriegel2008Angle]_
-Probabilistic        COPOD               COPOD: Copula-Based Outlier Detection                                                                   2020   [#Li2020COPOD]_
-Probabilistic        MAD                 Median Absolute Deviation (MAD)                                                                         1993   [#Iglewicz1993How]_
-Probabilistic        SOS                 Stochastic Outlier Selection                                                                            2012   [#Janssens2012Stochastic]_
-Probabilistic        QMCD                Quasi-Monte Carlo Discrepancy outlier detection                                                         2001   [#Fang2001Wrap]_
-Probabilistic        KDE                 Outlier Detection with Kernel Density Functions                                                         2007   [#Latecki2007Outlier]_
-Probabilistic        Sampling            Rapid distance-based outlier detection via sampling                                                     2013   [#Sugiyama2013Rapid]_
-Probabilistic        GMM                 Probabilistic Mixture Modeling for Outlier Analysis                                                            [#Aggarwal2015Outlier]_ [Ch.2]
-Linear Model         PCA                 Principal Component Analysis (the sum of weighted projected distances to the eigenvector hyperplanes)   2003   [#Shyu2003A]_
-Linear Model         KPCA                Kernel Principal Component Analysis                                                                     2007   [#Hoffmann2007Kernel]_
-Linear Model         MCD                 Minimum Covariance Determinant (use the mahalanobis distances as the outlier scores)                    1999   [#Hardin2004Outlier]_ [#Rousseeuw1999A]_
-Linear Model         CD                  Use Cook's distance for outlier detection                                                               1977   [#Cook1977Detection]_
-Linear Model         OCSVM               One-Class Support Vector Machines                                                                       2001   [#Scholkopf2001Estimating]_
-Linear Model         LMDD                Deviation-based Outlier Detection (LMDD)                                                                1996   [#Arning1996A]_
-Proximity-Based      LOF                 Local Outlier Factor                                                                                    2000   [#Breunig2000LOF]_
-Proximity-Based      COF                 Connectivity-Based Outlier Factor                                                                       2002   [#Tang2002Enhancing]_
-Proximity-Based      (Incremental) COF   Memory Efficient Connectivity-Based Outlier Factor (slower but reduce storage complexity)               2002   [#Tang2002Enhancing]_
-Proximity-Based      CBLOF               Clustering-Based Local Outlier Factor                                                                   2003   [#He2003Discovering]_
-Proximity-Based      LOCI                LOCI: Fast outlier detection using the local correlation integral                                       2003   [#Papadimitriou2003LOCI]_
-Proximity-Based      HBOS                Histogram-based Outlier Score                                                                           2012   [#Goldstein2012Histogram]_
-Proximity-Based      kNN                 k Nearest Neighbors (use the distance to the kth nearest neighbor as the outlier score)                 2000   [#Ramaswamy2000Efficient]_
-Proximity-Based      AvgKNN              Average kNN (use the average distance to k nearest neighbors as the outlier score)                      2002   [#Angiulli2002Fast]_
-Proximity-Based      MedKNN              Median kNN (use the median distance to k nearest neighbors as the outlier score)                        2002   [#Angiulli2002Fast]_
-Proximity-Based      SOD                 Subspace Outlier Detection                                                                              2009   [#Kriegel2009Outlier]_
-Proximity-Based      ROD                 Rotation-based Outlier Detection                                                                        2020   [#Almardeny2020A]_
-Outlier Ensembles    IForest             Isolation Forest                                                                                        2008   [#Liu2008Isolation]_
-Outlier Ensembles    INNE                Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                      2018   [#Bandaragoda2018Isolation]_
-Outlier Ensembles    FB                  Feature Bagging                                                                                         2005   [#Lazarevic2005Feature]_
-Outlier Ensembles    LSCP                LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                       2019   [#Zhao2019LSCP]_
-Outlier Ensembles    XGBOD               Extreme Boosting Based Outlier Detection **(Supervised)**                                               2018   [#Zhao2018XGBOD]_
-Outlier Ensembles    LODA                Lightweight On-line Detector of Anomalies                                                               2016   [#Pevny2016Loda]_
-Outlier Ensembles    SUOD                SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**          2021   [#Zhao2021SUOD]_
-Neural Networks      AutoEncoder         Fully connected AutoEncoder (use reconstruction error as the outlier score)                                    [#Aggarwal2015Outlier]_ [Ch.3]
-Neural Networks      VAE                 Variational AutoEncoder (use reconstruction error as the outlier score)                                 2013   [#Kingma2013Auto]_
-Neural Networks      Beta-VAE            Variational AutoEncoder (all customized loss term by varying gamma and capacity)                        2018   [#Burgess2018Understanding]_
-Neural Networks      SO_GAAL             Single-Objective Generative Adversarial Active Learning                                                 2019   [#Liu2019Generative]_
-Neural Networks      MO_GAAL             Multiple-Objective Generative Adversarial Active Learning                                               2019   [#Liu2019Generative]_
-Neural Networks      DeepSVDD            Deep One-Class Classification                                                                           2018   [#Ruff2018Deep]_
-Neural Networks      AnoGAN              Anomaly Detection with Generative Adversarial Networks                                                  2017   [#Schlegl2017Unsupervised]_
-Neural Networks      ALAD                Adversarially learned anomaly detection                                                                 2018   [#Zenati2018Adversarially]_
-Graph-based          R-Graph             Outlier detection by R-graph                                                                            2017   [#You2017Provable]_
-Graph-based          LUNAR               LUNAR: Unifying Local Outlier Detection Methods via Graph Neural Networks                               2022   [#Goodge2022Lunar]_
-===================  ==================  ======================================================================================================  =====  ========================================
-
-
-**(ii) Outlier Ensembles & Outlier Detector Combination Frameworks**:
-
-===================  ================  =====================================================================================================  =====  ========================================
-Type                 Abbr              Algorithm                                                                                              Year   Ref
-===================  ================  =====================================================================================================  =====  ========================================
-Outlier Ensembles    FB                Feature Bagging                                                                                        2005   [#Lazarevic2005Feature]_
-Outlier Ensembles    LSCP              LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                      2019   [#Zhao2019LSCP]_
-Outlier Ensembles    XGBOD             Extreme Boosting Based Outlier Detection **(Supervised)**                                              2018   [#Zhao2018XGBOD]_
-Outlier Ensembles    LODA              Lightweight On-line Detector of Anomalies                                                              2016   [#Pevny2016Loda]_
-Outlier Ensembles    SUOD              SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**         2021   [#Zhao2021SUOD]_
-Outlier Ensembles    INNE              Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                     2018   [#Bandaragoda2018Isolation]_
-Combination          Average           Simple combination by averaging the scores                                                             2015   [#Aggarwal2015Theoretical]_
-Combination          Weighted Average  Simple combination by averaging the scores with detector weights                                       2015   [#Aggarwal2015Theoretical]_
-Combination          Maximization      Simple combination by taking the maximum scores                                                        2015   [#Aggarwal2015Theoretical]_
-Combination          AOM               Average of Maximum                                                                                     2015   [#Aggarwal2015Theoretical]_
-Combination          MOA               Maximization of Average                                                                                2015   [#Aggarwal2015Theoretical]_
-Combination          Median            Simple combination by taking the median of the scores                                                  2015   [#Aggarwal2015Theoretical]_
-Combination          majority Vote     Simple combination by taking the majority vote of the labels (weights can be used)                     2015   [#Aggarwal2015Theoretical]_
-===================  ================  =====================================================================================================  =====  ========================================
-
-
-**(iii) Utility Functions**:
-
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-Type                 Name                    Function                                                                                                                                               Documentation
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-Data                 generate_data           Synthesized data generation; normal data is generated by a multivariate Gaussian and outliers are generated by a uniform distribution                  `generate_data <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.data.generate_data>`_
-Data                 generate_data_clusters  Synthesized data generation in clusters; more complex data patterns can be created with multiple clusters                                              `generate_data_clusters <https://pyod.readthedocs.io/en/latest/pyod.utils.html#pyod.utils.data.generate_data_clusters>`_
-Stat                 wpearsonr               Calculate the weighted Pearson correlation of two samples                                                                                              `wpearsonr <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.stat_models.wpearsonr>`_
-Utility              get_label_n             Turn raw outlier scores into binary labels by assign 1 to top n outlier scores                                                                         `get_label_n <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.get_label_n>`_
-Utility              precision_n_scores      calculate precision @ rank n                                                                                                                           `precision_n_scores <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.precision_n_scores>`_
-===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
-
-----
-
-Quick Start for Outlier Detection
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-PyOD has been well acknowledged by the machine learning community with a few featured posts and tutorials.
-
-**Analytics Vidhya**: `An Awesome Tutorial to Learn Outlier Detection in Python using PyOD Library <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_
-
-**KDnuggets**: `Intuitive Visualization of Outlier Detection Methods <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, `An Overview of Outlier Detection Methods from PyOD <https://www.kdnuggets.com/2019/06/overview-outlier-detection-methods-pyod.html>`_
-
-**Towards Data Science**: `Anomaly Detection for Dummies <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_
-
-**Computer Vision News (March 2019)**: `Python Open Source Toolbox for Outlier Detection <https://rsipvision.com/ComputerVisionNews-2019March/18/>`_
-
-`"examples/knn_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/knn_example.py>`_
-demonstrates the basic API of using kNN detector. **It is noted that the API across all other algorithms are consistent/similar**.
-
-More detailed instructions for running examples can be found in `examples directory <https://github.com/yzhao062/pyod/blob/master/examples>`_.
-
-
-#. Initialize a kNN detector, fit the model, and make the prediction.
-
-   .. code-block:: python
-
-
-       from pyod.models.knn import KNN   # kNN detector
-
-       # train kNN detector
-       clf_name = 'KNN'
-       clf = KNN()
-       clf.fit(X_train)
-
-       # get the prediction label and outlier scores of the training data
-       y_train_pred = clf.labels_  # binary labels (0: inliers, 1: outliers)
-       y_train_scores = clf.decision_scores_  # raw outlier scores
-
-       # get the prediction on the test data
-       y_test_pred = clf.predict(X_test)  # outlier labels (0 or 1)
-       y_test_scores = clf.decision_function(X_test)  # outlier scores
-
-       # it is possible to get the prediction confidence as well
-       y_test_pred, y_test_pred_confidence = clf.predict(X_test, return_confidence=True)  # outlier labels (0 or 1) and confidence in the range of [0,1]
-
-#. Evaluate the prediction by ROC and Precision @ Rank n (p@n).
-
-   .. code-block:: python
-
-       from pyod.utils.data import evaluate_print
-       
-       # evaluate and print the results
-       print("\nOn Training Data:")
-       evaluate_print(clf_name, y_train, y_train_scores)
-       print("\nOn Test Data:")
-       evaluate_print(clf_name, y_test, y_test_scores)
-
-
-#. See a sample output & visualization.
-
-
-   .. code-block:: python
-
-
-       On Training Data:
-       KNN ROC:1.0, precision @ rank n:1.0
-
-       On Test Data:
-       KNN ROC:0.9989, precision @ rank n:0.9
-
-   .. code-block:: python
-
-
-       visualize(clf_name, X_train, y_train, X_test, y_test, y_train_pred,
-           y_test_pred, show_figure=True, save_figure=False)
-
-Visualization (\ `knn_figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png>`_\ ):
-
-.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
-   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
-   :alt: kNN example figure
-
-----
-
-How to Contribute
-^^^^^^^^^^^^^^^^^
-
-You are welcome to contribute to this exciting project:
-
-
-* Please first check Issue lists for "help wanted" tag and comment the one
-  you are interested. We will assign the issue to you.
-
-* Fork the master branch and add your improvement/modification/fix.
-
-* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-
-* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
-
-
-To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
-
-You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
-
-
-Inclusion Criteria
-^^^^^^^^^^^^^^^^^^
-
-Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
-We mainly consider well-established algorithms for inclusion.
-A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
-
-However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
-for boosting ML accessibility and reproducibility.
-This exception only applies if you could commit to the maintenance of your model for at least two year period.
-
-
-----
-
-Reference
-^^^^^^^^^
-
-
-.. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
-
-.. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
-
-.. [#Aggarwal2017Outlier] Aggarwal, C.C. and Sathe, S., 2017. Outlier ensembles: An introduction. Springer.
-
-.. [#Almardeny2020A] Almardeny, Y., Boujnah, N. and Cleary, F., 2020. A Novel Outlier Detection Method for Multivariate Data. *IEEE Transactions on Knowledge and Data Engineering*.
-
-.. [#Angiulli2002Fast] Angiulli, F. and Pizzuti, C., 2002, August. Fast outlier detection in high dimensional spaces. In *European Conference on Principles of Data Mining and Knowledge Discovery* pp. 15-27.
-
-.. [#Arning1996A] Arning, A., Agrawal, R. and Raghavan, P., 1996, August. A Linear Method for Deviation Detection in Large Databases. In *KDD* (Vol. 1141, No. 50, pp. 972-981).
-
-.. [#Bandaragoda2018Isolation] Bandaragoda, T. R., Ting, K. M., Albrecht, D., Liu, F. T., Zhu, Y., and Wells, J. R., 2018, Isolation-based anomaly detection using nearest-neighbor ensembles. *Computational Intelligence*\ , 34(4), pp. 968-998.
-
-.. [#Breunig2000LOF] Breunig, M.M., Kriegel, H.P., Ng, R.T. and Sander, J., 2000, May. LOF: identifying density-based local outliers. *ACM Sigmod Record*\ , 29(2), pp. 93-104.
-
-.. [#Burgess2018Understanding] Burgess, Christopher P., et al. "Understanding disentangling in beta-VAE." arXiv preprint arXiv:1804.03599 (2018).
-
-.. [#Cook1977Detection] Cook, R.D., 1977. Detection of influential observation in linear regression. Technometrics, 19(1), pp.15-18.
-
-.. [#Fang2001Wrap] Fang, K.T. and Ma, C.X., 2001. Wrap-around L2-discrepancy of random sampling, Latin hypercube and uniform designs. Journal of complexity, 17(4), pp.608-624.
-
-.. [#Goldstein2012Histogram] Goldstein, M. and Dengel, A., 2012. Histogram-based outlier score (hbos): A fast unsupervised anomaly detection algorithm. In *KI-2012: Poster and Demo Track*\ , pp.59-63.
-
-.. [#Goodge2022Lunar] Goodge, A., Hooi, B., Ng, S.K. and Ng, W.S., 2022, June. Lunar: Unifying local outlier detection methods via graph neural networks. In Proceedings of the AAAI Conference on Artificial Intelligence.
-
-.. [#Gopalan2019PIDForest] Gopalan, P., Sharan, V. and Wieder, U., 2019. PIDForest: Anomaly Detection via Partial Identification. In Advances in Neural Information Processing Systems, pp. 15783-15793.
-
-.. [#Han2022ADBench] Han, S., Hu, X., Huang, H., Jiang, M. and Zhao, Y., 2022. ADBench: Anomaly Detection Benchmark. arXiv preprint arXiv:2206.09426.
-
-.. [#Hardin2004Outlier] Hardin, J. and Rocke, D.M., 2004. Outlier detection in the multiple cluster setting using the minimum covariance determinant estimator. *Computational Statistics & Data Analysis*\ , 44(4), pp.625-638.
-
-.. [#He2003Discovering] He, Z., Xu, X. and Deng, S., 2003. Discovering cluster-based local outliers. *Pattern Recognition Letters*\ , 24(9-10), pp.1641-1650.
-
-.. [#Hoffmann2007Kernel] Hoffmann, H., 2007. Kernel PCA for novelty detection. Pattern recognition, 40(3), pp.863-874.
-
-.. [#Iglewicz1993How] Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
-
-.. [#Janssens2012Stochastic] Janssens, J.H.M., Huszár, F., Postma, E.O. and van den Herik, H.J., 2012. Stochastic outlier selection. Technical report TiCC TR 2012-001, Tilburg University, Tilburg Center for Cognition and Communication, Tilburg, The Netherlands.
-
-.. [#Kingma2013Auto] Kingma, D.P. and Welling, M., 2013. Auto-encoding variational bayes. arXiv preprint arXiv:1312.6114.
-
-.. [#Kriegel2008Angle] Kriegel, H.P. and Zimek, A., 2008, August. Angle-based outlier detection in high-dimensional data. In *KDD '08*\ , pp. 444-452. ACM.
-
-.. [#Kriegel2009Outlier] Kriegel, H.P., Kröger, P., Schubert, E. and Zimek, A., 2009, April. Outlier detection in axis-parallel subspaces of high dimensional data. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*\ , pp. 831-838. Springer, Berlin, Heidelberg.
-
-.. [#Latecki2007Outlier] Latecki, L.J., Lazarevic, A. and Pokrajac, D., 2007, July. Outlier detection with kernel density functions. In International Workshop on Machine Learning and Data Mining in Pattern Recognition (pp. 61-75). Springer, Berlin, Heidelberg.
-
-.. [#Lazarevic2005Feature] Lazarevic, A. and Kumar, V., 2005, August. Feature bagging for outlier detection. In *KDD '05*. 2005.
-
-.. [#Li2019MADGAN] Li, D., Chen, D., Jin, B., Shi, L., Goh, J. and Ng, S.K., 2019, September. MAD-GAN: Multivariate anomaly detection for time series data with generative adversarial networks. In *International Conference on Artificial Neural Networks* (pp. 703-716). Springer, Cham.
-
-.. [#Li2020COPOD] Li, Z., Zhao, Y., Botta, N., Ionescu, C. and Hu, X. COPOD: Copula-Based Outlier Detection. *IEEE International Conference on Data Mining (ICDM)*, 2020.
-
-.. [#Li2021ECOD] Li, Z., Zhao, Y., Hu, X., Botta, N., Ionescu, C. and Chen, H. G. ECOD: Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions. *IEEE Transactions on Knowledge and Data Engineering (TKDE)*, 2022.
-
-.. [#Liu2008Isolation] Liu, F.T., Ting, K.M. and Zhou, Z.H., 2008, December. Isolation forest. In *International Conference on Data Mining*\ , pp. 413-422. IEEE.
-
-.. [#Liu2019Generative] Liu, Y., Li, Z., Zhou, C., Jiang, Y., Sun, J., Wang, M. and He, X., 2019. Generative adversarial active learning for unsupervised outlier detection. *IEEE Transactions on Knowledge and Data Engineering*.
-
-.. [#Papadimitriou2003LOCI] Papadimitriou, S., Kitagawa, H., Gibbons, P.B. and Faloutsos, C., 2003, March. LOCI: Fast outlier detection using the local correlation integral. In *ICDE '03*, pp. 315-326. IEEE.
-
-.. [#Pevny2016Loda] Pevný, T., 2016. Loda: Lightweight on-line detector of anomalies. *Machine Learning*, 102(2), pp.275-304.
-
-.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
-
-.. [#Ramaswamy2000Efficient] Ramaswamy, S., Rastogi, R. and Shim, K., 2000, May. Efficient algorithms for mining outliers from large data sets. *ACM Sigmod Record*\ , 29(2), pp. 427-438.
-
-.. [#Rousseeuw1999A] Rousseeuw, P.J. and Driessen, K.V., 1999. A fast algorithm for the minimum covariance determinant estimator. *Technometrics*\ , 41(3), pp.212-223.
-
-.. [#Ruff2018Deep] Ruff, L., Vandermeulen, R., Goernitz, N., Deecke, L., Siddiqui, S.A., Binder, A., Müller, E. and Kloft, M., 2018, July. Deep one-class classification. In *International conference on machine learning* (pp. 4393-4402). PMLR.
-
-.. [#Schlegl2017Unsupervised] Schlegl, T., Seeböck, P., Waldstein, S.M., Schmidt-Erfurth, U. and Langs, G., 2017, June. Unsupervised anomaly detection with generative adversarial networks to guide marker discovery. In International conference on information processing in medical imaging (pp. 146-157). Springer, Cham.
-
-.. [#Scholkopf2001Estimating] Scholkopf, B., Platt, J.C., Shawe-Taylor, J., Smola, A.J. and Williamson, R.C., 2001. Estimating the support of a high-dimensional distribution. *Neural Computation*, 13(7), pp.1443-1471.
-
-.. [#Shyu2003A] Shyu, M.L., Chen, S.C., Sarinnapakorn, K. and Chang, L., 2003. A novel anomaly detection scheme based on principal component classifier. *MIAMI UNIV CORAL GABLES FL DEPT OF ELECTRICAL AND COMPUTER ENGINEERING*.
-
-.. [#Sugiyama2013Rapid] Sugiyama, M. and Borgwardt, K., 2013. Rapid distance-based outlier detection via sampling. Advances in neural information processing systems, 26.
-
-.. [#Tang2002Enhancing] Tang, J., Chen, Z., Fu, A.W.C. and Cheung, D.W., 2002, May. Enhancing effectiveness of outlier detections for low density patterns. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*, pp. 535-548. Springer, Berlin, Heidelberg.
-
-.. [#Wang2020adVAE] Wang, X., Du, Y., Lin, S., Cui, P., Shen, Y. and Yang, Y., 2019. adVAE: A self-adversarial variational autoencoder with Gaussian anomaly prior knowledge for anomaly detection. *Knowledge-Based Systems*.
-
-.. [#You2017Provable] You, C., Robinson, D.P. and Vidal, R., 2017. Provable self-representation based outlier detection in a union of subspaces. In Proceedings of the IEEE conference on computer vision and pattern recognition.
-
-.. [#Zenati2018Adversarially] Zenati, H., Romain, M., Foo, C.S., Lecouat, B. and Chandrasekhar, V., 2018, November. Adversarially learned anomaly detection. In 2018 IEEE International conference on data mining (ICDM) (pp. 727-736). IEEE.
-
-.. [#Zhao2018XGBOD] Zhao, Y. and Hryniewicki, M.K. XGBOD: Improving Supervised Outlier Detection with Unsupervised Representation Learning. *IEEE International Joint Conference on Neural Networks*\ , 2018.
-
-.. [#Zhao2019LSCP] Zhao, Y., Nasrullah, Z., Hryniewicki, M.K. and Li, Z., 2019, May. LSCP: Locally selective combination in parallel outlier ensembles. In *Proceedings of the 2019 SIAM International Conference on Data Mining (SDM)*, pp. 585-593. Society for Industrial and Applied Mathematics.
-
-.. [#Zhao2021SUOD] Zhao, Y., Hu, X., Cheng, C., Wang, C., Wan, C., Wang, W., Yang, J., Bai, H., Li, Z., Xiao, C., Wang, Y., Qiao, Z., Sun, J. and Akoglu, L. (2021). SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection. *Conference on Machine Learning and Systems (MLSys)*.
-
-
+Metadata-Version: 2.1
+Name: pyod
+Version: 1.1.0
+Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
+Home-page: https://github.com/yzhao062/pyod
+Author: Yue Zhao
+Author-email: zhaoy@cmu.edu
+License: UNKNOWN
+Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
+Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Python Outlier Detection (PyOD)
+===============================
+
+**Deployment & Documentation & Stats & License**
+
+.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
+   :target: https://pypi.org/project/pyod/
+   :alt: PyPI version
+
+
+.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
+   :target: https://anaconda.org/conda-forge/pyod
+   :alt: Anaconda version
+
+
+.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
+   :target: https://pyod.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation status
+
+
+.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
+   :target: https://github.com/yzhao062/pyod/stargazers
+   :alt: GitHub stars
+
+
+.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
+   :target: https://github.com/yzhao062/pyod/network
+   :alt: GitHub forks
+
+
+.. image:: https://pepy.tech/badge/pyod
+   :target: https://pepy.tech/project/pyod
+   :alt: Downloads
+
+.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
+   :alt: testing
+
+
+.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
+   :target: https://coveralls.io/github/yzhao062/pyod
+   :alt: Coverage Status
+
+
+.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
+   :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
+   :alt: Maintainability
+
+
+.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
+   :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
+   :alt: License
+
+.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
+   :target: https://github.com/Minqi824/ADBench
+   :alt: Benchmark
+
+
+-----
+
+**News**: We just released a 45-page, the most comprehensive `anomaly detection benchmark paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_.
+The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
+
+**For time-series outlier detection**, please use `TODS <https://github.com/datamllab/tods>`_.
+**For graph outlier detection**, please use `PyGOD <https://pygod.org/>`_.
+
+PyOD is the most comprehensive and scalable **Python library** for **detecting outlying objects** in
+multivariate data. This exciting yet challenging field is commonly referred as 
+`Outlier Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_
+or `Anomaly Detection <https://en.wikipedia.org/wiki/Anomaly_detection>`_.
+
+PyOD includes more than 40 detection algorithms, from classical LOF (SIGMOD 2000) to
+the latest ECOD (TKDE 2022). Since 2017, PyOD has been successfully used in numerous academic researches and
+commercial products with more than `10 million downloads <https://pepy.tech/project/pyod>`_.
+It is also well acknowledged by the machine learning community with various dedicated posts/tutorials, including
+`Analytics Vidhya <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_,
+`KDnuggets <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, and
+`Towards Data Science <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_.
+
+
+**PyOD is featured for**:
+
+* **Unified APIs, detailed documentation, and interactive examples** across various algorithms.
+* **Advanced models**\, including **classical distance and density estimation**, **latest deep learning methods**, and **emerging algorithms like ECOD**.
+* **Optimized performance with JIT and parallelization** using `numba <https://github.com/numba/numba>`_ and `joblib <https://github.com/joblib/joblib>`_.
+* **Fast training & prediction with SUOD** [#Zhao2021SUOD]_.
+
+
+**Outlier Detection with 5 Lines of Code**\ :
+
+
+.. code-block:: python
+
+
+    # train an ECOD detector
+    from pyod.models.ecod import ECOD
+    clf = ECOD()
+    clf.fit(X_train)
+
+    # get outlier scores
+    y_train_scores = clf.decision_scores_  # raw outlier scores on the train data
+    y_test_scores = clf.decision_function(X_test)  # predict raw outlier scores on test
+
+
+**Personal suggestion on selecting an OD algorithm**. If you do not know which algorithm to try, go with:
+
+- `ECOD <https://github.com/yzhao062/pyod/blob/master/examples/ecod_example.py>`_: Example of using ECOD for outlier detection
+- `Isolation Forest <https://github.com/yzhao062/pyod/blob/master/examples/iforest_example.py>`_: Example of using Isolation Forest for outlier detection
+
+They are both fast and interpretable. Or, you could try more data-driven approach `MetaOD <https://github.com/yzhao062/MetaOD>`_.
+
+**Citing PyOD**\ :
+
+`PyOD paper <http://www.jmlr.org/papers/volume20/19-011/19-011.pdf>`_ is published in
+`Journal of Machine Learning Research (JMLR) <http://www.jmlr.org/>`_ (MLOSS track).
+If you use PyOD in a scientific publication, we would appreciate
+citations to the following paper::
+
+    @article{zhao2019pyod,
+        author  = {Zhao, Yue and Nasrullah, Zain and Li, Zheng},
+        title   = {PyOD: A Python Toolbox for Scalable Outlier Detection},
+        journal = {Journal of Machine Learning Research},
+        year    = {2019},
+        volume  = {20},
+        number  = {96},
+        pages   = {1-7},
+        url     = {http://jmlr.org/papers/v20/19-011.html}
+    }
+
+or::
+
+    Zhao, Y., Nasrullah, Z. and Li, Z., 2019. PyOD: A Python Toolbox for Scalable Outlier Detection. Journal of machine learning research (JMLR), 20(96), pp.1-7.
+
+If you want more general insights of anomaly detection and/or algorithm performance comparison, please see our
+NeurIPS 2022 paper `ADBench: Anomaly Detection Benchmark Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/22-neurips-adbench.pdf>`_::
+
+    @inproceedings{han2022adbench,
+        title={ADBench: Anomaly Detection Benchmark},
+        author={Songqiao Han and Xiyang Hu and Hailiang Huang and Mingqi Jiang and Yue Zhao},
+        booktitle={Neural Information Processing Systems (NeurIPS)}
+        year={2022},
+    }
+
+**Key Links and Resources**\ :
+
+
+* `View the latest codes on Github <https://github.com/yzhao062/pyod>`_
+* `Anomaly Detection Resources <https://github.com/yzhao062/anomaly-detection-resources>`_
+
+
+**Table of Contents**\ :
+
+
+* `Installation <#installation>`_
+* `API Cheatsheet & Reference <#api-cheatsheet--reference>`_
+* `ADBench Benchmark <#adbench-benchmark>`_
+* `Model Save & Load <#model-save--load>`_
+* `Fast Train with SUOD <#fast-train-with-suod>`_
+* `Thresholding Outlier Scores <#thresholding-outlier-scores>`_
+* `Implemented Algorithms <#implemented-algorithms>`_
+* `Quick Start for Outlier Detection <#quick-start-for-outlier-detection>`_
+* `How to Contribute <#how-to-contribute>`_
+* `Inclusion Criteria <#inclusion-criteria>`_
+
+
+----
+
+
+Installation
+^^^^^^^^^^^^
+
+It is recommended to use **pip** or **conda** for installation. Please make sure
+**the latest version** is installed, as PyOD is updated frequently:
+
+.. code-block:: bash
+
+   pip install pyod            # normal install
+   pip install --upgrade pyod  # or update if needed
+
+.. code-block:: bash
+
+   conda install -c conda-forge pyod
+
+Alternatively, you could clone and run setup.py file:
+
+.. code-block:: bash
+
+   git clone https://github.com/yzhao062/pyod.git
+   cd pyod
+   pip install .
+
+
+**Required Dependencies**\ :
+
+
+* Python 3.6+
+* joblib
+* matplotlib
+* numpy>=1.19
+* numba>=0.51
+* scipy>=1.5.1
+* scikit_learn>=0.20.0
+* six
+
+**Optional Dependencies (see details below)**\ :
+
+* combo (optional, required for models/combination.py and FeatureBagging)
+* keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
+* pandas (optional, required for running benchmark)
+* suod (optional, required for running SUOD model)
+* xgboost (optional, required for XGBOD)
+* pythresh to use thresholding
+
+**Warning**\ :
+PyOD has multiple neural network based models, e.g., AutoEncoders, which are
+implemented in both Tensorflow and PyTorch. However, PyOD does **NOT** install these deep learning libraries for you.
+This reduces the risk of interfering with your local copies.
+If you want to use neural-net based models, please make sure these deep learning libraries are installed.
+Instructions are provided: `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_.
+Similarly, models depending on **xgboost**, e.g., XGBOD, would **NOT** enforce xgboost installation by default.
+
+
+
+----
+
+
+API Cheatsheet & Reference
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Full API Reference: (https://pyod.readthedocs.io/en/latest/pyod.html). API cheatsheet for all detectors:
+
+
+* **fit(X)**\ : Fit detector. y is ignored in unsupervised methods.
+* **decision_function(X)**\ : Predict raw anomaly score of X using the fitted detector.
+* **predict(X)**\ : Predict if a particular sample is an outlier or not using the fitted detector.
+* **predict_proba(X)**\ : Predict the probability of a sample being outlier using the fitted detector.
+* **predict_confidence(X)**\ : Predict the model's sample-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
+
+
+Key Attributes of a fitted model:
+
+
+* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
+  Outliers tend to have higher scores.
+* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
+
+
+----
+
+
+ADBench Benchmark
+^^^^^^^^^^^^^^^^^
+
+We just released a 45-page, the most comprehensive `ADBench: Anomaly Detection Benchmark <https://arxiv.org/abs/2206.09426>`_ [#Han2022ADBench]_.
+The fully `open-sourced ADBench <https://github.com/Minqi824/ADBench>`_ compares 30 anomaly detection algorithms on 57 benchmark datasets.
+
+The organization of **ADBench** is provided below:
+
+.. image:: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
+   :target: https://github.com/Minqi824/ADBench/blob/main/figs/ADBench.png?raw=true
+   :alt: benchmark-fig
+
+
+**The comparison of selected models** is made available below
+(\ `Figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png>`_\ ,
+`compare_all_models.py <https://github.com/yzhao062/pyod/blob/master/examples/compare_all_models.py>`_\ ,
+`Interactive Jupyter Notebooks <https://mybinder.org/v2/gh/yzhao062/pyod/master>`_\ ).
+For Jupyter Notebooks, please navigate to **"/notebooks/Compare All Models.ipynb"**.
+
+
+.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
+   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/ALL.png
+   :alt: Comparision_of_All
+
+
+
+----
+
+Model Save & Load
+^^^^^^^^^^^^^^^^^
+
+PyOD takes a similar approach of sklearn regarding model persistence.
+See `model persistence <https://scikit-learn.org/stable/modules/model_persistence.html>`_ for clarification.
+
+In short, we recommend to use joblib or pickle for saving and loading PyOD models.
+See `"examples/save_load_model_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/save_load_model_example.py>`_ for an example.
+In short, it is simple as below:
+
+.. code-block:: python
+
+    from joblib import dump, load
+
+    # save the model
+    dump(clf, 'clf.joblib')
+    # load the model
+    clf = load('clf.joblib')
+
+It is known that there are challenges in saving neural network models.
+Check `#328 <https://github.com/yzhao062/pyod/issues/328#issuecomment-917192704>`_
+and `#88 <https://github.com/yzhao062/pyod/issues/88#issuecomment-615343139>`_
+for temporary workaround.
+
+
+----
+
+
+Fast Train with SUOD
+^^^^^^^^^^^^^^^^^^^^
+
+**Fast training and prediction**: it is possible to train and predict with
+a large number of detection models in PyOD by leveraging SUOD framework [#Zhao2021SUOD]_.
+See  `SUOD Paper <https://www.andrew.cmu.edu/user/yuezhao2/papers/21-mlsys-suod.pdf>`_
+and  `SUOD example <https://github.com/yzhao062/pyod/blob/master/examples/suod_example.py>`_.
+
+
+.. code-block:: python
+
+    from pyod.models.suod import SUOD
+
+    # initialized a group of outlier detectors for acceleration
+    detector_list = [LOF(n_neighbors=15), LOF(n_neighbors=20),
+                     LOF(n_neighbors=25), LOF(n_neighbors=35),
+                     COPOD(), IForest(n_estimators=100),
+                     IForest(n_estimators=200)]
+
+    # decide the number of parallel process, and the combination method
+    # then clf can be used as any outlier detection model
+    clf = SUOD(base_estimators=detector_list, n_jobs=2, combination='average',
+               verbose=False)
+
+----
+
+Thresholding Outlier Scores
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+A more data based approach can be taken when setting the contamination level.
+By using a thresholding method, guessing an abritrary value can be replaced
+with tested techniques for seperating inliers and outliers. Refer to 
+`PyThresh <https://github.com/KulikDM/pythresh>`_ for
+a more in depth look at thresholding.
+
+
+.. code-block:: python
+
+    from pyod.models.knn import KNN
+    from pyod.models.thresholds import FILTER
+
+    # Set the outlier detection and thresholding methods
+    clf = KNN(contamination=FILTER())
+
+
+----
+
+
+
+Implemented Algorithms
+^^^^^^^^^^^^^^^^^^^^^^
+
+PyOD toolkit consists of four major functional groups:
+
+**(i) Individual Detection Algorithms** :
+
+===================  ==================  ======================================================================================================  =====  ========================================
+Type                 Abbr                Algorithm                                                                                               Year   Ref
+===================  ==================  ======================================================================================================  =====  ========================================
+Probabilistic        ECOD                Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions                        2022   [#Li2021ECOD]_
+Probabilistic        ABOD                Angle-Based Outlier Detection                                                                           2008   [#Kriegel2008Angle]_
+Probabilistic        FastABOD            Fast Angle-Based Outlier Detection using approximation                                                  2008   [#Kriegel2008Angle]_
+Probabilistic        COPOD               COPOD: Copula-Based Outlier Detection                                                                   2020   [#Li2020COPOD]_
+Probabilistic        MAD                 Median Absolute Deviation (MAD)                                                                         1993   [#Iglewicz1993How]_
+Probabilistic        SOS                 Stochastic Outlier Selection                                                                            2012   [#Janssens2012Stochastic]_
+Probabilistic        QMCD                Quasi-Monte Carlo Discrepancy outlier detection                                                         2001   [#Fang2001Wrap]_
+Probabilistic        KDE                 Outlier Detection with Kernel Density Functions                                                         2007   [#Latecki2007Outlier]_
+Probabilistic        Sampling            Rapid distance-based outlier detection via sampling                                                     2013   [#Sugiyama2013Rapid]_
+Probabilistic        GMM                 Probabilistic Mixture Modeling for Outlier Analysis                                                            [#Aggarwal2015Outlier]_ [Ch.2]
+Linear Model         PCA                 Principal Component Analysis (the sum of weighted projected distances to the eigenvector hyperplanes)   2003   [#Shyu2003A]_
+Linear Model         KPCA                Kernel Principal Component Analysis                                                                     2007   [#Hoffmann2007Kernel]_
+Linear Model         MCD                 Minimum Covariance Determinant (use the mahalanobis distances as the outlier scores)                    1999   [#Hardin2004Outlier]_ [#Rousseeuw1999A]_
+Linear Model         CD                  Use Cook's distance for outlier detection                                                               1977   [#Cook1977Detection]_
+Linear Model         OCSVM               One-Class Support Vector Machines                                                                       2001   [#Scholkopf2001Estimating]_
+Linear Model         LMDD                Deviation-based Outlier Detection (LMDD)                                                                1996   [#Arning1996A]_
+Proximity-Based      LOF                 Local Outlier Factor                                                                                    2000   [#Breunig2000LOF]_
+Proximity-Based      COF                 Connectivity-Based Outlier Factor                                                                       2002   [#Tang2002Enhancing]_
+Proximity-Based      (Incremental) COF   Memory Efficient Connectivity-Based Outlier Factor (slower but reduce storage complexity)               2002   [#Tang2002Enhancing]_
+Proximity-Based      CBLOF               Clustering-Based Local Outlier Factor                                                                   2003   [#He2003Discovering]_
+Proximity-Based      LOCI                LOCI: Fast outlier detection using the local correlation integral                                       2003   [#Papadimitriou2003LOCI]_
+Proximity-Based      HBOS                Histogram-based Outlier Score                                                                           2012   [#Goldstein2012Histogram]_
+Proximity-Based      kNN                 k Nearest Neighbors (use the distance to the kth nearest neighbor as the outlier score)                 2000   [#Ramaswamy2000Efficient]_
+Proximity-Based      AvgKNN              Average kNN (use the average distance to k nearest neighbors as the outlier score)                      2002   [#Angiulli2002Fast]_
+Proximity-Based      MedKNN              Median kNN (use the median distance to k nearest neighbors as the outlier score)                        2002   [#Angiulli2002Fast]_
+Proximity-Based      SOD                 Subspace Outlier Detection                                                                              2009   [#Kriegel2009Outlier]_
+Proximity-Based      ROD                 Rotation-based Outlier Detection                                                                        2020   [#Almardeny2020A]_
+Outlier Ensembles    IForest             Isolation Forest                                                                                        2008   [#Liu2008Isolation]_
+Outlier Ensembles    INNE                Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                      2018   [#Bandaragoda2018Isolation]_
+Outlier Ensembles    FB                  Feature Bagging                                                                                         2005   [#Lazarevic2005Feature]_
+Outlier Ensembles    LSCP                LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                       2019   [#Zhao2019LSCP]_
+Outlier Ensembles    XGBOD               Extreme Boosting Based Outlier Detection **(Supervised)**                                               2018   [#Zhao2018XGBOD]_
+Outlier Ensembles    LODA                Lightweight On-line Detector of Anomalies                                                               2016   [#Pevny2016Loda]_
+Outlier Ensembles    SUOD                SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**          2021   [#Zhao2021SUOD]_
+Neural Networks      AutoEncoder         Fully connected AutoEncoder (use reconstruction error as the outlier score)                                    [#Aggarwal2015Outlier]_ [Ch.3]
+Neural Networks      VAE                 Variational AutoEncoder (use reconstruction error as the outlier score)                                 2013   [#Kingma2013Auto]_
+Neural Networks      Beta-VAE            Variational AutoEncoder (all customized loss term by varying gamma and capacity)                        2018   [#Burgess2018Understanding]_
+Neural Networks      SO_GAAL             Single-Objective Generative Adversarial Active Learning                                                 2019   [#Liu2019Generative]_
+Neural Networks      MO_GAAL             Multiple-Objective Generative Adversarial Active Learning                                               2019   [#Liu2019Generative]_
+Neural Networks      DeepSVDD            Deep One-Class Classification                                                                           2018   [#Ruff2018Deep]_
+Neural Networks      AnoGAN              Anomaly Detection with Generative Adversarial Networks                                                  2017   [#Schlegl2017Unsupervised]_
+Neural Networks      ALAD                Adversarially learned anomaly detection                                                                 2018   [#Zenati2018Adversarially]_
+Graph-based          R-Graph             Outlier detection by R-graph                                                                            2017   [#You2017Provable]_
+Graph-based          LUNAR               LUNAR: Unifying Local Outlier Detection Methods via Graph Neural Networks                               2022   [#Goodge2022Lunar]_
+===================  ==================  ======================================================================================================  =====  ========================================
+
+
+**(ii) Outlier Ensembles & Outlier Detector Combination Frameworks**:
+
+===================  ================  =====================================================================================================  =====  ========================================
+Type                 Abbr              Algorithm                                                                                              Year   Ref
+===================  ================  =====================================================================================================  =====  ========================================
+Outlier Ensembles    FB                Feature Bagging                                                                                        2005   [#Lazarevic2005Feature]_
+Outlier Ensembles    LSCP              LSCP: Locally Selective Combination of Parallel Outlier Ensembles                                      2019   [#Zhao2019LSCP]_
+Outlier Ensembles    XGBOD             Extreme Boosting Based Outlier Detection **(Supervised)**                                              2018   [#Zhao2018XGBOD]_
+Outlier Ensembles    LODA              Lightweight On-line Detector of Anomalies                                                              2016   [#Pevny2016Loda]_
+Outlier Ensembles    SUOD              SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection **(Acceleration)**         2021   [#Zhao2021SUOD]_
+Outlier Ensembles    INNE              Isolation-based Anomaly Detection Using Nearest-Neighbor Ensembles                                     2018   [#Bandaragoda2018Isolation]_
+Combination          Average           Simple combination by averaging the scores                                                             2015   [#Aggarwal2015Theoretical]_
+Combination          Weighted Average  Simple combination by averaging the scores with detector weights                                       2015   [#Aggarwal2015Theoretical]_
+Combination          Maximization      Simple combination by taking the maximum scores                                                        2015   [#Aggarwal2015Theoretical]_
+Combination          AOM               Average of Maximum                                                                                     2015   [#Aggarwal2015Theoretical]_
+Combination          MOA               Maximization of Average                                                                                2015   [#Aggarwal2015Theoretical]_
+Combination          Median            Simple combination by taking the median of the scores                                                  2015   [#Aggarwal2015Theoretical]_
+Combination          majority Vote     Simple combination by taking the majority vote of the labels (weights can be used)                     2015   [#Aggarwal2015Theoretical]_
+===================  ================  =====================================================================================================  =====  ========================================
+
+**(iii) Outlier Detection Score Thresholding Methods**:
+
+==================================  ================  ================================================================ ====================================================================================================================
+Type                                Abbr              Algorithm                                                        Documentation                                    
+==================================  ================  ================================================================ ====================================================================================================================
+Kernel-Based                        AUCP              Area Under Curve Percentage                                      `AUCP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.AUCP>`_
+Statistical Moment-Based            BOOT              Bootstrapping                                                    `BOOT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.BOOT>`_ 
+Normality-Based                     CHAU              Chauvenet's Criterion                                            `CHAU <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CHAU>`_
+Linear Model                        CLF               Trained Linear Classifier                                        `CLF <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLF>`_
+cluster-Based                       CLUST             Clustering Based                                                 `CLUST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CLUST>`_
+Kernel-Based                        CPD               Change Point Detection                                           `CPD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.CPD>`_
+Transformation-Based                DECOMP            Decomposition                                                    `DECOMP <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DECOMP>`_
+Normality-Based                     DSN               Distance Shift from Normal                                       `DSN <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.DSN>`_
+Curve-Based                         EB                Elliptical Boundary                                              `EB <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.EB>`_
+Kernel-Based                        FGD               Fixed Gradient Descent                                           `FGD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FGD>`_
+Filter-Based                        FILTER            Filtering Based                                                  `FILTER <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FILTER>`_
+Curve-Based                         FWFM              Full Width at Full Minimum                                       `FWFM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.FWFM>`_
+Statistical Test-Based              GESD              Generalized Extreme Studentized Deviate                          `GESD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.GESD>`_
+Filter-Based                        HIST              Histogram Based                                                  `HIST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.HIST>`_
+Quantile-Based                      IQR               Inter-Quartile Region                                            `IQR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.IQR>`_
+Statistical Moment-Based            KARCH             Karcher mean (Riemannian Center of Mass)                         `KARCH <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.KARCH>`_
+Statistical Moment-Based            MAD               Median Absolute Deviation                                        `MAD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MAD>`_
+Statistical Test-Based              MCST              Monte Carlo Shapiro Tests                                        `MCST <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MCST>`_
+Ensembles-Based                     META              Meta-model Trained Classifier                                    `META <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.META>`_
+Transformation-Based                MOLL              Friedrichs' Mollifier                                            `MOLL <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MOLL>`_
+Statistical Test-Based              MTT               Modified Thompson Tau Test                                       `MTT <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.MTT>`_
+Linear Model                        OCSVM             One-Class Support Vector Machine                                 `OCSVM <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.OCSVM>`_
+Quantile-Based                      QMCD              Quasi-Monte Carlo Discrepancy                                    `QMCD <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.QMCD>`_
+Linear Model                        REGR              Regression Based                                                 `REGR <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.REGR>`_
+Neural Networks                     VAE               Variational Autoencoder                                          `VAE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.VAE>`_
+Curve-Based                         WIND              Topological Winding Number                                       `WIND <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.WIND>`_
+Transformation-Based                YJ                Yeo-Johnson Transformation                                       `YJ <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.YJ>`_
+Normality-Based                     ZSCORE            Z-score                                                          `ZSCORE <https://pyod.readthedocs.io/en/latest/pyod.models.html#module-pyod.models.thresholds.ZSCORE>`_
+==================================  ================  ================================================================ ====================================================================================================================
+
+
+**(iV) Utility Functions**:
+
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+Type                 Name                    Function                                                                                                                                               Documentation
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+Data                 generate_data           Synthesized data generation; normal data is generated by a multivariate Gaussian and outliers are generated by a uniform distribution                  `generate_data <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.data.generate_data>`_
+Data                 generate_data_clusters  Synthesized data generation in clusters; more complex data patterns can be created with multiple clusters                                              `generate_data_clusters <https://pyod.readthedocs.io/en/latest/pyod.utils.html#pyod.utils.data.generate_data_clusters>`_
+Stat                 wpearsonr               Calculate the weighted Pearson correlation of two samples                                                                                              `wpearsonr <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.stat_models.wpearsonr>`_
+Utility              get_label_n             Turn raw outlier scores into binary labels by assign 1 to top n outlier scores                                                                         `get_label_n <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.get_label_n>`_
+Utility              precision_n_scores      calculate precision @ rank n                                                                                                                           `precision_n_scores <https://pyod.readthedocs.io/en/latest/pyod.utils.html#module-pyod.utils.utility.precision_n_scores>`_
+===================  ======================  =====================================================================================================================================================  ======================================================================================================================================
+
+----
+
+Quick Start for Outlier Detection
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+PyOD has been well acknowledged by the machine learning community with a few featured posts and tutorials.
+
+**Analytics Vidhya**: `An Awesome Tutorial to Learn Outlier Detection in Python using PyOD Library <https://www.analyticsvidhya.com/blog/2019/02/outlier-detection-python-pyod/>`_
+
+**KDnuggets**: `Intuitive Visualization of Outlier Detection Methods <https://www.kdnuggets.com/2019/02/outlier-detection-methods-cheat-sheet.html>`_, `An Overview of Outlier Detection Methods from PyOD <https://www.kdnuggets.com/2019/06/overview-outlier-detection-methods-pyod.html>`_
+
+**Towards Data Science**: `Anomaly Detection for Dummies <https://towardsdatascience.com/anomaly-detection-for-dummies-15f148e559c1>`_
+
+**Computer Vision News (March 2019)**: `Python Open Source Toolbox for Outlier Detection <https://rsipvision.com/ComputerVisionNews-2019March/18/>`_
+
+`"examples/knn_example.py" <https://github.com/yzhao062/pyod/blob/master/examples/knn_example.py>`_
+demonstrates the basic API of using kNN detector. **It is noted that the API across all other algorithms are consistent/similar**.
+
+More detailed instructions for running examples can be found in `examples directory <https://github.com/yzhao062/pyod/blob/master/examples>`_.
+
+
+#. Initialize a kNN detector, fit the model, and make the prediction.
+
+   .. code-block:: python
+
+
+       from pyod.models.knn import KNN   # kNN detector
+
+       # train kNN detector
+       clf_name = 'KNN'
+       clf = KNN()
+       clf.fit(X_train)
+
+       # get the prediction label and outlier scores of the training data
+       y_train_pred = clf.labels_  # binary labels (0: inliers, 1: outliers)
+       y_train_scores = clf.decision_scores_  # raw outlier scores
+
+       # get the prediction on the test data
+       y_test_pred = clf.predict(X_test)  # outlier labels (0 or 1)
+       y_test_scores = clf.decision_function(X_test)  # outlier scores
+
+       # it is possible to get the prediction confidence as well
+       y_test_pred, y_test_pred_confidence = clf.predict(X_test, return_confidence=True)  # outlier labels (0 or 1) and confidence in the range of [0,1]
+
+#. Evaluate the prediction by ROC and Precision @ Rank n (p@n).
+
+   .. code-block:: python
+
+       from pyod.utils.data import evaluate_print
+       
+       # evaluate and print the results
+       print("\nOn Training Data:")
+       evaluate_print(clf_name, y_train, y_train_scores)
+       print("\nOn Test Data:")
+       evaluate_print(clf_name, y_test, y_test_scores)
+
+
+#. See a sample output & visualization.
+
+
+   .. code-block:: python
+
+
+       On Training Data:
+       KNN ROC:1.0, precision @ rank n:1.0
+
+       On Test Data:
+       KNN ROC:0.9989, precision @ rank n:0.9
+
+   .. code-block:: python
+
+
+       visualize(clf_name, X_train, y_train, X_test, y_test, y_train_pred,
+           y_test_pred, show_figure=True, save_figure=False)
+
+Visualization (\ `knn_figure <https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png>`_\ ):
+
+.. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
+   :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
+   :alt: kNN example figure
+
+----
+
+How to Contribute
+^^^^^^^^^^^^^^^^^
+
+You are welcome to contribute to this exciting project:
+
+
+* Please first check Issue lists for "help wanted" tag and comment the one
+  you are interested. We will assign the issue to you.
+
+* Fork the master branch and add your improvement/modification/fix.
+
+* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
+
+* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
+
+
+To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
+
+You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
+
+
+Inclusion Criteria
+^^^^^^^^^^^^^^^^^^
+
+Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
+We mainly consider well-established algorithms for inclusion.
+A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
+
+However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
+for boosting ML accessibility and reproducibility.
+This exception only applies if you could commit to the maintenance of your model for at least two year period.
+
+
+----
+
+Reference
+^^^^^^^^^
+
+
+.. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
+
+.. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
+
+.. [#Aggarwal2017Outlier] Aggarwal, C.C. and Sathe, S., 2017. Outlier ensembles: An introduction. Springer.
+
+.. [#Almardeny2020A] Almardeny, Y., Boujnah, N. and Cleary, F., 2020. A Novel Outlier Detection Method for Multivariate Data. *IEEE Transactions on Knowledge and Data Engineering*.
+
+.. [#Angiulli2002Fast] Angiulli, F. and Pizzuti, C., 2002, August. Fast outlier detection in high dimensional spaces. In *European Conference on Principles of Data Mining and Knowledge Discovery* pp. 15-27.
+
+.. [#Arning1996A] Arning, A., Agrawal, R. and Raghavan, P., 1996, August. A Linear Method for Deviation Detection in Large Databases. In *KDD* (Vol. 1141, No. 50, pp. 972-981).
+
+.. [#Bandaragoda2018Isolation] Bandaragoda, T. R., Ting, K. M., Albrecht, D., Liu, F. T., Zhu, Y., and Wells, J. R., 2018, Isolation-based anomaly detection using nearest-neighbor ensembles. *Computational Intelligence*\ , 34(4), pp. 968-998.
+
+.. [#Breunig2000LOF] Breunig, M.M., Kriegel, H.P., Ng, R.T. and Sander, J., 2000, May. LOF: identifying density-based local outliers. *ACM Sigmod Record*\ , 29(2), pp. 93-104.
+
+.. [#Burgess2018Understanding] Burgess, Christopher P., et al. "Understanding disentangling in beta-VAE." arXiv preprint arXiv:1804.03599 (2018).
+
+.. [#Cook1977Detection] Cook, R.D., 1977. Detection of influential observation in linear regression. Technometrics, 19(1), pp.15-18.
+
+.. [#Fang2001Wrap] Fang, K.T. and Ma, C.X., 2001. Wrap-around L2-discrepancy of random sampling, Latin hypercube and uniform designs. Journal of complexity, 17(4), pp.608-624.
+
+.. [#Goldstein2012Histogram] Goldstein, M. and Dengel, A., 2012. Histogram-based outlier score (hbos): A fast unsupervised anomaly detection algorithm. In *KI-2012: Poster and Demo Track*\ , pp.59-63.
+
+.. [#Goodge2022Lunar] Goodge, A., Hooi, B., Ng, S.K. and Ng, W.S., 2022, June. Lunar: Unifying local outlier detection methods via graph neural networks. In Proceedings of the AAAI Conference on Artificial Intelligence.
+
+.. [#Gopalan2019PIDForest] Gopalan, P., Sharan, V. and Wieder, U., 2019. PIDForest: Anomaly Detection via Partial Identification. In Advances in Neural Information Processing Systems, pp. 15783-15793.
+
+.. [#Han2022ADBench] Han, S., Hu, X., Huang, H., Jiang, M. and Zhao, Y., 2022. ADBench: Anomaly Detection Benchmark. arXiv preprint arXiv:2206.09426.
+
+.. [#Hardin2004Outlier] Hardin, J. and Rocke, D.M., 2004. Outlier detection in the multiple cluster setting using the minimum covariance determinant estimator. *Computational Statistics & Data Analysis*\ , 44(4), pp.625-638.
+
+.. [#He2003Discovering] He, Z., Xu, X. and Deng, S., 2003. Discovering cluster-based local outliers. *Pattern Recognition Letters*\ , 24(9-10), pp.1641-1650.
+
+.. [#Hoffmann2007Kernel] Hoffmann, H., 2007. Kernel PCA for novelty detection. Pattern recognition, 40(3), pp.863-874.
+
+.. [#Iglewicz1993How] Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
+
+.. [#Janssens2012Stochastic] Janssens, J.H.M., Huszár, F., Postma, E.O. and van den Herik, H.J., 2012. Stochastic outlier selection. Technical report TiCC TR 2012-001, Tilburg University, Tilburg Center for Cognition and Communication, Tilburg, The Netherlands.
+
+.. [#Kingma2013Auto] Kingma, D.P. and Welling, M., 2013. Auto-encoding variational bayes. arXiv preprint arXiv:1312.6114.
+
+.. [#Kriegel2008Angle] Kriegel, H.P. and Zimek, A., 2008, August. Angle-based outlier detection in high-dimensional data. In *KDD '08*\ , pp. 444-452. ACM.
+
+.. [#Kriegel2009Outlier] Kriegel, H.P., Kröger, P., Schubert, E. and Zimek, A., 2009, April. Outlier detection in axis-parallel subspaces of high dimensional data. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*\ , pp. 831-838. Springer, Berlin, Heidelberg.
+
+.. [#Latecki2007Outlier] Latecki, L.J., Lazarevic, A. and Pokrajac, D., 2007, July. Outlier detection with kernel density functions. In International Workshop on Machine Learning and Data Mining in Pattern Recognition (pp. 61-75). Springer, Berlin, Heidelberg.
+
+.. [#Lazarevic2005Feature] Lazarevic, A. and Kumar, V., 2005, August. Feature bagging for outlier detection. In *KDD '05*. 2005.
+
+.. [#Li2019MADGAN] Li, D., Chen, D., Jin, B., Shi, L., Goh, J. and Ng, S.K., 2019, September. MAD-GAN: Multivariate anomaly detection for time series data with generative adversarial networks. In *International Conference on Artificial Neural Networks* (pp. 703-716). Springer, Cham.
+
+.. [#Li2020COPOD] Li, Z., Zhao, Y., Botta, N., Ionescu, C. and Hu, X. COPOD: Copula-Based Outlier Detection. *IEEE International Conference on Data Mining (ICDM)*, 2020.
+
+.. [#Li2021ECOD] Li, Z., Zhao, Y., Hu, X., Botta, N., Ionescu, C. and Chen, H. G. ECOD: Unsupervised Outlier Detection Using Empirical Cumulative Distribution Functions. *IEEE Transactions on Knowledge and Data Engineering (TKDE)*, 2022.
+
+.. [#Liu2008Isolation] Liu, F.T., Ting, K.M. and Zhou, Z.H., 2008, December. Isolation forest. In *International Conference on Data Mining*\ , pp. 413-422. IEEE.
+
+.. [#Liu2019Generative] Liu, Y., Li, Z., Zhou, C., Jiang, Y., Sun, J., Wang, M. and He, X., 2019. Generative adversarial active learning for unsupervised outlier detection. *IEEE Transactions on Knowledge and Data Engineering*.
+
+.. [#Papadimitriou2003LOCI] Papadimitriou, S., Kitagawa, H., Gibbons, P.B. and Faloutsos, C., 2003, March. LOCI: Fast outlier detection using the local correlation integral. In *ICDE '03*, pp. 315-326. IEEE.
+
+.. [#Pevny2016Loda] Pevný, T., 2016. Loda: Lightweight on-line detector of anomalies. *Machine Learning*, 102(2), pp.275-304.
+
+.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
+
+.. [#Ramaswamy2000Efficient] Ramaswamy, S., Rastogi, R. and Shim, K., 2000, May. Efficient algorithms for mining outliers from large data sets. *ACM Sigmod Record*\ , 29(2), pp. 427-438.
+
+.. [#Rousseeuw1999A] Rousseeuw, P.J. and Driessen, K.V., 1999. A fast algorithm for the minimum covariance determinant estimator. *Technometrics*\ , 41(3), pp.212-223.
+
+.. [#Ruff2018Deep] Ruff, L., Vandermeulen, R., Goernitz, N., Deecke, L., Siddiqui, S.A., Binder, A., Müller, E. and Kloft, M., 2018, July. Deep one-class classification. In *International conference on machine learning* (pp. 4393-4402). PMLR.
+
+.. [#Schlegl2017Unsupervised] Schlegl, T., Seeböck, P., Waldstein, S.M., Schmidt-Erfurth, U. and Langs, G., 2017, June. Unsupervised anomaly detection with generative adversarial networks to guide marker discovery. In International conference on information processing in medical imaging (pp. 146-157). Springer, Cham.
+
+.. [#Scholkopf2001Estimating] Scholkopf, B., Platt, J.C., Shawe-Taylor, J., Smola, A.J. and Williamson, R.C., 2001. Estimating the support of a high-dimensional distribution. *Neural Computation*, 13(7), pp.1443-1471.
+
+.. [#Shyu2003A] Shyu, M.L., Chen, S.C., Sarinnapakorn, K. and Chang, L., 2003. A novel anomaly detection scheme based on principal component classifier. *MIAMI UNIV CORAL GABLES FL DEPT OF ELECTRICAL AND COMPUTER ENGINEERING*.
+
+.. [#Sugiyama2013Rapid] Sugiyama, M. and Borgwardt, K., 2013. Rapid distance-based outlier detection via sampling. Advances in neural information processing systems, 26.
+
+.. [#Tang2002Enhancing] Tang, J., Chen, Z., Fu, A.W.C. and Cheung, D.W., 2002, May. Enhancing effectiveness of outlier detections for low density patterns. In *Pacific-Asia Conference on Knowledge Discovery and Data Mining*, pp. 535-548. Springer, Berlin, Heidelberg.
+
+.. [#Wang2020adVAE] Wang, X., Du, Y., Lin, S., Cui, P., Shen, Y. and Yang, Y., 2019. adVAE: A self-adversarial variational autoencoder with Gaussian anomaly prior knowledge for anomaly detection. *Knowledge-Based Systems*.
+
+.. [#You2017Provable] You, C., Robinson, D.P. and Vidal, R., 2017. Provable self-representation based outlier detection in a union of subspaces. In Proceedings of the IEEE conference on computer vision and pattern recognition.
+
+.. [#Zenati2018Adversarially] Zenati, H., Romain, M., Foo, C.S., Lecouat, B. and Chandrasekhar, V., 2018, November. Adversarially learned anomaly detection. In 2018 IEEE International conference on data mining (ICDM) (pp. 727-736). IEEE.
+
+.. [#Zhao2018XGBOD] Zhao, Y. and Hryniewicki, M.K. XGBOD: Improving Supervised Outlier Detection with Unsupervised Representation Learning. *IEEE International Joint Conference on Neural Networks*\ , 2018.
+
+.. [#Zhao2019LSCP] Zhao, Y., Nasrullah, Z., Hryniewicki, M.K. and Li, Z., 2019, May. LSCP: Locally selective combination in parallel outlier ensembles. In *Proceedings of the 2019 SIAM International Conference on Data Mining (SDM)*, pp. 585-593. Society for Industrial and Applied Mathematics.
+
+.. [#Zhao2021SUOD] Zhao, Y., Hu, X., Cheng, C., Wang, C., Wan, C., Wang, W., Yang, J., Bai, H., Li, Z., Xiao, C., Wang, Y., Qiao, Z., Sun, J. and Akoglu, L. (2021). SUOD: Accelerating Large-scale Unsupervised Heterogeneous Outlier Detection. *Conference on Machine Learning and Systems (MLSys)*.
+
+
```

### Comparing `pyod-1.0.9/pyod.egg-info/SOURCES.txt` & `pyod-1.1.0/pyod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyod-1.0.9/setup.py` & `pyod-1.1.0/setup.py`

 * *Files identical despite different names*

