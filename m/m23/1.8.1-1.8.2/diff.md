# Comparing `tmp/m23-1.8.1.tar.gz` & `tmp/m23-1.8.2.tar.gz`

## Comparing `m23-1.8.1.tar` & `m23-1.8.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.8.1/.flake8
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 m23-1.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.1/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.1/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.1/nights_csv.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.1/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.1/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.8.1/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.1/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.1/.vscode/settings.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/matrix/utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/__init__.py
--rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/align_combined_extract.py
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/README.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/__init__.py
--rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/m23_3.5_071.fit
--rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/reference/ref_no_na_w_2509_10.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.1/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.1/.gitignore
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.1/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 m23-1.8.2/.flake8
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 m23-1.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 m23-1.8.2/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.8.2/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.8.2/nights_csv.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 m23-1.8.2/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.8.2/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.8.2/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.8.2/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 m23-1.8.2/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21756 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/align_combined_extract.py
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725955 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/README.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0  4199040 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/m23_3.5_071.fit
+-rw-r--r--   0        0        0   304094 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/reference/ref_no_na_w_2509_10.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.8.2/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.8.2/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 m23-1.8.2/.gitignore
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 m23-1.8.2/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 m23-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 m23-1.8.2/PKG-INFO
```

### Comparing `m23-1.8.1/CHANGELOG.md` & `m23-1.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.2 (2023-06-25)
+
+### Fix
+
+* Use matplotlib in headless mode ([`bbb4bc2`](https://github.com/LutherAstrophysics/m23/commit/bbb4bc26a0be694d848a639fdf7402a3fd3c8e04))
+
 ## v1.8.1 (2023-06-25)
 
 ### Fix
 
 * Handle case for nan FWHM in extraction ([`954fcb7`](https://github.com/LutherAstrophysics/m23/commit/954fcb7bcbf44cc838de4c45c7fa7942b4cbafba))
 * Prevent deleting image data for process safety ([`a200d7f`](https://github.com/LutherAstrophysics/m23/commit/a200d7fdce3dca2c7fd04a489b39911fe95b33bc))
```

### Comparing `m23-1.8.1/brown.toml` & `m23-1.8.2/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/mf.toml` & `m23-1.8.2/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/nights_csv.toml` & `m23-1.8.2/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/rainbow.toml` & `m23-1.8.2/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/requirements.txt` & `m23-1.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/.github/workflows/python-publish.yml` & `m23-1.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/.vscode/settings.json` & `m23-1.8.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/__main__.py` & `m23-1.8.2/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/constants.py` & `m23-1.8.2/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/align/__init__.py` & `m23-1.8.2/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/calibrate/calibration.py` & `m23-1.8.2/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/calibrate/master_calibrate.py` & `m23-1.8.2/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/charts/__init__.py` & `m23-1.8.2/src/m23/charts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-import itertools
+import matplotlib
+
+# Use non interactive backend
+matplotlib.use("agg")
+
+import itertools  # noqa
 import sys
 from pathlib import Path
 from typing import Callable, Dict, Iterable
 
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `m23-1.8.1/src/m23/combine/__init__.py` & `m23-1.8.2/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/extract/__init__.py` & `m23-1.8.2/src/m23/extract/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,19 +228,19 @@
         ) * ((half_round_up_to_int(xweight) + axis) - xweight) ** 2
         weighted_row_sum += (
             data[half_round_up_to_int(xweight), half_round_up_to_int(yweight) + axis] - aduPerPixel
         ) * ((half_round_up_to_int(yweight) + axis) - yweight) ** 2
     col_sum = col_sum - (aduPerPixel * 11)
     row_sum = row_sum - (aduPerPixel * 11)
 
-    if weighted_col_sum < 0 or col_sum == 1:
+    if weighted_col_sum < 0 or col_sum <= 1:
         xFWHM = 0
     else:
         xFWHM = 2.355 * np.sqrt(weighted_col_sum / (col_sum - 1))
-    if weighted_row_sum < 0 or row_sum == 1:
+    if weighted_row_sum < 0 or row_sum <= 1:
         yFWHM = 0
     else:
         yFWHM = 2.355 * np.sqrt(weighted_row_sum / (row_sum - 1))
     average_FWHM = np.mean([xFWHM, yFWHM])
     return xFWHM, yFWHM, average_FWHM
```

### Comparing `m23-1.8.1/src/m23/file/__init__.py` & `m23-1.8.2/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/aligned_combined_file.py` & `m23-1.8.2/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/alignment_stats_file.py` & `m23-1.8.2/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/color_normalized_file.py` & `m23-1.8.2/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/flux_log_combined_file.py` & `m23-1.8.2/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/log_file_combined_file.py` & `m23-1.8.2/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/masterflat_file.py` & `m23-1.8.2/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/normfactor_file.py` & `m23-1.8.2/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/raw_image_file.py` & `m23-1.8.2/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/reference_log_file.py` & `m23-1.8.2/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/ri_color_file.py` & `m23-1.8.2/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/file/sky_bg_file.py` & `m23-1.8.2/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/internight_normalize/__init__.py` & `m23-1.8.2/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/matrix/fill.py` & `m23-1.8.2/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/norm/__init__.py` & `m23-1.8.2/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/norm/get_line.py` & `m23-1.8.2/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/align_combined_extract.py` & `m23-1.8.2/src/m23/processor/align_combined_extract.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/config_loader.py` & `m23-1.8.2/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/generate_masterflat.py` & `m23-1.8.2/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.8.2/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/nights_csv.py` & `m23-1.8.2/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/nights_csv_config_loader.py` & `m23-1.8.2/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/process_nights.py` & `m23-1.8.2/src/m23/processor/process_nights.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/processor/renormalize.py` & `m23-1.8.2/src/m23/processor/renormalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             night_date,
             color_ref_file_path,
             NIGHT_FOLDER,
             logfile_combined_reference_logfile,
         )
 
     with mp.Pool() as p:
-        print("foobar using pool")
         p.map(night_renorm_mapper, renormalize_dict["input"]["nights"])
 
 
 def renormalize(file_path: str):
     """
     Starts renormalization with the configuration file `file_path` provided as the argument.
     Calls auxiliary function `renormalize_auxiliary` if the configuration is valid.
```

### Comparing `m23-1.8.1/src/m23/processor/renormalize_config_loader.py` & `m23-1.8.2/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.8.2/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/reference/MeanRI100.txt` & `m23-1.8.2/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/reference/README.md` & `m23-1.8.2/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/reference/m23_3.5_071.fit` & `m23-1.8.2/src/m23/reference/m23_3.5_071.fit`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/reference/ref_no_na_w_2509_10.txt` & `m23-1.8.2/src/m23/reference/ref_no_na_w_2509_10.txt`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/sky/__init__.py` & `m23-1.8.2/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/sky/moon/__init__.py` & `m23-1.8.2/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/utils/__init__.py` & `m23-1.8.2/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/utils/date.py` & `m23-1.8.2/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/src/m23/utils/rename.py` & `m23-1.8.2/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/.gitignore` & `m23-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/README.md` & `m23-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.8.1/pyproject.toml` & `m23-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.8.1"
+version = "1.8.2"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.8.1/PKG-INFO` & `m23-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.8.1
+Version: 1.8.2
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multiprocess==0.70.14
 Requires-Dist: numpy==1.24.2
```

