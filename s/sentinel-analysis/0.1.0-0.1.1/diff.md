# Comparing `tmp/sentinel_analysis-0.1.0.tar.gz` & `tmp/sentinel_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinel_analysis-0.1.0.tar", max compression
+gzip compressed data, was "sentinel_analysis-0.1.1.tar", max compression
```

## Comparing `sentinel_analysis-0.1.0.tar` & `sentinel_analysis-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.0/README.md
--rw-r--r--   0        0        0      327 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0  2426645 2023-06-25 11:58:26.983350 sentinel_analysis-0.1.0/sentinel_analysis/GeoIP_DBs/GeoIP.dat
--rw-r--r--   0        0        0  6025934 2023-06-25 11:58:26.991351 sentinel_analysis-0.1.0/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.0/sentinel_analysis/__init__.py
--rw-r--r--   0        0        0     7219 2023-06-25 11:58:27.047352 sentinel_analysis-0.1.0/sentinel_analysis/__main__.py
--rw-r--r--   0        0        0     3670 2023-06-25 11:59:13.928759 sentinel_analysis-0.1.0/sentinel_analysis/alert.py
--rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.0/sentinel_analysis/report.py
--rw-r--r--   0        0        0      301 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.1/README.md
+-rw-r--r--   0        0        0      476 2023-06-25 12:08:37.630695 sentinel_analysis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0  2426645 2023-06-25 11:58:26.983350 sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIP.dat
+-rw-r--r--   0        0        0  6025934 2023-06-25 11:58:26.991351 sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.1/sentinel_analysis/__init__.py
+-rw-r--r--   0        0        0     7219 2023-06-25 11:58:27.047352 sentinel_analysis-0.1.1/sentinel_analysis/__main__.py
+-rw-r--r--   0        0        0     3670 2023-06-25 11:59:13.928759 sentinel_analysis-0.1.1/sentinel_analysis/alert.py
+-rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.1/sentinel_analysis/report.py
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.1/PKG-INFO
```

### Comparing `sentinel_analysis-0.1.0/sentinel_analysis/GeoIP_DBs/GeoIP.dat` & `sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIP.dat`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.0/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat` & `sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.0/sentinel_analysis/__main__.py` & `sentinel_analysis-0.1.1/sentinel_analysis/__main__.py`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.0/sentinel_analysis/alert.py` & `sentinel_analysis-0.1.1/sentinel_analysis/alert.py`

 * *Files identical despite different names*

