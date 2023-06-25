# Comparing `tmp/m23-1.6.0.tar.gz` & `tmp/m23-1.6.1.tar.gz`

## Comparing `m23-1.6.0.tar` & `m23-1.6.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.6.0/.flake8
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 m23-1.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.6.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.6.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.6.0/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.6.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.6.0/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.6.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.6.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 m23-1.6.0/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/reference/__init__.py
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.6.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.6.0/.gitignore
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 m23-1.6.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 m23-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.6.1/.flake8
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 m23-1.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.6.1/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.6.1/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.6.1/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.6.1/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.6.1/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.6.1/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.6.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.6.1/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 m23-1.6.1/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.6.1/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.6.1/.gitignore
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 m23-1.6.1/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 m23-1.6.1/PKG-INFO
```

### Comparing `m23-1.6.0/CHANGELOG.md` & `m23-1.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.6.1 (2023-06-25)
+
+### Fix
+
+* Include reference fit image as part of the package ([`5d6d766`](https://github.com/LutherAstrophysics/m23/commit/5d6d76600cf08ff22efdd13e9894e7cc453d01e3))
+
 ## v1.6.0 (2023-06-25)
 
 ### Feature
 
 * Add 2509 and 2510 in ref files ([`30cc695`](https://github.com/LutherAstrophysics/m23/commit/30cc695790326bc47b55980fdc5e2b134cc0065b))
 
 ### Documentation
```

### Comparing `m23-1.6.0/brown.toml` & `m23-1.6.1/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/mf.toml` & `m23-1.6.1/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/nights_csv.toml` & `m23-1.6.1/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/rainbow.toml` & `m23-1.6.1/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/requirements.txt` & `m23-1.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/.github/workflows/python-publish.yml` & `m23-1.6.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/.vscode/settings.json` & `m23-1.6.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/__main__.py` & `m23-1.6.1/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/constants.py` & `m23-1.6.1/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/align/__init__.py` & `m23-1.6.1/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/calibrate/calibration.py` & `m23-1.6.1/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/calibrate/master_calibrate.py` & `m23-1.6.1/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/charts/__init__.py` & `m23-1.6.1/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/combine/__init__.py` & `m23-1.6.1/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/extract/__init__.py` & `m23-1.6.1/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/__init__.py` & `m23-1.6.1/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/aligned_combined_file.py` & `m23-1.6.1/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/alignment_stats_file.py` & `m23-1.6.1/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/color_normalized_file.py` & `m23-1.6.1/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/flux_log_combined_file.py` & `m23-1.6.1/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/log_file_combined_file.py` & `m23-1.6.1/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/masterflat_file.py` & `m23-1.6.1/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/normfactor_file.py` & `m23-1.6.1/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/raw_image_file.py` & `m23-1.6.1/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/reference_log_file.py` & `m23-1.6.1/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/ri_color_file.py` & `m23-1.6.1/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/file/sky_bg_file.py` & `m23-1.6.1/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/internight_normalize/__init__.py` & `m23-1.6.1/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/matrix/fill.py` & `m23-1.6.1/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/norm/__init__.py` & `m23-1.6.1/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/norm/get_line.py` & `m23-1.6.1/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/config_loader.py` & `m23-1.6.1/src/m23/processor/config_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
     Returns True if reference_image and reference_file paths exist
     """
     img_path = Path(reference_image)
     file_path = Path(reference_file)
     color_path = Path(color_ref_file)
     logfile_path = Path(logfile)
     if not (img_path.exists() and img_path.is_file() and img_path.suffix == ".fit"):
-        sys.stderr.write("Make sure that the reference exists and has .fit extension")
+        sys.stderr.write("Make sure that the reference image exists and has .fit extension\n")
         return False
     if not (file_path.exists() and file_path.is_file() and file_path.suffix == ".txt"):
         sys.stderr.write("Make sure that the reference file exists and has .txt extension\n")
         return False
     if not (color_path.exists() and color_path.is_file() and color_path.suffix == ".txt"):
         sys.stderr.write("Make sure that the color reference file exists and has .txt extension\n")
         return False
@@ -440,18 +440,15 @@
             )
         ):
             # Check for the optional configurations
             # Optional configs should either not be declared or be
             # correctly declared
             on_success(sanity_check(create_processing_config(configuration)))
         case _:
-            sys.stderr.write(
-                "Stopping because the provided configuration file"
-                + " doesn't match the required format.\n"
-            )
+            sys.stderr.write("Invalid format.\n")
 
 
 def load_configuration_with_necessary_reference_files(configuration, pop=None):
     # Users need not define reference files optional
     reference_files_dict = get_reference_files_dict()
     if user_defined_reference := configuration.get("reference"):
         # If user defines any reference file, that takes precedence
```

### Comparing `m23-1.6.0/src/m23/processor/generate_masterflat.py` & `m23-1.6.1/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.6.1/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,8 +128,8 @@
         case {
             "input": _,
             "output": _,
             "image": {"rows": int(_), "columns": int(_)},
         } as masterflat_generator_config if is_valid(masterflat_generator_config):
             on_success(sanity_check(create_enhanced_config(masterflat_generator_config)))
         case _:
-            sys.stderr.write("Stopping because the provided configuration file has issues.\n")
+            sys.stderr.write("Invalid format.\n")
```

### Comparing `m23-1.6.0/src/m23/processor/nights_csv.py` & `m23-1.6.1/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.6.1/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/process_nights.py` & `m23-1.6.1/src/m23/processor/process_nights.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/renormalize.py` & `m23-1.6.1/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.6.1/src/m23/processor/renormalize_config_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,12 +211,12 @@
         case {
             "processing": {"radii_of_extraction": list(_)},
             "input": {"nights": list(_)},
             "reference": {"file": str(_), "color": str(_), "logfile": str(_)},
         } as renormalize_config if is_valid(renormalize_config):
             on_success(sanity_check(create_enhanced_config(renormalize_config)))
         case _:
-            sys.stderr.write("Stopping because the provided configuration file has issues.\n")
+            sys.stderr.write("Invalid format.\n")
 
 
 if __name__ == "__main__":
     validate_renormalize_config_file(Path("1.toml"), on_success=lambda *args: print("Success"))
```

### Comparing `m23-1.6.0/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.6.1/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/reference/MeanRI100.txt` & `m23-1.6.1/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/reference/README.md` & `m23-1.6.1/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.6.1/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/sky/__init__.py` & `m23-1.6.1/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/sky/moon/__init__.py` & `m23-1.6.1/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/utils/__init__.py` & `m23-1.6.1/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/utils/date.py` & `m23-1.6.1/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/src/m23/utils/rename.py` & `m23-1.6.1/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/.gitignore` & `m23-1.6.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 #
 #
 
 ### custom
 .DS_STORE
 
 *.fit
+!**/reference/*.fit
 m23/calibrate/m23_7.0-0607.xy
 *.xy
 
 ### 
 usage/rename/test.py
 
 experiment
```

### Comparing `m23-1.6.0/README.md` & `m23-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.6.0/pyproject.toml` & `m23-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.6.0"
+version = "1.6.1"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.6.0/PKG-INFO` & `m23-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.6.0
+Version: 1.6.1
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
```

