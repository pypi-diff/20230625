# Comparing `tmp/m23-1.4.0.tar.gz` & `tmp/m23-1.5.0.tar.gz`

## Comparing `m23-1.4.0.tar` & `m23-1.5.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.4.0/.flake8
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 m23-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.4.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.4.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.4.0/nights_csv.toml
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.4.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.4.0/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.4.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.4.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 m23-1.4.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22194 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725377 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.4.0/.gitignore
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.4.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.5.0/.flake8
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 m23-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.5.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.5.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.5.0/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.5.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.5.0/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.5.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.5.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 m23-1.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725377 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/reference/__init__.py
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.5.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.5.0/.gitignore
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.5.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.5.0/PKG-INFO
```

### Comparing `m23-1.4.0/CHANGELOG.md` & `m23-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.0 (2023-06-25)
+
+### Feature
+
+* Update intranight normalization to normalize to similar elevation images ([`c0dae10`](https://github.com/LutherAstrophysics/m23/commit/c0dae104876d7dcb0ba23be29a2fea9134dee883))
+* Make reference files optional ([`84f28d8`](https://github.com/LutherAstrophysics/m23/commit/84f28d8bbc10548400ce570b42c6826342aae94b))
+
+### Fix
+
+* Use natural round in sky bg file ([`bd1f43d`](https://github.com/LutherAstrophysics/m23/commit/bd1f43d94d62c7049f4e67c3e068aaef39520598))
+
 ## v1.4.0 (2023-06-24)
 
 ### Feature
 
 * Add cols for first/last logfile used in sky bg file ([`7093c10`](https://github.com/LutherAstrophysics/m23/commit/7093c10bbcc3caa679c7c8e2f7e0448691027f5f))
 * Account for surrounding boxes in sky adu calc ([`bef88e6`](https://github.com/LutherAstrophysics/m23/commit/bef88e69c78fe56ac16c6ca1f40a59e286171149))
```

### Comparing `m23-1.4.0/brown.toml` & `m23-1.5.0/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/mf.toml` & `m23-1.5.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/nights_csv.toml` & `m23-1.5.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/rainbow.toml` & `m23-1.5.0/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/requirements.txt` & `m23-1.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/.github/workflows/python-publish.yml` & `m23-1.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/.vscode/settings.json` & `m23-1.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/__main__.py` & `m23-1.5.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/constants.py` & `m23-1.5.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/align/__init__.py` & `m23-1.5.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/calibrate/calibration.py` & `m23-1.5.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/calibrate/master_calibrate.py` & `m23-1.5.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/charts/__init__.py` & `m23-1.5.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/combine/__init__.py` & `m23-1.5.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/extract/__init__.py` & `m23-1.5.0/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/__init__.py` & `m23-1.5.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/aligned_combined_file.py` & `m23-1.5.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/alignment_stats_file.py` & `m23-1.5.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/color_normalized_file.py` & `m23-1.5.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/flux_log_combined_file.py` & `m23-1.5.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/log_file_combined_file.py` & `m23-1.5.0/src/m23/file/log_file_combined_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import re
 from collections import namedtuple
 from datetime import date, datetime
 from pathlib import Path
-from typing import Dict, Iterable
+from typing import Dict, Iterable, Tuple
 
 import numpy as np
 import numpy.typing as npt
 
 from m23.constants import OBSERVATION_DATETIME_FORMAT
 from m23.file.aligned_combined_file import AlignedCombinedFile
+from m23.sky import angle_of_elevation
 
 
 # Note that LogFileCombined is the one that that has the data for aligned combined
 # images after extracting stars from the image. This is not to be confused with FluxLogCombined
 # that is created after intra-night normalization (note *not* internight normalization)
 class LogFileCombinedFile:
     # Class attributes
     header_rows = 9
     data_titles_row_zero_index = 8
     date_format = "%m-%d-%y"
     sky_adu_column = 5
     x_column = 0
     y_column = 1
-    file_name_re = re.compile("(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)-(\d{3})\.txt")
-    star_adu_radius_re = re.compile("Star ADU (\d+)")
+    file_name_re = re.compile(r"(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)-(\d{3})\.txt")
+    star_adu_radius_re = re.compile(r"Star ADU (\d+)")
 
     StarLogfileCombinedData = namedtuple(
         "StarLogfileCombinedData",
         ["x", "y", "xFWHM", "yFWHM", "avgFWHM", "sky_adu", "radii_adu"],
     )
     LogFileCombinedDataType = Dict[int, StarLogfileCombinedData]
 
@@ -45,14 +46,15 @@
 
     def __init__(self, file_path: str) -> None:
         self.__path = Path(file_path)
         self.__is_read = False
         self.__header = None
         self.__data = None
         self.__title_row = None
+        self.__cluster_angle = None
 
     def _read(self):
         with self.__path.open() as fd:
             lines = [line.strip() for line in fd.readlines()]
             # Save the title row
             # We split the title row by gap of more than two spaces
             self.__title_row = re.split(r"\s{2,}", lines[self.data_titles_row_zero_index])
@@ -72,14 +74,30 @@
     def _adu_radius_header_name(self, radius: int):
         return f"Star ADU {radius}"
 
     def _get_column_number_for_adu_radius(self, radius: int):
         titles = self._title_row()
         return titles.index(self._adu_radius_header_name(radius))
 
+    def get_cluster_angle_with_uncertainty(self) -> Tuple[float, float]:
+        """
+        Return the cluster angle along with uncertainty of measurement of the
+        time the image was taken
+        """
+        if not self.__cluster_angle:
+            self.__cluster_angle = angle_of_elevation(
+                datetime.strptime(self.datetime(), OBSERVATION_DATETIME_FORMAT)
+            )
+        # Note that cluster angle contains the angle as well as uncertainty
+        return self.__cluster_angle
+
+    def get_cluster_angle(self) -> float:
+        """Return the cluster angle of the time the image was taken"""
+        return self.get_cluster_angle_with_uncertainty()[0]
+
     def is_valid_file_name(self) -> bool:
         """
         Checks if the filename matches the naming convention
         """
         return bool(self.file_name_re.match(self.path().name))
 
     def header(self) -> Iterable[str]:
```

### Comparing `m23-1.4.0/src/m23/file/masterflat_file.py` & `m23-1.5.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/normfactor_file.py` & `m23-1.5.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/raw_image_file.py` & `m23-1.5.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/reference_log_file.py` & `m23-1.5.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/ri_color_file.py` & `m23-1.5.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/file/sky_bg_file.py` & `m23-1.5.0/src/m23/file/sky_bg_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 
 from m23.constants import OBSERVATION_DATETIME_FORMAT, SKY_BG_FILENAME_DATE_FORMAT
 from m23.sky import angle_of_elevation
 from m23.sky.moon import moon_distance
 from m23.sky.moon import phase as get_moon_phase_name
 from m23.sky.moon import position as get_moon_phase
+from m23.utils import half_round_up_to_int
 
 
 class SkyBgFile:
     file_name_re = re.compile(r"(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)_sky_bg\.txt")
     date_observed_datetime_format = OBSERVATION_DATETIME_FORMAT
 
     # We divide up the sky into several square sections (currently, sized 64px)
@@ -55,14 +56,15 @@
         sky_bg_data: SkyBGDataType,
         color_normfactors_title: Iterable[str],
         color_normfactors_values: Iterable[float],
         brightness_normfactors_title: Iterable[str],
         brightness_normfactors_values: Iterable[float],
         first_img_number: int,
         last_img_number: int,
+        normalized_cluster_angle: int,
     ):
         """
         Creates/Updates sky background file based on the `sky_bg_data`
         """
         if len(sky_bg_data) == 0:
             # Nothing to do
             with open(self.path(), "w") as fd:
@@ -85,14 +87,15 @@
             fd.write(
                 f"{'Date':<26s}"
                 f"{'Image_number':<15s}"
                 f"{'First_img':<15s}"  # Img number of the first logfile combined used
                 f"{'Last_img':<15s}"  # Img number of the last logfile combined used
                 f"{'Moon_Phase':<16s}"
                 f"{'Moon_Phase_Name':<20s}"
+                f"{'Normalized_cluster_angle':<30s}"
                 f"{'Cluster_Angle_Round':<20s}"
                 f"{'Cluster_Angle':<20s}"
                 f"{'Cluster_Angle_Uncertainty':<30s}"
                 f"{'Moon_Distance':<20s}"
                 f"{'Mean':<10s}{'Median':<10s}"
                 f"{'Std':<10s}"
                 f"{color_normfactors_title_str}"
@@ -123,15 +126,16 @@
                 fd.write(
                     f"{night_datetime:<26s}"
                     f"{img_number:<15d}"
                     f"{first_img_number:<15d}"
                     f"{last_img_number:<15d}"
                     f"{moon_phase:<16.5f}"
                     f"{moon_phase_name:<20s}"
-                    f"{np.round(cluster_angle):<20.0f}"
+                    f"{normalized_cluster_angle:<30d}"
+                    f"{half_round_up_to_int(cluster_angle):<20.0f}"
                     f"{cluster_angle:<20.1f}"
                     f"{cluster_angle_uncertainty:<30.1f}"
                     f"{moon_dist_degrees:<20.2f}"
                     f"{mean:<10.2f}{median:<10.2f}"
                     f"{std:<10.2f}"
                     f"{color_normfactors_values_str}"
                     f"{brightness_normfactors_values_str}"
```

### Comparing `m23-1.4.0/src/m23/internight_normalize/__init__.py` & `m23-1.5.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/matrix/fill.py` & `m23-1.5.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/norm/get_line.py` & `m23-1.5.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/config_loader.py` & `m23-1.5.0/src/m23/processor/config_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CAMERA_CHANGE_2022_DATE,
     INPUT_CALIBRATION_FOLDER_NAME,
     M23_RAW_IMAGES_FOLDER_NAME,
     TYPICAL_NEW_CAMERA_CROP_REGION,
 )
 from m23.exceptions import InvalidDatetimeInConfig
 from m23.file.log_file_combined_file import LogFileCombinedFile
+from m23.reference import get_reference_files_dict
 from m23.utils import (
     get_darks,
     get_date_from_input_night_folder_name,
     get_flats,
     get_raw_images,
 )
 
@@ -400,15 +401,17 @@
     """
     This method reads data processing configuration from the file path
     provided and calls the unary function on_success if the configuration
     file is valid with the configuration dictionary (Note, *not* config file).
     """
     if not file_path.exists() or not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
-    match configuration := toml.load(file_path):
+    configuration = toml.load(file_path)
+    load_configuration_with_necessary_reference_files(configuration)
+    match configuration:
         case {
             "image": {
                 "rows": int(_),
                 "columns": int(_),
                 **optional_image_options,
             },
             "processing": {
@@ -441,7 +444,23 @@
             # correctly declared
             on_success(sanity_check(create_processing_config(configuration)))
         case _:
             sys.stderr.write(
                 "Stopping because the provided configuration file"
                 + " doesn't match the required format.\n"
             )
+
+
+def load_configuration_with_necessary_reference_files(configuration, pop=None):
+    # Users need not define reference files optional
+    reference_files_dict = get_reference_files_dict()
+    if user_defined_reference := configuration.get("reference"):
+        # If user defines any reference file, that takes precedence
+        # over files configured to be used as default
+        for key in reference_files_dict:
+            if key not in user_defined_reference:
+                user_defined_reference[key] = reference_files_dict[key]
+    else:
+        configuration["reference"] = reference_files_dict
+    if pop:
+        for item_to_pop in pop:
+            configuration["reference"].pop(item_to_pop)
```

### Comparing `m23-1.4.0/src/m23/processor/generate_masterflat.py` & `m23-1.5.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.5.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/nights_csv.py` & `m23-1.5.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.5.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/process_nights.py` & `m23-1.5.0/src/m23/processor/process_nights.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     for radius in radii_of_extraction:
         logger.info(f"Normalizing for radius of extraction {radius} px")
         RADIUS_FOLDER = FLUX_LOGS_COMBINED_OUTPUT_FOLDER / get_radius_folder_name(radius)
         RADIUS_FOLDER.mkdir(exist_ok=True)  # Create folder if it doesn't exist
         for file in RADIUS_FOLDER.glob("*"):
             if file.is_file():
                 file.unlink()  # Remove each file in the folder
-        normalize_log_files(
+        intranight_norm_result = normalize_log_files(
             reference_log_file,
             log_files_to_use,
             RADIUS_FOLDER,
             radius,
             img_duration,
             night_date,
         )
@@ -135,25 +135,27 @@
         SkyBgFile(sky_bg_filename),
         log_files_to_use,
         night_date,
         color_normfactors_titles,
         color_normfactors_values,
         brightness_normfactors_titles,
         brightness_normfactors_values,
+        intranight_norm_result.get("normalized_cluster_angle"),
     )
 
 
 def create_sky_bg_file(
     sky_bg_file: SkyBgFile,
     log_files_to_use: Iterable[LogFileCombinedFile],
     night_date: date,
     color_normfactors_title: Iterable[str],
     color_normfactors_values: Iterable[float],
     brightness_normfactors_title: Iterable[str],
     brightness_normfactors_values: Iterable[float],
+    normalized_cluster_angle: int,
 ):
     """
     Creates sky bg data. Note that this isn't performed right after extraction
     is that we want to re-perform it after re-normalization. If we do it as part
     of `normalization_helper` which is what both `process_night` and `renorm`
     use, we wouldn't have to do it twice.
 
@@ -196,14 +198,15 @@
         bg_data_of_all_images,
         color_normfactors_title,
         color_normfactors_values,
         brightness_normfactors_title,
         brightness_normfactors_values,
         log_files_to_use[0].img_number(),
         log_files_to_use[-1].img_number(),
+        normalized_cluster_angle,
     )
     logger.info("Completed generating sky background file")
 
 
 def get_datetime_to_use(
     aligned_combined: AlignedCombinedFile,
     night_config: ConfigInputNight,
```

### Comparing `m23-1.4.0/src/m23/processor/renormalize.py` & `m23-1.5.0/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.5.0/src/m23/processor/renormalize_config_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing_extensions import NotRequired
 
 from m23.constants import LOG_FILES_COMBINED_FOLDER_NAME
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.processor.config_loader import (
     is_night_name_valid,
     is_valid_radii_of_extraction,
+    load_configuration_with_necessary_reference_files,
 )
 from m23.utils import get_image_number_in_log_file_combined_file
 
 
 class RenormalizeConfigProcessing(TypedDict):
     radii_of_extraction: List[int]
 
@@ -200,15 +201,17 @@
     """
     This method reads data processing configuration from the file path
     provided and calls the unary function on_success if the configuration
     file is valid with the configuration dictionary (Note, *not* config file).
     """
     if not file_path.exists() or not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
-    match toml.load(file_path):
+    configuration = toml.load(file_path)
+    load_configuration_with_necessary_reference_files(configuration, pop=("image",))
+    match configuration:
         case {
             "processing": {"radii_of_extraction": list(_)},
             "input": {"nights": list(_)},
             "reference": {"file": str(_), "color": str(_), "logfile": str(_)},
         } as renormalize_config if is_valid(renormalize_config):
             on_success(sanity_check(create_enhanced_config(renormalize_config)))
         case _:
```

### Comparing `m23-1.4.0/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.5.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/reference/MeanRI100.txt` & `m23-1.5.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/reference/README.md` & `m23-1.5.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/reference/ref_revised_71.txt` & `m23-1.5.0/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/sky/__init__.py` & `m23-1.5.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/sky/moon/__init__.py` & `m23-1.5.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/utils/__init__.py` & `m23-1.5.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/utils/date.py` & `m23-1.5.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/src/m23/utils/rename.py` & `m23-1.5.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/.gitignore` & `m23-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/README.md` & `m23-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.4.0/pyproject.toml` & `m23-1.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.4.0"
+version = "1.5.0"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.4.0/PKG-INFO` & `m23-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.4.0
+Version: 1.5.0
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
```

