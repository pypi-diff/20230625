# Comparing `tmp/joserfc-0.1.0.tar.gz` & `tmp/joserfc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.1.0.tar", last modified: Sun Mar  5 08:30:48 2023, max compression
+gzip compressed data, was "joserfc-0.2.0.tar", last modified: Sun Jun 25 09:39:52 2023, max compression
```

## Comparing `joserfc-0.1.0.tar` & `joserfc-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1501 2023-02-05 12:56:49.000000 joserfc-0.1.0/LICENSE
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2062 2023-03-05 08:30:48.179327 joserfc-0.1.0/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)       54 2023-03-05 08:29:32.000000 joserfc-0.1.0/README.md
--rw-r--r--   0 lepture   (1000) lepture   (1000)      915 2023-02-21 13:50:08.000000 joserfc-0.1.0/pyproject.toml
--rw-r--r--   0 lepture   (1000) lepture   (1000)       38 2023-03-05 08:30:48.179327 joserfc-0.1.0/setup.cfg
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.169327 joserfc-0.1.0/src/
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      142 2023-03-05 08:30:18.000000 joserfc-0.1.0/src/joserfc/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2320 2023-02-27 07:16:58.000000 joserfc-0.1.0/src/joserfc/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1809 2023-03-02 08:24:13.000000 joserfc-0.1.0/src/joserfc/jwe.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1906 2023-02-27 05:32:16.000000 joserfc-0.1.0/src/joserfc/jwk.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5608 2023-02-27 05:32:16.000000 joserfc-0.1.0/src/joserfc/jws.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2310 2023-02-23 12:07:56.000000 joserfc-0.1.0/src/joserfc/jwt.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5246 2023-03-02 08:26:26.000000 joserfc-0.1.0/src/joserfc/registry.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7515/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2023-02-16 12:40:56.000000 joserfc-0.1.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2086 2023-02-27 05:38:59.000000 joserfc-0.1.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3937 2023-02-27 05:38:59.000000 joserfc-0.1.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1031 2023-02-21 04:17:27.000000 joserfc-0.1.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1682 2023-03-02 08:26:15.000000 joserfc-0.1.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2381 2023-02-27 05:38:59.000000 joserfc-0.1.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7516/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2023-02-05 13:16:39.000000 joserfc-0.1.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1681 2023-03-02 08:24:13.000000 joserfc-0.1.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3586 2023-03-01 05:38:07.000000 joserfc-0.1.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1946 2023-02-27 13:07:30.000000 joserfc-0.1.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3283 2023-03-02 08:24:13.000000 joserfc-0.1.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1903 2023-03-01 05:38:07.000000 joserfc-0.1.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7517/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      241 2023-02-26 13:20:10.000000 joserfc-0.1.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      835 2023-02-26 13:20:10.000000 joserfc-0.1.0/src/joserfc/rfc7517/keygen.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1631 2023-02-26 13:33:12.000000 joserfc-0.1.0/src/joserfc/rfc7517/keyset.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     8047 2023-02-26 13:38:57.000000 joserfc-0.1.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3789 2023-02-26 07:09:08.000000 joserfc-0.1.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      549 2023-02-26 07:43:19.000000 joserfc-0.1.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7518/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2023-02-05 13:16:45.000000 joserfc-0.1.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4573 2023-02-26 13:09:03.000000 joserfc-0.1.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    13517 2023-03-01 05:38:07.000000 joserfc-0.1.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4728 2023-02-27 08:07:39.000000 joserfc-0.1.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      520 2023-02-19 02:16:48.000000 joserfc-0.1.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6510 2023-02-21 04:17:28.000000 joserfc-0.1.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1777 2023-02-26 12:58:53.000000 joserfc-0.1.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5489 2023-02-26 13:01:50.000000 joserfc-0.1.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      265 2023-02-16 01:39:38.000000 joserfc-0.1.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7519/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2023-02-05 13:16:49.000000 joserfc-0.1.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1320 2023-02-20 01:43:50.000000 joserfc-0.1.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      639 2023-02-23 12:07:56.000000 joserfc-0.1.0/src/joserfc/rfc7519/registry.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5249 2023-02-23 10:47:40.000000 joserfc-0.1.0/src/joserfc/rfc7519/validators.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc7638/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      457 2023-02-26 13:22:52.000000 joserfc-0.1.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc8037/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2023-02-05 13:17:05.000000 joserfc-0.1.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      639 2023-02-16 12:47:23.000000 joserfc-0.1.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5112 2023-02-26 13:10:29.000000 joserfc-0.1.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc/rfc8812/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      422 2023-02-26 13:05:32.000000 joserfc-0.1.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1568 2023-02-20 12:59:46.000000 joserfc-0.1.0/src/joserfc/util.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-03-05 08:30:48.179327 joserfc-0.1.0/src/joserfc.egg-info/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2062 2023-03-05 08:30:48.000000 joserfc-0.1.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1484 2023-03-05 08:30:48.000000 joserfc-0.1.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2023-03-05 08:30:48.000000 joserfc-0.1.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)       13 2023-03-05 08:30:48.000000 joserfc-0.1.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        8 2023-03-05 08:30:48.000000 joserfc-0.1.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.151733 joserfc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 09:39:43.000000 joserfc-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 09:39:52.151733 joserfc-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-25 09:39:43.000000 joserfc-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 09:39:43.000000 joserfc-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:39:52.151733 joserfc-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 09:39:43.000000 joserfc-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/keygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/keyset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/top_level.txt
```

### Comparing `joserfc-0.1.0/LICENSE` & `joserfc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.1.0/src/joserfc/errors.py` & `joserfc-0.2.0/src/joserfc/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,128 @@
 from typing import Optional
 
 
 class JoseError(Exception):
     """Base Exception for all errors in joserfc."""
 
     #: short-string error code
-    error: str = ''
+    error = ""
     #: long-string to describe this error
-    description: str = ''
+    description = ""
 
-    def __init__(self, description: Optional[str]=None, error: Optional[str]=None):
+    def __init__(self, description: Optional[str] = None, error: Optional[str] = None):
         if error is not None:
             self.error = error
         if description is not None:
             self.description = description
 
-        message = '{}: {}'.format(self.error, self.description)
+        message = "{}: {}".format(self.error, self.description)
         super(JoseError, self).__init__(message)
 
     def __repr__(self):
         return '<{} "{}">'.format(self.__class__.__name__, self.error)
 
 
 class DecodeError(JoseError):
-    error: str = 'decode_error'
+    error = "decode_error"
+
+
+class UnsupportedKeyUseError(JoseError):
+    error = "unsupported_key_use"
+
+
+class UnsupportedKeyAlgorithmError(JoseError):
+    error = "unsupported_key_alg"
+
+
+class UnsupportedKeyOperationError(JoseError):
+    error = "unsupported_key_operation"
+
+
+class InvalidKeyLengthError(JoseError):
+    error = "invalid_key_length"
+
+
+class InvalidKeyTypeError(JoseError):
+    error = "invalid_key_type"
+
+
+class InvalidEncryptedKeyError(JoseError):
+    error = "invalid_encrypted_key"
+    description = "JWE Encrypted Key value SHOULD be an empty octet sequence"
 
 
 class MissingAlgorithmError(JoseError):
-    error: str = 'missing_algorithm'
-    description: str = 'Missing "alg" value in header'
+    error = "missing_algorithm"
+    description = 'Missing "alg" value in header'
 
 
 class MissingEncryptionError(JoseError):
-    error: str = 'missing_encryption'
-    description: str = 'Missing "enc" value in header'
+    error = "missing_encryption"
+    description = 'Missing "enc" value in header'
 
 
-class InvalidKeyManagementModeError(JoseError):
-    error: str = 'invalid_key_management_mode'
-    description: str = ''
+class BadSignatureError(JoseError):
+    """This error is designed for JWS/JWT. It is raised when signature
+    does not match.
+    """
+    error = "bad_signature"
 
 
-class BadSignatureError(JoseError):
-    error: str = 'bad_signature'
+class InvalidEncryptionAlgorithmError(JoseError):
+    """This error is designed for JWE. It is raised when "enc" value
+    does not work together with "alg" value.
+    """
+    error = 'invalid_encryption_algorithm'
+
+
+class UnwrapError(JoseError):
+    error = "unwrap_error"
+    description = "Unwrap AES key failed"
+
+
+class InvalidCEKLengthError(JoseError):
+    error = "invalid_cek_length"
+    description = 'Invalid "cek" length'
 
 
 class InvalidClaimError(JoseError):
-    error: str = 'invalid_claim'
+    error = "invalid_claim"
 
     def __init__(self, claim):
         description = f'Invalid claim: "{claim}"'
         super(InvalidClaimError, self).__init__(description=description)
 
 
 class MissingClaimError(JoseError):
-    error: str = 'missing_claim'
+    error = "missing_claim"
 
     def __init__(self, claim):
         description = f'Missing claim: "{claim}"'
         super(MissingClaimError, self).__init__(description=description)
 
 
 class InsecureClaimError(JoseError):
-    error: str = 'insecure_claim'
+    error = "insecure_claim"
 
     def __init__(self, claim):
         description = f'Insecure claim "{claim}"'
         super(InsecureClaimError, self).__init__(description=description)
 
 
 class ExpiredTokenError(JoseError):
-    error: str = 'expired_token'
-    description: str = 'The token is expired'
+    error = "expired_token"
+    description = "The token is expired"
 
 
 class InvalidTokenError(JoseError):
-    error: str = 'invalid_token'
-    description: str = 'The token is not valid yet'
+    error = "invalid_token"
+    description = "The token is not valid yet"
 
 
 class InvalidTypeError(JoseError):
-    error: str = 'invalid_type'
-    description: str = 'The "typ" value in header is invalid'
+    error = "invalid_type"
+    description = 'The "typ" value in header is invalid'
 
 
 class InvalidPayloadError(JoseError):
-    error: str = 'invalid_payload'
+    error = "invalid_payload"
```

### Comparing `joserfc-0.1.0/src/joserfc/jwk.py` & `joserfc-0.2.0/src/joserfc/jwk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random
-from typing import Callable, Union, Any, Protocol
+from typing import Callable, Union, Any, AnyStr, Protocol
 from .rfc7517 import (
     SymmetricKey,
     AsymmetricKey,
+    CurveKey,
     Key,
     KeySet,
     JWK_REGISTRY,
 )
 from .rfc7517.keygen import (
     import_key,
     generate_key,
@@ -17,64 +18,68 @@
 from .rfc7518.ec_key import ECKey
 from .rfc8037.okp_key import OKPKey
 from .rfc8812 import register_secp256k1
 from .registry import Header
 
 
 KeyCallable = Callable[[Any, bool], Key]
-KeyFlexible = Union[Key, KeySet, KeyCallable]
+KeyFlexible = Union[AnyStr, Key, KeySet, KeyCallable]
 
 __all__ = [
-    'types',
-    'JWK_REGISTRY',
-    'SymmetricKey',
-    'AsymmetricKey',
-    'Key',
-    'KeyCallable',
-    'KeyFlexible',
-    'OctKey',
-    'RSAKey',
-    'ECKey',
-    'OKPKey',
-    'KeySet',
-    'generate_key',
-    'import_key',
-    'guess_key',
+    "types",
+    "JWK_REGISTRY",
+    "SymmetricKey",
+    "AsymmetricKey",
+    "CurveKey",
+    "Key",
+    "KeyCallable",
+    "KeyFlexible",
+    "OctKey",
+    "RSAKey",
+    "ECKey",
+    "OKPKey",
+    "KeySet",
+    "generate_key",
+    "import_key",
+    "guess_key",
 ]
 
 # register thumbprint method
 register_secp256k1()
 
 # register all key types
 JWK_REGISTRY[OctKey.key_type] = OctKey
 JWK_REGISTRY[RSAKey.key_type] = RSAKey
 JWK_REGISTRY[ECKey.key_type] = ECKey
 JWK_REGISTRY[OKPKey.key_type] = OKPKey
 
 
-class GuestProtocol(Protocol):
+class GuestProtocol(Protocol):  # pragma: no cover
     def headers(self) -> Header:
         ...
 
     def set_kid(self, kid: str):
         ...
 
 
 def guess_key(key: KeyFlexible, obj: GuestProtocol) -> Key:
     """Guess key from a various sources.
 
     :param key: a very flexible key
     :param obj: a protocol that has ``headers`` and ``set_kid`` methods
     """
-    if isinstance(key, (SymmetricKey, AsymmetricKey)):
+    if isinstance(key, (str, bytes)):
+        return OctKey.import_key(key)
+
+    elif isinstance(key, (SymmetricKey, AsymmetricKey)):
         return key
 
     elif isinstance(key, KeySet):
         headers = obj.headers()
-        kid = headers.get('kid')
+        kid = headers.get("kid")
 
         if not kid:
             # choose one key by random
             key: Key = random.choice(key.keys)
             # use side effect to add kid information
             obj.set_kid(key.kid)
             return key
```

### Comparing `joserfc-0.1.0/src/joserfc/jws.py` & `joserfc-0.2.0/src/joserfc/jws.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import Optional, AnyStr, List, Union
 from .rfc7515 import types
-from .rfc7515.model import JWSAlgModel
+from .rfc7515.model import (
+    JWSAlgModel,
+    HeaderMember,
+    CompactSignature,
+    JSONSignature,
+)
 from .rfc7515.registry import (
     JWSRegistry,
     default_registry,
 )
 from .rfc7515.compact import (
     sign_compact,
     extract_compact,
@@ -12,181 +17,236 @@
 )
 from .rfc7515.json import (
     sign_json,
     verify_json,
     extract_json,
 )
 from .rfc7515.types import (
-    Header,
-    HeaderMember,
     HeaderDict,
-    SignatureData,
     JSONSerialization,
 )
 from .rfc7518.jws_algs import JWS_ALGORITHMS
 from .rfc8037.jws_eddsa import EdDSA
 from .rfc8812 import ES256K
 from .errors import BadSignatureError
 from .jwk import Key, KeyFlexible, guess_key
 from .util import to_bytes, urlsafe_b64encode
+from .registry import Header
 
 __all__ = [
-    'types',
-    'JWSAlgModel',
-    'JWSRegistry',
-    'SignatureData',
-
-    'serialize_compact',
-    'deserialize_compact',
-    'extract_compact',
-    'validate_compact',
-
-    'serialize_json',
-    'deserialize_json',
-    'extract_json',
-    'validate_json',
+    "types",
+    "JWSAlgModel",
+    "JWSRegistry",
+    "CompactSignature",
+    "JSONSignature",
+    "serialize_compact",
+    "deserialize_compact",
+    "extract_compact",
+    "validate_compact",
+    "serialize_json",
+    "deserialize_json",
+    "extract_json",
+    "validate_json",
+    "default_registry",
 ]
 
+
 # register supported alg models
 def __register():
     # register alg in RFC7518
     for _alg in JWS_ALGORITHMS:
         JWSRegistry.register(_alg)
     # register alg in RFC8037
     JWSRegistry.register(EdDSA)
     # register alg in RFC8812
     JWSRegistry.register(ES256K)
 
+
 __register()
 
 
 def serialize_compact(
         header: Header,
         payload: bytes,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None) -> bytes:
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None) -> bytes:
     """Generate a JWS Compact Serialization. The JWS Compact Serialization
     represents digitally signed or MACed content as a compact, URL-safe
     string, per Section 7.1.
 
     .. code-block:: text
 
         BASE64URL(UTF8(JWS Protected Header)) || '.' ||
         BASE64URL(JWS Payload) || '.' ||
         BASE64URL(JWS Signature)
 
     :param header: protected header part of the JWS, in dict
     :param payload: payload data of the JWS, in bytes
     :param key: a flexible private key to sign the signature
+    :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :return: JWS in bytes
 
     .. note:: The returned value is in bytes
     """
-    if registry is None:
+    if algorithms:
+        registry = JWSRegistry(algorithms=algorithms)
+    elif registry is None:
         registry = default_registry
 
     registry.check_header(header)
-    member = HeaderMember(header)
-    obj = SignatureData([member], payload)
-    obj.compact = True
-    alg: JWSAlgModel = registry.get_alg(header['alg'])
-    key: Key = guess_key(key, member)
+    obj = CompactSignature(header, payload)
+    alg: JWSAlgModel = registry.get_alg(header["alg"])
+    key: Key = guess_key(key, obj)
     return sign_compact(obj, alg, key)
 
 
 def validate_compact(
-        obj: SignatureData,
+        obj: CompactSignature,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None):
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None):
     """Validate the JWS Compact Serialization with the given key.
     This method is usually used together with ``extract_compact``.
 
     :param obj: object of the JWS Compact Serialization
     :param key: a flexible public key to verify the signature
+    :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :raise: ValueError or BadSignatureError
     """
-    if registry is None:
+    if algorithms:
+        registry = JWSRegistry(algorithms=algorithms)
+    elif registry is None:
         registry = default_registry
-    member = obj.members[0]
-    alg: JWSAlgModel = registry.get_alg(member.protected['alg'])
-    key: Key = guess_key(key, member)
+
+    headers = obj.headers()
+    alg: JWSAlgModel = registry.get_alg(headers["alg"])
+    key: Key = guess_key(key, obj)
     if not verify_compact(obj, alg, key):
         raise BadSignatureError()
 
 
 def deserialize_compact(
         value: AnyStr,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None) -> SignatureData:
-    """Extract and validate the JWS (in string) with the given key.
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None) -> CompactSignature:
+    """Extract and validate the JWS Compact Serialization (in string, or bytes)
+    with the given key. An JWE Compact Serialization looks like:
 
-    :param value: a string (or bytes) of the JWS
+    .. code-block:: text
+        :caption: line breaks for display purposes only
+
+        eyJ0eXAiOiJKV1QiLA0KICJhbGciOiJIUzI1NiJ9
+        .
+        eyJpc3MiOiJqb2UiLA0KICJleHAiOjEzMDA4MTkzODAsDQogImh0dHA6Ly9leGFt
+        cGxlLmNvbS9pc19yb290Ijp0cnVlfQ
+        .
+        dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk
+
+    :param value: a string (or bytes) of the JWS Compact Serialization
     :param key: a flexible public key to verify the signature
+    :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
-    :return: object of the JWS Compact Serialization
+    :return: object of the ``CompactSignature``
     """
     obj = extract_compact(to_bytes(value))
-    validate_compact(obj, key, registry)
+    validate_compact(obj, key, algorithms, registry)
     return obj
 
 
 def serialize_json(
         members: Union[HeaderDict, List[HeaderDict]],
         payload: bytes,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None) -> JSONSerialization:
-    if registry is None:
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None) -> JSONSerialization:
+    """Generate a JWS JSON Serialization (in dict). The JWS JSON Serialization
+    represents digitally signed or MACed content as a JSON object. This representation
+    is neither optimized for compactness nor URL-safe.
+
+    A general JWS JSON Serialization contains:
+
+    payload
+        The "payload" member MUST be present and contain the value
+        BASE64URL(JWS Payload).
+
+    signatures
+        The "signatures" member value MUST be an array of JSON objects.
+        Each object represents a signature or MAC over the JWS Payload and
+        the JWS Protected Header.
+
+    A flatten JWS JSON Serialization looks like:
+
+    .. code-block:: text
+
+        {
+            "payload":"<payload contents>",
+            "protected":"<integrity-protected header contents>",
+            "header":<non-integrity-protected header contents>,
+            "signature":"<signature contents>"
+        }
+    """
+    if algorithms:
+        registry = JWSRegistry(algorithms=algorithms)
+    elif registry is None:
         registry = default_registry
 
     if isinstance(members, dict):
         flatten = True
-        registry.check_header(members['protected'])
+        registry.check_header(members["protected"])
         members = [members]
     else:
         flatten = False
         for member in members:
-            registry.check_header(member['protected'])
+            registry.check_header(member["protected"])
 
     members = [HeaderMember(**member) for member in members]
-    obj = SignatureData(members, payload)
-    obj.segments['payload'] = urlsafe_b64encode(payload)
+    obj = JSONSignature(members, payload)
+    obj.segments["payload"] = urlsafe_b64encode(payload)
     obj.flatten = flatten
 
     find_key = lambda d: guess_key(key, d)
     return sign_json(obj, registry.get_alg, find_key)
 
 
 def validate_json(
-        obj: SignatureData,
+        obj: JSONSignature,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None):
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None):
     """Validate the JWS JSON Serialization with the given key.
     This method is usually used together with ``extract_json``.
 
     :param obj: object of the JWS JSON Serialization
     :param key: a flexible public key to verify the signature
+    :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :raise: ValueError or BadSignatureError
     """
-    if registry is None:
+    if algorithms:
+        registry = JWSRegistry(algorithms=algorithms)
+    elif registry is None:
         registry = default_registry
     find_key = lambda d: guess_key(key, d)
     if not verify_json(obj, registry.get_alg, find_key):
         raise BadSignatureError()
 
 
 def deserialize_json(
         value: JSONSerialization,
         key: KeyFlexible,
-        registry: Optional[JWSRegistry]=None) -> SignatureData:
+        algorithms: Optional[List[str]] = None,
+        registry: Optional[JWSRegistry] = None) -> JSONSignature:
     """Extract and validate the JWS (in string) with the given key.
 
     :param value: a dict of the JSON signature
     :param key: a flexible public key to verify the signature
+    :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :return: object of the SignatureData
     """
     obj = extract_json(value)
-    validate_json(obj, key, registry)
+    validate_json(obj, key, algorithms, registry)
     return obj
```

### Comparing `joserfc-0.1.0/src/joserfc/jwt.py` & `joserfc-0.2.0/src/joserfc/jwt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,124 @@
-from typing import Optional, AnyStr
-from .rfc7515.compact import extract_compact
-from .rfc7519.claims import Claims, convert_claims
-from .rfc7519.validators import ClaimsOption, JWTClaimsRequests
-from .rfc7519.registry import JWTRegistry, default_registry
-from .jws import serialize_compact, validate_compact
+import typing as t
+from .rfc7519.claims import Claims, convert_claims, check_sensitive_data
+from .rfc7519.registry import ClaimsOption, JWTClaimsRegistry
+from .jws import (
+    JWSRegistry,
+    CompactSignature,
+    serialize_compact,
+    validate_compact as validate_jws,
+    extract_compact as extract_jws,
+)
+from .jwe import (
+    JWERegistry,
+    CompactEncryption,
+    encrypt_compact,
+    validate_compact as validate_jwe,
+    extract_compact as extract_jwe,
+)
 from .jwk import KeyFlexible
 from .errors import InvalidTypeError, InvalidPayloadError
 from .util import to_bytes
 from .registry import Header
 
-
 __all__ = [
-    'Header',
-    'Claims',
-    'Token',
-    'ClaimsOption',
-    'JWTRegistry',
-    'JWTClaimsRequests',
-    'encode',
-    'decode',
+    "Header",
+    "Claims",
+    "Token",
+    "ClaimsOption",
+    "JWTClaimsRegistry",
+    "encode",
+    "decode",
+    "check_sensitive_data",
 ]
 
+JWTRegistry = t.Union[JWSRegistry, JWERegistry]
+
 
 class Token:
+    """The extracted token object, which contains ``header`` and ``claims``.
+
+    :param header: the header part of the JWT
+    :param claims: the payload part of the JWT
+    """
     def __init__(self, header: Header, claims: Claims):
         self.header = header
         self.claims = claims
 
+    def __repr__(self):
+        return str(self.claims)
+
 
 def encode(
         header: Header,
         claims: Claims,
         key: KeyFlexible,
-        registry: Optional[JWTRegistry]=None) -> str:
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWTRegistry] = None) -> str:
     """Encode a JSON Web Token with the given header, and claims.
 
     :param header: A dict of the JWT header
     :param claims: A dict of the JWT claims to be encoded
     :param key: key used to sign the signature
-    :param registry: a JWTRegistry to use
+    :param algorithms: a list of allowed algorithms
+    :param registry: a ``JWSRegistry`` or ``JWERegistry`` to use
     """
     # add ``typ`` in header
-    header['typ'] = 'JWT'
+    header["typ"] = "JWT"
     payload = convert_claims(claims)
-    if registry is None:
-        registry = default_registry
-    result = serialize_compact(header, payload, key, registry)
-    return result.decode('utf-8')
+    if "enc" in header:
+        result = encrypt_compact(header, payload, key, algorithms, registry)
+    else:
+        result = serialize_compact(header, payload, key, algorithms, registry)
+    return result.decode("utf-8")
+
+
+def extract(value: t.AnyStr) -> Token:
+    """Extract the JSON Web Token string, without validating with the key,
+    without validating the header and claims."""
+    obj = _extract_segment(value)
+    return Token(obj.headers(), obj.claims)
 
 
 def decode(
-        value: AnyStr,
+        value: t.AnyStr,
         key: KeyFlexible,
-        registry: Optional[JWTRegistry]=None) -> Token:
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWTRegistry] = None) -> Token:
     """Decode the JSON Web Token string with the given key, and validate
     it with the claims requests. This method is a combination of the
     :function:`extract` and :function:`validate`.
 
     :param value: text of the JWT
     :param key: key used to verify the signature
-    :param registry: a JWTRegistry to use
+    :param algorithms: a list of allowed algorithms
+    :param registry: a ``JWSRegistry`` or ``JWERegistry`` to use
     :raise: BadSignatureError
     """
-    obj = extract_compact(to_bytes(value))
-    try:
-        token = Token(obj.headers(), obj.claims)
-    except ValueError:
-        raise InvalidPayloadError('Payload should be a JSON dict')
-    if registry is None:
-        registry = default_registry
+    obj = _extract_segment(value)
 
-    typ = token.header.get('typ')
-    if typ and typ != 'JWT':
+    token = Token(obj.headers(), obj.claims)
+    typ = token.header.get("typ")
+    # https://www.rfc-editor.org/rfc/rfc7519#section-5.1
+    # If present, it is RECOMMENDED that its value be "JWT".
+    if typ and typ != "JWT":
         raise InvalidTypeError()
 
-    registry.check_claims(token.claims)
-    validate_compact(obj, key, registry)
+    if isinstance(obj, CompactSignature):
+        validate_jws(obj, key, algorithms=algorithms, registry=registry)
+    else:
+        validate_jwe(obj, key, algorithms=algorithms, registry=registry)
     return token
+
+
+def _extract_segment(value: t.AnyStr) -> t.Union[CompactSignature, CompactEncryption]:
+    segment = to_bytes(value)
+    if segment.count(b".") == 4:
+        obj = extract_jwe(segment)
+    else:
+        obj = extract_jws(segment)
+
+    try:
+        assert isinstance(obj.claims, dict)
+    except (ValueError, TypeError):
+        raise InvalidPayloadError("Payload should be a JSON dict")
+    return obj
```

### Comparing `joserfc-0.1.0/src/joserfc/registry.py` & `joserfc-0.2.0/src/joserfc/registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,167 @@
 import typing as t
 from collections import namedtuple
 
 Header = t.Dict[str, t.Any]
 
-#: Define header parameters for JWS and JWE
-HeaderParameter = namedtuple('HeaderParameter', ['description', 'required', 'check_value'])
-HeaderRegistryDict = t.Dict[str, HeaderParameter]
-
-#: Define parameters for JWK
-KeyParameter = namedtuple('KeyParameter', ['description', 'required', 'private', 'check_value'])
-KeyParameterRegistryDict = t.Dict[str, KeyParameter]
-
-KeyOperation = namedtuple('KeyOperation', ['description', 'use', 'private'])
-KeyOperationRegistryDict = t.Dict[str, KeyOperation]
-
 
 def is_str(value: str):
     if not isinstance(value, str):
-        raise ValueError('must be a str')
+        raise ValueError("must be a str")
 
 
 def is_url(value: str):
     is_str(value)
-    if not value.startswith(('http://', 'https://')):
-        raise ValueError('must be a URL')
+    if not value.startswith(("http://", "https://")):
+        raise ValueError("must be a URL")
+
 
 def is_int(value: int):
     if not isinstance(value, int):
-        raise ValueError('must be an int')
+        raise ValueError("must be an int")
+
+
+def is_bool(value: bool):
+    if not isinstance(value, bool):
+        raise ValueError("must be an bool")
 
 
 def is_list_str(values):
     if not isinstance(values, list):
-        raise ValueError('must be a list[str]')
+        raise ValueError("must be a list[str]")
 
     for value in values:
         if not isinstance(value, str):
-            raise ValueError('must be a list[str]')
+            raise ValueError("must be a list[str]")
 
 
 def is_jwk(value):
     if not isinstance(value, dict):
-        raise ValueError('must be a JWK')
+        raise ValueError("must be a JWK")
 
 
 def in_choices(choices: t.List[str]):
     def _is_one_of(value):
         if isinstance(value, list):
             for v in value:
                 if v not in choices:
-                    raise ValueError(f'must be one of {choices}')
+                    raise ValueError(f"must be one of {choices}")
 
         elif value not in choices:
-            raise ValueError(f'must be one of {choices}')
+            raise ValueError(f"must be one of {choices}")
+
     return _is_one_of
 
 
 def not_support(_):
-    raise ValueError('is not supported')
+    raise ValueError("is not supported")
 
 
+Validate = t.Callable[[t.Any], t.NoReturn]
+_value_validators = {
+    "str": is_str,
+    "list[str]": is_list_str,
+    "int": is_int,
+    "bool": is_bool,
+    "url": is_url,
+    "jwk": is_jwk,
+    "none": not_support,
+}
+
+class HeaderParameter:
+    def __init__(self, description: str, validate: t.Union[str, Validate], required: bool=False):
+        self.description: str = description
+        if isinstance(validate, str):
+            self.validate: Validate = _value_validators[validate]
+        else:
+            self.validate: Validate = validate
+        self.required = required
+
+#: Define header parameters for JWS and JWE
+HeaderRegistryDict = t.Dict[str, HeaderParameter]
+
+
+class KeyParameter:
+    def __init__(
+            self,
+             description: str,
+             validate: t.Union[str, Validate],
+             private: t.Optional[bool]=None,
+             required: bool=False):
+        self.description: str = description
+        if isinstance(validate, str):
+            self.validate: Validate = _value_validators[validate]
+        else:
+            self.validate: Validate = validate
+        self.private = private
+        self.required = required
+
+#: Define parameters for JWK
+KeyParameterRegistryDict = t.Dict[str, KeyParameter]
+KeyOperation = namedtuple("KeyOperation", ["description", "use", "private"])
+KeyOperationRegistryDict = t.Dict[str, KeyOperation]
+
 #: Basic JWS header registry
 JWS_HEADER_REGISTRY: HeaderRegistryDict = {
-    'alg': HeaderParameter('Algorithm', True, is_str),
-    'jku': HeaderParameter('JWK Set URL', False, is_url),
-    'jwk': HeaderParameter('JSON Web Key', False, is_jwk),
-    'kid': HeaderParameter('Key ID', False, is_str),
-    'x5u': HeaderParameter('X.509 URL', False, is_url),
-    'x5c': HeaderParameter('X.509 Certificate Chain', False, is_list_str),
-    'x5t': HeaderParameter('X.509 Certificate SHA-1 Thumbprint', False, is_str),
-    'x5t#S256': HeaderParameter('X.509 Certificate SHA-256 Thumbprint', False, is_str),
-    'typ': HeaderParameter('Type', False, is_str),
-    'cty': HeaderParameter('Content Type', False, is_str),
-    'crit': HeaderParameter('Critical', False, is_list_str),
+    "alg": HeaderParameter("Algorithm", is_str, True),
+    "jku": HeaderParameter("JWK Set URL", is_url),
+    "jwk": HeaderParameter("JSON Web Key",  is_jwk),
+    "kid": HeaderParameter("Key ID", is_str),
+    "x5u": HeaderParameter("X.509 URL", is_url),
+    "x5c": HeaderParameter("X.509 Certificate Chain", is_list_str),
+    "x5t": HeaderParameter("X.509 Certificate SHA-1 Thumbprint", is_str),
+    "x5t#S256": HeaderParameter("X.509 Certificate SHA-256 Thumbprint", is_str),
+    "typ": HeaderParameter("Type", is_str),
+    "cty": HeaderParameter("Content Type", is_str),
+    "crit": HeaderParameter("Critical", is_list_str),
 }
 
 #: Basic JWE header registry
 JWE_HEADER_REGISTRY = {
-    'enc': HeaderParameter('Encryption Algorithm', True, is_str),
-    'zip': HeaderParameter('Compression Algorithm', False, is_str),
-    **JWS_HEADER_REGISTRY
+    "enc": HeaderParameter("Encryption Algorithm", is_str, True),
+    "zip": HeaderParameter("Compression Algorithm", is_str),
+    **JWS_HEADER_REGISTRY,
 }
 
 #: Basic JWK parameter registry
 JWK_PARAMETER_REGISTRY = {
-    'kty': KeyParameter('Key ID', True, None, is_str),  # This member MUST be present in a JWK.
-    'use': KeyParameter('Public Key Use', False, None, in_choices(['sig', 'enc'])),
-    'key_ops': KeyParameter(
-        'Key Operations',
-        False, None,
+    "kty": KeyParameter("Key ID", is_str, required=True),  # This member MUST be present in a JWK.
+    "use": KeyParameter("Public Key Use", in_choices(["sig", "enc"])),
+    "key_ops": KeyParameter(
+        "Key Operations",
         in_choices([
-            'sign', 'verify',
-            'encrypt', 'decrypt',
-            'wrapKey', 'unwrapKey',
-            'deriveKey', 'deriveBits'
-        ])
+            "sign",
+            "verify",
+            "encrypt",
+            "decrypt",
+            "wrapKey",
+            "unwrapKey",
+            "deriveKey",
+            "deriveBits",
+        ]),
     ),
-    'alg': KeyParameter('Algorithm', False, None, is_str),
-    'kid': KeyParameter('Key ID', False, None, is_str),
-    'x5u': KeyParameter('X.509 URL', False, None, is_url),
-    'x5c': KeyParameter('X.509 Certificate Chain',  False, None, is_list_str),
-    'x5t': KeyParameter('X.509 Certificate SHA-1 Thumbprint',  False, None, is_str),
-    'x5t#S256': KeyParameter('X.509 Certificate SHA-256 Thumbprint',  False, None, is_str),
+    "alg": KeyParameter("Algorithm", is_str),
+    "kid": KeyParameter("Key ID", is_str),
+    "x5u": KeyParameter("X.509 URL", is_url),
+    "x5c": KeyParameter("X.509 Certificate Chain", is_list_str),
+    "x5t": KeyParameter("X.509 Certificate SHA-1 Thumbprint", is_str),
+    "x5t#S256": KeyParameter("X.509 Certificate SHA-256 Thumbprint", is_str),
 }
 
 #: Common JWK operations
 #: https://www.rfc-editor.org/rfc/rfc7517#section-4.3
 JWK_OPERATION_REGISTRY = {
-    'sign': KeyOperation('compute digital signature or MAC', 'sig', True),
-    'verify': KeyOperation('verify digital signature or MAC', 'sig', False),
-    'encrypt': KeyOperation('encrypt content', 'enc', False),
-    'decrypt': KeyOperation('decrypt content and validate decryption, if applicable', 'enc', True),
-    'wrapKey': KeyOperation('encrypt key', 'enc', False),
-    'unwrapKey': KeyOperation('decrypt key and validate decryption, if applicable', 'enc', True),
-    'deriveKey': KeyOperation('derive key', 'enc', False),
-    'deriveBits': KeyOperation('derive bits not to be used as a key', 'enc', None),
+    "sign": KeyOperation("compute digital signature or MAC", "sig", True),
+    "verify": KeyOperation("verify digital signature or MAC", "sig", False),
+    "encrypt": KeyOperation("encrypt content", "enc", False),
+    "decrypt": KeyOperation("decrypt content and validate decryption, if applicable", "enc", True),
+    "wrapKey": KeyOperation("encrypt key", "enc", False),
+    "unwrapKey": KeyOperation("decrypt key and validate decryption, if applicable", "enc", True),
+    "deriveKey": KeyOperation("derive key", "enc", False),
+    "deriveBits": KeyOperation("derive bits not to be used as a key", "enc", None),
 }
 
 
 def check_supported_header(registry: HeaderRegistryDict, header: Header):
     allowed_keys = set(registry.keys())
     unsupported_keys = set(header.keys()) - allowed_keys
     if unsupported_keys:
@@ -128,18 +171,18 @@
 def check_registry_header(registry: HeaderRegistryDict, header: Header):
     for key in registry:
         reg: HeaderParameter = registry[key]
         if reg.required and key not in header:
             raise ValueError(f'Required "{key}" is missing in header')
         if key in header:
             try:
-                reg.check_value(header[key])
+                reg.validate(header[key])
             except ValueError as error:
                 raise ValueError(f'"{key}" in header {error}')
 
 
 def check_crit_header(header: Header):
     # check crit header
-    if 'crit' in header:
-        for k in header['crit']:
+    if "crit" in header:
+        for k in header["crit"]:
             if k not in header:
                 raise ValueError(f'"{k}" is a critical header')
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.2.0/src/joserfc/rfc7515/compact.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,57 @@
 import binascii
-from .model import JWSAlgModel
-from .types import HeaderMember, SignatureData
+from .model import JWSAlgModel, CompactSignature
 from ..errors import DecodeError, MissingAlgorithmError
 from ..util import (
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 
 
-def sign_compact(obj: SignatureData, alg: JWSAlgModel, key) -> bytes:
-    key.check_use('sig')
-    member = obj.members[0]
-    if 'header' not in obj.segments:
-        obj.segments['header'] = json_b64encode(member.protected)
-    if 'payload' not in obj.segments:
-        obj.segments['payload'] = urlsafe_b64encode(obj.payload)
-    signing_input = obj.segments['header'] + b'.' +  obj.segments['payload']
+def sign_compact(obj: CompactSignature, alg: JWSAlgModel, key) -> bytes:
+    key.check_use("sig")
+    header_segment = json_b64encode(obj.headers())
+    payload_segment = urlsafe_b64encode(obj.payload)
+    signing_input = header_segment + b"." + payload_segment
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
-    obj.segments['signature'] = signature
-    return signing_input + b'.' + signature
+    return signing_input + b"." + signature
 
 
-def extract_compact(value: bytes) -> SignatureData:
+def extract_compact(value: bytes) -> CompactSignature:
     """Extract the JWS Compact Serialization from bytes to object.
 
     :param value: JWS in bytes
     :raise: DecodeError
     """
-    parts = value.split(b'.')
+    parts = value.split(b".")
     if len(parts) != 3:
-        raise ValueError('Invalid JSON Web Signature')
+        raise ValueError("Invalid JSON Web Signature")
 
     header_segment, payload_segment, signature_segment = parts
     try:
         protected = json_b64decode(header_segment)
-        if 'alg' not in protected:
+        if "alg" not in protected:
             raise MissingAlgorithmError()
     except (TypeError, ValueError, binascii.Error):
-        raise DecodeError('Invalid header')
+        raise DecodeError("Invalid header")
 
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
-        raise DecodeError('Invalid payload')
+        raise DecodeError("Invalid payload")
 
-    obj = SignatureData([HeaderMember(protected)], payload)
-    obj.compact = True
+    obj = CompactSignature(protected, payload)
     obj.segments.update({
-        'header': header_segment,
-        'payload': payload_segment,
-        'signature': signature_segment,
+        "header": header_segment,
+        "payload": payload_segment,
+        "signature": signature_segment,
     })
     return obj
 
 
-def verify_compact(obj: SignatureData, alg: JWSAlgModel, key) -> bool:
-    key.check_use('sig')
-    signing_input = obj.segments['header'] + b'.' + obj.segments['payload']
-    sig = urlsafe_b64decode(obj.segments['signature'])
+def verify_compact(obj: CompactSignature, alg: JWSAlgModel, key) -> bool:
+    key.check_use("sig")
+    signing_input = obj.segments["header"] + b"." + obj.segments["payload"]
+    sig = urlsafe_b64decode(obj.segments["signature"])
     return alg.verify(signing_input, sig, key)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7515/json.py` & `joserfc-0.2.0/src/joserfc/rfc7515/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import typing as t
 import binascii
-from .model import JWSAlgModel
+from .model import JWSAlgModel, HeaderMember, JSONSignature
 from .types import (
-    HeaderMember,
-    SignatureData,
     JSONSignatureDict,
     JSONSerialization,
     CompleteJSONSerialization,
     FlattenJSONSerialization,
 )
 from ..util import (
     json_b64encode,
@@ -16,108 +14,108 @@
     urlsafe_b64decode,
 )
 from ..errors import DecodeError
 
 FindAlgorithm = t.Callable[[str], JWSAlgModel]
 
 
-def sign_json(obj: SignatureData, find_alg: FindAlgorithm, find_key) -> JSONSerialization:
+def sign_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> JSONSerialization:
     signatures: t.List[JSONSignatureDict] = []
 
-    payload_segment = obj.segments['payload']
+    payload_segment = obj.segments["payload"]
     for member in obj.members:
-        alg = find_alg(member.protected['alg'])
+        alg = find_alg(member.protected["alg"])
         key = find_key(member)
-        key.check_use('sig')
+        key.check_use("sig")
         signature = _sign_member(payload_segment, member, alg, key)
         signatures.append(signature)
 
-    rv = {'payload': payload_segment.decode('utf-8')}
+    rv = {"payload": payload_segment.decode("utf-8")}
     if obj.flatten and len(signatures) == 1:
         rv.update(dict(signatures[0]))
     else:
-        rv['signatures'] = signatures
+        rv["signatures"] = signatures
 
     obj.signatures = signatures
     return rv
 
 
 def _sign_member(payload_segment, member: HeaderMember, alg: JWSAlgModel, key) -> JSONSignatureDict:
     protected_segment = json_b64encode(member.protected)
-    signing_input = b'.'.join([protected_segment, payload_segment])
+    signing_input = b".".join([protected_segment, payload_segment])
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
     rv = {
-        'protected': protected_segment.decode('utf-8'),
-        'signature': signature.decode('utf-8'),
+        "protected": protected_segment.decode("utf-8"),
+        "signature": signature.decode("utf-8"),
     }
     if member.header:
-        rv['header'] = member.header
+        rv["header"] = member.header
     return rv
 
 
-def extract_json(value: JSONSerialization) -> SignatureData:
+def extract_json(value: JSONSerialization) -> JSONSignature:
     """Extract the JWS JSON Serialization from dict to object.
 
     :param value: JWS in dict
     """
-    payload_segment: bytes = value['payload'].encode('utf-8')
+    payload_segment: bytes = value["payload"].encode("utf-8")
 
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
-        raise DecodeError('Invalid payload')
+        raise DecodeError("Invalid payload")
 
-    if 'signatures' in value:
+    if "signatures" in value:
         flatten = False
         value: CompleteJSONSerialization
-        signatures: t.List[JSONSignatureDict] = value['signatures']
+        signatures: t.List[JSONSignatureDict] = value["signatures"]
     else:
         flatten = True
         value: FlattenJSONSerialization
         _sig: JSONSignatureDict = {
-            'protected': value['protected'],
-            'signature': value['signature'],
+            "protected": value["protected"],
+            "signature": value["signature"],
         }
-        if 'header' in value:
-            _sig['header'] = value['header']
+        if "header" in value:
+            _sig["header"] = value["header"]
         signatures = [_sig]
 
     members = []
     for sig in signatures:
-        protected_segment = sig['protected']
+        protected_segment = sig["protected"]
         protected = json_b64decode(protected_segment)
         member = HeaderMember(protected)
-        if 'header' in sig:
-            member.header = sig['header']
+        if "header" in sig:
+            member.header = sig["header"]
         members.append(member)
 
-    obj = SignatureData(members, payload)
-    obj.segments.update({'payload': payload_segment})
+    obj = JSONSignature(members, payload)
+    obj.segments.update({"payload": payload_segment})
     obj.flatten = flatten
     obj.signatures = signatures
     return obj
 
 
-def verify_json(obj: SignatureData, find_alg: FindAlgorithm, find_key) -> bool:
+def verify_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> bool:
     """Verify the signature of this JSON serialization with the given
     algorithm and key.
 
     :param obj: instance of the SignatureData
     :param find_alg: a function to return "alg" model
     :param find_key: a function to return public key
     """
-    payload_segment = obj.segments['payload']
+    payload_segment = obj.segments["payload"]
     for index, signature in enumerate(obj.signatures):
         member = obj.members[index]
-        alg = find_alg(member.protected['alg'])
+        alg = find_alg(member.protected["alg"])
         key = find_key(member)
-        key.check_use('sig')
+        key.check_use("sig")
         if not _verify_signature(signature, payload_segment, alg, key):
             return False
     return True
 
 
 def _verify_signature(signature: JSONSignatureDict, payload_segment, alg: JWSAlgModel, key) -> bool:
-    protected_segment = signature['protected'].encode('utf-8')
-    sig = urlsafe_b64decode(signature['signature'].encode('utf-8'))
-    signing_input = b'.'.join([protected_segment, payload_segment])
+    protected_segment = signature["protected"].encode("utf-8")
+    sig = urlsafe_b64decode(signature["signature"].encode("utf-8"))
+    signing_input = b".".join([protected_segment, payload_segment])
     return alg.verify(signing_input, sig, key)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.2.0/src/joserfc/rfc7516/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,91 +7,87 @@
     check_supported_header,
     check_registry_header,
     check_crit_header,
 )
 
 JWEAlgorithm = t.Union[JWEAlgModel, JWEEncModel, JWEZipModel]
 
-AlgorithmsDict = t.TypedDict('AlgorithmsDict', {
-    'alg': t.Dict[str, JWEAlgModel],
-    'enc': t.Dict[str, JWEEncModel],
-    'zip': t.Dict[str, JWEZipModel],
+AlgorithmsDict = t.TypedDict("AlgorithmsDict", {
+    "alg": t.Dict[str, JWEAlgModel],
+    "enc": t.Dict[str, JWEEncModel],
+    "zip": t.Dict[str, JWEZipModel],
 })
-AlgorithmNamesDict = t.TypedDict('AlgorithmNamesDict', {
-    'alg': t.List[str],
-    'enc': t.List[str],
-    'zip': t.List[str],
+AlgorithmNamesDict = t.TypedDict("AlgorithmNamesDict", {
+    "alg": t.List[str],
+    "enc": t.List[str],
+    "zip": t.List[str],
 }, total=False)
 
 
 class JWERegistry:
     algorithms: AlgorithmsDict = {
-        'alg': {},
-        'enc': {},
-        'zip': {},
-    }
-    recommended: AlgorithmNamesDict = {
-        'alg': [],
-        'enc': [],
-        'zip': [],
+        "alg": {},
+        "enc": {},
+        "zip": {},
     }
+    recommended: t.List[str] = []
 
     def __init__(
             self,
-            headers: t.Optional[HeaderRegistryDict]=None,
-            algorithms: t.Optional[AlgorithmNamesDict]=None,
-            strict_check_header: bool=True):
+            headers: t.Optional[HeaderRegistryDict] = None,
+            algorithms: t.Optional[t.List[str]] = None,
+            strict_check_header: bool = True):
         self.header_registry: HeaderRegistryDict = {}
         self.header_registry.update(JWE_HEADER_REGISTRY)
         if headers is not None:
             self.header_registry.update(headers)
         self.allowed = algorithms
         self.strict_check_header = strict_check_header
 
     @classmethod
     def register(cls, model: JWEAlgorithm):
-        location = model.algorithm_location
-        cls.algorithms[location][model.name] = model  # type: ignore
+        location: t.Literal["alg", "enc", "zip"] = model.algorithm_location
+        cls.algorithms[location][model.name] = model
         if model.recommended:
-            cls.recommended[location].append(model.name) # type: ignore
+            cls.recommended.append(model.name)
 
     def check_header(self, header: Header, check_more=False):
         check_crit_header(header)
         check_registry_header(self.header_registry, header)
         if check_more:
-            alg = self.get_alg(header['alg'])
+            alg = self.get_alg(header["alg"])
             if alg.more_header_registry:
                 check_registry_header(alg.more_header_registry, header)
             if self.strict_check_header:
                 allowed_registry = self.header_registry.copy()
                 allowed_registry.update(alg.more_header_registry)
                 check_supported_header(allowed_registry, header)
         elif self.strict_check_header:
             check_supported_header(self.header_registry, header)
 
     def get_alg(self, name: str) -> JWEAlgModel:
-        return self._get_algorithm('alg', name)
+        return self._get_algorithm("alg", name)
 
     def get_enc(self, name: str) -> JWEEncModel:
-        return self._get_algorithm('enc', name)
+        return self._get_algorithm("enc", name)
 
     def get_zip(self, name: str) -> JWEZipModel:
-        return self._get_algorithm('zip', name)
+        return self._get_algorithm("zip", name)
 
     def _get_algorithm(self, location: str, name: str):
         if location not in self.algorithms:
             raise ValueError(f'Invalid location "{location}"')
         registry: t.Dict[str, JWEAlgorithm] = self.algorithms[location]  # type: ignore
         if name not in registry:
             raise ValueError(f'Algorithm of "{name}" is not supported')
 
         if self.allowed:
-            allowed: t.List[str] = self.allowed[location] # type: ignore
+            allowed = self.allowed
         else:
-            allowed: t.List[str] = self.recommended[location] # type: ignore
+            allowed = self.recommended
 
         if name not in allowed:
             raise ValueError(f'Algorithm of "{name}" is not allowed')
         return registry[name]
 
 
 default_registry = JWERegistry()
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7517/keygen.py` & `joserfc-0.2.0/src/joserfc/rfc7517/keygen.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 from .models import Key
 from .types import KeyAny, KeyOptions
 from ..util import to_bytes
 
 JWK_REGISTRY: Dict[str, Type[Key]] = {}
 
 
-def import_key(
-    key_type: str,
-    value: KeyAny,
-    options: KeyOptions=None) -> Key:
-
+def import_key(key_type: str, value: KeyAny, options: KeyOptions = None) -> Key:
     if key_type not in JWK_REGISTRY:
         raise ValueError(f'Invalid key type: "{key_type}"')
 
     if isinstance(value, str):
         value = to_bytes(value)
 
     key_cls = JWK_REGISTRY[key_type]
-    return key_cls.import_key(value, options)
+    return key_cls.import_key(value, options)  # type: ignore
 
 
 def generate_key(
-    key_type: str,
-    crv_or_size: Union[str, int],
-    options: KeyOptions=None,
-    private: bool=True):
-
+        key_type: str,
+        crv_or_size: Union[str, int],
+        options: KeyOptions = None,
+        private: bool = True):
     if key_type not in JWK_REGISTRY:
         raise ValueError(f'Invalid key type: "{key_type}"')
 
     key_cls = JWK_REGISTRY[key_type]
     return key_cls.generate_key(crv_or_size, options, private)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7517/keyset.py` & `joserfc-0.2.0/src/joserfc/rfc7517/keyset.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,41 +16,40 @@
             assert key.kid is not None
             if isinstance(key, SymmetricKey):
                 keys.append(key.as_dict(**params))
             else:
                 keys.append(key.as_dict(private=private, **params))
         return {"keys": keys}
 
-    def get_by_kid(self, kid: Optional[str]=None) -> Key:
+    def get_by_kid(self, kid: Optional[str] = None) -> Key:
         if kid is None and len(self.keys) == 1:
             return self.keys[0]
 
         for key in self.keys:
             if key.kid == kid:
                 return key
         raise ValueError(f'No key for kid: "{kid}"')
 
     @classmethod
-    def import_key_set(cls, value: KeySetDict, options: KeyOptions=None) -> 'KeySet':
+    def import_key_set(cls, value: KeySetDict, options: KeyOptions = None) -> "KeySet":
         keys = []
 
-        for data in value['keys']:
-            key_type = data['kty']
+        for data in value["keys"]:
+            key_type = data["kty"]
             keys.append(import_key(key_type, data, options))
 
         return cls(keys)
 
     @classmethod
     def generate_key_set(
             cls,
             key_type: str,
             crv_or_size: Union[str, int],
-            options: KeyOptions=None,
-            private: bool=True,
-            count: int=4) -> 'KeySet':
-
+            options: KeyOptions = None,
+            private: bool = True,
+            count: int = 4) -> "KeySet":
         keys = []
         for i in range(count):
             key = generate_key(key_type, crv_or_size, options, private)
             keys.append(key)
 
         return cls(keys)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7517/models.py` & `joserfc-0.2.0/src/joserfc/rfc7517/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,29 @@
     KeyParameterRegistryDict,
     JWK_PARAMETER_REGISTRY,
     KeyOperationRegistryDict,
     JWK_OPERATION_REGISTRY,
 )
 from ..util import to_bytes
 from ..rfc7638 import thumbprint
+from ..errors import (
+    UnsupportedKeyUseError,
+    UnsupportedKeyAlgorithmError,
+    UnsupportedKeyOperationError,
+)
+
 
-if hasattr(t, 'Self'):
-    SelfKey = t.Self
-else:
-    SelfKey = t.TypeVar('SelfKey', bound='BaseKey')
+NativePublicKey = t.TypeVar("NativePublicKey")
+NativePrivateKey = t.TypeVar("NativePrivateKey")
 
 
 class NativeKeyBinding(object, metaclass=ABCMeta):
     use_key_ops_registry = {
-        'sig': ['sign', 'verify'],
-        'enc': ['encrypt', 'decrypt', 'wrapKey', 'unwrapKey', 'deriveKey', 'deriveBits']
+        "sig": ["sign", "verify"],
+        "enc": ["encrypt", "decrypt", "wrapKey", "unwrapKey", "deriveKey", "deriveBits"],
     }
 
     @classmethod
     @abstractmethod
     def convert_raw_key_to_dict(cls, raw_key, private: bool) -> KeyDict:
         pass
 
@@ -34,52 +38,52 @@
 
     @classmethod
     @abstractmethod
     def import_from_bytes(cls, value: bytes):
         pass
 
     @staticmethod
-    def as_bytes(key: 'BaseKey', encoding=None, private=None, password=None) -> bytes:
+    def as_bytes(key: "BaseKey", encoding=None, private=None, password=None) -> bytes:
         return key.raw_value
 
     @classmethod
     def validate_dict_key_registry(cls, dict_key: KeyDict, registry: KeyParameterRegistryDict):
         for k in registry:
             if registry[k].required and k not in dict_key:
                 raise ValueError(f'"{k}" is required')
 
             if k in dict_key:
                 try:
-                    registry[k].check_value(dict_key[k])
+                    registry[k].validate(dict_key[k])
                 except ValueError as error:
                     raise ValueError(f'"{k}" {error}')
 
     @classmethod
     def validate_dict_key_use_operations(cls, dict_key: KeyDict):
-        if 'use' in dict_key and 'key_ops' in dict_key:
-            operations = cls.use_key_ops_registry[dict_key['use']]
-            for op in dict_key['key_ops']:
+        if "use" in dict_key and "key_ops" in dict_key:
+            operations = cls.use_key_ops_registry[dict_key["use"]]
+            for op in dict_key["key_ops"]:
                 if op not in operations:
                     raise ValueError(f'"use" and "key_ops" does not match')
 
 
-class BaseKey(object):
+class BaseKey(t.Generic[NativePublicKey, NativePrivateKey]):
     key_type: str
     value_registry: KeyParameterRegistryDict
     param_registry: KeyParameterRegistryDict = JWK_PARAMETER_REGISTRY
     operation_registry: KeyOperationRegistryDict = JWK_OPERATION_REGISTRY
     binding = NativeKeyBinding
 
-    def __init__(self, raw_value, original_value, options: KeyOptions=None):
+    def __init__(self, raw_value, original_value, options: KeyOptions = None):
         self._raw_value = raw_value
         self.original_value = original_value
         self.options = options
         if isinstance(original_value, dict):
             data = original_value.copy()
-            data['kty'] = self.key_type
+            data["kty"] = self.key_type
             if options:
                 data.update(dict(options))
 
             self.validate_dict_key(data)
             self._dict_value = data
         else:
             self._dict_value = None
@@ -91,18 +95,18 @@
         return self.dict_value[k]
 
     def get(self, k: str, default=None):
         return self.dict_value.get(k, default)
 
     @property
     def kid(self) -> str:
-        kid = self.get('kid')
+        kid = self.get("kid")
         if not kid:
             kid = self.thumbprint()
-            self._dict_value['kid'] = kid
+            self._dict_value["kid"] = kid
         return kid
 
     @property
     def raw_value(self):
         return self._raw_value
 
     @property
@@ -114,107 +118,113 @@
         """Property of the Key in Dict (JSON)."""
         if self._dict_value:
             return self._dict_value
 
         data = self.binding.convert_raw_key_to_dict(self.raw_value, self.is_private)
         if self.options:
             data.update(dict(self.options))
-        data['kty'] = self.key_type
+        data["kty"] = self.key_type
         self.validate_dict_key(data)
         self._dict_value = data
         return data
 
     @property
-    def public_key(self):
+    def public_key(self) -> NativePublicKey:
         raise NotImplementedError()
 
     @property
-    def private_key(self):
+    def private_key(self) -> t.Optional[NativePrivateKey]:
         raise NotImplementedError()
 
     def thumbprint(self) -> str:
         """Call this method will generate the thumbprint with algorithm
         defined in RFC7638."""
         fields = [k for k in self.value_registry if self.value_registry[k].required]
-        fields.append('kty')
+        fields.append("kty")
         return thumbprint(self.dict_value, fields)
 
-    def as_dict(self, private: t.Optional[bool]=None, **params) -> KeyDict:
-        """Output this key to a JWK format (in dict). By default it will return
+    def as_dict(self, private: t.Optional[bool] = None, **params) -> KeyDict:
+        """Output this key to a JWK format (in dict). By default, it will return
         the :property:`dict_value` of this key.
 
         :param private: determine whether this method should output private key or not
         :param params: other parameters added into this key
         :raise: ValueError
         """
         # check private conflicts
         if private and not self.is_private:
             raise ValueError("This key is not a private key.")
 
         data = self.dict_value.copy()
         if private is not False:
-            # keep original
+            data.update(params)
             return data
 
         # clear private fields
         for k in self.dict_value:
             if k in self.value_registry and self.value_registry[k].private:
                 del data[k]
 
         data.update(params)
         return data
 
     def check_use(self, use: str):
-        designed_use = self.get('use')
+        designed_use = self.get("use")
         if designed_use and designed_use != use:
-            raise ValueError(f'This key is designed to by used for "{designed_use}"')
+            raise UnsupportedKeyUseError(f'This key is designed to be used for "{designed_use}"')
+
+    def check_alg(self, alg: str):
+        designed_alg = self.get("alg")
+        if designed_alg and designed_alg != alg:
+            raise UnsupportedKeyAlgorithmError(f'This key is designed for algorithm "{designed_alg}"')
+
     def check_key_op(self, operation: str):
         """Check if the given key_op is supported by this key.
 
         :param operation: key operation value, such as "sign", "encrypt".
         :raise: ValueError
         """
-        key_ops = self.get('key_ops')
+        key_ops = self.get("key_ops")
         if key_ops is not None and operation not in key_ops:
-            raise ValueError(f'Unsupported key_op "{operation}"')
+            raise UnsupportedKeyOperationError(f'Unsupported key_op "{operation}"')
 
         assert operation in self.operation_registry
         reg = self.operation_registry[operation]
         if reg.private and not self.is_private:
-            raise ValueError(f'Invalid key_op "{operation}" for public key')
+            raise UnsupportedKeyOperationError(f'Invalid key_op "{operation}" for public key')
 
-    def get_op_key(self, operation: str):
+    def get_op_key(self, operation: str) -> t.Union[NativePublicKey, NativePrivateKey]:
         self.check_key_op(operation)
         reg = self.operation_registry[operation]
         if reg.private:
             return self.private_key
         return self.public_key
 
     @classmethod
     def validate_dict_key(cls, data: KeyDict):
         cls.binding.validate_dict_key_registry(data, cls.param_registry)
         cls.binding.validate_dict_key_registry(data, cls.value_registry)
         cls.binding.validate_dict_key_use_operations(data)
 
     @classmethod
-    def import_key(cls, value: KeyAny, options: KeyOptions=None) -> SelfKey:
+    def import_key(cls, value: KeyAny, options: KeyOptions = None) -> "BaseKey":
         if isinstance(value, dict):
             cls.validate_dict_key(value)
             raw_key = cls.binding.import_from_dict(value)
             return cls(raw_key, value, options)
 
         raw_key = cls.binding.import_from_bytes(to_bytes(value))
         return cls(raw_key, value, options)
 
     @classmethod
-    def generate_key(cls, size_or_crv, options: KeyOptions = None, private: bool=True) -> SelfKey:
+    def generate_key(cls, size_or_crv, options: KeyOptions = None, private: bool = True) -> "BaseKey":
         raise NotImplementedError()
 
 
-class SymmetricKey(BaseKey, metaclass=ABCMeta):
+class SymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
     @property
     def raw_value(self) -> bytes:
         return self._raw_value
 
     @property
     def is_private(self) -> bool:
         return True
@@ -224,31 +234,34 @@
         return self.raw_value
 
     @property
     def private_key(self) -> bytes:
         return self.raw_value
 
 
-class AsymmetricKey(BaseKey, metaclass=ABCMeta):
+class AsymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
+    @property
+    def raw_value(self) -> t.Union[NativePublicKey, NativePrivateKey]:
+        return self._raw_value
+
     def as_bytes(
             self,
-            encoding: t.Optional[str]=None,
-            private: t.Optional[bool]=None,
-            password: t.Optional[str]=None) -> bytes:
+            encoding: t.Optional[str] = None,
+            private: t.Optional[bool] = None,
+            password: t.Optional[str] = None) -> bytes:
         return self.binding.as_bytes(self, encoding, private, password)
 
     def as_pem(self, private=None, password=None) -> bytes:
         return self.as_bytes(private=private, password=password)
 
     def as_der(self, private=None, password=None) -> bytes:
-        return self.as_bytes(encoding='DER', private=private, password=password)
-
+        return self.as_bytes(encoding="DER", private=private, password=password)
 
 
-class CurveKey(AsymmetricKey):
+class CurveKey(AsymmetricKey[NativePublicKey, NativePrivateKey]):
     @property
     @abstractmethod
     def curve_name(self) -> str:
         pass
 
     @abstractmethod
     def exchange_shared_key(self, pubkey) -> bytes:
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.2.0/src/joserfc/rfc7517/pem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from abc import ABCMeta, abstractmethod
-from typing import Optional
 
 from cryptography.x509 import load_pem_x509_certificate
 from cryptography.hazmat.primitives.serialization import (
-    load_pem_private_key, load_pem_public_key, load_ssh_public_key,
-    Encoding, PrivateFormat, PublicFormat,
-    BestAvailableEncryption, NoEncryption,
+    load_pem_private_key,
+    load_pem_public_key,
+    load_ssh_public_key,
+    Encoding,
+    PrivateFormat,
+    PublicFormat,
+    BestAvailableEncryption,
+    NoEncryption,
 )
 from cryptography.hazmat.backends import default_backend
 from .models import NativeKeyBinding
 from .types import KeyDict
 from ..util import to_bytes
 
 
 def load_pem_key(raw: bytes, ssh_type=None, key_type=None, password=None):
     if ssh_type and raw.startswith(ssh_type):
         return load_ssh_public_key(raw, backend=default_backend())
 
-    if key_type == 'public':
+    if key_type == "public":
         return load_pem_public_key(raw, backend=default_backend())
 
-    if key_type == 'private' or password is not None:
+    if key_type == "private" or password is not None:
         return load_pem_private_key(raw, password=password, backend=default_backend())
 
-    if b'PUBLIC' in raw:
+    if b"PUBLIC" in raw:
         return load_pem_public_key(raw, backend=default_backend())
 
-    if b'PRIVATE' in raw:
+    if b"PRIVATE" in raw:
         return load_pem_private_key(raw, password=password, backend=default_backend())
 
-    if b'CERTIFICATE' in raw:
+    if b"CERTIFICATE" in raw:
         cert = load_pem_x509_certificate(raw, default_backend())
         return cert.public_key()
 
     try:
         return load_pem_private_key(raw, password=password, backend=default_backend())
     except ValueError:
         return load_pem_public_key(raw, backend=default_backend())
@@ -45,20 +49,20 @@
     :param key: native cryptography key
     :param encoding: "PEM" or "DER"
     :param private: export private key or public key
     :param password: encrypt private key with password
     :return: bytes
     """
 
-    if encoding is None or encoding == 'PEM':
+    if encoding is None or encoding == "PEM":
         encoding = Encoding.PEM
-    elif encoding == 'DER':
+    elif encoding == "DER":
         encoding = Encoding.DER
     else:
-        raise ValueError('Invalid encoding: {!r}'.format(encoding))
+        raise ValueError("Invalid encoding: {!r}".format(encoding))
 
     if private:
         if password is None:
             encryption_algorithm = NoEncryption()
         else:
             encryption_algorithm = BestAvailableEncryption(to_bytes(password))
         return key.private_bytes(
@@ -79,15 +83,15 @@
     def convert_raw_key_to_dict(cls, raw_key, private: bool) -> KeyDict:
         if private:
             return cls.export_private_key(raw_key)
         return cls.export_public_key(raw_key)
 
     @classmethod
     def import_from_dict(cls, value: KeyDict):
-        if 'd' in value:
+        if "d" in value:
             return cls.import_private_key(value)
         return cls.import_public_key(value)
 
     @classmethod
     def import_from_bytes(cls, value: bytes):
         return load_pem_key(value, cls.ssh_type)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7517/types.py` & `joserfc-0.2.0/src/joserfc/rfc7517/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import typing as t
 
-__all__ = ['KeyDict', 'KeyAny', 'KeyOptions', 'KeySetDict']
+__all__ = ["KeyDict", "KeyAny", "KeyOptions", "KeySetDict"]
 
 #: JSON Web Key in dict
 KeyDict = t.Dict[str, t.Union[str, t.List[str]]]
 
 #: Key in str, bytes and dict
 KeyAny = t.Union[str, bytes, KeyDict]
 
 #: extra options for JWK
-KeyOptions = t.TypedDict('KeyOptions', {
-    'use': str,
-    'key_ops': t.List[str],
-    'alg': str,
-    'kid': str,
-    'x5u': str,
-    'x5c': t.List[str],
-    'x5t': str,
-    'x5t#S256': str,
+KeyOptions = t.TypedDict("KeyOptions", {
+    "use": str,
+    "key_ops": t.List[str],
+    "alg": str,
+    "kid": str,
+    "x5u": str,
+    "x5c": t.List[str],
+    "x5t": str,
+    "x5t#S256": str,
 }, total=False)
 
 #: JWKs in dict
-KeySetDict = t.TypedDict('KeySetDict', {
-    'keys': t.List[KeyDict],
+KeySetDict = t.TypedDict("KeySetDict", {
+    "keys": t.List[KeyDict],
 })
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.2.0/src/joserfc/rfc7518/ec_key.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,135 +1,134 @@
-from typing import Optional, Union, Dict
+from typing import Optional, Dict
 from functools import cached_property
-from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric.ec import (
-    EllipticCurvePublicKey, EllipticCurvePrivateKeyWithSerialization,
-    EllipticCurvePrivateNumbers, EllipticCurvePublicNumbers,
-    SECP256R1, SECP384R1, SECP521R1
+    generate_private_key,
+    ECDH,
+    EllipticCurvePublicKey,
+    EllipticCurvePrivateKey,
+    EllipticCurvePrivateNumbers,
+    EllipticCurvePublicNumbers,
+    SECP256R1,
+    SECP384R1,
+    SECP521R1,
 )
 from cryptography.hazmat.backends import default_backend
 from ..rfc7517.models import CurveKey
 from ..rfc7517.pem import CryptographyBinding
 from ..rfc7517.types import KeyDict, KeyOptions
 from ..util import base64_to_int, int_to_base64
-from ..registry import KeyParameter, is_str
+from ..registry import KeyParameter
 
 
-NativeECKey = Union[EllipticCurvePublicKey, EllipticCurvePrivateKeyWithSerialization]
 DSS_CURVES = {
-    'P-256': SECP256R1,
-    'P-384': SECP384R1,
-    'P-521': SECP521R1,
+    "P-256": SECP256R1,
+    "P-384": SECP384R1,
+    "P-521": SECP521R1,
 }
 CURVES_DSS = {
-    SECP256R1.name: 'P-256',
-    SECP384R1.name: 'P-384',
-    SECP521R1.name: 'P-521',
+    SECP256R1.name: "P-256",
+    SECP384R1.name: "P-384",
+    SECP521R1.name: "P-521",
 }
 
+
 class ECBinding(CryptographyBinding):
-    ssh_type = b'ecdsa-sha2-'
+    ssh_type = b"ecdsa-sha2-"
 
     @staticmethod
-    def import_private_key(obj: KeyDict) -> EllipticCurvePrivateKeyWithSerialization:
-        curve = DSS_CURVES[obj['crv']]()
+    def import_private_key(obj: KeyDict) -> EllipticCurvePrivateKey:
+        curve = DSS_CURVES[obj["crv"]]()
         public_numbers = EllipticCurvePublicNumbers(
-            base64_to_int(obj['x']),
-            base64_to_int(obj['y']),
+            base64_to_int(obj["x"]),
+            base64_to_int(obj["y"]),
             curve,
         )
-        private_numbers = EllipticCurvePrivateNumbers(
-            base64_to_int(obj['d']),
-            public_numbers
-        )
+        private_numbers = EllipticCurvePrivateNumbers(base64_to_int(obj["d"]), public_numbers)
         return private_numbers.private_key(default_backend())
 
     @staticmethod
-    def export_private_key(key: EllipticCurvePrivateKeyWithSerialization) -> Dict[str, str]:
+    def export_private_key(key: EllipticCurvePrivateKey) -> Dict[str, str]:
         numbers = key.private_numbers()
         return {
-            'crv': CURVES_DSS[key.curve.name],
-            'x': int_to_base64(numbers.public_numbers.x),
-            'y': int_to_base64(numbers.public_numbers.y),
-            'd': int_to_base64(numbers.private_value),
+            "crv": CURVES_DSS[key.curve.name],
+            "x": int_to_base64(numbers.public_numbers.x),
+            "y": int_to_base64(numbers.public_numbers.y),
+            "d": int_to_base64(numbers.private_value),
         }
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> EllipticCurvePublicKey:
-        curve = DSS_CURVES[obj['crv']]()
+        curve = DSS_CURVES[obj["crv"]]()
         public_numbers = EllipticCurvePublicNumbers(
-            base64_to_int(obj['x']),
-            base64_to_int(obj['y']),
+            base64_to_int(obj["x"]),
+            base64_to_int(obj["y"]),
             curve,
         )
         return public_numbers.public_key(default_backend())
 
     @staticmethod
     def export_public_key(key: EllipticCurvePublicKey) -> Dict[str, str]:
         numbers = key.public_numbers()
         return {
-            'crv': CURVES_DSS[numbers.curve.name],
-            'x': int_to_base64(numbers.x),
-            'y': int_to_base64(numbers.y)
+            "crv": CURVES_DSS[numbers.curve.name],
+            "x": int_to_base64(numbers.x),
+            "y": int_to_base64(numbers.y),
         }
 
 
-class ECKey(CurveKey):
-    key_type: str = 'EC'
+class ECKey(CurveKey[EllipticCurvePublicKey, EllipticCurvePrivateKey]):
+    key_type: str = "EC"
     #: Registry definition for EC Key
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.2
     value_registry = {
-        'crv': KeyParameter('Curve', True, False, is_str),
-        'x': KeyParameter('X Coordinate', True, False, is_str),
-        'y': KeyParameter('Y Coordinate', True, False, is_str),
-        'd': KeyParameter('EC Private Key', False, True, is_str),
+        "crv": KeyParameter("Curve", "str", private=False, required=True),
+        "x": KeyParameter("X Coordinate", "str", private=False, required=True),
+        "y": KeyParameter("Y Coordinate", "str", private=False, required=True),
+        "d": KeyParameter("EC Private Key", "str", private=True, required=False),
     }
     binding = ECBinding
 
     def exchange_shared_key(self, pubkey: EllipticCurvePublicKey) -> bytes:
         # used in ECDHESAlgorithm
         if self.private_key:
-            return self.private_key.exchange(ec.ECDH(), pubkey)
-        raise ValueError('Invalid key for exchanging shared key')
-
-    @property
-    def raw_value(self) -> NativeECKey:
-        return self._raw_value
+            return self.private_key.exchange(ECDH(), pubkey)
+        raise ValueError("Invalid key for exchanging shared key")
 
     @property
     def is_private(self) -> bool:
-        return isinstance(self.raw_value, EllipticCurvePrivateKeyWithSerialization)
+        return isinstance(self.raw_value, EllipticCurvePrivateKey)
 
     @cached_property
     def public_key(self) -> EllipticCurvePublicKey:
-        if isinstance(self.raw_value, EllipticCurvePrivateKeyWithSerialization):
+        if isinstance(self.raw_value, EllipticCurvePrivateKey):
             return self.raw_value.public_key()
         return self.raw_value
 
     @property
-    def private_key(self) -> Optional[EllipticCurvePrivateKeyWithSerialization]:
+    def private_key(self) -> Optional[EllipticCurvePrivateKey]:
         if self.is_private:
             return self.raw_value
         return None
 
     @property
     def curve_name(self) -> str:
         return CURVES_DSS[self.raw_value.curve.name]
 
     @property
     def curve_key_size(self) -> int:
         return self.raw_value.curve.key_size
 
     @classmethod
     def generate_key(
-            cls, crv: str='P-256',
-            options: KeyOptions=None,
-            private: bool=True) -> 'ECKey':
+            cls,
+            crv: str = "P-256",
+            options: KeyOptions = None,
+            private: bool = True) -> "ECKey":
         if crv not in DSS_CURVES:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
-        raw_key = ec.generate_private_key(
+        raw_key = generate_private_key(
             curve=DSS_CURVES[crv](),
             backend=default_backend(),
         )
         if not private:
             raw_key = raw_key.public_key()
         return cls(raw_key, raw_key, options)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.2.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,357 +1,315 @@
 import os
-import struct
 import typing as t
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.keywrap import aes_key_wrap, aes_key_unwrap
+from cryptography.hazmat.primitives.keywrap import (
+    aes_key_wrap,
+    aes_key_unwrap,
+    InvalidUnwrap,
+)
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import GCM
-from cryptography.hazmat.primitives.kdf.concatkdf import ConcatKDFHash
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from .rsa_key import RSAKey
 from .oct_key import OctKey
-from ..rfc7516.models import JWEAlgModel, JWEEncModel
-from ..rfc7516.types import EncryptionData, Recipient, Header
+from .derive_key import derive_key_for_concat_kdf
 from ..rfc7517.models import CurveKey
+from ..rfc7516.models import (
+    JWEDirectEncryption,
+    JWEKeyEncryption,
+    JWEKeyWrapping,
+    JWEKeyAgreement,
+    JWEEncModel,
+    Recipient,
+)
 from ..util import to_bytes, urlsafe_b64encode, urlsafe_b64decode
-from ..registry import HeaderParameter, is_str, is_int, is_jwk
+from ..registry import HeaderParameter
+from ..errors import (
+    InvalidKeyLengthError,
+    InvalidKeyTypeError,
+    UnwrapError,
+)
 
 
-class DirectAlgModel(JWEAlgModel):
-    name = 'dir'
-    description = 'Direct use of a shared symmetric key'
+class DirectAlgModel(JWEDirectEncryption):
+    name = "dir"
+    description = "Direct use of a shared symmetric key"
     recommended = True
-    key_encryption = True
 
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        obj: EncryptionData = recipient.parent
-        assert obj.cek is None
-
-        cek = key.get_op_key('encrypt')
-        if len(cek) * 8 != enc.cek_size:
-            raise ValueError('Invalid "cek" length')
-
-        # attach CEK to parent
-        obj.cek = cek
-        return b''
-
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        cek = key.get_op_key('decrypt')
+    @staticmethod
+    def check_recipient_key(key) -> OctKey:
+        if isinstance(key, OctKey):
+            return key
+        raise InvalidKeyTypeError()
+
+    def compute_cek(self, size: int, recipient: Recipient):
+        key = self.check_recipient_key(recipient.recipient_key)
+        cek = key.raw_value
+        if len(cek) * 8 != size:
+            raise InvalidKeyLengthError(f"A key of size {size} bits MUST be used")
         return cek
 
 
-class RSAAlgModel(JWEAlgModel):
+class RSAAlgModel(JWEKeyEncryption):
     #: A key of size 2048 bits or larger MUST be used with these algorithms
     #: RSA1_5, RSA-OAEP, RSA-OAEP-256
     key_size = 2048
-    key_encryption = True
 
-    def __init__(self, name: str, description: str,
-                 pad_fn: padding.AsymmetricPadding,
-                 recommended: bool=False):
+    def __init__(
+            self,
+            name: str,
+            description: str,
+            pad_fn: padding.AsymmetricPadding,
+            recommended: bool = False):
         self.name = name
         self.description = description
         self.padding = pad_fn
         self.recommended = recommended
 
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: RSAKey) -> bytes:
-        op_key = key.get_op_key('encrypt')
+    @staticmethod
+    def check_recipient_key(key) -> RSAKey:
+        if isinstance(key, RSAKey):
+            return key
+        raise InvalidKeyTypeError()
+
+    def encrypt_cek(self, cek: bytes, recipient: Recipient):
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("encrypt")
         if op_key.key_size < self.key_size:
-            raise ValueError('A key of size 2048 bits or larger MUST be used')
-        return op_key.encrypt(recipient.parent.cek, self.padding)
+            raise InvalidKeyLengthError(f"A key of size {self.key_size} bits or larger MUST be used")
+        return op_key.encrypt(cek, self.padding)
 
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: RSAKey) -> bytes:
-        op_key = key.get_op_key('decrypt')
+    def decrypt_cek(self, recipient: Recipient) -> bytes:
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("decrypt")
         cek = op_key.decrypt(recipient.encrypted_key, self.padding)
         return cek
 
 
-class AESAlgModel(JWEAlgModel):
-    key_wrapping = True
-
-    def __init__(self, key_size: int, recommended: bool=False):
-        self.name = f'A{key_size}KW'
-        self.description = f'AES Key Wrap using {key_size}-bit key'
+class AESAlgModel(JWEKeyWrapping):
+    def __init__(self, key_size: int, recommended: bool = False):
+        self.name = f"A{key_size}KW"
+        self.description = f"AES Key Wrap using {key_size}-bit key"
         self.key_size = key_size
         self.recommended = recommended
 
-    def _check_key(self, key):
-        if len(key) * 8 != self.key_size:
-            raise ValueError(
-                'A key of size {} bits is required.'.format(self.key_size))
-
-    def wrap_cek(self, cek: bytes, key: OctKey) -> bytes:
-        op_key = key.get_op_key('wrapKey')
-        self._check_key(op_key)
-        return aes_key_wrap(op_key, cek, default_backend())
-
-    def unwrap_cek(self, encrypted_key: bytes, key: OctKey) -> bytes:
-        op_key = key.get_op_key('unwrapKey')
-        self._check_key(op_key)
-        return aes_key_unwrap(op_key, encrypted_key, default_backend())
-
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        return self.wrap_cek(recipient.parent.cek, key)
-
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        cek = self.unwrap_cek(recipient.encrypted_key, key)
-        if len(cek) * 8 != enc.cek_size:
-            raise ValueError('Invalid "cek" length')
+    def wrap_cek(self, cek: bytes, key: bytes) -> bytes:
+        self.check_op_key(key)
+        return aes_key_wrap(key, cek, default_backend())
+
+    def unwrap_cek(self, ek: bytes, key: bytes):
+        self.check_op_key(key)
+        try:
+            cek = aes_key_unwrap(key, ek, default_backend())
+        except InvalidUnwrap:
+            raise UnwrapError()
         return cek
 
+    def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("wrapKey")
+        return self.wrap_cek(cek, op_key)
+
+    def decrypt_cek(self, recipient: Recipient) -> bytes:
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("unwrapKey")
+        return self.unwrap_cek(recipient.encrypted_key, op_key)
 
-A128KW = AESAlgModel(128, True)  # A128KW, Recommended
-A192KW = AESAlgModel(192)  # A192KW
-A256KW = AESAlgModel(256, True)  # A256KW, Recommended
 
-AES_KW_MAP: t.Dict[int, AESAlgModel] = {
-    128: A128KW,
-    192: A192KW,
-    256: A256KW,
-}
-
-class AESGCMAlgModel(JWEAlgModel):
+class AESGCMAlgModel(JWEKeyWrapping):
     more_header_registry = {
-        'iv': HeaderParameter('Initialization vector', True, is_str),
-        'tag': HeaderParameter('Authentication tag', True, is_str),
+        "iv": HeaderParameter("Initialization vector", "str", True),
+        "tag": HeaderParameter("Authentication tag", "str", True),
     }
-    key_wrapping = True
 
     def __init__(self, key_size: int):
-        self.name = f'A{key_size}GCMKW'
-        self.description = f'Key wrapping with AES GCM using {key_size}-bit key'
+        self.name = f"A{key_size}GCMKW"
+        self.description = f"Key wrapping with AES GCM using {key_size}-bit key"
         self.key_size = key_size
 
-    def _check_key(self, key):
-        if len(key) * 8 != self.key_size:
-            raise ValueError(
-                'A key of size {} bits is required.'.format(self.key_size))
-
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        op_key = key.get_op_key('wrapKey')
-        self._check_key(op_key)
+    def wrap_cek(self, cek: bytes, key: bytes) -> bytes:
+        raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
+
+    def unwrap_cek(self, ek: bytes, key: bytes):
+        raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
+
+    def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("wrapKey")
+        self.check_op_key(op_key)
 
         #: https://tools.ietf.org/html/rfc7518#section-4.7.1.1
         #: The "iv" (initialization vector) Header Parameter value is the
         #: base64url-encoded representation of the 96-bit IV value
         iv_size = 96
         iv = os.urandom(iv_size // 8)
 
         cipher = Cipher(AES(op_key), GCM(iv), backend=default_backend())
         enc = cipher.encryptor()
-        obj: EncryptionData = recipient.parent
 
-        encrypted_key = enc.update(obj.cek) + enc.finalize()
-        recipient.add_header('iv', urlsafe_b64encode(iv).decode('ascii'))
-        recipient.add_header('tag', urlsafe_b64encode(enc.tag).decode('ascii'))
+        encrypted_key = enc.update(cek) + enc.finalize()
+        recipient.add_header("iv", urlsafe_b64encode(iv).decode("ascii"))
+        recipient.add_header("tag", urlsafe_b64encode(enc.tag).decode("ascii"))
         return encrypted_key
 
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        op_key = key.get_op_key('unwrapKey')
-        self._check_key(op_key)
+    def decrypt_cek(self, recipient: Recipient) -> bytes:
+        key = self.check_recipient_key(recipient.recipient_key)
+        op_key = key.get_op_key("unwrapKey")
+        self.check_op_key(op_key)
 
         headers = recipient.headers()
-        assert 'iv' in headers
-        assert 'tag' in headers
-        iv = urlsafe_b64decode(to_bytes(headers['iv']))
-        tag = urlsafe_b64decode(to_bytes(headers['tag']))
+        assert "iv" in headers
+        assert "tag" in headers
+        iv = urlsafe_b64decode(to_bytes(headers["iv"]))
+        tag = urlsafe_b64decode(to_bytes(headers["tag"]))
 
         cipher = Cipher(AES(op_key), GCM(iv, tag), backend=default_backend())
         d = cipher.decryptor()
         cek = d.update(recipient.encrypted_key) + d.finalize()
         return cek
 
 
-class ECDHESAlgModel(JWEAlgModel):
+class ECDHESAlgModel(JWEKeyAgreement):
     more_header_registry = {
-        'epk': HeaderParameter('Ephemeral Public Key', True, is_jwk),
-        'apu': HeaderParameter('Agreement PartyUInfo', False, is_str),
-        'apv': HeaderParameter('Agreement PartyVInfo', False, is_str),
+        "epk": HeaderParameter("Ephemeral Public Key", "jwk", True),
+        "apu": HeaderParameter("Agreement PartyUInfo", "str"),
+        "apv": HeaderParameter("Agreement PartyVInfo", "str"),
     }
-    key_agreement = True
 
     # https://tools.ietf.org/html/rfc7518#section-4.6
-    def __init__(self, key_size: t.Optional[int]=None, recommended: bool=False):
-        if key_size is None:
-            self.name = 'ECDH-ES'
-            self.description = 'ECDH-ES in the Direct Key Agreement mode'
-            self.key_wrapping = False
+    def __init__(self, key_wrapping: t.Optional[JWEKeyWrapping] = None):
+        if key_wrapping is None:
+            self.name = "ECDH-ES"
+            self.description = "ECDH-ES in the Direct Key Agreement mode"
+            self.key_size = None
+            self.recommended = True
         else:
-            self.name = f'ECDH-ES+A{key_size}KW'
-            self.description = f'ECDH-ES using Concat KDF and CEK wrapped with A{key_size}KW'
-            self.key_wrapping = True
-        self.key_size = key_size
-        self.recommended = recommended
-
-    def get_bit_size(self, enc: JWEEncModel) -> int:
-        if self.key_size is None:
-            bit_size = enc.cek_size
-        else:
-            bit_size = self.key_size
-        return bit_size
-
-    def compute_fixed_info(self, header: Header, bit_size: int):
-        # AlgorithmID
-        if self.key_size is None:
-            alg_id = u32be_len_input(header['enc'])
-        else:
-            alg_id = u32be_len_input(header['alg'])
-
-        # PartyUInfo
-        apu_info = u32be_len_input(header.get('apu'), True)
-        # PartyVInfo
-        apv_info = u32be_len_input(header.get('apv'), True)
-        # SuppPubInfo
-        pub_info = struct.pack('>I', bit_size)
-        return alg_id + apu_info + apv_info + pub_info
-
-    def compute_derived_key(self, shared_key: bytes, header: Header, bit_size: int) -> bytes:
-        fixed_info = self.compute_fixed_info(header, bit_size)
-        ckdf = ConcatKDFHash(
-            algorithm=hashes.SHA256(),
-            length=bit_size // 8,
-            otherinfo=fixed_info,
-            backend=default_backend()
-        )
-        return ckdf.derive(shared_key)
+            self.name = f"ECDH-ES+{key_wrapping.name}"
+            self.description = f"ECDH-ES using Concat KDF and CEK wrapped with {key_wrapping.name}"
+            self.key_size = key_wrapping.key_size
+            self.recommended = key_wrapping.recommended
+        self.key_wrapping = key_wrapping
+
+    def encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient):
+        recipient_key: CurveKey = recipient.recipient_key
+        ephemeral_key: CurveKey = recipient.ephemeral_key
+        pubkey = recipient_key.get_op_key("deriveKey")
+        shared_key = ephemeral_key.exchange_shared_key(pubkey)
+        header = recipient.headers()
+        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size)
+
+    def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
+        header = recipient.headers()
+        assert "epk" in header
+
+        recipient_key: CurveKey = self.check_recipient_key(recipient.recipient_key)
+        epk = recipient_key.import_key(header["epk"])
+        pubkey = epk.get_op_key("deriveKey")
+        shared_key = recipient_key.exchange_shared_key(pubkey)
+        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size)
 
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: CurveKey) -> bytes:
-        if recipient.ephemeral_key is None:
-            recipient.ephemeral_key = key.generate_key(key.curve_name, private=True)
-
-        bit_size = self.get_bit_size(enc)
-        pubkey = key.get_op_key('deriveKey')
-        shared_key = recipient.ephemeral_key.exchange_shared_key(pubkey)
-        headers = recipient.headers()
-        dk = self.compute_derived_key(shared_key, headers, bit_size)
 
-        obj: EncryptionData = recipient.parent
-        recipient.add_header('epk', recipient.ephemeral_key.as_dict(private=False))
-
-        if self.key_size is None:
-            assert obj.cek is None
-            obj.cek = dk
-            return b''
-        else:
-            aeskw: AESAlgModel = AES_KW_MAP[self.key_size]
-            return aeskw.wrap_cek(obj.cek, OctKey.import_key(dk))
-
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: CurveKey) -> bytes:
-        headers = recipient.headers()
-        assert 'epk' in headers
-        epk = key.import_key(headers['epk'])
-
-        bit_size = self.get_bit_size(enc)
-        pubkey = epk.get_op_key('deriveKey')
-        shared_key = key.exchange_shared_key(pubkey)
-
-        dk = self.compute_derived_key(shared_key, headers, bit_size)
-        if self.key_size is None:
-            # delivery_key is ciphertext's encrypt key
-            return dk
-        else:
-            aeskw: AESAlgModel = AES_KW_MAP[self.key_size]
-            return aeskw.unwrap_cek(recipient.encrypted_key, OctKey.import_key(dk))
-
-
-class PBES2HSAlgModel(JWEAlgModel):
+class PBES2HSAlgModel(JWEKeyEncryption):
     # https://www.rfc-editor.org/rfc/rfc7518#section-4.8
     more_header_registry = {
-        'p2s': HeaderParameter('PBES2 Salt Input', True, is_str),
-        'p2c': HeaderParameter('PBES2 Count', True, is_int),
+        "p2s": HeaderParameter("PBES2 Salt Input", "str", True),
+        "p2c": HeaderParameter("PBES2 Count", "int", True),
     }
-    key_wrapping = True
 
     # A minimum iteration count of 1000 is RECOMMENDED.
     DEFAULT_P2C = 2048
 
-    def __init__(self, hash_size: int, key_size: int):
-        self.name = f'PBES2-HS{hash_size}+A{key_size}KW'
-        self.description = f'PBES2 with HMAC SHA-{hash_size} and A{key_size}KW wrapping'
-        self.key_size = key_size
-        self.hash_alg = getattr(hashes, f'SHA{hash_size}')()
+    def __init__(self, hash_size: int, key_wrapping: JWEKeyWrapping):
+        self.name = f"PBES2-HS{hash_size}+{key_wrapping.name}"
+        self.description = f"PBES2 with HMAC SHA-{hash_size} and {key_wrapping.name} wrapping"
+        self.key_size = key_wrapping.key_size
+        self.key_wrapping = key_wrapping
+        self.hash_alg = getattr(hashes, f"SHA{hash_size}")()
+
+    @staticmethod
+    def check_recipient_key(key) -> OctKey:
+        if isinstance(key, OctKey):
+            return key
+        raise InvalidKeyTypeError()
 
-    def compute_derived_key(self, key: bytes, header: Header, p2c: int) -> bytes:
-        p2s = urlsafe_b64decode(to_bytes(header['p2s']))
+    def compute_derived_key(self, key: bytes, p2s: bytes, p2c: int) -> bytes:
         # The salt value used is (UTF8(Alg) || 0x00 || Salt Input)
-        salt = to_bytes(self.name) + b'\x00' + p2s
+        salt = to_bytes(self.name) + b"\x00" + p2s
         kdf = PBKDF2HMAC(
             algorithm=self.hash_alg,
             length=self.key_size // 8,
             salt=salt,
             iterations=p2c,
             backend=default_backend(),
         )
         return kdf.derive(key)
 
-    def encrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
-        obj: EncryptionData = recipient.parent
+    def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
         headers = recipient.headers()
-
-        if 'p2s' not in headers:
+        if "p2s" not in headers:
             p2s = os.urandom(16)
-            recipient.add_header('p2s', urlsafe_b64encode(p2s).decode('ascii'))
-
-        if 'p2c' in headers:
-            p2c = headers['p2c']
+            recipient.add_header("p2s", urlsafe_b64encode(p2s).decode("ascii"))
         else:
+            p2s = urlsafe_b64decode(to_bytes(headers["p2s"]))
+
+        if "p2c" not in headers:
             # A minimum iteration count of 1000 is RECOMMENDED.
             p2c = self.DEFAULT_P2C
-            recipient.add_header('p2c', p2c)
+            recipient.add_header("p2c", p2c)
+        else:
+            p2c = headers["p2c"]
 
-        kek = self.compute_derived_key(key.get_op_key('deriveKey'), headers, p2c)
-        aeskw: AESAlgModel = AES_KW_MAP[self.key_size]
-        return aeskw.wrap_cek(obj.cek, OctKey.import_key(kek))
+        key = self.check_recipient_key(recipient.recipient_key)
+        kek = self.compute_derived_key(key.get_op_key("deriveKey"), p2s, p2c)
+        return self.key_wrapping.wrap_cek(cek, kek)
 
-    def decrypt_recipient(self, enc: JWEEncModel, recipient: Recipient, key: OctKey) -> bytes:
+    def decrypt_cek(self, recipient: Recipient) -> bytes:
         headers = recipient.headers()
-        obj: EncryptionData = recipient.parent
+        assert "p2s" in headers
+        assert "p2c" in headers
+        p2s = urlsafe_b64decode(to_bytes(headers["p2s"]))
+        p2c = headers["p2c"]
+        key = self.check_recipient_key(recipient.recipient_key)
+        kek = self.compute_derived_key(key.get_op_key("deriveKey"), p2s, p2c)
+        return self.key_wrapping.unwrap_cek(recipient.encrypted_key, kek)
 
-        assert 'p2s' in headers
-        assert 'p2c' in headers
 
-        p2c = headers['p2c']
-        kek = self.compute_derived_key(key.get_op_key('deriveKey'), headers, p2c)
-        aeskw = AES_KW_MAP[self.key_size]
-        return aeskw.unwrap_cek(recipient.encrypted_key, OctKey.import_key(kek))
-
-
-def u32be_len_input(s, base64=False):
-    if not s:
-        return b'\x00\x00\x00\x00'
-    if base64:
-        s = urlsafe_b64decode(to_bytes(s))
-    else:
-        s = to_bytes(s)
-    return struct.pack('>I', len(s)) + s
+A128KW = AESAlgModel(128, True)  # A128KW, Recommended
+A192KW = AESAlgModel(192)  # A192KW
+A256KW = AESAlgModel(256, True)  # A256KW, Recommended
 
 
 #: https://www.rfc-editor.org/rfc/rfc7518#section-4.1
 JWE_ALG_MODELS = [
-    RSAAlgModel('RSA1_5', 'RSAES-PKCS1-v1_5', padding.PKCS1v15()),  # Recommended-
+    # Avoid all RSA-PKCS1 v1.5 encryption algorithms ([RFC8017], Section 7.2),
+    # preferring RSAES-OAEP ([RFC8017], Section 7.1).
+    # https://www.rfc-editor.org/rfc/rfc8725#section-3.2
+    RSAAlgModel("RSA1_5", "RSAES-PKCS1-v1_5", padding.PKCS1v15()),
     RSAAlgModel(
-        'RSA-OAEP', 'RSAES OAEP using default parameters',
+        "RSA-OAEP",
+        "RSAES OAEP using default parameters",
         padding.OAEP(padding.MGF1(hashes.SHA1()), hashes.SHA1(), None),
         True,
-    ),   # Recommended+
+    ),  # Recommended+
     RSAAlgModel(
-        'RSA-OAEP-256', 'RSAES OAEP using SHA-256 and MGF1 with SHA-256',
-        padding.OAEP(padding.MGF1(hashes.SHA256()), hashes.SHA256(), None)
+        "RSA-OAEP-256",
+        "RSAES OAEP using SHA-256 and MGF1 with SHA-256",
+        padding.OAEP(padding.MGF1(hashes.SHA256()), hashes.SHA256(), None),
     ),
     A128KW,
     A192KW,
     A256KW,
     DirectAlgModel(),  # dir, Recommended
     ECDHESAlgModel(None),  # ECDH-ES, Recommended+
-    ECDHESAlgModel(128, True),  # ECDH-ES+A128KW, Recommended
-    ECDHESAlgModel(192),  # ECDH-ES+A192KW
-    ECDHESAlgModel(256, True),  # ECDH-ES+A256KW, Recommended
+    ECDHESAlgModel(A128KW),  # ECDH-ES+A128KW, Recommended
+    ECDHESAlgModel(A192KW),  # ECDH-ES+A192KW
+    ECDHESAlgModel(A256KW),  # ECDH-ES+A256KW, Recommended
     AESGCMAlgModel(128),  # A128GCMKW
     AESGCMAlgModel(192),  # A192GCMKW
     AESGCMAlgModel(256),  # A256GCMKW
-    PBES2HSAlgModel(256, 128),  # PBES2-HS256+A128KW
-    PBES2HSAlgModel(384, 192),  # PBES2-HS384+A192KW
-    PBES2HSAlgModel(512, 256),  # PBES2-HS512+A256KW
+    PBES2HSAlgModel(256, A128KW),  # PBES2-HS256+A128KW
+    PBES2HSAlgModel(384, A192KW),  # PBES2-HS384+A192KW
+    PBES2HSAlgModel(512, A256KW),  # PBES2-HS512+A256KW
 ]
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.2.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,125 +10,97 @@
 import hmac
 import hashlib
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import GCM, CBC
 from cryptography.hazmat.primitives.padding import PKCS7
-from cryptography.exceptions import InvalidTag
 from ..rfc7516.models import JWEEncModel
-from ..rfc7516.types import EncryptionData
 from .util import encode_int
 
 
 class CBCHS2EncModel(JWEEncModel):
     # The IV used is a 128-bit value generated randomly or
     # pseudo-randomly for use in the cipher.
-    IV_SIZE = 128
+    iv_size = 128
 
     def __init__(self, key_size: int, hash_type: int):
-        self.name = f'A{key_size}CBC-HS{hash_type}'
-        self.description = f'AES_{key_size}_CBC_HMAC_SHA_{hash_type} authenticated encryption algorithm'
+        self.name = f"A{key_size}CBC-HS{hash_type}"
+        self.description = (
+            f"AES_{key_size}_CBC_HMAC_SHA_{hash_type} authenticated encryption algorithm"
+        )
 
-        # bit length
+        # key size in bit
         self.key_size = key_size
-        # byte length
+        # key size in byte
         self.key_len = key_size // 8
 
         self.cek_size = key_size * 2
-        self.hash_alg = getattr(hashlib, f'sha{hash_type}')
+        self.hash_alg = getattr(hashlib, f"sha{hash_type}")
 
     def _hmac(self, ciphertext: bytes, aad: bytes, iv: bytes, key: bytes) -> bytes:
         al = encode_int(len(aad) * 8, 64)
         msg = aad + iv + ciphertext + al
         d = hmac.new(key, msg, self.hash_alg).digest()
-        return d[:self.key_len]
+        return d[: self.key_len]
 
-    def encrypt(self,obj: EncryptionData) -> bytes:
-        """Key Encryption with AES_CBC_HMAC_SHA2.
-
-        :param obj: encryption data instance
-        """
-        iv = self.check_iv(obj)
-        hkey = obj.cek[:self.key_len]
-        ekey = obj.cek[self.key_len:]
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+        """Key Encryption with AES_CBC_HMAC_SHA2."""
+        hkey = cek[: self.key_len]
+        ekey = cek[self.key_len :]
 
         pad = PKCS7(AES.block_size).padder()
-        padded_data = pad.update(obj.plaintext) + pad.finalize()
+        padded_data = pad.update(plaintext) + pad.finalize()
 
         cipher = Cipher(AES(ekey), CBC(iv), backend=default_backend())
         enc = cipher.encryptor()
         ciphertext = enc.update(padded_data) + enc.finalize()
-        aad = obj.encoded['aad']
         tag = self._hmac(ciphertext, aad, iv, hkey)
-        obj.decoded['tag'] = tag
-        return ciphertext
-
-    def decrypt(self, obj: EncryptionData) -> bytes:
-        """Key Decryption with AES AES_CBC_HMAC_SHA2.
+        return ciphertext, tag
 
-        :param obj: encryption data instance
-        :return: payload in bytes
-        """
-        iv = self.check_iv(obj)
-        hkey = obj.cek[:self.key_len]
-        dkey = obj.cek[self.key_len:]
+    def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
+        """Key Decryption with AES AES_CBC_HMAC_SHA2."""
+        hkey = cek[: self.key_len]
+        dkey = cek[self.key_len :]
 
-        ciphertext = obj.decoded['ciphertext']
-        aad = obj.encoded['aad']
         ctag = self._hmac(ciphertext, aad, iv, hkey)
-        otag = obj.decoded['tag']
-        if not hmac.compare_digest(ctag, otag):
-            raise InvalidTag()
+        if not hmac.compare_digest(ctag, tag):
+            raise ValueError("tag does not match")
 
         cipher = Cipher(AES(dkey), CBC(iv), backend=default_backend())
         d = cipher.decryptor()
         data = d.update(ciphertext) + d.finalize()
         unpad = PKCS7(AES.block_size).unpadder()
         return unpad.update(data) + unpad.finalize()
 
 
 class GCMEncModel(JWEEncModel):
     # Use of an IV of size 96 bits is REQUIRED with this algorithm.
     # https://tools.ietf.org/html/rfc7518#section-5.3
-    IV_SIZE = 96
+    iv_size = 96
 
     def __init__(self, key_size: int):
-        self.name = f'A{key_size}GCM'
-        self.description = f'AES GCM using {key_size}-bit key'
+        self.name = f"A{key_size}GCM"
+        self.description = f"AES GCM using {key_size}-bit key"
         self.key_size = key_size
         self.cek_size = key_size
 
-    def encrypt(self, obj: EncryptionData) -> bytes:
-        """Key Encryption with AES GCM
-
-        :param obj: encryption data instance
-        """
-        iv = self.check_iv(obj)
-        cipher = Cipher(AES(obj.cek), GCM(iv), backend=default_backend())
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+        """Key Encryption with AES GCM"""
+        cipher = Cipher(AES(cek), GCM(iv), backend=default_backend())
         enc = cipher.encryptor()
-        aad = obj.encoded['aad']
         enc.authenticate_additional_data(aad)
-        ciphertext = enc.update(obj.plaintext) + enc.finalize()
-        obj.decoded['tag'] = enc.tag
-        return ciphertext
-
-    def decrypt(self, obj: EncryptionData) -> bytes:
-        """Key Decryption with AES GCM
-
-        :param obj: encryption data instance
-        :return: payload in bytes
-        """
-        iv = self.check_iv(obj)
-        tag = obj.decoded['tag']
-        cipher = Cipher(AES(obj.cek), GCM(iv, tag), backend=default_backend())
+        ciphertext = enc.update(plaintext) + enc.finalize()
+        return ciphertext, enc.tag
+
+    def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
+        """Key Decryption with AES GCM"""
+        cipher = Cipher(AES(cek), GCM(iv, tag), backend=default_backend())
         d = cipher.decryptor()
-        aad = obj.encoded['aad']
         d.authenticate_additional_data(aad)
-        ciphertext = obj.decoded['ciphertext']
         return d.update(ciphertext) + d.finalize()
 
 
 JWE_ENC_MODELS = [
     CBCHS2EncModel(128, 256),  # A128CBC-HS256
     CBCHS2EncModel(192, 384),  # A192CBC-HS384
     CBCHS2EncModel(256, 512),  # A256CBC-HS512
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.2.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import zlib
 from ..rfc7516.models import JWEZipModel
 
 
 class DeflateZipModel(JWEZipModel):
-    name = 'DEF'
-    description = 'DEFLATE'
+    name = "DEF"
+    description = "DEFLATE"
 
     def compress(self, s: bytes) -> bytes:
         """Compress bytes data with DEFLATE algorithm."""
         data = zlib.compress(s)
         # drop gzip headers and tail
         return data[2:-4]
 
     def decompress(self, s: bytes) -> bytes:
         """Decompress DEFLATE bytes data."""
         return zlib.decompress(s, -zlib.MAX_WBITS)
 
 
-JWE_ZIP_MODELS = [
-    DeflateZipModel()
-]
+JWE_ZIP_MODELS = [DeflateZipModel()]
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.2.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,123 +9,126 @@
     .. _`Section 3`: https://tools.ietf.org/html/rfc7518#section-3
 """
 
 import hmac
 import hashlib
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric.utils import (
-    decode_dss_signature, encode_dss_signature
+    decode_dss_signature,
+    encode_dss_signature,
 )
 from cryptography.hazmat.primitives.asymmetric.ec import ECDSA
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.exceptions import InvalidSignature
 from ..rfc7515.model import JWSAlgModel
 from .oct_key import OctKey
 from .rsa_key import RSAKey
 from .ec_key import ECKey
 from .util import encode_int, decode_int
 
 
 class NoneAlgModel(JWSAlgModel):
-    name = 'none'
-    description = 'No digital signature or MAC performed'
+    name = "none"
+    description = "No digital signature or MAC performed"
 
     def sign(self, msg, key):
-        return b''
+        return b""
 
     def verify(self, msg, sig, key):
         return False
 
 
 class HMACAlgModel(JWSAlgModel):
     """HMAC using SHA algorithms for JWS. Available algorithms:
 
     - HS256: HMAC using SHA-256
     - HS384: HMAC using SHA-384
     - HS512: HMAC using SHA-512
     """
+
     SHA256 = hashlib.sha256
     SHA384 = hashlib.sha384
     SHA512 = hashlib.sha512
 
-    def __init__(self, sha_type: int, recommended: bool=False):
-        self.name = f'HS{sha_type}'
-        self.description = f'HMAC using SHA-{sha_type}'
+    def __init__(self, sha_type: int, recommended: bool = False):
+        self.name = f"HS{sha_type}"
+        self.description = f"HMAC using SHA-{sha_type}"
         self.recommended = recommended
-        self.hash_alg = getattr(self, f'SHA{sha_type}')
+        self.hash_alg = getattr(self, f"SHA{sha_type}")
 
     def sign(self, msg: bytes, key: OctKey) -> bytes:
         # it is faster than the one in cryptography
-        op_key = key.get_op_key('sign')
+        op_key = key.get_op_key("sign")
         return hmac.new(op_key, msg, self.hash_alg).digest()
 
     def verify(self, msg: bytes, sig: bytes, key: OctKey) -> bool:
-        op_key = key.get_op_key('verify')
+        op_key = key.get_op_key("verify")
         v_sig = hmac.new(op_key, msg, self.hash_alg).digest()
         return hmac.compare_digest(sig, v_sig)
 
 
 class RSAAlgModel(JWSAlgModel):
     """RSA using SHA algorithms for JWS. Available algorithms:
 
     - RS256: RSASSA-PKCS1-v1_5 using SHA-256
     - RS384: RSASSA-PKCS1-v1_5 using SHA-384
     - RS512: RSASSA-PKCS1-v1_5 using SHA-512
     """
+
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
-    def __init__(self, sha_type: int, recommended: bool=False):
-        self.name = f'RS{sha_type}'
-        self.description = f'RSASSA-PKCS1-v1_5 using SHA-{sha_type}'
+    def __init__(self, sha_type: int, recommended: bool = False):
+        self.name = f"RS{sha_type}"
+        self.description = f"RSASSA-PKCS1-v1_5 using SHA-{sha_type}"
         self.recommended = recommended
-        self.hash_alg = getattr(self, f'SHA{sha_type}')
+        self.hash_alg = getattr(self, f"SHA{sha_type}")
         self.padding = padding.PKCS1v15()
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
-        op_key = key.get_op_key('sign')
+        op_key = key.get_op_key("sign")
         return op_key.sign(msg, self.padding, self.hash_alg())
 
     def verify(self, msg: bytes, sig: bytes, key: RSAKey) -> bool:
-        op_key = key.get_op_key('verify')
+        op_key = key.get_op_key("verify")
         try:
             op_key.verify(sig, msg, self.padding, self.hash_alg())
             return True
         except InvalidSignature:
             return False
 
 
 class ECAlgModel(JWSAlgModel):
     """ECDSA using SHA algorithms for JWS. Available algorithms:
 
     - ES256: ECDSA using P-256 and SHA-256
     - ES384: ECDSA using P-384 and SHA-384
     - ES512: ECDSA using P-521 and SHA-512
     """
+
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
-    def __init__(self, name: str, curve: str, sha_type: int, recommended: bool=False):
+    def __init__(self, name: str, curve: str, sha_type: int, recommended: bool = False):
         self.name = name
         self.curve = curve
-        self.description = f'ECDSA using {self.curve} and SHA-{sha_type}'
+        self.description = f"ECDSA using {self.curve} and SHA-{sha_type}"
         self.recommended = recommended
-        self.hash_alg = getattr(self, f'SHA{sha_type}')
+        self.hash_alg = getattr(self, f"SHA{sha_type}")
 
     def _check_key(self, key: ECKey):
         if key.curve_name != self.curve:
-            raise ValueError(
-                f'Key for "{self.name}" not supported, only "{self.curve}" allowed')
+            raise ValueError(f'Key for "{self.name}" not supported, only "{self.curve}" allowed')
         return key
 
     def sign(self, msg: bytes, key: ECKey) -> bytes:
         self._check_key(key)
-        op_key = key.get_op_key('sign')
+        op_key = key.get_op_key("sign")
         der_sig = op_key.sign(msg, ECDSA(self.hash_alg()))
         r, s = decode_dss_signature(der_sig)
         size = key.curve_key_size
         return encode_int(r, size) + encode_int(s, size)
 
     def verify(self, msg: bytes, sig: bytes, key: ECKey) -> bool:
         self._check_key(key)
@@ -136,51 +139,46 @@
             return False
 
         r = decode_int(sig[:length])
         s = decode_int(sig[length:])
         der_sig = encode_dss_signature(r, s)
 
         try:
-            op_key = key.get_op_key('verify')
+            op_key = key.get_op_key("verify")
             op_key.verify(der_sig, msg, ECDSA(self.hash_alg()))
             return True
         except InvalidSignature:
             return False
 
 
 class RSAPSSAlgModel(JWSAlgModel):
     """RSASSA-PSS using SHA algorithms for JWS. Available algorithms:
 
     - PS256: RSASSA-PSS using SHA-256 and MGF1 with SHA-256
     - PS384: RSASSA-PSS using SHA-384 and MGF1 with SHA-384
     - PS512: RSASSA-PSS using SHA-512 and MGF1 with SHA-512
     """
+
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
     def __init__(self, sha_type: int):
-        self.name = f'PS{sha_type}'
-        self.description = f'RSASSA-PSS using SHA-{sha_type} and MGF1 with SHA-{sha_type}'
-        self.hash_alg = getattr(self, f'SHA{sha_type}')
+        self.name = f"PS{sha_type}"
+        self.description = f"RSASSA-PSS using SHA-{sha_type} and MGF1 with SHA-{sha_type}"
+        self.hash_alg = getattr(self, f"SHA{sha_type}")
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
-        op_key = key.get_op_key('sign')
-        pad = padding.PSS(
-            mgf=padding.MGF1(self.hash_alg()),
-            salt_length=self.hash_alg.digest_size
-        )
+        op_key = key.get_op_key("sign")
+        pad = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
         return op_key.sign(msg, pad, self.hash_alg())
 
     def verify(self, msg: bytes, sig: bytes, key: RSAKey) -> bool:
-        op_key = key.get_op_key('verify')
-        pad = padding.PSS(
-            mgf=padding.MGF1(self.hash_alg()),
-            salt_length=self.hash_alg.digest_size
-        )
+        op_key = key.get_op_key("verify")
+        pad = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
         try:
             op_key.verify(sig, msg, pad, self.hash_alg())
             return True
         except InvalidSignature:
             return False
 
 
@@ -188,14 +186,14 @@
     NoneAlgModel(),  # none
     HMACAlgModel(256, True),  # HS256
     HMACAlgModel(384),  # HS384
     HMACAlgModel(512),  # HS512
     RSAAlgModel(256, True),  # RS256
     RSAAlgModel(384),  # RS384
     RSAAlgModel(512),  # RS512
-    ECAlgModel('ES256', 'P-256', 256, True),
-    ECAlgModel('ES384', 'P-384', 384),
-    ECAlgModel('ES512', 'P-521', 512),
+    ECAlgModel("ES256", "P-256", 256, True),
+    ECAlgModel("ES384", "P-384", 384),
+    ECAlgModel("ES512", "P-521", 512),
     RSAPSSAlgModel(256),  # PS256
     RSAPSSAlgModel(384),  # PS384
     RSAPSSAlgModel(512),  # PS512
 ]
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.2.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 import random
 import string
 from ..util import (
     to_bytes,
     urlsafe_b64decode,
     urlsafe_b64encode,
 )
-from ..registry import KeyParameter, is_str
+from ..registry import KeyParameter
 from ..rfc7517.models import SymmetricKey, NativeKeyBinding
 from ..rfc7517.types import KeyOptions, KeyDict
 
 
 POSSIBLE_UNSAFE_KEYS = (
-    b'-----BEGIN ',
-    b'ssh-rsa ',
-    b'ssh-ed25519 ',
-    b'ecdsa-sha2-',
+    b"-----BEGIN ",
+    b"ssh-rsa ",
+    b"ssh-ed25519 ",
+    b"ecdsa-sha2-",
 )
 
 
 class OctBinding(NativeKeyBinding):
     @classmethod
     def convert_raw_key_to_dict(cls, value: bytes, private: bool) -> KeyDict:
-        k = urlsafe_b64encode(value).decode('utf-8')
-        return {'k': k}
+        k = urlsafe_b64encode(value).decode("utf-8")
+        return {"k": k}
 
     @classmethod
     def import_from_dict(cls, value: KeyDict):
-        return urlsafe_b64decode(to_bytes(value['k']))
+        return urlsafe_b64decode(to_bytes(value["k"]))
 
     @classmethod
     def import_from_bytes(cls, value: bytes):
         # security check
         if value.startswith(POSSIBLE_UNSAFE_KEYS):
-            raise ValueError('This key may not be safe to import')
+            raise ValueError("This key may not be safe to import")
         return value
 
 
-class OctKey(SymmetricKey):
-    key_type: str = 'oct'
+class OctKey(SymmetricKey[bytes, bytes]):
+    key_type: str = "oct"
     binding = OctBinding
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.4
-    value_registry = {
-        'k': KeyParameter('Key Value', True, True, is_str)
-    }
+    value_registry = {"k": KeyParameter("Key Value", "str", True, True)}
 
     @classmethod
-    def generate_key(cls, key_size=256, options: KeyOptions=None, private: bool=True):
+    def generate_key(cls, key_size=256, options: KeyOptions = None, private: bool = True) -> "OctKey":
         """Generate a ``OctKey`` with the given bit size."""
         if not private:
-            raise ValueError('oct key can not be generated as public')
+            raise ValueError("oct key can not be generated as public")
 
         if key_size % 8 != 0:
-            raise ValueError('Invalid bit size for oct key')
+            raise ValueError("Invalid bit size for oct key")
 
         length = key_size // 8
         rand = random.SystemRandom()
         chars = string.ascii_letters + string.digits
-        value = ''.join(rand.choice(chars) for _ in range(length))
+        value = "".join(rand.choice(chars) for _ in range(length))
         raw_key = to_bytes(value)
         return cls(raw_key, raw_key, options)
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.2.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,154 +1,145 @@
-from typing import Optional, Union, Dict
+from typing import Optional, Dict
 from functools import cached_property
-from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives.asymmetric.rsa import (
-    RSAPublicKey, RSAPrivateKeyWithSerialization,
-    RSAPrivateNumbers, RSAPublicNumbers,
-    rsa_recover_prime_factors, rsa_crt_dmp1, rsa_crt_dmq1, rsa_crt_iqmp
+    generate_private_key,
+    RSAPublicKey,
+    RSAPrivateKey,
+    RSAPrivateNumbers,
+    RSAPublicNumbers,
+    rsa_recover_prime_factors,
+    rsa_crt_dmp1,
+    rsa_crt_dmq1,
+    rsa_crt_iqmp,
 )
 from cryptography.hazmat.backends import default_backend
-from ..registry import KeyParameter, is_str, not_support
+from ..registry import KeyParameter
 from ..rfc7517.models import AsymmetricKey
 from ..rfc7517.pem import CryptographyBinding
 from ..rfc7517.types import KeyDict, KeyOptions
 from ..util import int_to_base64, base64_to_int
 
-NativeRSAKey = Union[RSAPublicKey, RSAPrivateKeyWithSerialization]
-
 
 class RSABinding(CryptographyBinding):
-    ssh_type = b'ssh-rsa'
+    ssh_type = b"ssh-rsa"
 
     @staticmethod
-    def import_private_key(obj: KeyDict) -> RSAPrivateKeyWithSerialization:
-        if 'oth' in obj:  # pragma: no cover
+    def import_private_key(obj: KeyDict) -> RSAPrivateKey:
+        if "oth" in obj:  # pragma: no cover
             # https://tools.ietf.org/html/rfc7518#section-6.3.2.7
             raise ValueError('"oth" is not supported yet')
 
-        public_numbers = RSAPublicNumbers(
-            base64_to_int(obj['e']), base64_to_int(obj['n']))
+        public_numbers = RSAPublicNumbers(base64_to_int(obj["e"]), base64_to_int(obj["n"]))
 
         if has_all_prime_factors(obj):
             numbers = RSAPrivateNumbers(
-                d=base64_to_int(obj['d']),
-                p=base64_to_int(obj['p']),
-                q=base64_to_int(obj['q']),
-                dmp1=base64_to_int(obj['dp']),
-                dmq1=base64_to_int(obj['dq']),
-                iqmp=base64_to_int(obj['qi']),
-                public_numbers=public_numbers)
+                d=base64_to_int(obj["d"]),
+                p=base64_to_int(obj["p"]),
+                q=base64_to_int(obj["q"]),
+                dmp1=base64_to_int(obj["dp"]),
+                dmq1=base64_to_int(obj["dq"]),
+                iqmp=base64_to_int(obj["qi"]),
+                public_numbers=public_numbers,
+            )
         else:
-            d = base64_to_int(obj['d'])
-            p, q = rsa_recover_prime_factors(
-                public_numbers.n, d, public_numbers.e)
+            d = base64_to_int(obj["d"])
+            p, q = rsa_recover_prime_factors(public_numbers.n, d, public_numbers.e)
             numbers = RSAPrivateNumbers(
                 d=d,
                 p=p,
                 q=q,
                 dmp1=rsa_crt_dmp1(d, p),
                 dmq1=rsa_crt_dmq1(d, q),
                 iqmp=rsa_crt_iqmp(p, q),
-                public_numbers=public_numbers)
+                public_numbers=public_numbers,
+            )
 
         return numbers.private_key(default_backend())
 
     @staticmethod
-    def export_private_key(key: RSAPrivateKeyWithSerialization) -> Dict[str, str]:
+    def export_private_key(key: RSAPrivateKey) -> Dict[str, str]:
         numbers = key.private_numbers()
         return {
-            'n': int_to_base64(numbers.public_numbers.n),
-            'e': int_to_base64(numbers.public_numbers.e),
-            'd': int_to_base64(numbers.d),
-            'p': int_to_base64(numbers.p),
-            'q': int_to_base64(numbers.q),
-            'dp': int_to_base64(numbers.dmp1),
-            'dq': int_to_base64(numbers.dmq1),
-            'qi': int_to_base64(numbers.iqmp)
+            "n": int_to_base64(numbers.public_numbers.n),
+            "e": int_to_base64(numbers.public_numbers.e),
+            "d": int_to_base64(numbers.d),
+            "p": int_to_base64(numbers.p),
+            "q": int_to_base64(numbers.q),
+            "dp": int_to_base64(numbers.dmp1),
+            "dq": int_to_base64(numbers.dmq1),
+            "qi": int_to_base64(numbers.iqmp),
         }
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> RSAPublicKey:
-        numbers = RSAPublicNumbers(
-            base64_to_int(obj['e']),
-            base64_to_int(obj['n'])
-        )
+        numbers = RSAPublicNumbers(base64_to_int(obj["e"]), base64_to_int(obj["n"]))
         return numbers.public_key(default_backend())
 
     @staticmethod
     def export_public_key(key: RSAPublicKey) -> Dict[str, str]:
         numbers = key.public_numbers()
-        return {
-            'n': int_to_base64(numbers.n),
-            'e': int_to_base64(numbers.e)
-        }
+        return {"n": int_to_base64(numbers.n), "e": int_to_base64(numbers.e)}
 
 
-class RSAKey(AsymmetricKey):
-    key_type: str = 'RSA'
+class RSAKey(AsymmetricKey[RSAPublicKey, RSAPrivateKey]):
+    key_type: str = "RSA"
     #: Registry definition for RSA Key
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.3
     value_registry = {
-        'n': KeyParameter('Modulus', True, False, is_str),
-        'e': KeyParameter('Exponent', True, False, is_str),
-        'd': KeyParameter('Private Exponent', False, True, is_str),
-        'p': KeyParameter('First Prime Factor', False, True, is_str),
-        'q': KeyParameter('Second Prime Factor', False, True, is_str),
-        'dp': KeyParameter('First Factor CRT Exponent', False, True, is_str),
-        'dq': KeyParameter('Second Factor CRT Exponent', False, True, is_str),
-        'qi': KeyParameter('First CRT Coefficient', False, True, is_str),
-        'oth': KeyParameter('Other Primes Info', False, True, not_support),
+        "n": KeyParameter("Modulus", "str", private=False, required=True),
+        "e": KeyParameter("Exponent", "str", private=False, required=True),
+        "d": KeyParameter("Private Exponent", "str", private=True, required=False),
+        "p": KeyParameter("First Prime Factor", "str", private=True, required=False),
+        "q": KeyParameter("Second Prime Factor", "str", private=True, required=False),
+        "dp": KeyParameter("First Factor CRT Exponent", "str", private=True, required=False),
+        "dq": KeyParameter("Second Factor CRT Exponent", "str", private=True, required=False),
+        "qi": KeyParameter("First CRT Coefficient", "str", private=True, required=False),
+        "oth": KeyParameter("Other Primes Info", "none", private=True, required=False),
     }
     binding = RSABinding
 
     @property
-    def raw_value(self) -> NativeRSAKey:
-        return self._raw_value
-
-    @property
     def is_private(self) -> bool:
-        return isinstance(self.raw_value, RSAPrivateKeyWithSerialization)
+        return isinstance(self.raw_value, RSAPrivateKey)
 
     @cached_property
     def public_key(self) -> RSAPublicKey:
-        if isinstance(self.raw_value, RSAPrivateKeyWithSerialization):
+        if isinstance(self.raw_value, RSAPrivateKey):
             return self.raw_value.public_key()
         return self.raw_value
 
     @property
-    def private_key(self) -> Optional[RSAPrivateKeyWithSerialization]:
+    def private_key(self) -> Optional[RSAPrivateKey]:
         if self.is_private:
             return self.raw_value
         return None
 
     @classmethod
     def generate_key(
             cls,
-            key_size: int=2048,
-            options: KeyOptions=None,
-            private: bool=True) -> 'RSAKey':
+            key_size: int = 2048,
+            options: KeyOptions = None,
+            private: bool = True) -> "RSAKey":
         if key_size < 512:
-            raise ValueError('key_size must not be less than 512')
+            raise ValueError("key_size must not be less than 512")
         if key_size % 8 != 0:
-            raise ValueError('Invalid key_size for RSAKey')
-        raw_key = rsa.generate_private_key(
+            raise ValueError("Invalid key_size for RSAKey")
+        raw_key = generate_private_key(
             public_exponent=65537,
             key_size=key_size,
             backend=default_backend(),
         )
         if not private:
             raw_key = raw_key.public_key()
         return cls(raw_key, raw_key, options)
 
 
 def has_all_prime_factors(obj) -> bool:
-    props = ['p', 'q', 'dp', 'dq', 'qi']
+    props = ["p", "q", "dp", "dq", "qi"]
     props_found = [prop in obj for prop in props]
     if all(props_found):
         return True
 
     if any(props_found):
-        raise ValueError(
-            'RSA key must include all parameters '
-            'if any are present besides d')
+        raise ValueError("RSA key must include all parameters " "if any are present besides d")
 
     return False
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.2.0/src/joserfc/rfc7519/claims.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 import datetime
 import calendar
 from typing import Dict, Any
 from ..util import to_bytes, json_dumps
 from ..errors import InsecureClaimError
 
 
-SENSITIVE_NAMES = ('password', 'token', 'secret', 'secret_key', 'api_key')
-SENSITIVE_VALUES = re.compile(r'|'.join([
-    # http://www.richardsramblings.com/regex/credit-card-numbers/
-    r'\b(?:3[47]\d|(?:4\d|5[1-5]|65)\d{2}|6011)\d{12}\b',
-    # various private keys
-    r'-----BEGIN[A-Z ]+PRIVATE KEY-----.+-----END[A-Z ]+PRIVATE KEY-----',
-    # social security numbers (US)
-    r'^\b(?!(000|666|9))\d{3}-(?!00)\d{2}-(?!0000)\d{4}\b',
-]), re.DOTALL)
+SENSITIVE_NAMES = ("password", "token", "secret", "secret_key", "api_key")
+SENSITIVE_VALUES = re.compile(
+    r"|".join([
+        # http://www.richardsramblings.com/regex/credit-card-numbers/
+        r"\b(?:3[47]\d|(?:4\d|5[1-5]|65)\d{2}|6011)\d{12}\b",
+        # various private keys
+        r"-----BEGIN[A-Z ]+PRIVATE KEY-----.+-----END[A-Z ]+PRIVATE KEY-----",
+        # social security numbers (US)
+        r"^\b(?!(000|666|9))\d{3}-(?!00)\d{2}-(?!0000)\d{4}\b",
+    ]),
+    re.DOTALL,
+)
 
 Claims = Dict[str, Any]
 
 
 def convert_claims(claims: Claims) -> bytes:
     """Turn claims into bytes payload."""
-    for k in ['exp', 'iat', 'nbf']:
+    for k in ["exp", "iat", "nbf"]:
         claim = claims.get(k)
         if isinstance(claim, datetime.datetime):
             claims[k] = calendar.timegm(claim.utctimetuple())
     return to_bytes(json_dumps(claims))
 
 
 def check_sensitive_data(claims: Claims):
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc7519/validators.py` & `joserfc-0.2.0/src/joserfc/rfc7519/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,129 +5,132 @@
     InvalidClaimError,
     ExpiredTokenError,
     InvalidTokenError,
 )
 
 
 #: http://openid.net/specs/openid-connect-core-1_0.html#IndividualClaimsRequests
-ClaimsOption = TypedDict('ClaimsOption', {
-    'essential': bool,
-    'value': Union[str, int],
-    'values': List[Union[str, int]],
-})
+ClaimsOption = TypedDict("ClaimsOption", {
+    "essential": bool,
+    "value": Union[str, int],
+    "values": List[Union[str, int]],
+}, total=False)
 
 
-class ClaimsRequests:
+class ClaimsRegistry:
     """Requesting "claims" for JWT with the given conditions."""
 
     def __init__(self, **kwargs: ClaimsOption):
         self.options = kwargs
+        self.essential_keys = {key for key in kwargs if kwargs[key].get("essential")}
 
     def check_value(self, claim_name: str, value: Any):
         option: ClaimsOption = self.options.get(claim_name)
-        option_value = option.get('value')
-        if option_value and value != option_value:
-            raise InvalidClaimError(claim_name)
-
-        option_values = option.get('values')
-        if option_values and value not in option_values:
-            raise InvalidClaimError(claim_name)
+        if option:
+            option_value = option.get("value")
+            if option_value and value != option_value:
+                raise InvalidClaimError(claim_name)
+
+            option_values = option.get("values")
+            if option_values and value not in option_values:
+                raise InvalidClaimError(claim_name)
 
     def validate(self, claims: Dict[str, Any]):
-        for key in self.options:
-            option: ClaimsOption = self.options[key]
-            if key not in claims:
-                # validate essential claims
-                if option.get('essential'):
-                    raise MissingClaimError(key)
-            else:
-                value = claims[key]
-                func = getattr(self, 'validate_' + key, None)
-                if func:
-                    func(value)
-                else:
-                    self.check_value(key, value)
+        missed_key = self.essential_keys - set(claims.keys())
+        if missed_key:
+            raise MissingClaimError(",".join(missed_key))
+
+        for key in claims:
+            value = claims[key]
+            func = getattr(self, "validate_" + key, None)
+            if func:
+                func(value)
+            elif key in self.options:
+                self.check_value(key, value)
 
 
-class JWTClaimsRequests(ClaimsRequests):
-    def __init__(self, now: Optional[int]=None, leeway=0, **kwargs: ClaimsOption):
+class JWTClaimsRegistry(ClaimsRegistry):
+    def __init__(self, now: Optional[int] = None, leeway=0, **kwargs: ClaimsOption):
         if now is None:
             now = int(time.time())
         self.now = now
         self.leeway = leeway
         super().__init__(**kwargs)
 
     def validate_aud(self, value):
         """The "aud" (audience) claim identifies the recipients that the JWT is
         intended for.  Each principal intended to process the JWT MUST
         identify itself with a value in the audience claim.  If the principal
         processing the claim does not identify itself with a value in the
         "aud" claim when this claim is present, then the JWT MUST be
-        rejected.  In the general case, the "aud" value is an array of case-
-        sensitive strings, each containing a StringOrURI value.  In the
+        rejected.  In the general case, the "aud" value is an array of
+        case-sensitive strings, each containing a StringOrURI value.  In the
         special case when the JWT has one audience, the "aud" value MAY be a
         single case-sensitive string containing a StringOrURI value.  The
         interpretation of audience values is generally application specific.
         Use of this claim is OPTIONAL.
         """
-        option: ClaimsOption = self.options['aud']
-        option_values = option.get('values')
+        option: ClaimsOption = self.options.get("aud")
+        if not option:
+            return
+
+        option_values = option.get("values")
 
         if not option_values:
-            option_value = option.get('value')
+            option_value = option.get("value")
             if option_value:
                 option_values = option_value
 
         if not option_values:
             return
 
         if isinstance(value, list):
             aud_list = value
         else:
             aud_list = [value]
 
         if not any([v in aud_list for v in option_values]):
-            raise InvalidClaimError('aud')
+            raise InvalidClaimError("aud")
 
     def validate_exp(self, value: int):
         """The "exp" (expiration time) claim identifies the expiration time on
         or after which the JWT MUST NOT be accepted for processing.  The
         processing of the "exp" claim requires that the current date/time
         MUST be before the expiration date/time listed in the "exp" claim.
         Implementers MAY provide for some small leeway, usually no more than
         a few minutes, to account for clock skew.  Its value MUST be a number
         containing a NumericDate value.  Use of this claim is OPTIONAL.
         """
         if not _validate_numeric_time(value):
-            raise InvalidClaimError('exp')
+            raise InvalidClaimError("exp")
         if value < (self.now - self.leeway):
             raise ExpiredTokenError()
-        self.check_value('exp', value)
+        self.check_value("exp", value)
 
     def validate_nbf(self, value: int):
         """The "nbf" (not before) claim identifies the time before which the JWT
         MUST NOT be accepted for processing.  The processing of the "nbf"
         claim requires that the current date/time MUST be after or equal to
         the not-before date/time listed in the "nbf" claim.  Implementers MAY
         provide for some small leeway, usually no more than a few minutes, to
         account for clock skew.  Its value MUST be a number containing a
         NumericDate value.  Use of this claim is OPTIONAL.
         """
         if not _validate_numeric_time(value):
-            raise InvalidClaimError('nbf')
+            raise InvalidClaimError("nbf")
         if value > (self.now + self.leeway):
             raise InvalidTokenError()
-        self.check_value('nbf', value)
+        self.check_value("nbf", value)
 
     def validate_iat(self, value: int):
         """The "iat" (issued at) claim identifies the time at which the JWT was
         issued.  This claim can be used to determine the age of the JWT.  Its
         value MUST be a number containing a NumericDate value.  Use of this
         claim is OPTIONAL.
         """
         if not _validate_numeric_time(value):
-            raise InvalidClaimError('iat')
-        self.check_value('iat', value)
+            raise InvalidClaimError("iat")
+        self.check_value("iat", value)
 
 
 def _validate_numeric_time(s):
     return isinstance(s, (int, float))
```

### Comparing `joserfc-0.1.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.2.0/src/joserfc/rfc8037/okp_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,97 @@
 from typing import Optional, Union, Dict
 from functools import cached_property
-from cryptography.hazmat.primitives.asymmetric.ed25519 import (
-    Ed25519PublicKey, Ed25519PrivateKey
-)
-from cryptography.hazmat.primitives.asymmetric.ed448 import (
-    Ed448PublicKey, Ed448PrivateKey
-)
-from cryptography.hazmat.primitives.asymmetric.x25519 import (
-    X25519PublicKey, X25519PrivateKey
-)
-from cryptography.hazmat.primitives.asymmetric.x448 import (
-    X448PublicKey, X448PrivateKey
-)
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey, Ed25519PrivateKey
+from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PublicKey, Ed448PrivateKey
+from cryptography.hazmat.primitives.asymmetric.x25519 import X25519PublicKey, X25519PrivateKey
+from cryptography.hazmat.primitives.asymmetric.x448 import X448PublicKey, X448PrivateKey
 from cryptography.hazmat.primitives.serialization import (
-    Encoding, PublicFormat, PrivateFormat, NoEncryption
+    Encoding,
+    PublicFormat,
+    PrivateFormat,
+    NoEncryption,
 )
 from ..rfc7517.models import CurveKey
-from ..rfc7517.types import KeyDict, KeyAny, KeyOptions
+from ..rfc7517.types import KeyDict, KeyOptions
 from ..rfc7517.pem import CryptographyBinding
 from ..util import to_bytes, urlsafe_b64decode, urlsafe_b64encode
-from ..registry import KeyParameter, is_str
-
+from ..registry import KeyParameter
 
 PUBLIC_KEYS_MAP = {
-    'Ed25519': Ed25519PublicKey,
-    'Ed448': Ed448PublicKey,
-    'X25519': X25519PublicKey,
-    'X448': X448PublicKey,
+    "Ed25519": Ed25519PublicKey,
+    "Ed448": Ed448PublicKey,
+    "X25519": X25519PublicKey,
+    "X448": X448PublicKey,
 }
 PRIVATE_KEYS_MAP = {
-    'Ed25519': Ed25519PrivateKey,
-    'Ed448': Ed448PrivateKey,
-    'X25519': X25519PrivateKey,
-    'X448': X448PrivateKey,
+    "Ed25519": Ed25519PrivateKey,
+    "Ed448": Ed448PrivateKey,
+    "X25519": X25519PrivateKey,
+    "X448": X448PrivateKey,
 }
-
-PRIVATE_KEY_TYPES = tuple(PRIVATE_KEYS_MAP.values())
-
-PublicOKPKey = Union[
-    Ed25519PublicKey,
-    Ed448PublicKey,
-    X25519PublicKey,
-    X448PublicKey
-]
-
-PrivateOKPKey = Union[
-    Ed25519PrivateKey,
-    Ed448PrivateKey,
-    X25519PrivateKey,
-    X448PrivateKey,
-]
-
-NativeOKPKey = Union[PublicOKPKey, PrivateOKPKey]
-
-ExchangePublicKeys = (X25519PublicKey, X448PublicKey)
-ExchangePrivateKeys = (X25519PrivateKey, X448PrivateKey)
+PrivateKeyTypes = tuple(PRIVATE_KEYS_MAP.values())
+PublicOKPKey = Union[Ed25519PublicKey, Ed448PublicKey, X25519PublicKey, X448PublicKey]
+PrivateOKPKey = Union[Ed25519PrivateKey, Ed448PrivateKey, X25519PrivateKey, X448PrivateKey]
 
 
 class OKPBinding(CryptographyBinding):
-    ssh_type = b'ssh-ed25519'
+    ssh_type = b"ssh-ed25519"
 
     @staticmethod
     def import_private_key(obj: KeyDict) -> PrivateOKPKey:
-        crv_key = PRIVATE_KEYS_MAP[obj['crv']]
-        d_bytes = urlsafe_b64decode(to_bytes(obj['d']))
+        crv_key = PRIVATE_KEYS_MAP[obj["crv"]]
+        d_bytes = urlsafe_b64decode(to_bytes(obj["d"]))
         return crv_key.from_private_bytes(d_bytes)
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> PublicOKPKey:
-        crv_key = PUBLIC_KEYS_MAP[obj['crv']]
-        x_bytes = urlsafe_b64decode(to_bytes(obj['x']))
+        crv_key = PUBLIC_KEYS_MAP[obj["crv"]]
+        x_bytes = urlsafe_b64decode(to_bytes(obj["x"]))
         return crv_key.from_public_bytes(x_bytes)
 
     @staticmethod
     def export_private_key(key: PrivateOKPKey) -> Dict[str, str]:
         obj = OKPBinding.export_public_key(key.public_key())
-        d_bytes = key.private_bytes(
-            Encoding.Raw,
-            PrivateFormat.Raw,
-            NoEncryption()
-        )
-        obj['d'] = urlsafe_b64encode(d_bytes).decode('utf-8')
+        d_bytes = key.private_bytes(Encoding.Raw, PrivateFormat.Raw, NoEncryption())
+        obj["d"] = urlsafe_b64encode(d_bytes).decode("utf-8")
         return obj
 
     @staticmethod
     def export_public_key(key: PublicOKPKey) -> Dict[str, str]:
         x_bytes = key.public_bytes(Encoding.Raw, PublicFormat.Raw)
         return {
-            'crv': get_key_curve(key),
-            'x': urlsafe_b64encode(x_bytes).decode('utf-8'),
+            "crv": get_key_curve(key),
+            "x": urlsafe_b64encode(x_bytes).decode("utf-8"),
         }
 
 
-class OKPKey(CurveKey):
+class OKPKey(CurveKey[PublicOKPKey, PrivateOKPKey]):
     """Key class of the ``OKP`` key type."""
 
-    key_type: str = 'OKP'
+    key_type: str = "OKP"
     #: Registry definition for OKP Key
     #: https://www.rfc-editor.org/rfc/rfc8037#section-2
     value_registry = {
-        'crv': KeyParameter('Curve', True, False, is_str),
-        'x': KeyParameter('X Coordinate', True, False, is_str),
-        'd': KeyParameter('OKP Private Key', False, True, is_str),
+        "crv": KeyParameter("Curve", "str", private=False, required=True),
+        "x": KeyParameter("X Coordinate", "str", private=False, required=True),
+        "d": KeyParameter("OKP Private Key", "str", private=True, required=False),
     }
     binding = OKPBinding
-    required_fields = frozenset(['crv', 'x'])
-    private_only_fields = frozenset(['d'])
+    required_fields = frozenset(["crv", "x"])
+    private_only_fields = frozenset(["d"])
 
     def exchange_shared_key(self, pubkey: Union[X25519PublicKey, X448PublicKey]) -> bytes:
         # used in ECDHESAlgorithm
-        if self.private_key and isinstance(self.private_key, ExchangePrivateKeys):
+        if self.private_key and isinstance(self.private_key, (X25519PrivateKey, X448PrivateKey)):
             return self.private_key.exchange(pubkey)
-        raise ValueError('Invalid key for exchanging shared key')
-
-    @property
-    def raw_value(self) -> NativeOKPKey:
-        return self._raw_value
+        raise ValueError("Invalid key for exchanging shared key")
 
     @property
     def is_private(self) -> bool:
-        return isinstance(self.raw_value, PRIVATE_KEY_TYPES)
+        return isinstance(self.raw_value, PrivateKeyTypes)
 
     @cached_property
     def public_key(self) -> PublicOKPKey:
         if self.is_private:
             return self.raw_value.public_key()
         return self.raw_value
 
@@ -134,30 +102,32 @@
         return None
 
     @property
     def curve_name(self) -> str:
         return get_key_curve(self.raw_value)
 
     @classmethod
-    def generate_key(cls, crv: str='Ed25519',
-                     options: KeyOptions=None,
-                     private: bool=True) -> 'OKPKey':
+    def generate_key(
+            cls,
+            crv: str = "Ed25519",
+            options: KeyOptions = None,
+            private: bool = True) -> "OKPKey":
         if crv not in PRIVATE_KEYS_MAP:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
 
         private_key_cls = PRIVATE_KEYS_MAP[crv]
         raw_key = private_key_cls.generate()
         if not private:
             raw_key = raw_key.public_key()
         return cls(raw_key, raw_key, options=options)
 
 
-def get_key_curve(key: NativeOKPKey):
+def get_key_curve(key: Union[PublicOKPKey, PrivateOKPKey]):
     if isinstance(key, (Ed25519PublicKey, Ed25519PrivateKey)):
-        return 'Ed25519'
+        return "Ed25519"
     elif isinstance(key, (Ed448PublicKey, Ed448PrivateKey)):
-        return 'Ed448'
+        return "Ed448"
     elif isinstance(key, (X25519PublicKey, X25519PrivateKey)):
-        return 'X25519'
+        return "X25519"
     elif isinstance(key, (X448PublicKey, X448PrivateKey)):
-        return 'X448'
+        return "X448"
     raise ValueError("Invalid key")
```

### Comparing `joserfc-0.1.0/src/joserfc/util.py` & `joserfc-0.2.0/src/joserfc/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 import base64
 import string
 import struct
 import json
 import random
 
 
-def to_bytes(x, charset='utf-8', errors='strict'):
+def to_bytes(x, charset="utf-8", errors="strict"):
     if isinstance(x, bytes):
         return x
     if isinstance(x, str):
         return x.encode(charset, errors)
     if isinstance(x, (int, float)):
         return str(x).encode(charset, errors)
     return bytes(x)
 
 
+def to_unicode(x, charset="utf-8") -> str:
+    if isinstance(x, bytes):
+        return x.decode(charset)
+    return x
+
+
 def json_dumps(data: dict, ensure_ascii=False):
-    return json.dumps(data, ensure_ascii=ensure_ascii, separators=(',', ':'))
+    return json.dumps(data, ensure_ascii=ensure_ascii, separators=(",", ":"))
 
 
 def urlsafe_b64decode(s: bytes) -> bytes:
-    s += b'=' * (-len(s) % 4)
+    s += b"=" * (-len(s) % 4)
     return base64.urlsafe_b64decode(s)
 
 
 def urlsafe_b64encode(s: bytes) -> bytes:
-    return base64.urlsafe_b64encode(s).rstrip(b'=')
+    return base64.urlsafe_b64encode(s).rstrip(b"=")
 
 
 def base64_to_int(s: str) -> int:
     data = urlsafe_b64decode(to_bytes(s))
-    buf = struct.unpack('%sB' % len(data), data)
-    return int(''.join(["%02x" % byte for byte in buf]), 16)
+    buf = struct.unpack("%sB" % len(data), data)
+    return int("".join(["%02x" % byte for byte in buf]), 16)
 
 
 def int_to_base64(num: int) -> str:
     if num < 0:
-        raise ValueError('Must be a positive integer')
+        raise ValueError("Must be a positive integer")
 
-    s = num.to_bytes((num.bit_length() + 7) // 8, 'big', signed=False)
-    return urlsafe_b64encode(s).decode('utf-8', 'strict')
+    s = num.to_bytes((num.bit_length() + 7) // 8, "big", signed=False)
+    return urlsafe_b64encode(s).decode("utf-8", "strict")
 
 
-def json_b64encode(text, charset='utf-8') -> bytes:
+def json_b64encode(text, charset="utf-8") -> bytes:
     if isinstance(text, dict):
         text = json_dumps(text)
     return urlsafe_b64encode(to_bytes(text, charset))
 
 
-def json_b64decode(text, charset='utf-8') -> dict:
+def json_b64decode(text, charset="utf-8") -> dict:
     return json.loads(urlsafe_b64decode(to_bytes(text, charset)))
 
 
 def generate_token(length=30):
     rand = random.SystemRandom()
     chars = string.ascii_letters + string.digits
-    return ''.join(rand.choice(chars) for _ in range(length))
+    return "".join(rand.choice(chars) for _ in range(length))
```

### Comparing `joserfc-0.1.0/src/joserfc.egg-info/SOURCES.txt` & `joserfc-0.2.0/src/joserfc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 LICENSE
-README.md
+README.rst
 pyproject.toml
+setup.py
 src/joserfc/__init__.py
 src/joserfc/errors.py
 src/joserfc/jwe.py
 src/joserfc/jwk.py
 src/joserfc/jws.py
 src/joserfc/jwt.py
 src/joserfc/registry.py
 src/joserfc/util.py
 src/joserfc.egg-info/PKG-INFO
 src/joserfc.egg-info/SOURCES.txt
 src/joserfc.egg-info/dependency_links.txt
 src/joserfc.egg-info/requires.txt
 src/joserfc.egg-info/top_level.txt
+src/joserfc/drafts/__init__.py
+src/joserfc/drafts/jwe_chacha20.py
+src/joserfc/drafts/jwe_ecdh_1pu.py
 src/joserfc/rfc7515/__init__.py
 src/joserfc/rfc7515/compact.py
 src/joserfc/rfc7515/json.py
 src/joserfc/rfc7515/model.py
 src/joserfc/rfc7515/registry.py
 src/joserfc/rfc7515/types.py
 src/joserfc/rfc7516/__init__.py
 src/joserfc/rfc7516/compact.py
+src/joserfc/rfc7516/json.py
 src/joserfc/rfc7516/message.py
 src/joserfc/rfc7516/models.py
 src/joserfc/rfc7516/registry.py
 src/joserfc/rfc7516/types.py
 src/joserfc/rfc7517/__init__.py
 src/joserfc/rfc7517/keygen.py
 src/joserfc/rfc7517/keyset.py
 src/joserfc/rfc7517/models.py
 src/joserfc/rfc7517/pem.py
 src/joserfc/rfc7517/types.py
 src/joserfc/rfc7518/__init__.py
+src/joserfc/rfc7518/derive_key.py
 src/joserfc/rfc7518/ec_key.py
 src/joserfc/rfc7518/jwe_algs.py
 src/joserfc/rfc7518/jwe_encs.py
 src/joserfc/rfc7518/jwe_zips.py
 src/joserfc/rfc7518/jws_algs.py
 src/joserfc/rfc7518/oct_key.py
 src/joserfc/rfc7518/rsa_key.py
 src/joserfc/rfc7518/util.py
 src/joserfc/rfc7519/__init__.py
 src/joserfc/rfc7519/claims.py
 src/joserfc/rfc7519/registry.py
-src/joserfc/rfc7519/validators.py
 src/joserfc/rfc7638/__init__.py
 src/joserfc/rfc8037/__init__.py
 src/joserfc/rfc8037/jws_eddsa.py
 src/joserfc/rfc8037/okp_key.py
 src/joserfc/rfc8812/__init__.py
```

