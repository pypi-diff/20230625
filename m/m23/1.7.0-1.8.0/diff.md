# Comparing `tmp/m23-1.7.0.tar.gz` & `tmp/m23-1.8.0.tar.gz`

## Comparing `m23-1.7.0.tar` & `m23-1.8.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.7.0/.flake8
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.7.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.7.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.7.0/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.7.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.7.0/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.7.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.7.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.7.0/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.7.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.7.0/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.7.0/.gitignore
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 m23-1.7.0/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 m23-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.8.0/.flake8
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 m23-1.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.0/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.0/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.8.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.0/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.0/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.0/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.0/PKG-INFO
```

### Comparing `m23-1.7.0/CHANGELOG.md` & `m23-1.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.0 (2023-06-25)
+
+### Feature
+
+* Use multiprocessing while running renormalization of multiple nights ([`28acbf6`](https://github.com/LutherAstrophysics/m23/commit/28acbf6cb97b3a84584c51a57853454b940da383))
+
 ## v1.7.0 (2023-06-25)
 
 ### Feature
 
 * Use multiprocessing to run `ailgn_combine_extract` in parallel ([`9cbc641`](https://github.com/LutherAstrophysics/m23/commit/9cbc64178e2195034f11812ecd255de9c260e720))
 
 ### Fix
```

### Comparing `m23-1.7.0/brown.toml` & `m23-1.8.0/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/mf.toml` & `m23-1.8.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/nights_csv.toml` & `m23-1.8.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/rainbow.toml` & `m23-1.8.0/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/requirements.txt` & `m23-1.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/.github/workflows/python-publish.yml` & `m23-1.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/.vscode/settings.json` & `m23-1.8.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/__main__.py` & `m23-1.8.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/constants.py` & `m23-1.8.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/align/__init__.py` & `m23-1.8.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/calibrate/calibration.py` & `m23-1.8.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/calibrate/master_calibrate.py` & `m23-1.8.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/charts/__init__.py` & `m23-1.8.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/combine/__init__.py` & `m23-1.8.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/extract/__init__.py` & `m23-1.8.0/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/__init__.py` & `m23-1.8.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/aligned_combined_file.py` & `m23-1.8.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/alignment_stats_file.py` & `m23-1.8.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/color_normalized_file.py` & `m23-1.8.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/flux_log_combined_file.py` & `m23-1.8.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/log_file_combined_file.py` & `m23-1.8.0/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/masterflat_file.py` & `m23-1.8.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/normfactor_file.py` & `m23-1.8.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/raw_image_file.py` & `m23-1.8.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/reference_log_file.py` & `m23-1.8.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/ri_color_file.py` & `m23-1.8.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/file/sky_bg_file.py` & `m23-1.8.0/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/internight_normalize/__init__.py` & `m23-1.8.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/matrix/fill.py` & `m23-1.8.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/norm/__init__.py` & `m23-1.8.0/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/norm/get_line.py` & `m23-1.8.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/align_combined_extract.py` & `m23-1.8.0/src/m23/processor/align_combined_extract.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/config_loader.py` & `m23-1.8.0/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/generate_masterflat.py` & `m23-1.8.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.8.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/nights_csv.py` & `m23-1.8.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.8.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/process_nights.py` & `m23-1.8.0/src/m23/processor/process_nights.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/processor/renormalize.py` & `m23-1.8.0/src/m23/processor/renormalize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
 import sys
 from pathlib import Path
 
+import multiprocess as mp
+
+from m23 import __version__
 from m23.constants import FLUX_LOGS_COMBINED_FOLDER_NAME
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.reference_log_file import ReferenceLogFile
 from m23.processor.process_nights import normalization_helper
 from m23.utils import get_date_from_input_night_folder_name, get_log_file_name
 
 from .renormalize_config_loader import (
     RenormalizeConfig,
     validate_renormalize_config_file,
 )
 
 
 def renormalize_auxiliary(renormalize_dict: RenormalizeConfig):
-    for night in renormalize_dict["input"]["nights"]:
+    def night_renorm_mapper(night):
         NIGHT_FOLDER = night["path"]
         night_date = get_date_from_input_night_folder_name(NIGHT_FOLDER.name)
         log_file_path = NIGHT_FOLDER / get_log_file_name(night_date)
         radii_of_extraction = renormalize_dict["processing"]["radii_of_extraction"]
 
         logger = logging.getLogger("LOGGER_" + str(night_date))
         logger.setLevel(logging.INFO)
@@ -31,15 +34,15 @@
         ch2 = logging.StreamHandler(sys.stdout)
         ch2.setFormatter(formatter)
         logger.addHandler(ch2)  # Write to stdout
 
         first_image = night["first_logfile_number"]
         last_image = night["last_logfile_number"]
         logger.info(
-            f"Running renormalization for radii {radii_of_extraction}. Img: {first_image}-{last_image}"  # noqa ES501
+            f"Running renormalization for radii {radii_of_extraction}. Img: {first_image}-{last_image} with m23 version: {__version__}"  # noqa ES501
         )
 
         FLUX_LOGS_COMBINED_FOLDER: Path = NIGHT_FOLDER / FLUX_LOGS_COMBINED_FOLDER_NAME
         # Create log files combined folder if it doesn't yet exist
         FLUX_LOGS_COMBINED_FOLDER.mkdir(exist_ok=True)
 
         reference_log_file = ReferenceLogFile(
@@ -63,14 +66,18 @@
             img_duration,
             night_date,
             color_ref_file_path,
             NIGHT_FOLDER,
             logfile_combined_reference_logfile,
         )
 
+    with mp.Pool() as p:
+        print("foobar using pool")
+        p.map(night_renorm_mapper, renormalize_dict["input"]["nights"])
+
 
 def renormalize(file_path: str):
     """
     Starts renormalization with the configuration file `file_path` provided as the argument.
     Calls auxiliary function `renormalize_auxiliary` if the configuration is valid.
     """
     validate_renormalize_config_file(Path(file_path), on_success=renormalize_auxiliary)
```

### Comparing `m23-1.7.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.8.0/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.8.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/reference/MeanRI100.txt` & `m23-1.8.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/reference/README.md` & `m23-1.8.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/reference/m23_3.5_071.fit` & `m23-1.8.0/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.8.0/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/sky/__init__.py` & `m23-1.8.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/sky/moon/__init__.py` & `m23-1.8.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/utils/__init__.py` & `m23-1.8.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/utils/date.py` & `m23-1.8.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/src/m23/utils/rename.py` & `m23-1.8.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/.gitignore` & `m23-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.7.0/README.md` & `m23-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: m23
+Version: 1.8.0
+Requires-Python: >=3.10
+Requires-Dist: astroalign==2.4.1
+Requires-Dist: astropy==5.2.1
+Requires-Dist: ephem==4.1.4
+Requires-Dist: matplotlib==3.7.0
+Requires-Dist: multiprocess==0.70.14
+Requires-Dist: numpy==1.24.2
+Requires-Dist: opencv-python==4.7.0.68
+Requires-Dist: toml==0.10.2
+Requires-Dist: typing-extensions==4.4.0
+Description-Content-Type: text/markdown
+
 # M23 Data Processing
 
 This is a library of tools that compose raw image processing of fits files. It
 includes modules for calibration, combination, alignment, extraction and
 normalization. Additionally we also have a data processor module that processes
 data based on a provided configuration file using all the aforementioned
 modules.
@@ -283,7 +298,17 @@
 and couple others:
 ![screenshot of summary of valid commitizen commits](https://raw.githubusercontent.com/commitizen/cz-cli/master/meta/screenshots/add-commit.png)
 
 Note that if any of your commits make breaking changes, your commit message must
 also contain the phrase "BREAKING CHANGE". This will trigger a major version
 update. See some of the previous commit messages for more information and feel
 free too ask if you have confusion.
+
+### Known issues
+
+We use multiprocessing to parallelize processing of our data. In macOS, we encounter
+a this issue described in [so post](https://stackoverflow.com/questions/50168647/multiprocessing-causes-python-to-crash-and-gives-an-error-may-have-been-in-progr). The post gives a solution as summarized below.
+
+```sh
+echo "export OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES" >> ~/.zshrc
+. ~/.zshrc
+```
```

### Comparing `m23-1.7.0/pyproject.toml` & `m23-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.7.0"
+version = "1.8.0"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.7.0/PKG-INFO` & `m23-1.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: m23
-Version: 1.7.0
-Requires-Python: >=3.10
-Requires-Dist: astroalign==2.4.1
-Requires-Dist: astropy==5.2.1
-Requires-Dist: ephem==4.1.4
-Requires-Dist: matplotlib==3.7.0
-Requires-Dist: multiprocess==0.70.14
-Requires-Dist: numpy==1.24.2
-Requires-Dist: opencv-python==4.7.0.68
-Requires-Dist: toml==0.10.2
-Requires-Dist: typing-extensions==4.4.0
-Description-Content-Type: text/markdown
-
 # M23 Data Processing
 
 This is a library of tools that compose raw image processing of fits files. It
 includes modules for calibration, combination, alignment, extraction and
 normalization. Additionally we also have a data processor module that processes
 data based on a provided configuration file using all the aforementioned
 modules.
@@ -298,7 +283,17 @@
 and couple others:
 ![screenshot of summary of valid commitizen commits](https://raw.githubusercontent.com/commitizen/cz-cli/master/meta/screenshots/add-commit.png)
 
 Note that if any of your commits make breaking changes, your commit message must
 also contain the phrase "BREAKING CHANGE". This will trigger a major version
 update. See some of the previous commit messages for more information and feel
 free too ask if you have confusion.
+
+### Known issues
+
+We use multiprocessing to parallelize processing of our data. In macOS, we encounter
+a this issue described in [so post](https://stackoverflow.com/questions/50168647/multiprocessing-causes-python-to-crash-and-gives-an-error-may-have-been-in-progr). The post gives a solution as summarized below.
+
+```sh
+echo "export OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES" >> ~/.zshrc
+. ~/.zshrc
+```
```

