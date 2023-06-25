# Comparing `tmp/open-prime-rando-0.7.1.tar.gz` & `tmp/open-prime-rando-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.7.1.tar", last modified: Sat Jun 24 00:44:49 2023, max compression
+gzip compressed data, was "open-prime-rando-0.8.0.tar", last modified: Sun Jun 25 17:27:49 2023, max compression
```

## Comparing `open-prime-rando-0.7.1.tar` & `open-prime-rando-0.8.0.tar`

### file list

```diff
@@ -1,115 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.970483 open-prime-rando-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/dol_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/user_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.970483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/elevator_rando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tests/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_all_prime_dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_dol_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 17:27:49.696555 open-prime-rando-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.672555 open-prime-rando-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/src/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/dol_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.684555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.684555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.672555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/elevator_rando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_all_prime_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_dol_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/echoes/test_echoes_dock_lock_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.7.1/.github/dependabot.yml` & `open-prime-rando-0.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/.github/workflows/python.yml` & `open-prime-rando-0.8.0/.github/workflows/python.yml`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         run: python -m pip install --upgrade pip
 
       - name: install built wheel
         run: python -m pip install "$(ls dist/*.whl)[test]"
         shell: bash
 
       - name: run pytest
-        run: python -m pytest
+        run: python -m pytest --skip-if-missing
 
   full_test:
     runs-on: self-hosted
     needs:
       - build
 
     steps:
```

### Comparing `open-prime-rando-0.7.1/.gitignore` & `open-prime-rando-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/LICENSE` & `open-prime-rando-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/PKG-INFO` & `open-prime-rando-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.7.1
+Version: 0.8.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.7.1/pyproject.toml` & `open-prime-rando-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.10"
 dynamic = ["version"]
 
 dependencies = [
-    "retro-data-structures>=0.20.1",
+    "retro-data-structures>=0.21.0",
     "jsonschema>=4.0.0",
     "ppc-asm",
     "py_randomprime",  # for Prime 1 symbols
 ]
 
 [project.optional-dependencies]
 test = [
@@ -58,10 +58,11 @@
     "ignore::DeprecationWarning",
 ]
 
 
 [tool.ruff]
 line-length = 120
 select = ["E", "F", "W", "C90", "I", "UP"]
+src = ["src"]
 
 # Version to target for generated code.
-target-version = "py310"
+target-version = "py310"
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/cli.py` & `open-prime-rando-0.8.0/src/open_prime_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/all_prime_dol_patches.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_versions.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/dol_version.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/dol_version.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/beam_configuration.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patcher.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patches.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_versions.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/user_preferences.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_patches.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_versions.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.8.0/src/open_prime_rando/dynamic_schema.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/agon_wastes.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/great_temple.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/great_temple.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/temple_grounds.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/torvus_bog.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/world.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0007 0080 0080 0000 0001 9d53 7c2f  .............S|/
 00000010: 9d53 39c8 7c2f 7c2f 7c2f 5aec 5aec 5aec  .S9.|/|/|/Z.Z.Z.
-00000020: 9d53 39c8 5aec 7c2f 9d53 7c2f abf5 0000  .S9.Z.|/.S|/....
-00000030: 0000 0000 6a0d 0000 0000 0000 6a0d 2005  ....j.......j. .
-00000040: abf5 abf5 abf5 0000 abf5 abf5 0000 dfbd  ................
-00000050: 6289 9d33 0000 9d33 6289 6289 0000 9d33  b..3...3b.b....3
-00000060: 0000 9d33 0000 9d33 9d33 9d33 9d12 7bee  ...3...3.3.3..{.
+00000020: 9d53 39c8 5aec 7c2f 9d53 7c2f ffff 8430  .S9.Z.|/.S|/...0
+00000030: 8430 8430 ef5d 8430 8430 8430 ef5d b5b6  .0.0.].0.0.0.]..
+00000040: ffff ffff ffff 8430 ffff ffff 9492 dfbd  .......0........
+00000050: 6289 9d33 9492 9d33 6289 6289 9492 9d33  b..3...3b.b....3
+00000060: 9492 9d33 9492 9d33 9d33 9d33 9d12 7bee  ...3...3.3.3..{.
 00000070: 39c7 9d12 5aca 7bee 39c7 9d12 7bee 7bee  9...Z.{.9...{.{.
 00000080: 39c7 9d12 7bee 7bee 39c7 7bee a5b3 7c2f  9...{.{.9.{...|/
 00000090: 6b6d 6b6d a5b3 a5b3 6b6d 7c2f a5b3 7c2f  kmkm....km|/..|/
 000000a0: 7c2f 6b6d 7c2f 6b6d 6b6d 7c2f 840f 7bce  |/km|/kmkm|/..{.
 000000b0: 7bce 73ae 73ae 7bce 7bce 6b6d 73ae 7bce  {.s.s.{.{.kms.{.
 000000c0: 7bce 73ae 840f 6b6d 73ae 6b6d 73ae 73ae  {.s...kms.kms.s.
 000000d0: 73ae 8c50 73ae 73ae 73ae 5aeb 5aeb 73ae  s..Ps.s.s.Z.Z.s.
@@ -60,43 +60,43 @@
 000003b0: 8c91 5b0b b616 b616 b616 b616 3186 3186  ..[.........1.1.
 000003c0: 3186 5b0b 3186 3186 3186 3186 636d 636d  1.[.1.1.1.1.cmcm
 000003d0: 9533 636d 9533 9533 9533 9533 31a7 31a7  .3cm.3.3.3.31.1.
 000003e0: 31a7 31a7 0001 31a7 31a7 0001 7bef 5aeb  1.1...1.1...{.Z.
 000003f0: 5aeb 5aeb b5f6 7bef 7bef 7bef 5aeb 94f2  Z.Z...{.{.{.Z...
 00000400: 7bef 7bef 5aeb b5f6 7bef 7bef 9532 9532  {.{.Z...{.{..2.2
 00000410: 73ce 9532 9532 9532 9532 5a89 73ce 73ce  s..2.2.2.2Z.s.s.
-00000420: ae77 5a89 73ce 9532 ae77 5a89 0000 0000  .wZ.s..2.wZ.....
-00000430: 1003 1003 0000 1003 1003 1003 0000 0000  ................
-00000440: 1003 1003 1003 68ce c278 c278 0000 0000  ......h..x.x....
-00000450: a4b2 a4b2 1002 0000 1002 a4b2 0000 0000  ................
-00000460: 1002 a4b2 a4b2 0000 832c a4b2 632c 7bef  .........,..c,{.
+00000420: ae77 5a89 73ce 9532 ae77 5a89 738e 738e  .wZ.s..2.wZ.s.s.
+00000430: a534 a534 738e a534 a534 a534 738e 738e  .4.4s..4.4.4s.s.
+00000440: a534 a534 a534 dedb ffff ffff 8410 8410  .4.4.4..........
+00000450: a4b2 a4b2 ad75 8410 ad75 a4b2 8410 8410  .....u...u......
+00000460: ad75 a4b2 a4b2 8410 832c a4b2 632c 7bef  .u.......,..c,{.
 00000470: 39e7 7bef 7bef 632c 39e7 7bef 632c 7bef  9.{.{.c,9.{.c,{.
 00000480: 39e7 7bef 7bef 7bef 39e7 7bef 840f 8c50  9.{.{.{.9.{....P
 00000490: 6b6d 6b6d 8c50 840f 840f 840f 8c50 73ae  kmkm.P.......Ps.
 000004a0: 6b6d 6b6d 840f 8c50 6b6d 73ae 8410 8410  kmkm...Pkms.....
 000004b0: 7bcf 6b4c 7bcf 7bcf 8410 7bcf 7bcf 6b4c  {.kL{.{...{.{.kL
 000004c0: 738d 8410 6b4c 8410 738d 8410 73ce 630b  s...kL..s...s.c.
 000004d0: 4a49 630b 8c90 4a49 4a49 630b 73ce 4a49  JIc...JIJIc.s.JI
 000004e0: 630b 630b 630b 4a49 4a49 630b 738d 94d2  c.c.c.JIJIc.s...
 000004f0: 94d2 94d2 738d 738d 738d 94d2 4a28 4a28  ....s.s.s...J(J(
-00000500: 94d2 4a28 738d 738d 738d 0000 840f 840f  ..J(s.s.s.......
-00000510: 840f 840f adf7 840f adf7 adf7 0000 0801  ................
-00000520: 0801 0000 0801 0801 0801 0801 8430 8430  .............0.0
-00000530: 8430 8430 ae17 ae17 ae17 ae17 0000 0000  .0.0............
-00000540: 0000 0000 0000 0000 0000 0000 840f 840f  ................
-00000550: 840f 840f 8c90 8c90 840f 4a07 0000 0000  ..........J.....
-00000560: 8c90 1020 0000 0000 8c90 4a07 94f3 94f3  ... ......J.....
+00000500: 94d2 4a28 738d 738d 738d 8430 840f 840f  ..J(s.s.s..0....
+00000510: 840f 840f adf7 840f adf7 adf7 7bcf ad75  ............{..u
+00000520: ad75 7bcf ad75 ad75 ad75 ad75 8430 8430  .u{..u.u.u.u.0.0
+00000530: 8430 8430 ae17 ae17 ae17 ae17 7bef 7bef  .0.0........{.{.
+00000540: 7bef 7bef 7bef 7bef 7bef 7bef 840f 840f  {.{.{.{.{.{.....
+00000550: 840f 840f ffff ffff 840f 4a07 7bcf 7bcf  ..........J.{.{.
+00000560: ffff 1020 7bcf 7bcf ffff 4a07 94f3 94f3  ... {.{...J.....
 00000570: 94f3 94f3 94f3 ce9a ce9a 2985 94f3 94f3  ..........).....
 00000580: 94f3 2985 632c 94f3 94f3 2985 94b2 94b2  ..).c,....).....
-00000590: 94b2 94b2 94b2 cefb 94b2 cefb 94b2 0000  ................
-000005a0: 0000 0000 cefb 0000 0000 0000 a555 a555  .............U.U
-000005b0: a555 a555 a555 a555 a555 7baf 0000 0000  .U.U.U.U.U{.....
-000005c0: 0000 0000 0000 0000 0000 1003 8c30 8c30  .............0.0
-000005d0: 8c30 b638 8c30 b638 b638 8c30 0802 0802  .0.8.0.8.8.0....
-000005e0: 0000 0802 0802 0802 0802 0000 94d2 94d2  ................
+00000590: 94b2 94b2 94b2 cefb 94b2 cefb 94b2 738e  ..............s.
+000005a0: 738e 738e cefb 738e 738e 738e a555 a555  s.s...s.s.s..U.U
+000005b0: a555 a555 a555 a555 a555 7baf 8410 8410  .U.U.U.U.U{.....
+000005c0: 8410 8410 8410 8410 8410 b596 8c30 8c30  .............0.0
+000005d0: 8c30 b638 8c30 b638 b638 8c30 ad75 ad75  .0.8.0.8.8.0.u.u
+000005e0: 7bcf ad75 ad75 ad75 ad75 7bcf 94d2 94d2  {..u.u.u.u{.....
 000005f0: 73ae 2965 73ae 73ae 73ae 4a89 94d2 4a89  s.)es.s.s.J...J.
 00000600: 4a89 73ae 73ae 73ae 4a89 73ae 6b6d 8450  J.s.s.s.J.s.km.P
 00000610: 8450 8450 4a69 8450 6b6d 8450 3186 6b6d  .P.PJi.Pkm.P1.km
 00000620: 8450 8450 3186 4a69 8450 8450 840f 31c6  .P.P1.Ji.P.P..1.
 00000630: 5aea 5aea 840f 31c6 31c6 5aea 840f 08a2  Z.Z...1.1.Z.....
 00000640: 08a2 08a2 840f 31c6 5aea 31c6 3a08 5b0c  ......1.Z.1.:.[.
 00000650: 3a08 5b0c 3a08 3a08 3a08 3a08 2124 2124  :.[.:.:.:.:.!$!$
@@ -124,45 +124,45 @@
 000007b0: 4a69 31a6 4a69 4a69 4a69 31a6 18e3 18e3  Ji1.JiJiJi1.....
 000007c0: 0841 0841 31a6 4a69 31a6 4a69 5b4d 1904  .A.A1.Ji1.Ji[M..
 000007d0: 5b4d 3a28 5b4d 3a28 3a28 1904 0000 1904  [M:([M:(:(......
 000007e0: 1904 0000 3a28 3a28 3a28 3a28 6b8e ad75  ....:(:(:(:(k..u
 000007f0: 8c71 ad75 4a8a ad75 8c71 4a8a 4a8a ad75  .q.uJ..u.qJ.J..u
 00000800: 8c71 6b8e 6b8e ad75 8c71 6b8e 7bef 62eb  .qk.k..u.qk.{.b.
 00000810: a5d6 62eb 7bef 62eb a5d6 62eb 7bef 62eb  ..b.{.b...b.{.b.
-00000820: a5d6 62eb 62eb 62eb a5d6 62eb 0000 7990  ..b.b.b...b...y.
-00000830: c338 c338 0000 0000 0000 0000 0000 0000  .8.8............
-00000840: 3007 3007 0000 0000 0000 0000 8c0f 0000  0.0.............
-00000850: 1003 adb5 0000 0000 7249 adb5 1003 0000  ........rI......
-00000860: 7249 adb5 0000 0000 7249 adb5 738d 8c50  rI......rI..s..P
+00000820: a5d6 62eb 62eb 62eb a5d6 62eb 8c51 e73c  ..b.b.b...b..Q.<
+00000830: ffff ffff 8c51 8c51 8c51 8c51 8c51 8c51  .....Q.Q.Q.Q.Q.Q
+00000840: b5b6 b5b6 8c51 8c51 8c51 8c51 8c0f 8430  .....Q.Q.Q.Q...0
+00000850: ad75 adb5 8430 8430 7249 adb5 ad75 8430  .u...0.0rI...u.0
+00000860: 7249 adb5 8430 8430 7249 adb5 738d 8c50  rI...0.0rI..s..P
 00000870: 39e7 8c50 738d 8c50 39e7 8c50 8c50 738d  9..Ps..P9..P.Ps.
 00000880: 39e7 8c50 8c50 738d 39e7 738d 840f 73ae  9..P.Ps.9.s...s.
 00000890: 73ae 6b6d 73ae 840f 6b6d 6b6d 840f 8c50  s.kms...kmkm...P
 000008a0: 6b6d 6b6d 8c50 73ae 73ae 6b6d 73ae 73ae  kmkm.Ps.s.kms.s.
 000008b0: 73ae 73ae 630c 73ae 73ae 73ae 73ae 73ae  s.s.c.s.s.s.s.s.
 000008c0: 8c71 4a49 73ae 73ae 73ae 4a49 4208 52aa  .qJIs.s.s.JIB.R.
 000008d0: 52aa 52aa 4208 6b6d 52aa 52aa 52aa 6b6d  R.R.B.kmR.R.R.km
-000008e0: 52aa 6b6d 52aa 52aa 6b6d 7c0f 2004 5a0c  R.kmR.R.km|. .Z.
-000008f0: 2004 5a0c 2004 5a0c 2004 9bf4 9bf4 0000   .Z. .Z. .......
-00000900: 0000 2004 2004 0000 2004 2004 c4f8 c4f8  .. . ... . .....
-00000910: c4f8 9352 c4f8 c4f8 c4f8 9352 2806 2806  ...R.......R(.(.
-00000920: 2806 2806 61ac 61ac 2806 2806 5a2d 3008  (.(.a.a.(.(.Z-0.
-00000930: 0002 0002 5a2d 3008 0002 0002 0002 0002  ....Z-0.........
-00000940: 0002 8c72 3008 0002 8c72 5a2d 0000 9d54  ...r0....rZ-...T
+000008e0: 52aa 6b6d 52aa 52aa 6b6d 7c0f b5b6 e73c  R.kmR.R.km|....<
+000008f0: b5b6 e73c b5b6 e73c b5b6 ffff ffff 8430  ...<...<.......0
+00000900: 8430 b5b6 b5b6 8430 b5b6 b5b6 ffff ffff  .0.....0........
+00000910: ffff ffff ffff ffff ffff ffff bdd7 bdd7  ................
+00000920: bdd7 bdd7 e71c e71c bdd7 bdd7 ef5d bdd7  .............]..
+00000930: 8c71 8c71 ef5d bdd7 8c71 8c71 8c71 8c71  .q.q.]...q.q.q.q
+00000940: 8c71 ffff bdd7 8c71 ffff ef5d 8c51 9d54  .q.....q...].Q.T
 00000950: 7bef 3104 9d54 9d54 5269 3104 9d54 5269  {.1..T.TRi1..TRi
 00000960: 5269 5269 5269 3104 9d54 3104 5aeb 5aeb  RiRiRi1..T1.Z.Z.
 00000970: b5d5 3186 8c70 8c70 8c70 3186 8c70 8c70  ..1..p.p.p1..p.p
 00000980: 8c70 3186 5aeb 8c70 8c70 3186 842f a5f6  .p1.Z..p.p1../..
-00000990: 0000 0000 6268 a5f6 a5f6 0000 6268 40c2  ....bh......bh@.
-000009a0: 842f a5f6 842f 842f 40c2 a5f6 0001 3008  ./..././@.....0.
-000009b0: 698e a375 0001 3008 698e a375 0001 0001  i..u..0.i..u....
-000009c0: 0001 3008 a375 0001 3008 3008 cd59 cd59  ..0..u..0.0..Y.Y
-000009d0: cd59 620c cd59 cd59 cd59 9392 3066 3066  .Yb..Y.Y.Y..0f0f
-000009e0: 3066 3066 3066 620c 620c 3066 732c 94b2  0f0f0fb.b.0fs,..
-000009f0: 732c 732c 0802 732c 732c 732c 0000 0000  s,s,..s,s,s,....
-00000a00: 94b2 732c 0802 0000 0802 94b2 52aa 39e7  ..s,........R.9.
+00000990: 8c51 8c51 6268 a5f6 a5f6 8c51 6268 40c2  .Q.Qbh.....Qbh@.
+000009a0: 842f a5f6 842f 842f 40c2 a5f6 8c51 b5b6  ./..././@....Q..
+000009b0: e71c ffff 8c51 b5b6 e71c ffff 8c51 8c51  .....Q.......Q.Q
+000009c0: 8c51 b5b6 ffff 8c51 b5b6 b5b6 ffff ffff  .Q.....Q........
+000009d0: ffff e73c ffff ffff ffff ffff c618 c618  ...<............
+000009e0: c618 c618 c618 e73c e73c c618 732c 94b2  .......<.<..s,..
+000009f0: 732c 732c a534 732c 732c 732c 8430 8430  s,s,.4s,s,s,.0.0
+00000a00: 94b2 732c a534 8430 a534 94b2 52aa 39e7  ..s,.4.0.4..R.9.
 00000a10: 6b6d 8430 6b6d 39e7 52aa 8430 52aa 52aa  km.0km9.R..0R.R.
 00000a20: 39e7 8430 52aa 6b6d 52aa 6b6d 94d2 b5d6  9..0R.kmR.km....
 00000a30: b5d6 94d2 94d2 7bcf 7bcf 5acb 94d2 7bcf  ......{.{.Z...{.
 00000a40: 7bcf 7bcf 94d2 7bcf 94d2 7bcf a574 a574  {.{...{...{..t.t
 00000a50: a574 8c91 5acb 73ae 5acb 5acb 73ae 73ae  .t..Z.s.Z.Z.s.s.
 00000a60: 73ae 73ae 73ae 73ae 73ae 73ae 9cf3 9cf3  s.s.s.s.s.s.....
 00000a70: 9cf3 9cf3 738e 738e 738e 5aeb 738e 738e  ....s.s.s.Z.s.s.
@@ -188,47 +188,47 @@
 00000bb0: 9d33 9d33 5aec 73ae 73ae 73ae 73ae 73ae  .3.3Z.s.s.s.s.s.
 00000bc0: 73ae 73ae 73ae 73ae 73ae 73ae a555 a555  s.s.s.s.s.s..U.U
 00000bd0: a555 a555 636d 636d 7c10 636d 636d 636d  .U.Ucmcm|.cmcmcm
 00000be0: 7c10 7c10 7c10 8cb2 8cb2 8cb2 8430 94b2  |.|.|........0..
 00000bf0: 8430 6b4d 7bcf 94b2 6b4d 6b4d 8430 8430  .0kM{...kMkM.0.0
 00000c00: 7bcf 7bcf 8430 8430 6b4d 7bcf 73ae 73ae  {.{..0.0kM{.s.s.
 00000c10: adf6 5a8a 94d2 73ae 94d2 73ae 73ae 73ae  ..Z...s...s.s.s.
-00000c20: 94d2 5a8a 73ae 73ae 94d2 5a8a 0000 71cf  ..Z.s.s...Z...q.
-00000c30: bbf6 bbf6 3007 3007 bbf6 bbf6 bbf6 0000  ....0.0.........
-00000c40: 0000 0000 bbf6 0000 3007 3007 526b 0000  ........0.0.Rk..
-00000c50: 2004 b658 2004 2004 526b 9450 0000 526b   ..X . .Rk.P..Rk
-00000c60: 2004 9450 0000 8cb1 2004 9450 9491 9491   ..P.... ..P....
+00000c20: 94d2 5a8a 73ae 73ae 94d2 5a8a 8410 ef5d  ..Z.s.s...Z....]
+00000c30: ffff ffff b5b6 b5b6 ffff ffff ffff 8410  ................
+00000c40: 8410 8410 ffff 8410 b5b6 b5b6 e73c 8430  .............<.0
+00000c50: b5b6 b658 b5b6 b5b6 e73c 9450 8430 e73c  ...X.....<.P.0.<
+00000c60: b5b6 9450 8430 ffff b5b6 9450 9491 9491  ...P.0.....P....
 00000c70: 39c7 73ae 9491 73ae 39c7 73ae 9491 73ae  9.s...s.9.s...s.
 00000c80: 39c7 73ae 9491 73ae 39c7 73ae 7c0f 7c0f  9.s...s.9.s.|.|.
 00000c90: 738e 738e 8c71 738e 738e 7c0f 7c0f 7c0f  s.s..qs.s.|.|.|.
 00000ca0: 632c 738e 632c 8c71 738e 632c 7bce 9490  c,s.c,.qs.c,{...
 00000cb0: 5aeb 4229 7bce 9490 4229 5aeb 7bce 5aeb  Z.B){...B)Z.{.Z.
 00000cc0: 4229 5aeb 7bce 4229 4229 4229 5228 5228  B)Z.{.B)B)B)R(R(
 00000cd0: 73ce 9554 5228 5228 9554 5228 5228 73ce  s..TR(R(.TR(R(s.
-00000ce0: 73ce 0000 5228 9554 0000 0000 0000 0000  s...R(.T........
-00000cf0: 2005 2005 0000 714f baf8 baf8 2005 714f   . ...qO.... .qO
-00000d00: baf8 baf8 0000 0000 2005 2005 2807 2807  ........ . .(.(.
-00000d10: 2807 2807 c4f8 c4f8 c4f8 9353 c4f8 c4f8  (.(........S....
-00000d20: c4f8 9353 2807 2807 2807 2807 0803 0803  ...S(.(.(.(.....
-00000d30: 8450 2005 82eb 0803 8450 82eb 82eb 0803  .P ......P......
-00000d40: 8450 82eb 0803 0803 8450 2005 2945 7c0f  .P.......P .)E|.
+00000ce0: 73ce 8430 5228 9554 8430 8430 8410 8410  s..0R(.T.0.0....
+00000cf0: b596 b596 8410 e71c ffff ffff b596 e71c  ................
+00000d00: ffff ffff 8410 8410 b596 b596 b5b6 b5b6  ................
+00000d10: b5b6 b5b6 ffff ffff ffff ffff ffff ffff  ................
+00000d20: ffff ffff b5b6 b5b6 b5b6 b5b6 94b2 94b2  ................
+00000d30: 8450 b596 82eb 94b2 8450 82eb 82eb 94b2  .P.......P......
+00000d40: 8450 82eb 94b2 94b2 8450 b596 2945 7c0f  .P.......P..)E|.
 00000d50: 5b2b 2945 4228 7c0f 5b2b 2945 4228 7c0f  [+)EB(|.[+)EB(|.
 00000d60: 5b2b 2945 4228 7c0f 4228 2945 8c71 8c71  [+)EB(|.B()E.q.q
 00000d70: 8c71 4227 6b4c 8c71 8c71 2123 6b4c 8c71  .qB'kL.q.q!#kL.q
 00000d80: 8c71 4227 6b4c 8c71 8c71 2123 4a49 a513  .qB'kL.q.q!#JI..
 00000d90: 4a49 4a49 4a49 8430 4a49 4a49 6b2c 6b2c  JIJIJI.0JIJIk,k,
-00000da0: 4a49 4a49 6b2c 6b2c 4a49 4a49 8b31 0802  JIJIk,k,JIJI.1..
-00000db0: 0802 3007 8b31 0802 614c 8b31 8b31 0802  ..0..1..aL.1.1..
-00000dc0: 614c 8b31 8b31 0802 0802 3007 3007 3007  aL.1.1....0.0.0.
-00000dd0: 3007 3007 cd59 cd59 cd59 9393 cd59 cd59  0.0..Y.Y.Y...Y.Y
-00000de0: cd59 9393 3007 3007 3007 3007 1804 0000  .Y..0.0.0.0.....
-00000df0: 0000 9a36 9a36 58ad 0000 1804 9a36 58ad  ...6.6X......6X.
-00000e00: 1804 0000 1804 0000 0000 0000 5b0b 5b0b  ............[.[.
+00000da0: 4a49 4a49 6b2c 6b2c 4a49 4a49 ffff 9492  JIJIk,k,JIJI....
+00000db0: 9492 b5b6 ffff 9492 defb ffff ffff 9492  ................
+00000dc0: defb ffff ffff 9492 9492 b5b6 bdf7 bdf7  ................
+00000dd0: bdf7 bdf7 ffff ffff ffff ffff ffff ffff  ................
+00000de0: ffff ffff bdf7 bdf7 bdf7 bdf7 ad55 7bef  .............U{.
+00000df0: 7bef ffdf ffdf d69a 7bef ad55 ffdf d69a  {.......{..U....
+00000e00: ad55 7bef ad55 7bef 7bef 7bef 5b0b 5b0b  .U{..U{.{.{.[.[.
 00000e10: 5b0b 5b0b 8491 5b0b 5b0b 5b0b 8491 8491  [.[...[.[.[.....
-00000e20: 5b0b 5b0b 0000 8491 5b0b 5b0b 94b2 738d  [.[.....[.[...s.
+00000e20: 5b0b 5b0b 7bcf 8491 5b0b 5b0b 94b2 738d  [.[.{...[.[...s.
 00000e30: 8430 738d 94b2 8430 94b2 738d 630b 94b2  .0s....0..s.c...
 00000e40: 8430 738d 630b 8430 94b2 738d 6b6d 7c10  .0s.c..0..s.km|.
 00000e50: 73cf 632c 73cf 6b6d 73cf 73cf 6b6d 632c  s.c,s.kms.s.kmc,
 00000e60: 73cf 73cf 6b6d 73cf 6b6d 73cf 73ae 73ae  s.s.kms.kms.s.s.
 00000e70: 7bef 8430 73ae 7bef 7bef 6b6d 73ae 7bef  {..0s.{.{.kms.{.
 00000e80: 6b6d 7bef 7bef 7bef 7bef 73ae 7bcf 8410  km{.{.{.{.s.{...
 00000e90: 7bcf 8410 7bcf 7bcf 8410 8410 738e 7bcf  {...{.{.....s.{.
@@ -252,47 +252,47 @@
 00000fb0: 73ce 73ce 8430 6b8d 73ce 8c71 8430 73ce  s.s..0k.s..q.0s.
 00000fc0: 8430 8c71 73ce 8430 73ce 8430 94b3 94b3  .0.qs..0s..0....
 00000fd0: 8450 94b3 94b3 94b3 8450 73ce 8450 73ce  .P.......Ps..Ps.
 00000fe0: 94b3 a535 73ce 73ce 94b3 73ce 8c51 7c0f  ...5s.s...s..Q|.
 00000ff0: 8c51 73ce 7c0f 9492 7c0f 7c0f 7c0f 9492  .Qs.|...|.|.|...
 00001000: 8c51 73ce 9492 8c51 7c0f 73ce 738d 738d  .Qs....Q|.s.s.s.
 00001010: ad74 738d 738d 738d ad74 528a ad74 738d  .ts.s.s..tR..ts.
-00001020: 8c71 738d 8c71 528a ad74 528a 9bb2 0001  .qs..qR..tR.....
-00001030: 0001 0001 9bb2 0001 9bb2 9bb2 9bb2 0001  ................
-00001040: 9bb2 9bb2 9bb2 0001 0001 0001 0000 9534  ...............4
-00001050: 7b8e 9534 0802 9534 0802 9534 0802 9534  {..4...4...4...4
-00001060: 7b8e 7b8e 0000 9534 0802 9534 840f 840f  {.{....4...4....
+00001020: 8c71 738d 8c71 528a ad74 528a ffff 8c71  .qs..qR..tR....q
+00001030: 8c71 8c71 ffff 8c71 ffff ffff ffff 8c71  .q.q...q.......q
+00001040: ffff ffff ffff 8c71 8c71 8c71 7bef 9534  .......q.q.q{..4
+00001050: 7b8e 9534 ad55 9534 ad55 9534 ad55 9534  {..4.U.4.U.4.U.4
+00001060: 7b8e 7b8e 7bef 9534 ad55 9534 840f 840f  {.{.{..4.U.4....
 00001070: 3165 840f 840f 840f 3165 840f 840f 840f  1e......1e......
 00001080: 4a48 840f 6b2b 840f 3165 840f 8c50 7bef  JH..k+..1e...P{.
 00001090: 632d 7bef 7bef 738e 7bef 738e 7bef 7bef  c-{.{.s.{.s.{.{.
 000010a0: 738e 7bef 7bef 8c50 7bef 632d 73cf 4228  s.{.{..P{.c-s.B(
 000010b0: 5b0b 4228 5b0b 4228 4228 4228 4228 4228  [.B([.B(B(B(B(B(
 000010c0: 4228 73cf 4228 4228 5b0b 8cb2 7bae 7bae  B(s.B(B([...{.{.
-000010d0: 0000 0000 9575 0000 0000 0000 1003 0000  .....u..........
-000010e0: 0000 0000 0000 0000 0000 0000 0001 0001  ................
-000010f0: 4009 4009 0001 0001 0001 4009 4009 8110  @.@.......@.@...
-00001100: c278 c278 4009 8110 c278 c278 400a 716f  .x.x@....x.x@.qo
-00001110: 400a 400a 400a 400a 400a 400a c4b8 c4b8  @.@.@.@.@.@.....
-00001120: c4b8 9b14 c4b8 c4b8 c4b8 9b14 3006 0802  ............0...
-00001130: 722e 50aa 3006 0802 50aa 722e 722e 50aa  r.P.0...P.r.r.P.
-00001140: 3006 722e 722e 50aa 3006 0802 2944 52ca  0.r.r.P.0...)DR.
+000010d0: 8410 8410 9575 8410 8410 8410 ad75 8410  .....u.......u..
+000010e0: 8410 8410 8410 8410 8410 8410 9492 9492  ................
+000010f0: bdd7 bdd7 9492 9492 9492 bdd7 bdd7 e71c  ................
+00001100: ffff ffff bdd7 e71c ffff ffff c618 e73c  ...............<
+00001110: c618 c618 c618 c618 c618 c618 ffff ffff  ................
+00001120: ffff ffff ffff ffff ffff ffff ad75 8c71  .............u.q
+00001130: ef7d ce79 ad75 8c71 ce79 ef7d ef7d ce79  .}.y.u.q.y.}.}.y
+00001140: ad75 ef7d ef7d ce79 ad75 8c71 2944 52ca  .u.}.}.y.u.q)DR.
 00001150: 52ca 2944 3a07 2944 52ca 2944 6bae 2944  R.)D:.)DR.)Dk.)D
 00001160: 2944 2944 6bae 6bae 3a07 2944 5b0c 7c10  )D)Dk.k.:.)D[.|.
 00001170: 7c10 2924 5b0c 7c10 7c10 2924 5b0c 7c10  |.)$[.|.|.)$[.|.
 00001180: 7c10 2924 5b0c 7c10 7c10 2924 634c 634c  |.)$[.|.|.)$cLcL
 00001190: 30c3 634c 634c 30c3 4a07 7c91 30c3 4a07  0.cLcL0.J.|.0.J.
-000011a0: 7c91 7c91 4a07 7c91 7c91 0000 baf6 0803  |.|.J.|.|.......
-000011b0: 480a 480a 8130 0803 0803 480a 0803 480a  H.H..0....H...H.
-000011c0: 8130 baf6 480a 8130 8130 baf6 616e 616e  .0..H..0.0..anan
-000011d0: 616e 3009 3009 3009 3009 3009 c4d8 c4d8  an0.0.0.0.0.....
-000011e0: c4d8 9333 c4d8 c4d8 c4d8 9333 380a 0002  ...3.......38...
-000011f0: 0002 0002 0002 0002 0002 0002 c178 8051  .............x.Q
-00001200: 380a 0002 c178 8051 380a 0002 0000 6b4d  8....x.Q8.....kM
-00001210: 84d3 51a6 0000 0000 84d3 6b4d 0000 0000  ..Q.......kM....
-00001220: 6b4d 84d3 0000 0000 0000 84d3 52aa 6b6d  kM..........R.km
+000011a0: 7c91 7c91 4a07 7c91 7c91 8c51 ffff 8c71  |.|.J.|.|..Q...q
+000011b0: bdd7 bdd7 e73c 8c71 8c71 bdd7 8c71 bdd7  .....<.q.q...q..
+000011c0: e73c ffff bdd7 e73c e73c ffff defb defb  .<.....<.<......
+000011d0: defb bdd7 bdd7 bdd7 bdd7 bdd7 ffff ffff  ................
+000011e0: ffff ffff ffff ffff ffff ffff b5b6 9492  ................
+000011f0: 9492 9492 9492 9492 9492 9492 ffff dedb  ................
+00001200: b5b6 9492 ffff dedb b5b6 9492 7bef 6b4d  ............{.kM
+00001210: 84d3 51a6 7bef 7bef 84d3 6b4d 7bef 7bef  ..Q.{.{...kM{.{.
+00001220: 6b4d 84d3 7bef 7bef 7bef 84d3 52aa 6b6d  kM..{.{.{...R.km
 00001230: 9cf3 6b6d 52aa 52aa 9cf3 6b6d 52aa 52aa  ..kmR.R...kmR.R.
 00001240: 8430 8430 52aa 52aa 52aa 8430 6b6e 7bef  .0.0R.R.R..0kn{.
 00001250: 73ae 6b6e 6b6e 634d 73ae 73ae 73ae 73ae  s.knkncMs.s.s.s.
 00001260: 73ae 6b6e 73ae 73ae 7bef 6b6e 73ae 7c10  s.kns.s.{.kns.|.
 00001270: 73ae 73ae 73ae 73ae 7c10 8451 73ae 73ae  s.s.s.s.|..Qs.s.
 00001280: 73ae 7c10 7c10 7c10 73ae 6b6d 7c10 6b4d  s.|.|.|.s.km|.kM
 00001290: 7c10 7c10 8471 73ae 73ae 6b4d 73ae 7c10  |.|..qs.s.kMs.|.
@@ -316,49 +316,49 @@
 000013b0: 7bcf 7bcf 7c10 7bcf 7bcf 7bcf 8431 73ae  {.{.|.{.{.{..1s.
 000013c0: 7c10 8431 8431 7c10 8431 7c10 8c50 7c10  |..1.1|..1|..P|.
 000013d0: 73cf 7c10 7c10 7c10 73cf 8c50 7c10 7c10  s.|.|.|.s..P|.|.
 000013e0: 73cf 9491 8c50 9491 9491 8c50 842f 9d12  s....P.....P./..
 000013f0: 8c91 73ae 842f 842f 73ae 73ae 842f 73ae  ..s.././s.s../s.
 00001400: 842f 73ae 842f 73ae 73ae 73ae 7bce 630c  ./s../s.s.s.{.c.
 00001410: a553 630c 630c 8c91 a553 7bce a553 630c  .Sc.c....S{..Sc.
-00001420: a553 630c 8c91 630c 8c91 630c a473 1805  .Sc...c...c..s..
-00001430: 1805 1805 a473 1805 1805 1805 a473 1805  .....s.......s..
-00001440: 724e a473 a473 1805 724e a473 0000 a575  rN.s.s..rN.s...u
-00001450: 2865 a575 0000 a575 2865 a575 0000 a575  (e.u...u(e.u...u
-00001460: 2865 a575 0000 a575 2865 8bce 7bae 5aea  (e.u...u(e..{.Z.
+00001420: a553 630c 8c91 630c 8c91 630c ffff 9cd3  .Sc...c...c.....
+00001430: 9cd3 9cd3 ffff 9cd3 9cd3 9cd3 ffff 9cd3  ................
+00001440: f79e ffff ffff 9cd3 f79e ffff 94b2 a575  ...............u
+00001450: c618 a575 94b2 a575 c618 a575 94b2 a575  ...u...u...u...u
+00001460: c618 a575 94b2 a575 c618 8bce 7bae 5aea  ...u...u....{.Z.
 00001470: 3a07 7bae 9c92 7bae 3a07 7bae 7bae 7bae  :.{...{.:.{.{.{.
 00001480: 3a07 7bae 7bae 7bae 3a07 7bae 83ef 83ef  :.{.{.{.:.{.....
 00001490: 83ef 39c7 83ef 83ef 5acb 39c7 83ef 83ef  ..9.....Z.9.....
 000014a0: 5acb 39c7 83ef a513 5acb 39c7 3165 52ca  Z.9.....Z.9.1eR.
 000014b0: 7c0f 3165 3165 52ca 52ca 1021 3165 7c0f  |.1e1eR.R..!1e|.
-000014c0: 1021 1021 3165 7c0f 1021 1021 0000 0000  .!.!1e|..!.!....
-000014d0: 0000 0000 0000 0000 0000 0001 0000 0000  ................
-000014e0: 0000 0000 0001 0001 0001 2007 0000 0000  .......... .....
-000014f0: 0000 3008 0000 0000 3008 3008 0000 0000  ..0.....0.0.....
-00001500: 0000 3008 3008 7850 c158 c158 380a 380a  ..0.0.xP.X.X8.8.
-00001510: 380a 380a 68ce 68ce 68ce 380a 380a 380a  8.8.h.h.h.8.8.8.
-00001520: 380a 380a bb76 bb76 bb76 bb76 380a 380a  8.8..v.v.v.v8.8.
-00001530: 0002 0002 7831 380a 380a 0002 380a 380a  ....x18.8...8.8.
-00001540: 0002 0002 c138 c138 7831 7831 0000 63f0  .....8.8x1x1..c.
-00001550: 528b 4145 0000 63f0 528b 4145 0000 63f0  R.AE..c.R.AE..c.
-00001560: 528b 4145 0000 63f0 63f0 4145 6b6e 6b6e  R.AE..c.c.AEknkn
+000014c0: 1021 1021 3165 7c0f 1021 1021 0000 7bcf  .!.!1e|..!.!..{.
+000014d0: 7bcf 7bcf 7bcf 7bcf 7bcf 8c51 7bcf 7bcf  {.{.{.{.{..Q{.{.
+000014e0: 7bcf 7bcf 8c51 8c51 8c51 94b2 9492 9492  {.{..Q.Q.Q......
+000014f0: 9492 b596 9492 9492 b596 b596 9492 9492  ................
+00001500: 9492 b596 b596 d6ba ffdf ffdf b5b6 b5b6  ................
+00001510: b5b6 b5b6 dedb dedb dedb b5b6 b5b6 b5b6  ................
+00001520: b5b6 b5b6 ffff ffff ffff ffff b596 b596  ................
+00001530: 9492 9492 d6ba b596 b596 9492 b596 b596  ................
+00001540: 9492 9492 ffdf ffdf d6ba d6ba 7bef 63f0  ............{.c.
+00001550: 528b 4145 7bef 63f0 528b 4145 7bef 63f0  R.AE{.c.R.AE{.c.
+00001560: 528b 4145 7bef 63f0 63f0 4145 6b6e 6b6e  R.AE{.c.c.AEknkn
 00001570: 6b6e 2965 4a69 6b6e 6b6e 2965 4a69 6b6e  kn)eJiknkn)eJikn
 00001580: 8c72 2965 4a69 6b6e 6b6e 2965 730c 6c92  .r)eJiknkn)es.l.
-00001590: 0000 0000 730c 6c92 0000 0000 730c 6c92  ....s.l.....s.l.
-000015a0: 0000 0000 730c 6c92 0000 0802 0006 0006  ....s.l.........
-000015b0: 400b 400b 0006 400b 400b 400b 0006 0006  @.@...@.@.@.....
-000015c0: 400b 400b 8031 c117 c117 c117 300a 300a  @.@..1......0.0.
-000015d0: 300a 300a 610f 610f 610f 300a 300a 300a  0.0.a.a.a.0.0.0.
-000015e0: 300a 300a c3f8 c3f8 c3f8 9274 0000 0000  0.0........t....
-000015f0: 0000 0000 3007 3007 0000 0000 3007 0000  ....0.0.....0...
-00001600: 0000 0000 b8f8 700f 3007 0000 0000 0000  ......p.0.......
-00001610: 1000 0000 0000 0000 0000 1000 0000 0000  ................
-00001620: 0000 1000 0003 0003 0003 0000 9d54 4208  .............TB.
-00001630: 4208 73ae 73ae 73ae 4208 4208 0000 73ae  B.s.s.s.B.B...s.
-00001640: 4208 4208 0000 73ae 4208 1882 7bcf 7bcf  B.B...s.B...{.{.
+00001590: 8430 8430 730c 6c92 8430 8430 730c 6c92  .0.0s.l..0.0s.l.
+000015a0: 8430 8430 730c 6c92 8430 ad55 9cd3 9cd3  .0.0s.l..0.U....
+000015b0: b5b6 b5b6 9cd3 b5b6 b5b6 b5b6 9cd3 9cd3  ................
+000015c0: b5b6 b5b6 d6ba f7be f7be f7be b5b6 b5b6  ................
+000015d0: b5b6 b5b6 dedb dedb dedb b5b6 b5b6 b5b6  ................
+000015e0: b5b6 b5b6 ffff ffff ffff ffff 8430 8430  .............0.0
+000015f0: 8430 8430 ad55 ad55 8430 8430 ad55 8430  .0.0.U.U.0.0.U.0
+00001600: 8430 8430 f79e ce79 ad55 8430 7bcf 7bcf  .0.0...y.U.0{.{.
+00001610: 1000 8430 7bcf 7bcf 7bcf 1000 7bcf 7bcf  ...0{.{.{...{.{.
+00001620: 7bcf 1000 8c71 8c71 8c71 8430 9d54 4208  {....q.q.q.0.TB.
+00001630: 4208 73ae 73ae 73ae 4208 4208 7bef 73ae  B.s.s.s.B.B.{.s.
+00001640: 4208 4208 7bef 73ae 4208 1882 7bcf 7bcf  B.B.{.s.B...{.{.
 00001650: 6b8d 7bcf 8430 7bcf 6b8d 632c 7bcf 7bcf  k.{..0{.k.c,{.{.
 00001660: 7bcf 6b8d 632c 8430 7bcf 7bcf 6bae 6bae  {.k.c,.0{.{.k.k.
 00001670: 7bef 7bef 7bef 9492 6bae 7bef 9492 6bae  {.{.{...k.{...k.
 00001680: 8451 7bef 7bef 7bef 7bef 6bae 6b8e 73cf  .Q{.{.{.{.k.k.s.
 00001690: 73cf 8430 8430 6b8e 73cf 8430 6b8e 8c71  s..0.0k.s..0k..q
 000016a0: 73cf 73cf 8430 8c71 8c71 8430 73af 6b6e  s.s..0.q.q.0s.kn
 000016b0: 7c0f 8450 6b6e 73af 73af 7c0f 7c0f 7c0f  |..Pkns.s.|.|.|.
@@ -380,46 +380,46 @@
 000017b0: 8410 7bef 8410 7bef 8410 73ae 8410 8410  ..{...{...s.....
 000017c0: 7bef 7bef 8c51 7bef 7bef 8c51 73cf 73cf  {.{..Q{.{..Qs.s.
 000017d0: 8c70 6b6e 8c70 840f 73cf 8c70 840f 8c70  .pkn.p..s..p...p
 000017e0: 73cf 6b6e 73cf 73cf 840f 73cf 8490 7c2f  s.kns.s...s...|/
 000017f0: 73ae 7c2f 6b4d 73ae 73ae 73ae 7c2f 6b4d  s.|/kMs.s.s.|/kM
 00001800: 6b4d 73ae 7c2f 73ae 7c2f 6b4d 6b4d 6b4d  kMs.|/s.|/kMkMkM
 00001810: 8470 6b4d 6b4d 8470 9d74 5249 8470 8470  .pkMkM.p.tRI.p.p
-00001820: 8470 8470 9d74 6b4d 9d74 9d74 a3f3 0003  .p.p.tkM.t.t....
-00001830: 0003 0003 a3f3 0003 3809 3809 a3f3 0003  ........8.8.....
-00001840: 0003 0003 0003 3809 a3f3 a3f3 0000 a575  ......8........u
-00001850: 8bae 8bae 0000 a575 1003 a575 0000 a575  .......u...u...u
-00001860: a575 8bae 8bae 0000 a575 8bae 73ae 73ae  .u.......u..s.s.
+00001820: 8470 8470 9d74 6b4d 9d74 9d74 ffff 9492  .p.p.tkM.t.t....
+00001830: 9492 9492 ffff 9492 bdf7 bdf7 ffff 9492  ................
+00001840: 9492 9492 9492 bdf7 ffff ffff 8410 a575  ...............u
+00001850: 8bae 8bae 8410 a575 ad75 a575 8410 a575  .......u.u.u...u
+00001860: a575 8bae 8bae 8410 a575 8bae 73ae 73ae  .u.......u..s.s.
 00001870: 39c7 73ae 73ae 73ae 39c7 73ae 73ae 73ae  9.s.s.s.9.s.s.s.
 00001880: 39c7 73ae 73ae 8cb2 39c7 8cb2 8c91 6b8d  9.s.s...9.....k.
 00001890: 4a89 31a6 8c91 4a89 31a6 31a6 6b8d 31a6  J.1...J.1.1.k.1.
 000018a0: 31a6 31a6 4a89 31a6 31a6 31a6 3186 528a  1.1.J.1.1.1.1.R.
 000018b0: 738e 1082 3186 3186 528a 528a 3186 3186  s...1.1.R.R.1.1.
-000018c0: 1082 3186 3186 3186 3186 3186 0000 0000  ..1.1.1.1.1.....
-000018d0: 0000 0000 4aaa 4aaa 4aaa 4aaa 4aaa 4aaa  ....J.J.J.J.J.J.
-000018e0: 4aaa 4aaa 3965 3965 3965 3965 0000 0000  J.J.9e9e9e9e....
-000018f0: 0000 4a48 4a48 4b4c 0000 0000 4a48 4a48  ..JHJHKL....JHJH
-00001900: 4a48 4a48 4965 4965 4965 4965 4867 4867  JHJHIeIeIeIeHgHg
-00001910: 4867 4867 41c7 2003 41c7 41c7 41c7 41c7  HgHgA. .A.A.A.A.
-00001920: 41c7 41c7 2187 2187 2187 2187 1803 3806  A.A.!.!.!.!...8.
-00001930: 3806 3806 4208 4208 4208 4208 4208 4208  8.8.B.B.B.B.B.B.
-00001940: 4208 2b0c 4208 4208 4208 4208 0000 6bae  B.+.B.B.B.B...k.
+000018c0: 1082 3186 3186 3186 3186 3186 7bcf 7bcf  ..1.1.1.1.1.{.{.
+000018d0: 7bcf 7bcf 4aaa 4aaa 4aaa 4aaa 4aaa 4aaa  {.{.J.J.J.J.J.J.
+000018e0: 4aaa 4aaa 3965 3965 3965 3965 8c51 8c51  J.J.9e9e9e9e.Q.Q
+000018f0: 9cf3 4a48 4a48 4b4c 9cf3 9cf3 4a48 4a48  ..JHJHKL....JHJH
+00001900: 4a48 4a48 4965 4965 4965 4965 ce59 ce59  JHJHIeIeIeIe.Y.Y
+00001910: ce59 ce59 41c7 b5b6 41c7 41c7 41c7 41c7  .Y.YA...A.A.A.A.
+00001920: 41c7 41c7 2187 2187 2187 2187 a534 a514  A.A.!.!.!.!..4..
+00001930: a514 a514 4208 4208 4208 4208 4208 4208  ....B.B.B.B.B.B.
+00001940: 4208 2b0c 4208 4208 4208 4208 8430 6bae  B.+.B.B.B.B..0k.
 00001950: 52aa 20a2 52aa 6bae 52aa 20a2 52aa 39a6  R. .R.k.R. .R.9.
 00001960: 39a6 20a2 39a6 39a6 52aa 20a2 4269 6b8e  9. .9.9.R. .Bik.
 00001970: 94b2 2145 4269 6b8e 4269 2145 4269 6b8e  ..!EBik.Bi!EBik.
 00001980: 4269 2145 4269 6b8e 94b2 2145 4aca 5c0f  Bi!EBik...!EJ.\.
-00001990: 0000 0000 4aca 5c0f 0000 4aca 4aca 4165  ....J.\...J.J.Ae
-000019a0: 4aca 4aca 4aca 4165 4165 4165 5009 5009  J.J.J.AeAeAeP.P.
-000019b0: 5009 3006 49c7 49c7 49c7 49c7 2a8a 2a8a  P.0.I.I.I.I.*.*.
-000019c0: 2a8a 2a8a 49c7 49c7 49c7 49c7 588a 588a  *.*.I.I.I.I.X.X.
-000019d0: 588a 588a 4a08 0001 4a08 0001 29c7 4a08  X.X.J...J...).J.
-000019e0: 4a08 4a08 29c7 29c7 29c7 29c7 0000 0001  J.J.).).).).....
-000019f0: 0001 0001 49a7 3a6a 3a6a 3a6a 3a6a 3a6a  ....I.:j:j:j:j:j
-00001a00: 3a6a 3a6a 49a7 49a7 49a7 49a7 0000 0000  :j:jI.I.I.I.....
-00001a10: 0000 0000 0000 4acb 39c7 4acb 39c7 4acb  ......J.9.J.9.J.
+00001990: 8410 8410 4aca 5c0f 9cd3 4aca 4aca 4165  ....J.\...J.J.Ae
+000019a0: 4aca 4aca 4aca 4165 4165 4165 b596 b596  J.J.J.AeAeAe....
+000019b0: b596 ad75 49c7 49c7 49c7 49c7 2a8a 2a8a  ...uI.I.I.I.*.*.
+000019c0: 2a8a 2a8a 49c7 49c7 49c7 49c7 ce79 ce79  *.*.I.I.I.I..y.y
+000019d0: ce79 ce79 4a08 ad55 4a08 ad55 29c7 4a08  .y.yJ..UJ..U).J.
+000019e0: 4a08 4a08 29c7 29c7 29c7 29c7 9cd3 8c71  J.J.).).).)....q
+000019f0: 8c71 8c71 49a7 3a6a 3a6a 3a6a 3a6a 3a6a  .q.qI.:j:j:j:j:j
+00001a00: 3a6a 3a6a 49a7 49a7 49a7 49a7 7bcf 7bcf  :j:jI.I.I.I.{.{.
+00001a10: 7bcf 7bcf 9492 4acb 39c7 4acb 39c7 4acb  {.{...J.9.J.9.J.
 00001a20: 4acb 4acb 28e3 39c7 39c7 39c7 6b6d 6b6d  J.J.(.9.9.9.kmkm
 00001a30: 31a6 31a6 52ca 31a6 4228 31a6 31a6 31a6  1.1.R.1.B(1.1.1.
 00001a40: 4228 31a6 31a6 4228 4228 31a6 4229 7bef  B(1.1.B(B(1.B){.
 00001a50: 7bef 7bef 2966 7bef 7bef 7bef 2966 4229  {.{.)f{.{.{.)fB)
 00001a60: 7bef 7bef 2966 2966 7bef 5b0c 7c30 8c71  {.{.)f)f{.[.|0.q
 00001a70: 7c30 73cf 94d2 73cf 73cf 8c71 7c30 7c30  |0s...s.s..q|0|0
 00001a80: 94d2 94d2 73cf 7c30 8c71 73cf 9492 9492  ....s.|0.qs.....
@@ -444,19 +444,19 @@
 00001bb0: 8410 7bcf 7bcf 6b8e 7bcf 7bcf 8410 6b8e  ..{.{.k.{.{...k.
 00001bc0: 634d 6b8e 6b8e 634d 6b8e 634d 8c70 7bef  cMk.k.cMk.cM.p{.
 00001bd0: 6b6d 7bef 8c70 7bef 6b6d 6b6d 6b6d 8c70  km{..p{.kmkmkm.p
 00001be0: 5aec 7bef 6b6d 8c70 6b6d 7bef 73ae 73ae  Z.{.km.pkm{.s.s.
 00001bf0: 7c30 73ae 73ae 634d 7c30 634d 7c30 5acb  |0s.s.cM|0cM|0Z.
 00001c00: 634d 634d 73ae 7c30 73ae 634d 8471 8471  cMcMs.|0s.cM.q.q
 00001c10: ae38 5aa9 8471 8471 ae38 5aa9 8471 5aa9  .8Z..q.q.8Z..qZ.
-00001c20: ae38 5aa9 8471 5aa9 ae38 5aa9 0806 8992  .8Z..qZ..8Z.....
-00001c30: c358 c358 0806 0806 0806 0806 0806 0806  .X.X............
-00001c40: 480c 480c 0806 0806 0806 0806 8bcf 0004  H.H.............
-00001c50: 2007 9575 0004 0004 8a28 9575 2007 0004   ..u.....(.u ...
-00001c60: 8bcf 9575 0004 0004 8a28 9575 94b2 6b4d  ...u.....(.u..kM
+00001c20: ae38 5aa9 8471 5aa9 ae38 5aa9 94b2 ef7d  .8Z..qZ..8Z....}
+00001c30: ffff ffff 94b2 94b2 94b2 94b2 94b2 94b2  ................
+00001c40: c618 c618 94b2 94b2 94b2 94b2 8bcf 8c71  ...............q
+00001c50: b596 9575 8c71 8c71 8a28 9575 b596 8c71  ...u.q.q.(.u...q
+00001c60: 8bcf 9575 8c71 8c71 8a28 9575 94b2 6b4d  ...u.q.q.(.u..kM
 00001c70: 39e7 94b2 6b4d 6b4d c618 39e7 6b4d 6b4d  9...kMkM..9.kMkM
 00001c80: 94b2 39e7 6b4d 6b4d 94b2 39e7 528a 528a  ..9.kMkM..9.R.R.
 00001c90: 528a 528a 0821 528a 528a 20e4 20e4 39a7  R.R..!R.R. . .9.
 00001ca0: 39a7 20e4 20e4 528a 528a 20e4 52aa 39c7  9. . .R.R. .R.9.
 00001cb0: 52aa 73ae 39c7 8cb2 8cb2 73ae 39c7 8cb2  R.s.9.....s.9...
 00001cc0: 8cb2 52aa 39c7 8cb2 8cb2 52aa 526a 526a  ..R.9.....R.RjRj
 00001cd0: 526a 526a 7bcf 7bcf 7bcf 8c71 8c71 7bcf  RjRj{.{.{..q.q{.
@@ -506,21 +506,21 @@
 00001f90: 6b4d 73ae 8430 6b4d 73ae 6b4d 73ae 6b4d  kMs..0kMs.kMs.kM
 00001fa0: 6b4d 6b4d 73ae 8430 73ae 6b4d 73ae 73ae  kMkMs..0s.kMs.s.
 00001fb0: 632d 632d 73ae 73ae 632d 7c10 632d 632d  c-c-s.s.c-|.c-c-
 00001fc0: 632d 73ae 632d 73ae 632d 5acb 73ce 73ce  c-s.c-s.c-Z.s.s.
 00001fd0: 8450 73ce 73ce 6b4d 73ce 73ce 6b4d 5acb  .Ps.s.kMs.s.kMZ.
 00001fe0: 73ce 6b4d 73ce 73ce 6b4d 5acb 73ae 73ae  s.kMs.s.kMZ.s.s.
 00001ff0: 6b2d 73ae 73ae 6b2d 73ae 6b2d 73ae 6b2d  k-s.s.k-s.k-s.k-
-00002000: 524a 73ae 73ae 6b2d 73ae 6b2d 9d53 18a3  RJs.s.k-s.k-.S..
-00002010: b698 18a3 9d53 18a3 b698 18a3 840f 9d53  .....S.........S
-00002020: b698 18a3 9d53 9d53 b698 18a3 2809 9193  .....S.S....(...
-00002030: c358 c358 2809 9193 c358 c358 2809 2809  .X.X(....X.X(.(.
-00002040: 2809 2809 2809 2809 580e 580e 51ab 3008  (.(.(.(.X.X.Q.0.
-00002050: 51ab 9dd6 51ab 3008 51ab 9dd6 3008 3008  Q...Q.0.Q...0.0.
-00002060: 51ab 9dd6 4009 3008 51ab 9dd6 73ae 73ae  Q...@.0.Q...s.s.
+00002000: 524a 73ae 73ae 6b2d 73ae 6b2d 9d53 bdf7  RJs.s.k-s.k-.S..
+00002010: b698 bdf7 9d53 bdf7 b698 bdf7 840f 9d53  .....S.........S
+00002020: b698 bdf7 9d53 9d53 b698 bdf7 9cf3 ef7d  .....S.S.......}
+00002030: ffff ffff 9cf3 ef7d ffff ffff 9cf3 9cf3  .......}........
+00002040: 9cf3 9cf3 9cf3 9cf3 c638 c638 defb 9cd3  .........8.8....
+00002050: defb 9dd6 defb 9cd3 defb 9dd6 9cd3 9cd3  ................
+00002060: defb 9dd6 bdf7 9cd3 defb 9dd6 73ae 73ae  ............s.s.
 00002070: ad54 39e7 73ae 73ae ad54 39e7 73ae 73ae  .T9.s.s..T9.s.s.
 00002080: ad54 39e7 73ae 73ae ad54 39e7 0841 39e8  .T9.s.s..T9..A9.
 00002090: 39e8 0841 0841 39e8 39e8 0841 0841 5acc  9..A.A9.9..A.AZ.
 000020a0: 5acc 2104 2104 39e8 39e8 2104 39c7 ad95  Z.!.!.9.9.!.9...
 000020b0: 8450 5b0b 39c7 8450 8450 5b0b 39c7 8450  .P[.9..P.P[.9..P
 000020c0: 8450 5b0b 39c7 ad95 8450 5b0b 738e 5aec  .P[.9....P[.s.Z.
 000020d0: 738e 632d 738e 632d 5aec 738e 738e 738e  s.c-s.c-Z.s.s.s.
@@ -572,19 +572,19 @@
 000023b0: 6b8d 7c30 73cf 632c 73cf 7c30 6b8d 6b8d  k.|0s.c,s.|0k.k.
 000023c0: 632c 7c30 73cf 73cf 7c30 73cf 632c 6b8d  c,|0s.s.|0s.c,k.
 000023d0: 6b8d 6b8d 632c 7bce 6b8d 6b8d 7bce 632c  k.k.c,{.k.k.{.c,
 000023e0: 632c 7bce 6b8d 6b8d 7bce 842f 632c 73ae  c,{.k.k.{../c,s.
 000023f0: 632c 73ae 7c10 73ae 5aca 73ae 632c 632c  c,s.|.s.Z.s.c,c,
 00002400: 73ae 5aca 632c 632c 632c 632c 73ad 73ad  s.Z.c,c,c,c,s.s.
 00002410: 9d12 8450 8450 8450 9d12 73ad 9d12 9d12  ...P.P.P..s.....
-00002420: 9d12 5aeb 8450 9d12 9d12 73ad 2007 2007  ..Z..P....s. . .
-00002430: 2007 2007 9c73 2007 9c73 9c73 9c73 2007   . ..s ..s.s.s .
-00002440: 9c73 9c73 9c73 2007 2007 2007 0000 2004  .s.s.s . . ... .
-00002450: 8430 8430 2004 9617 2004 8430 2004 9617  .0.0 ... ..0 ...
-00002460: 2004 8430 0000 9617 8430 8430 7bef 7bef   ..0.....0.0{.{.
+00002420: 9d12 5aeb 8450 9d12 9d12 73ad a514 a514  ..Z..P....s.....
+00002430: a514 a514 ffff a514 ffff ffff ffff a514  ................
+00002440: ffff ffff ffff a514 a514 a514 8c51 b5b6  .............Q..
+00002450: 8430 8430 b5b6 9617 b5b6 8430 b5b6 9617  .0.0.......0....
+00002460: b5b6 8430 8c51 9617 8430 8430 7bef 7bef  ...0.Q...0.0{.{.
 00002470: b5b6 4208 7bef 7bef b5b6 4208 7bef 7bef  ..B.{.{...B.{.{.
 00002480: b5b6 4208 7bef 7bef b5b6 4208 18e3 52cb  ..B.{.{...B...R.
 00002490: 52cb 31c7 0000 31c7 31c7 18e3 0000 52cb  R.1...1.1.....R.
 000024a0: 52cb 18e3 18e3 52cb 31c7 18e3 31c7 ad54  R.....R.1...1..T
 000024b0: 8430 5aeb 31c7 ad54 8430 5aeb 31c7 ad54  .0Z.1..T.0Z.1..T
 000024c0: 8430 5aeb 31c7 ad54 8430 5aeb 634d 634d  .0Z.1..T.0Z.cMcM
 000024d0: 7c10 73ae 634d 5aeb 634d 634d 634d 634d  |.s.cMZ.cMcMcMcM
@@ -636,19 +636,19 @@
 000027b0: 7c0f 8c91 7c0f 7c0f 632c 73ae 7c0f 73ae  |...|.|.c,s.|.s.
 000027c0: 73ae 632c 7c0f 8c91 73ae 7c0f 73ae 842f  s.c,|...s.|.s../
 000027d0: 94b1 842f 842f 94b1 842f 632c 632c 842f  ..././.../c,c,./
 000027e0: 632c 632c 73ae 842f 632c 73ae 6b2c 5acb  c,c,s../c,s.k,Z.
 000027f0: 73ae 6b2c 840f 73ae 6b2c 6b2c 6b2c 6b2c  s.k,..s.k,k,k,k,
 00002800: 6b2c 5acb 6b2c 73ae 5acb 6b2c ad74 9491  k,Z.k,s.Z.k,.t..
 00002810: ad74 73ad 73ad 73ad 9491 73ad 9491 5aca  .ts.s.s...s...Z.
-00002820: ad74 5aca 5aca 73ad ad74 5aca a474 0804  .tZ.Z.s..tZ..t..
-00002830: 400a 400a a474 0804 0804 0804 722f 400a  @.@..t......r/@.
-00002840: a474 a474 a474 400a a474 a474 0000 9d75  .t.t.t@..t.t...u
-00002850: 2025 9d75 0000 9d75 8bae 8bae 2025 9d75   %.u...u.... %.u
-00002860: 2025 9d75 2025 9d75 2025 9d75 73cf 73cf   %.u %.u %.us.s.
+00002820: ad74 5aca 5aca 73ad ad74 5aca ffff 9492  .tZ.Z.s..tZ.....
+00002830: bdf7 bdf7 ffff 9492 9492 9492 ef7d bdf7  .............}..
+00002840: ffff ffff ffff bdf7 ffff ffff 9492 9d75  ...............u
+00002850: bdd7 9d75 9492 9d75 8bae 8bae bdd7 9d75  ...u...u.......u
+00002860: bdd7 9d75 bdd7 9d75 bdd7 9d75 73cf 73cf  ...u...u...us.s.
 00002870: ad96 3a08 73cf 73cf ad96 3a08 73cf 73cf  ..:.s.s...:.s.s.
 00002880: ad96 3a08 73cf 73cf ad96 3a08 1904 5b0c  ..:.s.s...:...[.
 00002890: 3a08 3a08 0000 3a08 3a08 1904 0000 3a08  :.:...:.:.....:.
 000028a0: 3a08 1904 1904 5b0c 5b0c 1904 39c7 ad54  :.....[.[...9..T
 000028b0: 8430 5aeb 39c7 ad54 8430 5aeb 39c7 ad54  .0Z.9..T.0Z.9..T
 000028c0: ad54 5aeb 39c7 ad54 8430 5aeb 6b8e 634d  .TZ.9..T.0Z.k.cM
 000028d0: 634d 7bce 6b8e 634d 6b8e 840f 634d 634d  cM{.k.cMk...cMcM
@@ -700,19 +700,19 @@
 00002bb0: 9492 8431 6b8e 7bef 8431 9492 7bef 7bef  ...1k.{..1..{.{.
 00002bc0: 7bef 9492 7bef 8431 8431 7bef 9cd3 8c51  {...{..1.1{....Q
 00002bd0: 73ef 636d 73ef 73ef 8c51 8c51 73ef 73ef  s.cms.s..Q.Qs.s.
 00002be0: 8c51 73ef 8c51 9cd3 73ef 73ef 6b8d 634c  .Qs..Q..s.s.k.cL
 00002bf0: 7c10 6b8d 73cf 6b8d 7c10 7c10 7c10 634c  |.k.s.k.|.|.|.cL
 00002c00: 73cf 73cf 6b8d 6b8d 73cf 7c10 73ae 73ae  s.s.k.k.s.|.s.s.
 00002c10: adf5 528a 73ae 73ae 8cd1 528a 8cd1 8cd1  ..R.s.s...R.....
-00002c20: 8cd1 528a 8cd1 8cd1 8cd1 528a 94d2 1806  ..R.......R.....
-00002c30: 1806 1806 94d2 1806 404a 404a 94d2 1806  ........@J@J....
-00002c40: 1806 1806 6a8e 1806 94d2 94d2 0000 95f7  ....j...........
-00002c50: 8430 95f7 0000 95f7 1804 8430 0000 95f7  .0.........0....
-00002c60: 1804 8430 1804 8430 1804 8430 8451 632c  ...0...0...0.Qc,
+00002c20: 8cd1 528a 8cd1 8cd1 8cd1 528a ffff 9cd3  ..R.......R.....
+00002c30: 9cd3 9cd3 ffff 9cd3 c638 c638 ffff 9cd3  .........8.8....
+00002c40: 9cd3 9cd3 f79e 9cd3 ffff ffff 8430 95f7  .............0..
+00002c50: 8430 95f7 8430 95f7 b596 8430 8430 95f7  .0...0.....0.0..
+00002c60: b596 8430 b596 8430 b596 8430 8451 632c  ...0...0...0.Qc,
 00002c70: a555 4228 632c 8451 a555 4228 632c 632c  .UB(c,.Q.UB(c,c,
 00002c80: a555 4228 632c 632c a555 4228 18e3 52aa  .UB(c,c,.UB(..R.
 00002c90: 31c6 31c6 18e3 52aa 52aa 31c6 0000 31c6  1.1...R.R.1...1.
 00002ca0: 31c6 18e3 0000 52aa 52aa 18e3 31c6 94b2  1.....R.R...1...
 00002cb0: 94b2 52aa 31c6 94b2 94b2 52aa 31c6 94b2  ..R.1.....R.1...
 00002cc0: 94b2 73ae 31c6 94b2 94b2 73ae 5aec 632d  ..s.1.....s.Z.c-
 00002cd0: 6b6d 73ae 73ae 6b6d 632d 73ae 5aec 73ae  kms.s.kmc-s.Z.s.
@@ -764,19 +764,19 @@
 00002fb0: 6baf 94b2 6baf 6baf 8430 94b2 5b2d 8430  k...k.k..0..[-.0
 00002fc0: 94b2 8430 6baf 94b2 8430 8430 8450 8c91  ...0k....0.0.P..
 00002fd0: 8410 7bcf 8450 8410 7bcf 8450 8c91 8410  ..{..P..{..P....
 00002fe0: 8410 7bcf 8450 8450 7bcf 7bcf 6b8e 73ae  ..{..P.P{.{.k.s.
 00002ff0: 7bef 7bef 73ae 73ae 7bef 6b8e 73ae 840f  {.{.s.s.{.k.s...
 00003000: 6b8e 7bef 7bef 7bef 7bef 7bef 7c0f 9d94  k.{.{.{.{.{.|...
 00003010: c6f9 52aa 7c0f 52aa 7c0f 7c0f 9d94 52aa  ..R.|.R.|.|...R.
-00003020: 9d94 9d94 7c0f 7c0f 9d94 52aa 7ab0 486b  ....|.|...R.z.Hk
-00003030: acf4 acf4 acf4 1807 1807 1807 1807 1807  ................
-00003040: 486b 486b 1807 1807 1807 1807 1805 95b6  HkHk............
-00003050: 1805 95b6 0001 95b6 95b6 93ef 0001 0001  ................
-00003060: 93ef 95b6 0001 0001 1805 95b6 73cf 73cf  ............s.s.
+00003020: 9d94 9d94 7c0f 7c0f 9d94 52aa ffdf ce59  ....|.|...R....Y
+00003030: ffff ffff ffff 9cd3 9cd3 9cd3 9cd3 9cd3  ................
+00003040: ce59 ce59 9cd3 9cd3 9cd3 9cd3 b5b6 95b6  .Y.Y............
+00003050: b5b6 95b6 8c71 95b6 95b6 93ef 8c71 8c71  .....q.......q.q
+00003060: 93ef 95b6 8c71 8c71 b5b6 95b6 73cf 73cf  .....q.q....s.s.
 00003070: ad75 3a08 73cf 73cf ad75 3a08 73cf 73cf  .u:.s.s..u:.s.s.
 00003080: ad75 3a08 73cf 73cf ad75 3a08 18e4 5aec  .u:.s.s..u:...Z.
 00003090: 39e8 18e4 18e4 5aec 39e8 39e8 0000 39e8  9.....Z.9.9...9.
 000030a0: 39e8 18e4 0000 39e8 39e8 18e4 39e7 9491  9.....9.9...9...
 000030b0: bdd6 632c 39e7 bdd6 9491 632c 39e7 bdd6  ..c,9.....c,9...
 000030c0: 9491 632c 39e7 bdd6 9491 632c 8450 73ae  ..c,9.....c,.Ps.
 000030d0: 6b4d 6b4d 6b4d 73ae 6b4d 8450 7bef 73ae  kMkMkMs.kM.P{.s.
@@ -826,21 +826,21 @@
 00003390: 73af 6b6e 8451 7c10 73af 7c10 7c10 8451  s.kn.Q|.s.|.|..Q
 000033a0: 8451 7c10 8451 8451 8451 73af 94d2 7c10  .Q|..Q.Q.Qs...|.
 000033b0: 7c10 8c71 7c10 8c71 7c10 7c10 7c10 7c10  |..q|..q|.|.|.|.
 000033c0: a533 8c71 7c10 8c71 7c10 8c71 8450 7bcf  .3.q|..q|..q.P{.
 000033d0: 6b6d 7bcf 8450 8450 6b6d 7bcf 8450 7bcf  km{..P.Pkm{..P{.
 000033e0: 7bcf 7bcf 8450 94b2 6b6d 7bcf 6b8e 6b8e  {.{..P..km{.k.k.
 000033f0: 842f 634d 7bee 7bee 7bee 7bee 634d 6b8e  ./cM{.{.{.{.cMk.
-00003400: 6b8e 842f 7bee 634d 842f 6b8e 20c4 20c4  k../{.cM./k. . .
-00003410: b6da 20c4 8c50 20c4 b6da 20c4 8c50 20c4  .. ..P ... ..P .
-00003420: b6da 20c4 8c50 20c4 b6da 20c4 480b 9b54  .. ..P ... .H..T
-00003430: cdb9 cdb9 480b 9b54 cdb9 cdb9 480b 480b  ....H..T....H.H.
-00003440: 480b 480b 480b 480b 70f0 70f0 9c92 482a  H.H.H.H.p.p...H*
-00003450: 482a a658 9c92 482a 482a a658 2006 2006  H*.X..H*H*.X . .
-00003460: 482a a658 482a 2006 482a a658 7bee 7bee  H*.XH* .H*.X{.{.
+00003400: 6b8e 842f 7bee 634d 842f 6b8e c618 c618  k../{.cM./k.....
+00003410: b6da c618 8c50 c618 b6da c618 8c50 c618  .....P.......P..
+00003420: b6da c618 8c50 c618 b6da c618 ad75 ffff  .....P.......u..
+00003430: ffff ffff ad75 ffff ffff ffff ad75 ad75  .....u.......u.u
+00003440: ad75 ad75 ad75 ad75 defb defb ffff c638  .u.u.u.u.......8
+00003450: c638 a658 ffff c638 c638 a658 9cd3 9cd3  .8.X...8.8.X....
+00003460: c638 a658 c638 9cd3 c638 a658 7bee 7bee  .8.X.8...8.X{.{.
 00003470: b5b5 4228 7bee 7bee b5b5 4228 7bee 7bee  ..B({.{...B({.{.
 00003480: b5b5 4228 7bee 7bee b5b5 4228 18c3 634d  ..B({.{...B(..cM
 00003490: 634d 18c3 18c3 4a69 3186 3186 18c3 634d  cM....Ji1.1...cM
 000034a0: 4a69 3186 18c3 3186 3186 18c3 39e7 ad75  Ji1...1.1...9..u
 000034b0: ad75 8450 39e7 ad75 8450 8450 39e7 ad75  .u.P9..u.P.P9..u
 000034c0: 8450 8450 39e7 ad75 8450 8450 9491 6b2b  .P.P9..u.P.P..k+
 000034d0: 840f 6b2b 840f 840f 7bad 9491 9491 840f  ..k+....{.......
@@ -892,19 +892,19 @@
 000037b0: 8430 6b8e 8c71 73cf 8430 8430 73cf 73cf  .0k..qs..0.0s.s.
 000037c0: 8430 6b8e 8430 73cf 8430 6b8e 7bcf 7bcf  .0k..0s..0k.{.{.
 000037d0: 7c0f 73ae 7bcf 7bcf 73ae 73ae 8430 7bcf  |.s.{.{.s.s..0{.
 000037e0: 73ae 7bcf 73ae 7c0f 73ae 7bcf 6b6d 6b6d  s.{.s.|.s.{.kmkm
 000037f0: 7bee 6b6d 7bee 5b0d 5b0d 52ac 6b6d 6b6d  {.km{.[.[.R.kmkm
 00003800: 6b6d 6b6d 6b6d 7bee 7bee 6b6d 94d2 94d2  kmkmkm{.{.km....
 00003810: cffd 734c 734c 734c ae78 734c 94d2 94d2  ..sLsLsL.xsL....
-00003820: ae78 734c 734c 734c 94d2 94d2 3809 3809  .xsLsLsL....8.8.
-00003830: 3809 3809 3809 9b73 cdd9 cdd9 3809 9b73  8.8.8..s....8..s
-00003840: cdd9 cdd9 3809 3809 3809 3809 0804 0804  ....8.8.8.8.....
-00003850: 3848 b679 94d2 3848 3848 b679 94d2 0804  8H.y..8H8H.y....
-00003860: 3848 b679 0804 0804 94d2 ac71 9492 6b6d  8H.y.......q..km
+00003820: ae78 734c 734c 734c 94d2 94d2 ad55 ad55  .xsLsLsL.....U.U
+00003830: ad55 ad55 ad55 ffff ffff ffff ad55 ffff  .U.U.U.......U..
+00003840: ffff ffff ad55 ad55 ad55 ad55 94b2 94b2  .....U.U.U.U....
+00003850: c618 b679 ffff c618 c618 b679 ffff 94b2  ...y.......y....
+00003860: c618 b679 94b2 94b2 ffff ac71 9492 6b6d  ...y.......q..km
 00003870: b596 4a69 6b6d 6b6d b596 4a69 6b6d 6b6d  ..Jikmkm..Jikmkm
 00003880: b596 4a69 9492 6b6d b596 4a69 0000 5acb  ..Ji..km..Ji..Z.
 00003890: 5acb 18e3 18e3 5acb 39c7 18e3 18e3 5acb  Z.....Z.9.....Z.
 000038a0: 5acb 39c7 0000 39c7 39c7 18e3 39e7 ad54  Z.9...9.9...9..T
 000038b0: 8430 8430 39e7 ad54 8430 8430 39e7 ad54  .0.09..T.0.09..T
 000038c0: 8430 8430 39e7 ad54 8430 5b0b 9491 8430  .0.09..T.0[....0
 000038d0: 7bae 9491 9491 7bae 9491 8430 8430 6b4d  {.....{....0.0kM
@@ -956,19 +956,19 @@
 00003bb0: 73ae 6b4d 840f 73ae 73ae 73ae 8c70 73ae  s.kM..s.s.s..ps.
 00003bc0: 840f 73ae 73ae 840f 73ae 6b4d 7bef 7bef  ..s.s...s.kM{.{.
 00003bd0: 73ae 6b6d 6b6d 73ae 73ae 73ae 73ae 6b6d  s.kmkms.s.s.s.km
 00003be0: 8430 6b6d 7bef 6b6d 73ae 8430 73ae 632c  .0km{.kms..0s.c,
 00003bf0: 632c 632c 73ae 632c 73ae 5aeb 73ae 5aeb  c,c,s.c,s.Z.s.Z.
 00003c00: 6b6d 73ae 73ae 6b6d 73ae 5aeb 5aeb 7c0f  kms.s.kms.Z.Z.|.
 00003c10: a512 7c0f 7c0f 7c0f a512 5aeb a512 7c0f  ..|.|.|...Z...|.
-00003c20: a512 7c0f a512 a512 8c90 5aeb ad55 1806  ..|.......Z..U..
-00003c30: 484b 484b ad55 1806 1806 484b 7ad0 484b  HKHK.U....HKz.HK
-00003c40: ad55 ad55 7ad0 484b ad55 ad55 0000 9e38  .U.Uz.HK.U.U...8
-00003c50: 9471 9471 0000 9e38 2045 9471 2045 9e38  .q.q...8 E.q E.8
-00003c60: 2045 9471 2045 9e38 2045 9e38 9491 6b6d   E.q E.8 E.8..km
+00003c20: a512 7c0f a512 a512 ffff 5aeb ffff 94b2  ..|.......Z.....
+00003c30: ce59 ce59 ffff 94b2 94b2 ce59 ffdf ce59  .Y.Y.......Y...Y
+00003c40: ffff ffff ffdf ce59 ffff ffff 8c51 9e38  .......Y.....Q.8
+00003c50: 9471 9471 8c51 9e38 bdf7 9471 bdf7 9e38  .q.q.Q.8...q...8
+00003c60: bdf7 9471 bdf7 9e38 bdf7 9e38 9491 6b6d  ...q...8...8..km
 00003c70: b595 4a69 9491 6b6d b595 4a69 9491 6b6d  ..Ji..km..Ji..km
 00003c80: b595 4a69 9491 6b6d b595 4a69 0861 5aeb  ..Ji..km..Ji.aZ.
 00003c90: 5aeb 2124 0861 5aeb 3a07 2124 2124 5aeb  Z.!$.aZ.:.!$!$Z.
 00003ca0: 3a07 2124 0861 5aeb 3a07 0861 4208 bdd6  :.!$.aZ.:..aB...
 00003cb0: 9491 6b4d 4208 bdd6 9491 6b4d 4208 9491  ..kMB.....kMB...
 00003cc0: 9491 6b4d 4208 bdd6 9491 6b4d 8c30 6b4d  ..kMB.....kM.0kM
 00003cd0: 8c30 8c30 6b4d 7bae 7bae 8c30 7bae 7bae  .0.0kM{.{..0{.{.
@@ -1020,19 +1020,19 @@
 00003fb0: 6b6d 73ce 7c0f 73ce 73ae 73ce 73ae 73ce  kms.|.s.s.s.s.s.
 00003fc0: 73ae 73ae 73ce 73ae 6b6d 73ae 6b6d 7bcf  s.s.s.s.kms.km{.
 00003fd0: 6b6d 7bcf 8450 7bcf 6b6d 8450 7bcf 6b6d  km{..P{.km.P{.km
 00003fe0: 94b2 94b2 7bcf 8450 8450 94b2 8450 73ce  ....{..P.P...Ps.
 00003ff0: 632d 632d 8450 632d 632d 73ce 8450 52ab  c-c-.Pc-c-s..PR.
 00004000: 73ce 8450 8450 632d 8450 632d b5b5 94b1  s..P.Pc-.Pc-....
 00004010: 94b1 73ce 73ce 94b1 b5b5 52ca 52ca 73ce  ..s.s.....R.R.s.
-00004020: b5b5 52ca 73ce 73ce b5b5 52ca 72ee 2007  ..R.s.s...R.r. .
-00004030: 2007 2007 72ee 2007 488b 488b ad95 2007   . .r. .H.H... .
-00004040: 2007 2007 72ee 488b bbef ad95 0000 9575   . .r.H........u
-00004050: 8bcf 8bcf 0000 9575 1803 9575 0000 9575  .......u...u...u
-00004060: 1803 9575 1803 9575 1803 9575 6b6d 6b6d  ...u...u...ukmkm
+00004020: b5b5 52ca 73ce 73ce b5b5 52ca ffdf 9cf3  ..R.s.s...R.....
+00004030: 9cf3 9cf3 ffdf 9cf3 ce59 ce59 ad95 9cf3  .........Y.Y....
+00004040: 9cf3 9cf3 ffdf ce59 bbef ad95 8c71 9575  .......Y.....q.u
+00004050: 8bcf 8bcf 8c71 9575 b596 9575 8c71 9575  .....q.u...u.q.u
+00004060: b596 9575 b596 9575 b596 9575 6b6d 6b6d  ...u...u...ukmkm
 00004070: b5d5 4a49 6b6d 6b6d b5d5 4a49 6b6d 6b6d  ..JIkmkm..JIkmkm
 00004080: b5d5 4a49 94b1 6b6d b5d5 4a49 0841 52aa  ..JI..km..JI.AR.
 00004090: 39c7 0841 0841 52aa 52aa 0841 0841 52aa  9..A.AR.R..A.AR.
 000040a0: 52aa 2104 2104 52aa 52aa 39c7 4208 a533  R.!.!.R.R.9.B..3
 000040b0: a533 842f 4208 a533 842f 630c 4208 a533  .3./B..3./c.B..3
 000040c0: 842f 630c 4208 a533 842f 630c 73ce 8c70  ./c.B..3./c.s..p
 000040d0: 630b 4a69 8c70 630b 4a69 4a69 73ce 4a69  c.Ji.pc.JiJis.Ji
@@ -1084,19 +1084,19 @@
 000043b0: 7c10 94b3 7c10 7c10 7c10 73ce 73ce 8c71  |...|.|.|.s.s..q
 000043c0: 7c10 73ce 8c71 7c10 73ce 7c10 8430 8430  |.s..q|.s.|..0.0
 000043d0: 8430 6b8e 8430 9491 7bef 6b8e 7bef 7bef  .0k..0..{.k.{.{.
 000043e0: 7bef 6b8e 6b8e 6b8e 7bef 9491 6b8d 7bef  {.k.k.k.{...k.{.
 000043f0: 73ce 6b8d 73ce 7bef 6b8d 7bef 73ce 6b8d  s.k.s.{.k.{.s.k.
 00004400: 73ce 7bef 8430 6b8d 7bef 73ce 6b4d 6b4d  s.{..0k.{.s.kMkM
 00004410: a575 4a49 8471 6b4d 8471 4a49 6b4d 6b4d  .uJI.qkM.qJIkMkM
-00004420: 8471 6b4d 8471 6b4d a575 4a49 72ce 486a  .qkM.qkM.uJIr.Hj
-00004430: bbef ad95 ad95 1806 1806 1806 72ce 1806  ............r...
-00004440: 486a 486a 72ce 1806 1806 1806 1003 9595  HjHjr...........
-00004450: 1003 9595 0000 9595 1003 8bef 0000 9595  ................
-00004460: 8bef 8bef 0000 9595 1003 9595 73ae 73ae  ............s.s.
+00004420: 8471 6b4d 8471 6b4d a575 4a49 f7be ce59  .qkM.qkM.uJI...Y
+00004430: bbef ad95 ad95 9cd3 9cd3 9cd3 f7be 9cd3  ................
+00004440: ce59 ce59 f7be 9cd3 9cd3 9cd3 ad75 9595  .Y.Y.........u..
+00004450: ad75 9595 8430 9595 ad75 8bef 8430 9595  .u...0...u...0..
+00004460: 8bef 8bef 8430 9595 ad75 9595 73ae 73ae  .....0...u..s.s.
 00004470: ad95 39e7 73ae 73ae ad95 39e7 73ae 73ae  ..9.s.s...9.s.s.
 00004480: ad95 39e7 73ae 73ae ad95 39e7 0000 4208  ..9.s.s...9...B.
 00004490: 4208 2104 0000 4208 4208 2104 0000 630c  B.!...B.B.!...c.
 000044a0: 630c 2104 2104 4208 2104 2104 39c7 a533  c.!.!.B.!.!.9..3
 000044b0: 840f 840f 39c7 a533 840f 5aeb 39c7 a533  ....9..3..Z.9..3
 000044c0: a533 5aeb 39c7 a533 840f 5aeb 528a 528a  .3Z.9..3..Z.R.R.
 000044d0: 528a 528a 4208 528a 4208 4208 630c 630c  R.R.B.R.B.B.c.c.
@@ -1148,19 +1148,19 @@
 000047b0: 8430 8430 94d2 94d2 94d2 8430 94d2 94d2  .0.0.......0....
 000047c0: 8430 8430 bdf6 ad54 ad54 ad54 736d 736d  .0.0...T.T.Tsmsm
 000047d0: 7bef 7bef 7bef 7bef 736d 736d 8c50 7bef  {.{.{.{.smsm.P{.
 000047e0: 736d 736d 94d2 94d2 8c50 94d2 7bce 842f  smsm.....P..{../
 000047f0: 7bce 7bce 6b4c 7bce 842f 6b4c 7bce 6b4c  {.{.kL{../kL{.kL
 00004800: 7bce 6b4c 94b1 842f 842f 7bce 62cb 73cf  {.kL..././{.b.s.
 00004810: 8cd2 73cf 73cf 62cb 8cd2 9dd6 73cf 62cb  ..s.s.b.....s.b.
-00004820: 9dd6 62cb 8cd2 62cb 9dd6 62cb bcf7 502d  ..b...b...b...P-
-00004830: bcf7 bcf7 2008 8a92 bcf7 bcf7 2008 2008  .... ....... . .
-00004840: 2008 2008 2008 502d 502d 502d 3828 9e58   . . .P-P-P-8(.X
-00004850: 5a6b a471 5a6b 1805 9e58 a471 1805 1805  Zk.qZk...X.q....
-00004860: 3828 9e58 3828 1805 3828 9e58 7bce 7bce  8(.X8(..8(.X{.{.
+00004820: 9dd6 62cb 8cd2 62cb 9dd6 62cb ffff ce59  ..b...b...b....Y
+00004830: ffff ffff 9cd3 ffdf ffff ffff 9cd3 9cd3  ................
+00004840: 9cd3 9cd3 9cd3 ce59 ce59 ce59 c618 9e58  .......Y.Y.Y...X
+00004850: ef5d a471 ef5d 94b2 9e58 a471 94b2 94b2  .].q.]...X.q....
+00004860: c618 9e58 c618 94b2 c618 9e58 7bce 7bce  ...X.......X{.{.
 00004870: b594 4228 7bce 7bce b594 4228 7bce 7bce  ..B({.{...B({.{.
 00004880: b594 4228 4228 7bce b594 4228 1903 5acb  ..B(B({...B(..Z.
 00004890: 5acb 1903 0020 39e7 39e7 1903 0020 5acb  Z.... 9.9.... Z.
 000048a0: 5acb 1903 1903 5acb 39e7 1903 39c7 9471  Z.....Z.9...9..q
 000048b0: 9471 630c 39c7 bdd6 9471 630c 39c7 bdd6  .qc.9....qc.9...
 000048c0: 9471 630c 39c7 9471 9471 630c 6b4d 7bef  .qc.9..q.qc.kM{.
 000048d0: 6b4d 7bef 6b4d 6b4d 6b4d 7bef 6b4d 7bef  kM{.kMkMkM{.kM{.
@@ -1212,33 +1212,33 @@
 00004bb0: b575 b575 b575 a534 b575 a534 a534 b575  .u.u.u.4.u.4.4.u
 00004bc0: b575 b575 a534 a534 b575 a534 ad95 94d2  .u.u.4.4.u.4....
 00004bd0: a534 a534 94d2 94d2 a534 94d2 ad95 a534  .4.4.....4.....4
 00004be0: a534 ad95 a534 8c71 94d2 94d2 a534 9cf3  .4...4.q.....4..
 00004bf0: 9cf3 9cf3 9cf3 8c91 a534 9cf3 9cf3 9cf3  .........4......
 00004c00: 9cf3 8450 8c91 8450 9cf3 a534 734c 734c  ...P...P...4sLsL
 00004c10: a658 734c 8450 734c a658 734c 8450 734c  .XsL.PsL.XsL.PsL
-00004c20: a658 734c 734c 734c a658 734c 400b 400b  .XsLsLsL.XsL@.@.
-00004c30: 400b 400b 400b 9b14 cd79 cd79 400b 9b14  @.@.@....y.y@...
-00004c40: cd79 cd79 400b 400b 400b 400b 3008 3008  .y.y@.@.@.@.0.0.
-00004c50: 506b b6d9 9cd2 506b 506b b6d9 9cd2 3008  Pk....PkPk....0.
-00004c60: 506b b6d9 3008 3008 506b b6d9 6b4c 6b4c  Pk..0.0.Pk..kLkL
+00004c20: a658 734c 734c 734c a658 734c ad75 ad75  .XsLsLsL.XsL.u.u
+00004c30: ad75 ad75 ad75 ffff ffff ffff ad75 ffff  .u.u.u.......u..
+00004c40: ffff ffff ad75 ad75 ad75 ad75 a534 a534  .....u.u.u.u.4.4
+00004c50: ce79 b6d9 ffff ce79 ce79 b6d9 ffff a534  .y.....y.y.....4
+00004c60: ce79 b6d9 a534 a534 ce79 b6d9 6b4c 6b4c  .y...4.4.y..kLkL
 00004c70: bdb5 4228 6b4c 6b4c bdb5 4228 6b4c 6b4c  ..B(kLkL..B(kLkL
 00004c80: bdb5 4228 9491 6b4c bdb5 4228 1904 5b0c  ..B(..kL..B(..[.
 00004c90: 5b0c 3a08 0000 5b0c 5b0c 1904 0000 3a08  [.:...[.[.....:.
 00004ca0: 3a08 1904 0000 5b0c 5b0c 1904 4208 94b1  :.....[.[...B...
 00004cb0: 94b1 6b4d 4208 94b1 94b1 6b4d 4208 bdf6  ..kMB.....kMB...
 00004cc0: 94b1 6b4d 4208 94b1 94b1 6b4d 8430 6b4d  ..kMB.....kM.0kM
 00004cd0: 4a49 a534 8430 6b4d 6b4d 6b4d 8430 4a49  JI.4.0kMkMkM.0JI
 00004ce0: 8430 4a49 8430 6b4d 8430 8430 49e7 49e7  .0JI.0kM.0.0I.I.
-00004cf0: 8c12 0000 49e7 8c12 0000 0000 8c12 0000  ....I...........
-00004d00: 0000 0000 41e9 0000 0000 0000 0000 0000  ....A...........
-00004d10: 0000 0000 61ac 61ac 2845 0000 2845 2845  ....a.a.(E..(E(E
-00004d20: 2845 0000 2845 2845 2845 0000 94b3 a555  (E..(E(E(E.....U
-00004d30: 41e7 a555 0000 7bd0 a555 41e7 0000 0000  A..U..{..UA.....
-00004d40: a555 73ae 0000 0000 0000 a555 630c 4a28  .Us........Uc.J(
+00004cf0: ffff a534 49e7 ffff a534 738e ffff a534  ...4I....4s....4
+00004d00: 738e a534 defb 738e a534 a534 73ae 9cd3  s..4..s..4.4s...
+00004d10: 73ae 73ae e71c e71c bdf7 9cd3 bdf7 bdf7  s.s.............
+00004d20: bdf7 9cd3 bdf7 bdf7 bdf7 9cd3 c659 a555  .............Y.U
+00004d30: 41e7 a555 7bef ffff a555 41e7 7bef 7bef  A..U{....UA.{.{.
+00004d40: a555 73ae 7bef 7bef ad75 a555 630c 4a28  .Us.{.{..u.Uc.J(
 00004d50: 630c 4a28 630c 4a28 630c 630c 73cf 73cf  c.J(c.J(c.c.s.s.
 00004d60: 630c 4a28 73cf 8cb3 4a28 630c 94d3 94d3  c.J(s...J(c.....
 00004d70: 6b8e 5aeb 94d3 8430 94d3 6b8e 94d3 6b8e  k.Z....0..k...k.
 00004d80: 6b8e 94d3 8430 8430 94d3 8430 2965 4a89  k....0.0...0)eJ.
 00004d90: 632c 632c 2965 39e7 4a89 632c 39e7 39e7  c,c,)e9.J.c,9.9.
 00004da0: 2965 4a89 2965 2965 39e7 39e7 844f a553  )eJ.)e)e9.9..O.S
 00004db0: a553 844f 4228 4228 632c 632c 632c 4228  .S.OB(B(c,c,c,B(
@@ -1276,33 +1276,33 @@
 00004fb0: 8450 8450 18e4 18e4 18e4 18e4 4a8a 4a8a  .P.P........J.J.
 00004fc0: 4a8a 4a8a 18e4 18e4 18e4 18e4 94b2 94b2  J.J.............
 00004fd0: 94b2 94b2 10a2 10a2 10a2 10a2 52aa 52aa  ............R.R.
 00004fe0: 52aa 52aa 10a2 10a2 10a2 10a2 94b2 94b2  R.R.............
 00004ff0: 94b2 94b2 18c3 18c3 18c3 18c3 52aa 52aa  ............R.R.
 00005000: 52aa 52aa 18c3 18c3 18c3 18c3 736d 8450  R.R.........sm.P
 00005010: ae37 736d 9d54 9d54 ae37 736d 736d 8450  .7sm.T.T.7smsm.P
-00005020: 8450 8450 736d 736d 9d54 736d 1807 480c  .P.Psmsm.Tsm..H.
-00005030: 480c 480c 1807 1807 480c 480c 480c 480c  H.H.....H.H.H.H.
-00005040: bcd6 bcd6 8271 480c bcd6 bcd6 3868 1805  .....qH.....8h..
-00005050: 3868 96da 1805 1805 3868 96da 3868 3868  8h......8h..8h8h
-00005060: 9cd2 9cd2 3868 9cd2 3868 9cd2 6b2c 8c71  ....8h..8h..k,.q
+00005020: 8450 8450 736d 736d 9d54 736d 9492 c638  .P.Psmsm.Tsm...8
+00005030: c638 c638 9492 9492 c638 c638 c638 c638  .8.8.....8.8.8.8
+00005040: ffff ffff ffdf c638 ffff ffff c638 94b2  .......8.....8..
+00005050: c638 96da 94b2 94b2 c638 96da c638 c638  .8.......8...8.8
+00005060: 9cd2 9cd2 c638 9cd2 c638 9cd2 6b2c 8c71  .....8...8..k,.q
 00005070: b595 4208 6b2c 8c71 b595 4208 8c71 6b2c  ..B.k,.q..B..qk,
 00005080: b595 4208 8c71 6b2c b595 4208 18e3 5acb  ..B..qk,..B...Z.
 00005090: 39c7 39c7 18e3 5acb 5acb 39c7 0000 39c7  9.9...Z.Z.9...9.
 000050a0: 39c7 18e3 0000 5acb 5acb 18e3 41e7 bdf6  9.....Z.Z...A...
 000050b0: 9491 6b2c 41e7 bdf6 9491 6b2c 41e7 bdf6  ..k,A.....k,A...
 000050c0: 9491 6b2c 41e7 bdf6 9491 6b2c 8430 630c  ..k,A.....k,.0c.
 000050d0: 8430 8430 8430 630c 8430 7bcf 7bcf 6b6d  .0.0.0c..0{.{.km
-000050e0: 6b6d 6b6d 8430 630c 8430 8430 618e 0000  kmkm.0c..0.0a...
-000050f0: 0000 0000 618e 0000 2827 618e 618e 0000  ....a...('a.a...
-00005100: 2827 618e 618e 0000 0000 2827 3869 3869  ('a.a.....('8i8i
-00005110: 3869 0803 a355 a355 69ef 3869 a355 a355  8i...U.Ui.8i.U.U
-00005120: 69ef 3869 3869 3869 3869 0803 0000 0000  i.8i8i8i8i......
-00005130: 2926 94b2 0002 0000 2926 94b2 0002 0000  )&......)&......
-00005140: 2926 94b2 0000 0000 2926 94b2 7bcf 8c71  )&......)&..{..q
+000050e0: 6b6d 6b6d 8430 630c 8430 8430 e71c 738e  kmkm.0c..0.0..s.
+000050f0: 94b2 94b2 e71c 738e bdf7 e71c e71c 738e  ......s.......s.
+00005100: bdf7 e71c e71c 738e 94b2 bdf7 c638 c638  ......s......8.8
+00005110: c638 a514 ffff ffff ef5d c638 ffff ffff  .8.......].8....
+00005120: ef5d c638 c638 c638 c638 a514 7bef 7bef  .].8.8.8.8..{.{.
+00005130: ce59 94b2 a534 7bef ce59 94b2 a534 7bef  .Y...4{..Y...4{.
+00005140: ce59 94b2 7bef 7bef ce59 94b2 7bcf 8c71  .Y..{.{..Y..{..q
 00005150: 52aa 52aa 8c71 7bcf 52aa 52aa 8c71 634c  R.R..q{.R.R..qcL
 00005160: 52aa 52aa 8c71 7bcf 634c 634c 8c71 8c71  R.R..q{.cLcL.q.q
 00005170: 7c0f 632c 8c71 738e 8c71 8c71 7c0f 632c  |.c,.qs..q.q|.c,
 00005180: 8c71 738e 7c0f 632c 8c71 738e 3186 3186  .qs.|.c,.qs.1.1.
 00005190: 3186 4229 20e3 4229 4229 5aec 3186 4229  1.B) .B)B)Z.1.B)
 000051a0: 4229 4229 20e3 5aec 4229 4229 3a08 5aca  B)B) .Z.B)B):.Z.
 000051b0: 4a69 5aca 3a08 5aca 4a69 5aca 4a69 31a7  JiZ.:.Z.JiZ.Ji1.
@@ -1340,43 +1340,43 @@
 000053b0: 6b6d 6b6d 94d2 94d2 94d2 94d2 6b6d 6b6d  kmkm........kmkm
 000053c0: 5acb 5acb 6b6d 6b6d 6b6d 6b6d 6b6d 6b6d  Z.Z.kmkmkmkmkmkm
 000053d0: 6b6d 6b6d 9cd2 9cd2 9cd2 9cd2 52aa 52aa  kmkm........R.R.
 000053e0: 52aa 52aa 6b6d 6b6d 6b6d 6b6d 632c 632c  R.R.kmkmkmkmc,c,
 000053f0: 632c 632c 8c71 8c71 8c71 8c71 5289 5289  c,c,.q.q.q.qR.R.
 00005400: 5289 5289 632c 632c 7bce 632c 73ad 73ad  R.R.c,c,{.c,s.s.
 00005410: a593 5aaa 8c90 a593 a593 73ad a593 a593  ..Z.......s.....
-00005420: a593 5aaa 8c90 73ad 8c90 73ad 9473 0805  ..Z...s...s..s..
-00005430: 0805 0805 9473 0805 3829 3829 9473 0805  .....s..8)8).s..
-00005440: 0805 0805 624e 0805 9473 9473 0000 9574  ....bN...s.s...t
-00005450: 2023 9574 0000 9574 2023 9574 0000 9574   #.t...t #.t...t
-00005460: 2023 9574 2023 9574 8bad 8bad 7bce 7bce   #.t #.t....{.{.
+00005420: a593 5aaa 8c90 73ad 8c90 73ad ffff 94b2  ..Z...s...s.....
+00005430: 94b2 94b2 ffff 94b2 c618 c618 ffff 94b2  ................
+00005440: 94b2 94b2 ef7d 94b2 ffff ffff 8c51 9574  .....}.......Q.t
+00005450: b5b6 9574 8c51 9574 b5b6 9574 8c51 9574  ...t.Q.t...t.Q.t
+00005460: b5b6 9574 b5b6 9574 8bad 8bad 7bce 7bce  ...t...t....{.{.
 00005470: b595 4208 7bce 7bce b595 4208 7bce 7bce  ..B.{.{...B.{.{.
 00005480: b595 4208 7bce 7bce b595 4208 18c3 528a  ..B.{.{...B...R.
 00005490: 528a 18c3 18c3 528a 528a 31a6 0000 528a  R.....R.R.1...R.
 000054a0: 31a6 18c3 0000 31a6 31a6 18c3 39e7 9cf3  1.....1.1...9...
 000054b0: 9cf3 7bef 39e7 9cf3 7bef 7bef 39e7 9cf3  ..{.9...{.{.9...
 000054c0: 9cf3 5aeb 39e7 9cf3 7bef 5aeb 8430 5acb  ..Z.9...{.Z..0Z.
 000054d0: 6b6d 94d2 8430 5acb 8430 8430 8430 5acb  km...0Z..0.0.0Z.
-000054e0: 8430 94d2 6b6d 5acb 8430 94d2 718f 0000  .0..kmZ..0..q...
-000054f0: 0803 4029 718f 0000 0803 0803 718f 0000  ..@)q.......q...
-00005500: 4029 718f 718f 0000 4029 718f 58ad 58ad  @)q.q...@)q.X.X.
-00005510: 58ad 3809 58ad 58ad 58ad 3809 a2d5 a2d5  X.8.X.X.X.8.....
-00005520: a2d5 58ad a2d5 a2d5 a2d5 58ad 0003 0003  ..X.......X.....
-00005530: 4129 94d3 0003 0003 4129 94d3 2006 0003  A)......A).. ...
-00005540: 5acb 94d3 2006 0003 4129 94d3 8c92 7c10  Z... ...A)....|.
+000054e0: 8430 94d2 6b6d 5acb 8430 94d2 e73c 7bef  .0..kmZ..0...<{.
+000054f0: a514 c618 e73c 7bef a514 a514 e73c 7bef  .....<{......<{.
+00005500: c618 e73c e73c 7bef c618 e73c d6ba d6ba  ...<.<{....<....
+00005510: d6ba bdd7 d6ba d6ba d6ba bdd7 ffff ffff  ................
+00005520: ffff d6ba ffff ffff ffff d6ba 9492 9492  ................
+00005530: d69a 94d3 9492 9492 d69a 94d3 b596 9492  ................
+00005540: ef7d 94d3 b596 9492 d69a 94d3 8c92 7c10  .}............|.
 00005550: 630b 630b 7c10 7c10 630b 630b 8c92 7c10  c.c.|.|.c.c...|.
 00005560: 630b 738d 8c92 7c10 7c10 738d 8c51 6b2c  c.s...|.|.s..Qk,
 00005570: 7bce 8c51 7bce 6b2c 7bce 8c51 8c51 6b2c  {..Q{.k,{..Q.Qk,
 00005580: 8c51 9cf3 8c51 6b2c 8c51 9cf3 2965 2965  .Q...Qk,.Q..)e)e
 00005590: 2965 4a89 2965 2965 4a89 6bce 2965 4a89  )eJ.)e)eJ.k.)eJ.
-000055a0: 6bce 0000 2965 6bce 2965 0000 5b0c 0000  k...)ek.)e..[...
-000055b0: 7491 18c3 0000 0000 0000 18c3 0000 0000  t...............
-000055c0: 0000 0000 0000 0000 0000 0000 4228 4228  ............B(B(
-000055d0: 4228 4228 5b4d 5b4d 4228 4228 0000 5b4d  B(B([M[MB(B(..[M
-000055e0: 5b4d 4228 0000 0000 4228 5b4d 4269 39e7  [MB(....B([MBi9.
+000055a0: 6bce 8410 2965 6bce 2965 8410 5b0c 9cf3  k...)ek.)e..[...
+000055b0: 7491 bdf7 9cf3 7bef 7bef bdf7 7bef 7bef  t.....{.{...{.{.
+000055c0: 7bef 7bef 7bef 7bef 7bef 7bef 4228 4228  {.{.{.{.{.{.B(B(
+000055d0: 4228 4228 5b4d 5b4d 4228 4228 8430 5b4d  B(B([M[MB(B(.0[M
+000055e0: 5b4d 4228 8430 8430 4228 5b4d 4269 39e7  [MB(.0.0B([MBi9.
 000055f0: 39e7 39e7 39e7 4269 39e7 39e7 39e7 4269  9.9.9.Bi9.9.9.Bi
 00005600: 4269 52eb 636e 39e7 4269 52eb 4269 52eb  BiR.cn9.BiR.BiR.
 00005610: 39e7 52eb 4269 39e7 4269 4269 3186 39e7  9.R.Bi9.BiBi1.9.
 00005620: 39e7 52eb 39e7 4269 39e7 39e7 5aca 4a49  9.R.9.Bi9.9.Z.JI
 00005630: 5289 5289 4a49 5aca 4a49 4a49 632b 632b  R.R.JIZ.JIJIc+c+
 00005640: 5aca 5289 5aca 4a49 632b 5289 5aeb 73ce  Z.R.Z.JIc+R.Z.s.
 00005650: 73ce 73ce 3166 4228 5aeb 73ce 4228 5aeb  s.s.1fB(Z.s.B(Z.
@@ -1404,49 +1404,49 @@
 000057b0: 7bae 840f 840f 840f 7bae 8c51 8c51 8c51  {.......{..Q.Q.Q
 000057c0: 8c51 94b2 94b2 94b2 8c51 94b2 73ae 73ae  .Q.......Q..s.s.
 000057d0: 7c0f 73ae 73ae 7c0f 7c0f 73ae 8c71 8c71  |.s.s.|.|.s..q.q
 000057e0: 7c0f 7c0f 8c71 8c71 94d2 8c71 6b8d 6b8d  |.|..q.q...qk.k.
 000057f0: 6b8d 6b8d 73ee 73ee 6b8d 6b8d 8430 8c91  k.k.s.s.k.k..0..
 00005800: 73ee 73ee 8c91 8c91 8430 73ee 8c91 52aa  s.s......0s...R.
 00005810: ad95 52aa 52aa 73ae ad95 52aa 8c91 73ae  ..R.R.s...R...s.
-00005820: ad95 52aa 8c91 52aa 8c91 52aa 69ed 3808  ..R...R...R.i.8.
-00005830: 9c12 9c12 9c12 0003 0003 0003 9c12 0003  ................
-00005840: 3808 3808 9c12 0003 0003 0003 0802 9554  8.8............T
-00005850: 0802 9554 0000 9554 0802 9554 0000 9554  ...T...T...T...T
-00005860: 0802 9554 0000 9554 0802 9554 4a69 6b6d  ...T...T...TJikm
+00005820: ad95 52aa 8c91 52aa 8c91 52aa e73c bdd7  ..R...R...R..<..
+00005830: ffff ffff ffff 8c71 8c71 8c71 ffff 8c71  .......q.q.q...q
+00005840: bdd7 bdd7 ffff 8c71 8c71 8c71 ad55 9554  .......q.q.q.U.T
+00005850: ad55 9554 8410 9554 ad55 9554 8410 9554  .U.T...T.U.T...T
+00005860: ad55 9554 8410 9554 ad55 9554 4a69 6b6d  .U.T...T.U.TJikm
 00005870: ad75 4a69 6b6d 6b6d ad75 4a69 8c71 6b6d  .uJikmkm.uJi.qkm
 00005880: ad75 4a69 6b6d 6b6d ad75 4a69 1082 630c  .uJikmkm.uJi..c.
 00005890: 630c 1082 1082 4228 2945 2945 1082 630c  c.....B()E)E..c.
 000058a0: 630c 2945 1082 2945 2945 1082 39c7 9cf3  c.)E..)E)E..9...
 000058b0: 7bef 7bef 39c7 9cf3 7bef 5acb 39c7 9cf3  {.{.9...{.Z.9...
 000058c0: 9cf3 5acb 39c7 9cf3 7bef 5acb 52aa 6bae  ..Z.9...{.Z.R.k.
 000058d0: a595 8c91 6bae 6bae 8c91 8c91 6bae 52aa  ....k.k.....k.R.
-000058e0: 8c91 a595 6bae 52aa a595 8c91 71f0 0000  ....k.R.....q...
-000058f0: 1805 486b 71f0 0000 1805 486b 71f0 0000  ..Hkq.....Hkq...
-00005900: 1805 486b 71f0 0000 486b 71f0 6910 6910  ..Hkq...Hkq.i.i.
-00005910: 480d 480d 6910 6910 6910 480d 6910 6910  H.H.i.i.i.H.i.i.
-00005920: 6910 480d abb6 abb6 abb6 8a73 0804 0804  i.H........s....
-00005930: 4149 9534 2807 0804 4149 9534 2807 0804  AI.4(...AI.4(...
-00005940: 4149 9534 2807 0804 4149 9534 94b2 8430  AI.4(...AI.4...0
+000058e0: 8c91 a595 6bae 52aa a595 8c91 ef7d 8430  ....k.R......}.0
+000058f0: a534 ce59 ef7d 8430 a534 ce59 ef7d 8430  .4.Y.}.0.4.Y.}.0
+00005900: a534 ce59 ef7d 8430 ce59 ef7d defb defb  .4.Y.}.0.Y.}....
+00005910: c618 c618 defb defb defb c618 defb defb  ................
+00005920: defb c618 ffff ffff ffff ffdf 9492 9492  ................
+00005930: d6ba 9534 b596 9492 d6ba 9534 b596 9492  ...4.......4....
+00005940: d6ba 9534 b596 9492 d6ba 9534 94b2 8430  ...4.......4...0
 00005950: 7bcf 6b4d 94b2 8430 6b4d 6b4d 8430 7bcf  {.kM...0kMkM.0{.
 00005960: 6b4d 7bcf 94b2 94b2 6b4d 7bcf 8430 736d  kM{.....kM{..0sm
 00005970: 8430 94d2 8430 736d 736d 94d2 94d2 736d  .0...0smsm....sm
 00005980: 736d a595 8430 736d 8430 8430 41e7 73ef  sm...0sm.0.0A.s.
-00005990: 41e7 0000 41e7 73ef 41e7 0000 41e7 73ef  A...A.s.A...A.s.
-000059a0: 41e7 0000 41e7 73ef 41e7 0000 0803 2809  A...A.s.A.....(.
-000059b0: 0000 0000 2809 2809 0000 0000 2809 500e  ....(.(.....(.P.
-000059c0: 0000 0803 2809 500e 0000 0803 0000 1003  ....(.P.........
-000059d0: 0000 0000 0000 400c 400c 0000 0000 400c  ......@.@.....@.
-000059e0: 400c 0000 1003 7834 7834 1003 0000 83cf  @.....x4x4......
-000059f0: 1865 0000 0000 0000 83cf 83cf 0000 0000  .e..............
-00005a00: 0000 0000 0000 0000 83cf 1865 4228 4228  ...........eB(B(
+00005990: 41e7 738e 41e7 73ef 41e7 738e 41e7 73ef  A.s.A.s.A.s.A.s.
+000059a0: 41e7 738e 41e7 73ef 41e7 738e 9492 9cf3  A.s.A.s.A.s.....
+000059b0: 8430 8430 9cf3 9cf3 8430 8430 9cf3 ad55  .0.0.....0.0...U
+000059c0: 8430 9492 9cf3 ad55 8430 9492 7bef 9cf3  .0.....U.0..{...
+000059d0: 7bef 7bef 7bef bdd7 bdd7 7bef 7bef bdd7  {.{.{.....{.{...
+000059e0: bdd7 7bef 9cf3 dedb dedb 9cf3 9cf3 83cf  ..{.............
+000059f0: bdf7 9cf3 7bef 7bef 83cf 83cf 9cf3 7bef  ....{.{.......{.
+00005a00: 9cf3 9cf3 9cf3 9cf3 83cf bdf7 4228 4228  ............B(B(
 00005a10: 634c 4228 4228 4228 4228 4228 634c 634c  cLB(B(B(B(B(cLcL
-00005a20: 4228 4228 0000 0000 634c 634c 52ca 4248  B(B(....cLcLR.BH
+00005a20: 4228 4228 7bef 7bef 634c 634c 52ca 4248  B(B({.{.cLcLR.BH
 00005a30: 3186 4248 4248 52ca 4248 39e7 39e7 52ca  1.BHBHR.BH9.9.R.
-00005a40: 52ca 39e7 52ca 0000 39e7 4248 4228 4a89  R.9.R...9.BHB(J.
+00005a40: 52ca 39e7 52ca 94b2 39e7 4248 4228 4a89  R.9.R...9.BHB(J.
 00005a50: 4a89 4228 39e7 4a89 5aeb 5aeb 39e7 4228  J.B(9.J.Z.Z.9.B(
 00005a60: 39e7 4a89 39e7 4228 39e7 39e7 632c 8c71  9.J.9.B(9.9.c,.q
 00005a70: 632c 632c 39e7 8c71 8c71 632c 39e7 8c71  c,c,9..q.qc,9..q
 00005a80: 8c71 8c71 39e7 39e7 8c71 b5b6 632d 73cf  .q.q9.9..q..c-s.
 00005a90: 9d33 8c91 632d 73cf 9d33 8c91 73cf 632d  .3..c-s..3..s.c-
 00005aa0: 8c91 8c91 73cf 73cf 8c91 8c91 8c30 8c30  ....s.s......0.0
 00005ab0: ad54 ad54 bdf6 bdf6 9cd2 bdf6 8c30 9cd2  .T.T.........0..
@@ -1468,49 +1468,49 @@
 00005bb0: 94d2 94d2 94d2 8c71 8c71 94d2 8430 8430  .......q.q...0.0
 00005bc0: 8c71 8430 7bcf 7bcf 8430 8430 94d3 94d3  .q.0{.{..0.0....
 00005bd0: 94d3 8c92 94d3 94d3 8c92 8c92 8430 8430  .............0.0
 00005be0: 8430 94d3 7bef 7bef 7bef 7bef 94b2 94b2  .0..{.{.{.{.....
 00005bf0: 8430 8430 94b2 8430 8430 94b2 73cf 8430  .0.0...0.0..s..0
 00005c00: 73cf 73cf 8430 634d 8430 634d 6b4d 6b4d  s.s..0cM.0cMkMkM
 00005c10: 8470 4a49 6b4d 6b4d 8470 4a49 8470 8470  .pJIkMkM.pJI.p.p
-00005c20: a574 4a49 8470 6b4d 8470 a574 a413 2807  .tJI.pkM.p.t..(.
-00005c30: a413 a413 7a0f 2807 a413 a413 a413 2807  ....z.(.......(.
-00005c40: 2807 2807 a413 2807 500b 500b 0801 95b6  (.(...(.P.P.....
-00005c50: 2845 83cf 0801 83cf 2845 83cf 0801 95b6  (E......(E......
-00005c60: 0801 95b6 0801 95b6 95b6 83cf 7bef 7bef  ............{.{.
+00005c20: a574 4a49 8470 6b4d 8470 a574 ffff 9cf3  .tJI.pkM.p.t....
+00005c30: ffff ffff ef7d 9cf3 ffff ffff ffff 9cf3  .....}..........
+00005c40: 9cf3 9cf3 ffff 9cf3 c638 c638 9cd3 95b6  .........8.8....
+00005c50: bdf7 83cf 9cd3 83cf bdf7 83cf 9cd3 95b6  ................
+00005c60: 9cd3 95b6 9cd3 95b6 95b6 83cf 7bef 7bef  ............{.{.
 00005c70: b575 4249 7bef 7bef b575 4249 7bef 7bef  .uBI{.{..uBI{.{.
 00005c80: b575 4249 7bef 7bef b575 4249 1082 6b6d  .uBI{.{..uBI..km
 00005c90: 6b6d 2965 1082 4a69 2965 2965 1082 6b6d  km)e..Ji)e)e..km
 00005ca0: 4a69 2965 1082 2965 2965 1082 4208 9cf3  Ji)e..)e)e..B...
 00005cb0: 6b8d 6b8d 4208 c678 9cf3 6b8d 4208 9cf3  k.k.B..x..k.B...
 00005cc0: 9cf3 6b8d 4208 9cf3 9cf3 6b8d 736d 5a49  ..k.B.....k.smZI
 00005cd0: 8c91 8c91 8c91 736d 8c91 a5b5 8c91 5a49  ......sm......ZI
-00005ce0: a5b5 8c91 736d 8c91 8c91 a5b5 9292 0804  ....sm..........
-00005cf0: 60ed 9292 60ed 0804 3809 60ed 9292 0804  `...`...8.`.....
-00005d00: 3809 60ed 9292 0804 3809 60ed ac16 ac16  8.`.....8.`.....
-00005d10: ac16 81b2 81b2 81b2 81b2 7090 9ad4 9ad4  ..........p.....
-00005d20: 81b2 7090 9ad4 9ad4 81b2 7090 3809 2007  ..p.......p.8. .
-00005d30: 59eb 59eb 3809 2007 59eb 9617 3809 2007  Y.Y.8. .Y...8. .
-00005d40: 59eb 9617 3809 2007 59eb 9617 9d13 b5b6  Y...8. .Y.......
+00005ce0: a5b5 8c91 736d 8c91 8c91 a5b5 ffdf 9492  ....sm..........
+00005cf0: dedb ffdf dedb 9492 b5b6 dedb ffdf 9492  ................
+00005d00: b5b6 dedb ffdf 9492 b5b6 dedb ffff ffff  ................
+00005d10: ffff ef7d ef7d ef7d ef7d dedb ffff ffff  ...}.}.}.}......
+00005d20: ef7d dedb ffff ffff ef7d dedb bdf7 94b2  .}.......}......
+00005d30: e71c e71c bdf7 94b2 e71c 9617 bdf7 94b2  ................
+00005d40: e71c 9617 bdf7 94b2 e71c 9617 9d13 b5b6  ................
 00005d50: 8c51 73ae 8c51 8c51 73ae 8c51 9d13 b5b6  .Qs..Q.Qs..Q....
 00005d60: 8c51 8c51 8c51 73ae 73ae 9d13 8430 5aec  .Q.Q.Qs.s....0Z.
 00005d70: 8430 a554 8430 5aec 8430 a554 8430 5aec  .0.T.0Z..0.T.0Z.
 00005d80: 5aec ce98 a554 8430 8430 ce98 5248 6c91  Z....T.0.0..RHl.
-00005d90: 5248 0000 5248 5248 5248 0000 5248 6c91  RH..RHRHRH..RHl.
-00005da0: 5248 0000 5248 6c91 5248 0000 6010 9016  RH..RHl.RH..`...
-00005db0: 1005 1005 9016 9016 1005 1005 9016 9016  ................
-00005dc0: 1005 380a 9016 9016 380a 380a 1003 7891  ..8.....8.8...x.
-00005dd0: b158 1003 1003 b158 b158 1003 1003 b158  .X.....X.X.....X
-00005de0: b158 1003 1003 b158 b158 1003 1804 1804  .X.....X.X......
-00005df0: 8a71 8a71 1804 1804 c3f8 c3f8 1804 1804  .q.q............
-00005e00: c3f8 c3f8 1804 1804 c3f8 c3f8 0000 0000  ................
-00005e10: 0000 3086 0000 3086 0000 7a6f 0000 3086  ..0...0...zo..0.
-00005e20: 0000 bc58 3086 7a6f 3086 bc58 520a 520a  ...X0.zo0..XR.R.
-00005e30: 6aca 6aca 1002 1002 520a 520a 9412 0000  j.j.....R.R.....
-00005e40: 0000 520a 9412 1002 1002 0000 39e7 39e7  ..R.........9.9.
+00005d90: 5248 7bcf 5248 5248 5248 7bcf 5248 6c91  RH{.RHRHRH{.RHl.
+00005da0: 5248 7bcf 5248 6c91 5248 7bcf bdd7 ce59  RH{.RHl.RH{....Y
+00005db0: 9cd3 9cd3 ce59 ce59 9cd3 9cd3 ce59 ce59  .....Y.Y.....Y.Y
+00005dc0: 9cd3 ad55 ce59 ce59 ad55 ad55 a514 dedb  ...U.Y.Y.U.U....
+00005dd0: f7be a514 a514 f7be f7be a514 a514 f7be  ................
+00005de0: f7be a514 a514 f7be f7be a514 ad55 ad55  .............U.U
+00005df0: ffdf ffdf ad55 ad55 ffff ffff ad55 ad55  .....U.U.....U.U
+00005e00: ffff ffff ad55 ad55 ffff ffff 9492 9492  .....U.U........
+00005e10: 9492 c618 9492 c618 9492 f79e 9492 c618  ................
+00005e20: 9492 ffff c618 f79e c618 ffff e71c e71c  ................
+00005e30: 6aca 6aca ad75 ad75 e71c e71c ffff 7bef  j.j..u.u......{.
+00005e40: 7bef e71c ffff ad75 ad75 7bef 39e7 39e7  {......u.u{.9.9.
 00005e50: 4269 52eb 39e7 39e7 4269 4269 636e 4269  BiR.9.9.BiBicnBi
 00005e60: 4269 4269 52eb 636e 4269 52eb 4228 4228  BiBiR.cnBiR.B(B(
 00005e70: 4228 8c51 4228 5aeb 4228 738e 4228 5aeb  B(.QB(Z.B(s.B(Z.
 00005e80: 4228 5aeb 4228 5aeb 4228 738e 9492 73ce  B(Z.B(Z.B(s...s.
 00005e90: 73ce 73ce ad75 9492 73ce 73ce ad75 73ce  s.s..u..s.s..us.
 00005ea0: 73ce 9492 ad75 73ce 5aeb 5aeb 840f 840f  s....us.Z.Z.....
 00005eb0: 840f 840f 6b6d 6b6d 840f 840f 840f 6b6d  ....kmkm......km
@@ -1532,51 +1532,51 @@
 00005fb0: 73ae 632c 52aa 632c 73ae 632c 632c 52aa  s.c,R.c,s.c,c,R.
 00005fc0: 52aa 52aa 4228 4228 4228 4228 6b2c 738d  R.R.B(B(B(B(k,s.
 00005fd0: 738d 6b2c 6b2c 5aeb 6b2c 6b2c 5aeb 52aa  s.k,k,Z.k,k,Z.R.
 00005fe0: 6b2c 5aeb 52aa 5aeb 738d 52aa 634c 73ce  k,Z.R.Z.s.R.cLs.
 00005ff0: 634c 73ce 634c 52ca 634c 634c 52ca 4a49  cLs.cLR.cLcLR.JI
 00006000: 4a49 52ca 4a49 4a49 4a49 4a49 8cd2 62ca  JIR.JIJIJIJI..b.
 00006010: a5d6 a5d6 7bce 7bce a5d6 62ca 8cd2 62ca  ....{.{...b...b.
-00006020: a5d6 62ca 8cd2 62ca a5d6 7bce 3008 3008  ..b...b...{.0.0.
-00006030: 3008 3008 3008 7950 c458 c458 3008 7950  0.0.0.yP.X.X0.yP
-00006040: c458 c458 3008 3008 3008 3008 2006 2006  .X.X0.0.0.0. . .
-00006050: ac71 ac71 624c 2006 4029 be79 624c 2006  .q.qbL .@).ybL .
-00006060: 4029 be79 2006 2006 624c be79 738e 738e  @).y . .bL.ys.s.
+00006020: a5d6 62ca 8cd2 62ca a5d6 7bce a514 a514  ..b...b...{.....
+00006030: a514 a514 a514 e73c ffff ffff a514 e73c  .......<.......<
+00006040: ffff ffff a514 a514 a514 a514 9cd3 9cd3  ................
+00006050: ac71 ac71 ef5d 9cd3 c618 be79 ef5d 9cd3  .q.q.].....y.]..
+00006060: c618 be79 9cd3 9cd3 ef5d be79 738e 738e  ...y.....].ys.s.
 00006070: bdf7 4a69 94d2 738e bdf7 4a69 738e 94d2  ..Ji..s...Jis...
 00006080: bdf7 4a69 94d2 94d2 bdf7 4a69 1082 7bef  ..Ji......Ji..{.
 00006090: 7bef 31a6 1082 52ca 31a6 31a6 1082 7bef  {.1...R.1.1...{.
 000060a0: 52ca 31a6 1082 52ca 31a6 1082 528a c638  R.1...R.1...R..8
 000060b0: 7bcf 528a 528a c638 7bcf 7bcf 528a c638  {.R.R..8{.{.R..8
 000060c0: 9cf3 7bcf 528a c638 9cf3 7bcf 630b 630b  ..{.R..8..{.c.c.
 000060d0: a5b7 a5b7 8471 630b 8471 a5b7 8471 630b  .....qc..q...qc.
-000060e0: a5b7 a5b7 8471 630b a5b7 c71c a394 380a  .....qc.......8.
-000060f0: 81b1 a394 a394 380a 81b1 a394 81b1 380a  ......8.......8.
-00006100: 580d 81b1 81b1 380a 580d 81b1 b496 b496  X.....8.X.......
-00006110: b496 9b14 b496 b496 b496 9b14 8191 9b14  ................
-00006120: 8191 680f 9b14 9b14 8191 680f 580d 480b  ..h.......h.X.H.
-00006130: 724e b638 580d 480b 724e b638 580d 480b  rN.8X.H.rN.8X.H.
-00006140: 724e b638 580d 480b 724e b638 8c72 a514  rN.8X.H.rN.8.r..
+000060e0: a5b7 a5b7 8471 630b a5b7 c71c ffff a514  .....qc.........
+000060f0: ef5d ffff ffff a514 ef5d ffff ef5d a514  .].......]...]..
+00006100: c638 ef5d ef5d a514 c638 ef5d ffff ffff  .8.].]...8.]....
+00006110: ffff ffff ffff ffff ffff ffff ef5d ffff  .............]..
+00006120: ef5d ce79 ffff ffff ef5d ce79 ce59 a514  .].y.....].y.Y..
+00006130: ef7d b638 ce59 a514 ef7d b638 ce59 a514  .}.8.Y...}.8.Y..
+00006140: ef7d b638 ce59 a514 ef7d b638 8c72 a514  .}.8.Y...}.8.r..
 00006150: 8c72 a514 bdb6 bdb6 8c72 8c72 ce58 bdb6  .r.......r.r.X..
 00006160: bdb6 8c72 bdb6 a514 bdb6 a514 a534 840f  ...r.........4..
-00006170: a534 a534 a534 a534 840f 94d2 840f 840f  .4.4.4.4........
-00006180: 840f a534 840f 62eb 840f a534 0804 7d55  ...4..b....4..}U
-00006190: 73ae 0000 73ae 7d55 0804 0000 0804 7d55  s...s.}U......}U
-000061a0: 0804 0000 0000 7d55 0804 0000 9013 b817  ......}U........
-000061b0: 480c 480c b817 b817 480c 7010 b817 b817  H.H.....H.p.....
-000061c0: 480c 480c b817 b817 7010 480c 2807 c238  H.H.....p.H.(..8
-000061d0: c238 2807 2807 c238 c238 2807 2807 c238  .8(.(..8.8(.(..8
-000061e0: c238 2807 2807 9112 c238 2807 3808 3808  .8(.(....8(.8.8.
-000061f0: c498 c498 3808 3808 c498 c498 3808 3808  ....8.8.....8.8.
-00006200: c498 c498 3808 3808 c498 c498 1803 516a  ....8.8.......Qj
-00006210: 516a cd79 1803 516a 516a cd79 1803 516a  Qj.y..QjQj.y..Qj
-00006220: 516a cd79 1803 516a 516a cd79 cd79 2805  Qj.y..QjQj.y.y(.
-00006230: 2805 2805 cd79 2805 2805 2805 cd79 2805  (.(..y(.(.(..y(.
-00006240: 2805 2805 cd79 2805 2805 2805 0000 3147  (.(..y(.(.(...1G
-00006250: 3147 1803 3147 0000 52ab 1803 3147 0000  1G..1G..R...1G..
-00006260: 1803 3147 3147 1803 0000 3147 4a69 634d  ..1G1G....1GJicM
+00006170: a534 a534 a534 a534 840f ffff 840f 840f  .4.4.4.4........
+00006180: 840f a534 840f 62eb 840f a534 ad75 7d55  ...4..b....4.u}U
+00006190: 73ae 8430 73ae 7d55 ad75 8430 ad75 7d55  s..0s.}U.u.0.u}U
+000061a0: ad75 8430 8430 7d55 ad75 8430 ce59 dedb  .u.0.0}U.u.0.Y..
+000061b0: b596 b596 dedb dedb b596 bdf7 dedb dedb  ................
+000061c0: b596 b596 dedb dedb bdf7 b596 ad55 ffff  .............U..
+000061d0: ffff ad55 ad55 ffff ffff ad55 ad55 ffff  ...U.U.....U.U..
+000061e0: ffff ad55 ad55 e73c ffff ad55 bdf7 bdf7  ...U.U.<...U....
+000061f0: ffff ffff bdf7 bdf7 ffff ffff bdf7 bdf7  ................
+00006200: ffff ffff bdf7 bdf7 ffff ffff ad75 dedb  .............u..
+00006210: dedb ffff ad75 dedb dedb ffff ad75 dedb  .....u.......u..
+00006220: dedb ffff ad75 dedb dedb ffff ffff bdd7  .....u..........
+00006230: bdd7 bdd7 ffff bdd7 bdd7 bdd7 ffff bdd7  ................
+00006240: bdd7 bdd7 ffff bdd7 bdd7 bdd7 94b2 ce79  ...............y
+00006250: ce79 b596 ce79 94b2 ef7d b596 ce79 94b2  .y...y...}...y..
+00006260: b596 ce79 ce79 b596 94b2 ce79 4a69 634d  ...y.y.....yJicM
 00006270: 4208 4a69 4a69 634d 4208 5acb 4208 5acb  B.JiJicMB.Z.B.Z.
 00006280: 4208 5acb 4208 4a69 4208 634d 9cd1 632b  B.Z.B.JiB.cM..c+
 00006290: 31a6 31a6 9cd1 632b ce57 ce57 9cd1 632b  1.1...c+.W.W..c+
 000062a0: 632b 632b 9cd1 632b 31a6 31a6 31a6 31a6  c+c+..c+1.1.1.1.
 000062b0: 31a6 31a6 ce57 ce57 ce57 ce57 632b 632b  1.1..W.W.W.Wc+c+
 000062c0: 632b 632b 31a6 31a6 31a6 31a6 3166 630c  c+c+1.1.1.1.1fc.
 000062d0: 3166 3166 c678 c678 c678 94d2 630c 630c  1f1f.x.x.x..c.c.
@@ -1596,51 +1596,51 @@
 000063b0: 2945 52aa b5b5 b5b5 b5b5 b5b5 52aa 52aa  )ER.........R.R.
 000063c0: 52aa 52aa 2945 2945 2945 2945 3186 3186  R.R.)E)E)E)E1.1.
 000063d0: 3186 3186 bdd5 bdd5 bdd5 bdd5 5aeb 5aeb  1.1.........Z.Z.
 000063e0: 5aeb 5aeb 3186 3186 3186 3186 3186 3186  Z.Z.1.1.1.1.1.1.
 000063f0: 3186 3186 b5d5 b5d5 b5d5 b5d5 5aeb 5aeb  1.1.........Z.Z.
 00006400: 5aeb 5aeb 3186 3186 3186 3186 8c70 7b4c  Z.Z.1.1.1.1..p{L
 00006410: b6b8 7b4c a594 8c70 b6b8 7b4c 8c70 a594  ..{L...p..{L.p..
-00006420: b6b8 7b4c 8c70 8c70 b6b8 7b4c 2808 2808  ..{L.p.p..{L(.(.
-00006430: 580d 580d 2808 2808 2808 580d 2808 9253  X.X.(.(.(.X.(..S
-00006440: c498 c498 2808 9253 c498 c498 380a 380a  ....(..S....8.8.
-00006450: 58cd c75b 380a 380a 58cd c75b 7b30 380a  X..[8.8.X..[{08.
-00006460: 58cd c75b 7b30 380a 58cd c75b 8410 8410  X..[{08.X..[....
+00006420: b6b8 7b4c 8c70 8c70 b6b8 7b4c 9cd3 9cd3  ..{L.p.p..{L....
+00006430: ce59 ce59 9cd3 9cd3 9cd3 ce59 9cd3 ffdf  .Y.Y.......Y....
+00006440: ffff ffff 9cd3 ffdf ffff ffff a534 a534  .............4.4
+00006450: d6ba c75b a534 a534 d6ba c75b ffff a534  ...[.4.4...[...4
+00006460: d6ba c75b ffff a534 d6ba c75b 8410 8410  ...[...4...[....
 00006470: d699 5acb 8410 8410 d699 5acb ad54 8410  ..Z.......Z..T..
 00006480: d699 5acb ad54 8410 d699 5acb 0001 4a69  ..Z..T....Z...Ji
 00006490: 4a69 0001 0001 73ae 73ae 2125 2125 4a69  Ji....s.s.!%!%Ji
 000064a0: 4a69 2125 2125 73ae 73ae 2125 4229 b5b5  Ji!%!%s.s.!%B)..
 000064b0: b5b5 6b4d 4229 b5b5 b5b5 6b4d 4229 b5b5  ..kMB)....kMB)..
 000064c0: b5b5 6b4d 4229 b5b5 b5b5 6b4d 738d 738d  ..kMB)....kMs.s.
 000064d0: 9d75 ae59 8471 738d 9d75 9d75 738d 738d  .u.Y.qs..u.us.s.
-000064e0: 9d75 9d75 8471 738d 8471 ae59 9a93 1807  .u.u.qs..q.Y....
-000064f0: 400b 68ef 9a93 1807 68ef 9a93 9a93 1807  @.h.....h.......
-00006500: 68ef 9a93 9a93 1807 400b 400b 92b3 92b3  h.......@.@.....
-00006510: 8171 680e ac16 ac16 ac16 8171 ac16 ac16  .qh........q....
-00006520: ac16 8171 8171 92b3 8171 680e 400a 2808  ...q.q...qh.@.(.
-00006530: 61ec add6 400a 2808 61ec add6 400a 2808  a...@.(.a...@.(.
-00006540: 61ec add6 2808 2808 61ec add6 be17 a554  a...(.(.a......T
+000064e0: 9d75 9d75 8471 738d 8471 ae59 ffff 9492  .u.u.qs..q.Y....
+000064f0: b5b6 dedb ffff 9492 dedb ffff ffff 9492  ................
+00006500: dedb ffff ffff 9492 b5b6 b5b6 ffff ffff  ................
+00006510: e73c ce79 ffff ffff ffff e73c ffff ffff  .<.y.......<....
+00006520: ffff e73c e73c ffff e73c ce79 bdf7 9cd3  ...<.<...<.y....
+00006530: e73c add6 bdf7 9cd3 e73c add6 bdf7 9cd3  .<.......<......
+00006540: e73c add6 9cd3 9cd3 e73c add6 be17 a554  .<.......<.....T
 00006550: 8c71 73ae a554 be17 73ae 73ae a554 be17  .qs..T..s.s..T..
 00006560: 8c71 73ae 8c71 a554 8c71 73ae 7bcf 7bcf  .qs..q.T.qs.{.{.
 00006570: 7bcf adb6 7bcf 7bcf 7bcf c69a 94b3 7bcf  {...{.{.{.....{.
-00006580: 7bcf adb6 7bcf 7bcf 7bcf c69a 20e5 5c50  {...{.{.{... .\P
-00006590: 20e5 0004 20e5 5c50 20e5 0004 20e5 5c50   ... .\P ... .\P
-000065a0: 20e5 0004 1004 5c50 20e5 0004 b817 b817   .....\P .......
-000065b0: 500c 7810 b817 b817 500c 7810 b817 b817  P.x.....P.x.....
-000065c0: 500c 500c b817 b817 500c 7810 380a c1d8  P.P.....P.x.8...
-000065d0: c1d8 380a 380a c1d8 c1d8 380a 380a c1d8  ..8.8.....8.8...
-000065e0: c1d8 380a 380a c1d8 c1d8 380a 400a 400a  ..8.8.....8.@.@.
-000065f0: c3d8 c3d8 400a 400a c3d8 c3d8 400a 400a  ....@.@.....@.@.
-00006600: c3d8 c3d8 400a 400a 9a74 c3d8 3006 3006  ....@.@..t..0.0.
-00006610: 3006 c498 3006 3006 3006 c498 3006 3006  0...0.0.0...0.0.
-00006620: 3006 c498 3006 3006 3006 9312 bc58 1804  0...0.0.0....X..
-00006630: 510b 1804 bc58 1804 1804 1804 bc58 1804  Q....X.......X..
-00006640: 1804 1804 bc58 1804 1804 1804 61ad 1002  .....X......a...
-00006650: 0000 61ad 61ad 1002 0000 3888 61ad 1002  ..a.a.....8.a...
-00006660: 0000 61ad 61ad 0000 0000 61ad 4208 4208  ..a.a.....a.B.B.
+00006580: 7bcf adb6 7bcf 7bcf 7bcf c69a c618 5c50  {...{.{.{.....\P
+00006590: c618 8c71 c618 5c50 c618 8c71 c618 5c50  ...q..\P...q..\P
+000065a0: c618 8c71 a534 5c50 c618 8c71 e71c e71c  ...q.4\P...q....
+000065b0: b596 c618 e71c e71c b596 c618 e71c e71c  ................
+000065c0: b596 b596 e71c e71c b596 c618 ad75 ffff  .............u..
+000065d0: ffff ad75 ad75 ffff ffff ad75 ad75 ffff  ...u.u.....u.u..
+000065e0: ffff ad75 ad75 ffff ffff ad75 bdf7 bdf7  ...u.u.....u....
+000065f0: ffff ffff bdf7 bdf7 ffff ffff bdf7 bdf7  ................
+00006600: ffff ffff bdf7 bdf7 ffff ffff bdd7 bdd7  ................
+00006610: bdd7 ffff bdd7 bdd7 bdd7 ffff bdd7 bdd7  ................
+00006620: bdd7 ffff bdd7 bdd7 bdd7 ffff ffff ad75  ...............u
+00006630: d6ba ad75 ffff ad75 ad75 ad75 ffff ad75  ...u...u.u.u...u
+00006640: ad75 ad75 ffff ad75 ad75 ad75 e71c ad75  .u.u...u.u.u...u
+00006650: 9492 e71c e71c ad75 9492 c638 e71c ad75  .......u...8...u
+00006660: 9492 e71c e71c 9492 9492 e71c 4208 4208  ............B.B.
 00006670: 3186 630c 3186 528a 528a 630c 3186 4208  1.c.1.R.R.c.1.B.
 00006680: 4208 630c 4208 630c 4208 630c 8450 4a89  B.c.B.c.B.c..PJ.
 00006690: 4a89 4a89 8450 8450 18e3 18e3 8450 4a89  J.J..P.P.....PJ.
 000066a0: bdf7 bdf7 8450 4a89 8450 4a89 4a69 4a69  .....PJ..PJ.JiJi
 000066b0: 4a69 4a69 18c3 18c3 18c3 18c3 bdd6 bdd6  JiJi............
 000066c0: bdd6 bdd6 4a69 4a69 4a69 8430 4aaa 4aaa  ....JiJiJi.0J.J.
 000066d0: 4aaa 4aaa 1904 1904 1904 1904 bdf6 bdf6  J.J.............
@@ -1660,51 +1660,51 @@
 000067b0: 4a89 4a89 18e3 18e3 18e3 18e3 bdd6 bdd6  J.J.............
 000067c0: bdd6 bdd6 4a89 4a89 4a89 4a89 2124 5acb  ....J.J.J.J.!$Z.
 000067d0: 5acb 2124 2124 2124 2124 2124 ce58 ce58  Z.!$!$!$!$!$.X.X
 000067e0: ce58 ce58 5acb 5acb 5acb 5acb 5aca 5aca  .X.XZ.Z.Z.Z.Z.Z.
 000067f0: 2124 5aca 2124 2124 2124 2124 c617 c617  !$Z.!$!$!$!$....
 00006800: c617 c617 5aca 5aca 5aca 5aca a553 8470  ....Z.Z.Z.Z..S.p
 00006810: be57 6b6c 8470 8470 a553 a553 6b6c 8470  .Wkl.p.p.S.Skl.p
-00006820: a553 6b6c a553 8470 8470 6b6c 0001 0001  .Skl.S.p.pkl....
-00006830: 3007 3007 3007 0001 3007 3007 a3f4 0001  0.0.0...0.0.....
-00006840: 0001 3007 a3f4 3007 a3f4 a3f4 0000 0000  ..0...0.........
-00006850: 526b b679 0000 2005 b679 b679 0000 b679  Rk.y.. ..y.y...y
-00006860: 526b 9c71 2005 b679 526b 9c71 7bef 7bef  Rk.q ..yRk.q{.{.
+00006820: a553 6b6c a553 8470 8470 6b6c 8c51 8c51  .Skl.S.p.pkl.Q.Q
+00006830: bdd7 bdd7 bdd7 8c51 bdd7 bdd7 ffff 8c51  .......Q.......Q
+00006840: 8c51 bdd7 ffff bdd7 ffff ffff 8c51 8c51  .Q...........Q.Q
+00006850: ef5d b679 8c51 bdd7 b679 b679 8c51 b679  .].y.Q...y.y.Q.y
+00006860: ef5d 9c71 bdd7 b679 ef5d 9c71 7bef 7bef  .].q...y.].q{.{.
 00006870: ce78 52aa a533 7bef ce78 52aa a533 7bef  .xR..3{..xR..3{.
 00006880: ce78 52aa a533 a533 ce78 52aa 0841 3a07  .xR..3.3.xR..A:.
 00006890: 3a07 2124 0841 5aeb 5aeb 0841 0841 5aeb  :.!$.AZ.Z..A.AZ.
 000068a0: 3a07 2124 2124 5aeb 3a07 3a07 39e7 a553  :.!$!$Z.:.:.9..S
 000068b0: a553 842f 39e7 842f a553 842f 39e7 a553  .S./9../.S./9..S
 000068c0: a553 5b0b 39e7 a553 a553 5b0b 9491 73cf  .S[.9..S.S[...s.
-000068d0: 9491 ad74 9491 73cf ad74 ad74 9491 0863  ...t..s..t.t...c
-000068e0: 9491 9491 9491 73cf 9491 9491 718f 0000  ......s.....q...
-000068f0: 2006 718f 718f 0000 2006 718f 718f 0000   .q.q... .q.q...
-00006900: 2006 718f 718f 0000 2006 718f 8271 8271   .q.q... .q..q.q
-00006910: 692e 480a 8271 692e 480a 480a a394 a394  i.H..qi.H.H.....
-00006920: 8271 692e a394 a394 8271 692e 1004 0000  .qi......qi.....
-00006930: 4188 a534 1004 0000 4188 a534 1004 0000  A..4....A..4....
-00006940: 4188 a534 1004 0000 4188 a534 840f a554  A..4....A..4...T
+000068d0: 9491 ad74 9491 73cf ad74 ad74 9491 b5b6  ...t..s..t.t....
+000068e0: 9491 9491 9491 73cf 9491 9491 e73c 7bef  ......s......<{.
+000068f0: b596 e73c e73c 7bef b596 e73c e73c 7bef  ...<.<{....<.<{.
+00006900: b596 e73c e73c 7bef b596 e73c f7be f7be  ...<.<{....<....
+00006910: defb c638 f7be defb c638 c638 ffff ffff  ...8.....8.8....
+00006920: f7be defb ffff ffff f7be defb ad75 8430  .............u.0
+00006930: d6ba a534 ad75 8430 d6ba a534 ad75 8430  ...4.u.0...4.u.0
+00006940: d6ba a534 ad75 8430 d6ba a534 840f a554  ...4.u.0...4...T
 00006950: 94b2 840f a554 94b2 840f 94b2 94b2 94b2  .....T..........
 00006960: 840f 736d 94b2 94b2 736d 736d 8c71 6b4c  ..sm....smsm.qkL
 00006970: 6b4c ad75 8c71 8c71 6b4c ce9a 6b4c 6b4c  kL.u.q.qkL..kLkL
-00006980: 8c71 ce9a 8c71 ad75 6b4c ce9a 1003 5491  .q...q.ukL....T.
-00006990: 1003 0001 1003 5491 7a48 0001 1003 5491  ......T.zH....T.
-000069a0: 7a48 0001 7a48 5491 1003 0001 b015 b015  zH..zHT.........
-000069b0: 480b 8010 b015 b015 480b 8010 8010 b015  H.......H.......
-000069c0: 480b 480b 8010 8010 1005 1005 500c c098  H.H.........P...
-000069d0: c098 500c 500c c098 c098 500c 1005 8812  ..P.P.....P.....
-000069e0: 8812 1005 1005 500c 500c 1005 500b 500b  ......P.P...P.P.
-000069f0: c1d8 c1d8 500b 500b c1d8 c1d8 1004 1004  ....P.P.........
-00006a00: 8871 8871 1004 1004 500b 500b 1805 584d  .q.q....P.P...XM
-00006a10: 1805 9195 1805 1805 1805 9195 0000 1805  ................
-00006a20: 0000 584d 0000 0000 0000 1805 9175 1003  ..XM.........u..
-00006a30: 1003 1003 9175 1003 1003 1003 502c 0000  .....u......P,..
-00006a40: 0000 0000 1003 0000 0000 0000 1002 0000  ................
-00006a50: 0001 734b 0001 0000 0001 734b 0001 0000  ..sK......sK....
-00006a60: 0001 734b 0000 0000 0001 734b 39e7 5aea  ..sK......sK9.Z.
+00006980: 8c71 ce9a 8c71 ad75 6b4c ce9a a534 5491  .q...q.ukL...4T.
+00006990: a534 8c51 a534 5491 7a48 8c51 a534 5491  .4.Q.4T.zH.Q.4T.
+000069a0: 7a48 8c51 7a48 5491 a534 8c51 defb defb  zH.QzHT..4.Q....
+000069b0: ad75 c638 defb defb ad75 c638 c638 defb  .u.8.....u.8.8..
+000069c0: ad75 ad75 c638 c638 9492 9492 b596 ef7d  .u.u.8.8.......}
+000069d0: ef7d b596 b596 ef7d ef7d b596 9492 d69a  .}.....}.}......
+000069e0: d69a 9492 9492 b596 b596 9492 b5b6 b5b6  ................
+000069f0: ffff ffff b5b6 b5b6 ffff ffff 9492 9492  ................
+00006a00: dedb dedb 9492 9492 b5b6 b5b6 a534 ce79  .............4.y
+00006a10: a534 f79e a534 a534 a534 f79e 8410 a534  .4...4.4.4.....4
+00006a20: 8410 ce79 8410 8410 8410 a534 ef7d a514  ...y.......4.}..
+00006a30: a514 a514 ef7d a514 a514 a514 ce59 7bcf  .....}.......Y{.
+00006a40: 7bcf 7bcf a514 7bcf 7bcf 7bcf b596 8430  {.{...{.{.{....0
+00006a50: 9cd3 734b 9cd3 8430 9cd3 734b 9cd3 8430  ..sK...0..sK...0
+00006a60: 9cd3 734b 8430 8430 9cd3 734b 39e7 5aea  ..sK.0.0..sK9.Z.
 00006a70: 39e7 5aea 39e7 5aea 39e7 39e7 39e7 4a68  9.Z.9.Z.9.9.9.Jh
 00006a80: 3186 5aea 39e7 39e7 3186 4a68 842f 4a8a  1.Z.9.9.1.Jh./J.
 00006a90: 4a8a 4a8a a512 a512 842f 842f a512 842f  J.J.....././.../
 00006aa0: 6b6d 842f 842f 842f 842f 842f 2986 4249  km./././././).BI
 00006ab0: 4249 632c 840f 840f 840f 632c 840f 632c  BIc,......c,..c,
 00006ac0: 632c 840f 840f 632c 840f 840f 4208 4208  c,....c,....B.B.
 00006ad0: 5acb 4208 8430 8430 6b6d 8430 8430 6b6d  Z.B..0.0km.0.0km
@@ -1724,38 +1724,38 @@
 00006bb0: 4208 4208 8c70 73ad 8c70 8c70 8c70 8c70  B.B..ps..p.p.p.p
 00006bc0: 8c70 8c70 8c70 73ad 8c70 8c70 4207 5aca  .p.p.ps..p.pB.Z.
 00006bd0: 4207 5aca 8450 8450 8450 8450 8450 8450  B.Z..P.P.P.P.P.P
 00006be0: 8450 8450 8450 6b8d 6b8d 6b8d 4a69 4a69  .P.P.Pk.k.k.JiJi
 00006bf0: 4a69 4a69 8c50 8c50 8c50 8c50 73ae 8c50  JiJi.P.P.P.Ps..P
 00006c00: 73ae 73ae 8c50 73ae 8c50 73ae a594 8cb1  s.s..Ps..Ps.....
 00006c10: 8cb1 7bcd 7bcd 62ea a594 62ea 8cb1 7bcd  ..{.{.b...b...{.
-00006c20: 8cb1 7bcd a594 8cb1 a594 62ea 9451 0002  ..{.......b..Q..
-00006c30: 9451 9451 9451 0002 0002 0002 9451 0002  .Q.Q.Q.......Q..
-00006c40: 3007 3007 9451 0002 0002 0002 1002 add5  0.0..Q..........
-00006c50: 8c0f add5 0000 add5 1002 add5 0000 add5  ................
-00006c60: 8c0f 8c0f 0000 add5 1002 add5 7bef 7bef  ............{.{.
+00006c20: 8cb1 7bcd a594 8cb1 a594 62ea ffff 9492  ..{.......b.....
+00006c30: ffff ffff ffff 9492 9492 9492 ffff 9492  ................
+00006c40: bdf7 bdf7 ffff 9492 9492 9492 b596 add5  ................
+00006c50: 8c0f add5 8410 add5 b596 add5 8410 add5  ................
+00006c60: 8c0f 8c0f 8410 add5 b596 add5 7bef 7bef  ............{.{.
 00006c70: bdb6 4208 7bef 7bef bdb6 4208 7bef 7bef  ..B.{.{...B.{.{.
 00006c80: bdb6 4208 7bef 7bef bdb6 4208 0821 4228  ..B.{.{...B..!B(
 00006c90: 4228 2124 0821 4228 4228 2124 0821 634c  B(!$.!B(B(!$.!cL
 00006ca0: 634c 0821 2124 4228 2124 2124 3a07 ad34  cL.!!$B(!$!$:..4
 00006cb0: ad34 5b0b 3a07 ad34 ad34 5b0b 3a07 ad34  .4[.:..4.4[.:..4
 00006cc0: 8430 5b0b 3a07 ad34 ad34 5b0b 6b2c 5228  .0[.:..4.4[.k,R(
 00006cd0: 7c0f 9513 7c0f 6b2c 7c0f 9513 6b2c 6b2c  |...|.k,|...k,k,
-00006ce0: 7c0f 7c0f 7c0f 6b2c 7c0f 6b2c 61ee 0000  |.|.|.k,|.k,a...
-00006cf0: 0000 2866 2866 0000 0000 2866 61ee 0000  ..(f(f....(fa...
-00006d00: 0000 0000 61ee 2866 0000 2866 40a8 40a8  ....a.(f..(f@.@.
-00006d10: 1803 1803 40a8 61ad 40a8 1803 40a8 40a8  ....@.a.@...@.@.
-00006d20: 1803 1803 61ad 8ad2 61ad 40a8 0000 0000  ....a...a.@.....
-00006d30: 41c7 a534 0000 0000 41c7 a534 0000 0000  A..4....A..4....
-00006d40: 41c7 a534 0000 0000 a534 736d 9471 73ce  A..4.....4sm.qs.
+00006ce0: 7c0f 7c0f 7c0f 6b2c 7c0f 6b2c e73c 738e  |.|.|.k,|.k,.<s.
+00006cf0: 94b2 bdf7 bdf7 738e 94b2 bdf7 e73c 738e  ......s......<s.
+00006d00: 94b2 94b2 e73c bdf7 738e bdf7 ce59 ce59  .....<..s....Y.Y
+00006d10: ad75 ad75 ce59 e71c ce59 ad75 ce59 ce59  .u.u.Y...Y.u.Y.Y
+00006d20: ad75 ad75 e71c ffff e71c ce59 7bef 7bef  .u.u.......Y{.{.
+00006d30: dedb a534 7bef 7bef dedb a534 7bef 7bef  ...4{.{....4{.{.
+00006d40: dedb a534 7bef 7bef a534 736d 9471 73ce  ...4{.{..4sm.qs.
 00006d50: 73ce 73ce 9471 73ce 73ce 9471 ad34 9471  s.s..qs.s..q.4.q
 00006d60: 73ce 73ce 9471 9471 5b0b 73ce a534 a534  s.s..q.q[.s..4.4
-00006d70: 632b 94b2 a534 842f 842f c638 a534 842f  c+...4././.8.4./
+00006d70: 632b ffff a534 842f 842f c638 a534 842f  c+...4././.8.4./
 00006d80: a534 c638 a534 842f 842f 842f 738d 738d  .4.8.4./././s.s.
-00006d90: 738d 8c90 4a28 4a28 4a28 738d c637 738d  s...J(J(J(s..7s.
+00006d90: 738d ffff 4a28 4a28 4a28 738d c637 738d  s...J(J(J(s..7s.
 00006da0: 738d 738d c637 c637 c637 c637 a5d6 84b1  s.s..7.7.7.7....
 00006db0: a5d6 a5d6 4a68 4a68 4a68 4a68 6b8d 6b8d  ....JhJhJhJhk.k.
 00006dc0: 6b8d 6b8d a5d6 a5d6 84b1 a5d6 9db6 7c91  k.k...........|.
 00006dd0: 7c91 7c91 4248 4248 4248 4248 636d 636d  |.|.BHBHBHBHcmcm
 00006de0: 636d 7c91 9db6 9db6 9db6 7c91 94f2 94f2  cm|.......|.....
 00006df0: 94f2 94f2 4248 4248 4248 4248 6bad 6bad  ....BHBHBHBHk.k.
 00006e00: 4248 4248 be57 94f2 be57 94f2 8430 8430  BHBH.W...W...0.0
@@ -1788,32 +1788,32 @@
 00006fb0: 83ef 83ef 83ef 9491 9491 8c50 9491 8c50  ...........P...P
 00006fc0: 9491 9cf2 9491 9cf2 9491 9491 7bce 840f  ............{...
 00006fd0: 9470 9cb1 840f 7bce 9470 9470 9cb1 840f  .p....{..p.p....
 00006fe0: 9cb1 9cb1 9cb1 9cb1 840f 9cb1 8c70 7bce  .............p{.
 00006ff0: 842f 842f 94d1 842f 8c70 7bce 8c70 8c70  ././.../.p{..p.p
 00007000: 7bce 842f 94d1 842f 7bce 842f 73ae 9491  {../.../{../s...
 00007010: ad94 5aab 5aab ad94 ad94 5aab 73ae 5aab  ..Z.Z.....Z.s.Z.
-00007020: ad94 5aab 9491 9491 9491 5aab 9bf3 0001  ..Z.......Z.....
-00007030: 9bf3 9bf3 9bf3 0001 9bf3 9bf3 9bf3 0001  ................
-00007040: 0001 0001 9bf3 0001 0001 3007 1003 9d13  ..........0.....
-00007050: 1003 9d13 1003 9d13 836d 9d13 0000 9d13  .........m......
-00007060: 1003 9d13 0000 9d13 1003 9d13 6b8d 6b8d  ............k.k.
+00007020: ad94 5aab 9491 9491 9491 5aab ffff 8c71  ..Z.......Z....q
+00007030: ffff ffff ffff 8c71 ffff ffff ffff 8c71  .......q.......q
+00007040: 8c71 8c71 ffff 8c71 8c71 bdd7 ad75 9d13  .q.q...q.q...u..
+00007050: ad75 9d13 ad75 9d13 836d 9d13 8430 9d13  .u...u...m...0..
+00007060: ad75 9d13 8430 9d13 ad75 9d13 6b8d 6b8d  .u...0...u..k.k.
 00007070: b5b6 4a69 9492 6b8d b5b6 4a69 6b8d 6b8d  ..Ji..k...Jik.k.
 00007080: b5b6 4a69 6b8d 6b8d b5b6 4a69 1903 5b0b  ..Jik.k...Ji..[.
 00007090: 5b0b 3a07 0000 3a07 3a07 1903 0000 5b0b  [.:...:.:.....[.
 000070a0: 5b0b 1903 0000 5b0b 3a07 1903 4207 ad53  [.....[.:...B..S
 000070b0: ad53 632b 4207 ad53 ad53 632b 4207 ad53  .Sc+B..S.Sc+B..S
 000070c0: ad53 8c2f 4207 ad53 ad53 632b 8c4f 632b  .S./B..S.Sc+.Oc+
 000070d0: 528a 8c4f 632b 7bad 528a 7bad 7bad 7bad  R..Oc+{.R.{.{.{.
-000070e0: 632b 528a 632b 7bad 528a 632b 7bae 3987  c+R.c+{.R.c+{.9.
-000070f0: 0801 0000 9d13 0801 6b2c 0801 7bae 9d13  ........k,..{...
-00007100: 0000 6b2c 0801 0801 9d13 0801 3106 6aac  ..k,........1.j.
-00007110: 3106 0000 0000 0000 0000 0000 3106 0000  1...........1...
-00007120: 0000 6aac 3106 3106 3106 3106 0000 7bce  ..j.1.1.1.1...{.
-00007130: a574 73ce 7bce 94d2 4208 a574 7bce 4208  .ts.{...B..t{.B.
+000070e0: 632b 528a 632b 7bad 528a 632b 7bae d6ba  c+R.c+{.R.c+{...
+000070f0: ad75 8c51 9d13 ad75 ffdf ad75 7bae 9d13  .u.Q...u...u{...
+00007100: 8c51 ffdf ad75 ad75 9d13 ad75 ce59 f79e  .Q...u.u...u.Y..
+00007110: ce59 a514 7bcf 7bcf 7bcf 7bcf ce59 a514  .Y..{.{.{.{..Y..
+00007120: a514 f79e ce59 ce59 ce59 ce59 73ae ffff  .....Y.Y.Y.Ys...
+00007130: a574 73ce ffff c678 4208 a574 ffff 4208  .ts....xB..t..B.
 00007140: a574 73ce 4208 a574 73ce 73ce 8450 73ae  .ts.B..ts.s..Ps.
 00007150: 5b0c 73ae 9cf2 73ae 73ae 8450 73ae 8450  [.s...s.s..Ps..P
 00007160: 8450 8450 5b0c 73ae 8450 5b0c ad53 634c  .P.P[.s..P[..ScL
 00007170: 8c50 4249 ad53 634c 8c50 8c50 8c50 8c50  .PBI.ScL.P.P.P.P
 00007180: 8c50 634c ad53 8c50 8c50 8c50 4228 4228  .PcL.S.P.P.PB(B(
 00007190: 2124 6b4c 8c50 8c50 6b4c 8c50 8c50 8c50  !$kL.P.PkL.P.P.P
 000071a0: 8c50 8c50 8c50 8c50 6b4c 8c50 4228 4228  .P.P.P.PkL.PB(B(
@@ -1852,19 +1852,19 @@
 000073b0: 9cb1 8430 9cb1 9cb1 9cb1 8430 8c70 8430  ...0.......0.p.0
 000073c0: 8c70 9cb1 73ef 9cb1 8c70 9cb1 94b1 94b1  .p..s....p......
 000073d0: 83ef 8c50 94b1 83ef 94b1 94b1 83ef 94b1  ...P............
 000073e0: 7b8e 8c50 83ef 8c50 94b1 83ef 8c50 8c50  {..P...P.....P.P
 000073f0: 842f 73ce 8c50 842f 8c50 7bef 842f 8c50  ./s..P./.P{../.P
 00007400: 842f 8c50 842f 73ce 842f 7bef 8cb1 8cb1  ./.P./s../{.....
 00007410: 8cb1 6bae 8cb1 8cb1 adb4 4aab 8cb1 8cb1  ..k.......J.....
-00007420: 8cb1 6bae 8cb1 6bae 8cb1 adb4 a393 0000  ..k...k.........
-00007430: 0000 0000 a393 0000 a393 a393 a393 0000  ................
-00007440: a393 a393 0000 0000 0000 2806 0000 ad74  ..........(....t
-00007450: 8bae 8bae 0801 ad74 0801 ad74 0801 ad74  .......t...t...t
-00007460: ad74 8bae 0000 0000 ad74 8bae 738d 738d  .t.......t..s.s.
+00007420: 8cb1 6bae 8cb1 6bae 8cb1 adb4 ffff 8c51  ..k...k........Q
+00007430: 8c51 8c51 ffff 8c51 ffff ffff ffff 8c51  .Q.Q...Q.......Q
+00007440: ffff ffff 8c51 8c51 8c51 b5b6 7bef ad74  .....Q.Q.Q..{..t
+00007450: 8bae 8bae ad55 ad74 ad55 ad74 ad55 ad74  .....U.t.U.t.U.t
+00007460: ad74 8bae 7bef 7bef ad74 8bae 738d 738d  .t..{.{..t..s.s.
 00007470: c5f6 4a69 738d 738d c5f6 4a69 738d 738d  ..Jis.s...Jis.s.
 00007480: c5f6 4a69 738d 738d c5f6 4a69 18e3 5aeb  ..Jis.s...Ji..Z.
 00007490: 5aeb 39e7 0000 39e7 39e7 18e3 0000 39e7  Z.9...9.9.....9.
 000074a0: 39e7 18e3 0000 5aeb 5aeb 18e3 4207 bdf6  9.....Z.Z...B...
 000074b0: 94b1 94b1 4207 bdf6 94b1 94b1 4207 bdf6  ....B.......B...
 000074c0: 94b1 6b4c 4207 bdf6 94b1 94b1 9cd1 5289  ..kLB.........R.
 000074d0: 6b4c 5289 840e 840e 5289 5289 9cd1 9cd1  kLR.....R.R.....
@@ -1916,19 +1916,19 @@
 000077b0: 9492 8c50 8c50 8c50 73ad 8c50 7bef 8c50  ...P.P.Ps..P{..P
 000077c0: 7bef 7bef 9492 73ad 8c50 7bef 7bce 8410  {.{...s..P{.{...
 000077d0: 738d 7bce 8410 7bce 8c51 8410 8c51 8c51  s.{...{..Q...Q.Q
 000077e0: 8410 7bce 8410 7bce 8410 7bce 840f 8c50  ..{...{...{....P
 000077f0: 840f 840f 840f 73ae 73ae 73ae 8c50 6b6d  ......s.s.s..Pkm
 00007800: 840f 840f 73ae 840f 840f 6b6d 842f 842f  ....s.....km././
 00007810: b658 6b0b 842f 6b0b b658 6b0b 842f 842f  .Xk../k..Xk.././
-00007820: b658 6b0b 842f 6b0b b658 6b0b 0000 0000  .Xk../k..Xk.....
-00007830: 4008 4008 0000 0000 0000 0000 0000 81d0  @.@.............
-00007840: c3d8 c3d8 0000 81d0 c3d8 c3d8 0001 0001  ................
-00007850: 3026 bdf6 0001 0001 3026 bdf6 5a2b 0001  0&......0&..Z+..
-00007860: 3026 bdf6 5a2b 0001 3026 bdf6 6b8d 6b8d  0&..Z+..0&..k.k.
+00007820: b658 6b0b 842f 6b0b b658 6b0b 8c71 8c71  .Xk../k..Xk..q.q
+00007830: bdf7 bdf7 8c71 8c71 8c71 8c71 8c71 ef7d  .....q.q.q.q.q.}
+00007840: ffff ffff 8c71 ef7d ffff ffff 9492 9492  .....q.}........
+00007850: bdf7 bdf6 9492 9492 bdf7 bdf6 e73c 9492  .............<..
+00007860: bdf7 bdf6 e73c 9492 bdf7 bdf6 6b8d 6b8d  .....<......k.k.
 00007870: b5d6 4a69 6b8d 6b8d b5d6 4a69 94b2 6b8d  ..Jik.k...Ji..k.
 00007880: b5d6 4a69 6b8d 6b8d b5d6 4a69 1062 4208  ..Jik.k...Ji.bB.
 00007890: 2925 2925 1062 5aeb 5aeb 2925 1062 4208  )%)%.bZ.Z.)%.bB.
 000078a0: 4208 2925 1062 5aeb 5aeb 1062 4208 b5f5  B.)%.bZ.Z..bB...
 000078b0: 8cb1 8cb1 4208 b5f5 8cb1 8cb1 4208 b5f5  ....B.......B...
 000078c0: 8cb1 6b4c 4208 8cb1 8cb1 6b4c 94b0 842f  ..kLB.....kL.../
 000078d0: 842f 842f 94b0 842f 94b0 842f 7bad 6b2c  ././.../.../{.k,
@@ -1980,19 +1980,19 @@
 00007bb0: 7bef 7bef 7bef 8c50 7bef 632c 8c50 7bef  {.{.{..P{.c,.P{.
 00007bc0: 7bef 738d 738d 738d 738d 632c 8450 7bef  {.s.s.s.s.c,.P{.
 00007bd0: 738d 738d 7bef 8450 6b2c 7bef 7bef 8450  s.s.{..Pk,{.{..P
 00007be0: 7bef 738d 7bef 6b2c 6b2c 738d 8410 73ae  {.s.{.k,k,s...s.
 00007bf0: 6b6d 8410 7bcf 73ae 73ae 73ae 6b6d 6b6d  km..{.s.s.s.kmkm
 00007c00: 8410 6b6d 7bcf 6b6d 73ae 6b6d 8c91 738d  ..km{.kms.km..s.
 00007c10: c6b8 738d 738d 738d c6b8 738d 738d 8c91  ..s.s.s...s.s...
-00007c20: c6b8 738d 8c91 adb4 c6b8 738d 0000 0000  ..s.......s.....
-00007c30: 0001 0001 0000 0001 2005 2005 0000 0001  ........ . .....
-00007c40: 2005 2005 0000 0001 2005 2005 0000 0000   . ..... . .....
-00007c50: 5a48 be78 5a48 0000 5a48 be78 5a48 0000  ZH.xZH..ZH.xZH..
-00007c60: 5a48 be78 5a48 0000 5a48 be78 6b6c 9471  ZH.xZH..ZH.xkl.q
+00007c20: c6b8 738d 8c91 adb4 c6b8 738d 738e 8430  ..s.......s.s..0
+00007c30: 9cd3 9cd3 738e 9cd3 ad75 ad75 738e 9cd3  ....s....u.us...
+00007c40: ad75 ad75 738e 9cd3 ad75 ad75 73ae 73ae  .u.us....u.us.s.
+00007c50: 5a48 be78 5a48 73ae 5a48 be78 5a48 73ae  ZH.xZHs.ZH.xZHs.
+00007c60: 5a48 be78 5a48 73ae 5a48 be78 6b6c 9471  ZH.xZHs.ZH.xkl.q
 00007c70: b595 4a48 9471 6b6c b595 4a48 9471 9471  ..JH.qkl..JH.q.q
 00007c80: b595 4a48 9471 6b6c b595 4a48 18e3 528a  ..JH.qkl..JH..R.
 00007c90: 528a 18e3 18e3 528a 528a 31a6 0020 528a  R.....R.R.1.. R.
 00007ca0: 31a6 18e3 0020 528a 528a 18e3 39e8 b5d6  1.... R.R...9...
 00007cb0: 8c91 632d 39e8 8c91 b5d6 632d 39e8 b5d6  ..c-9.....c-9...
 00007cc0: 8c91 632d 39e8 b5d6 8c91 632d 7bee 7bee  ..c-9.....c-{.{.
 00007cd0: 8c4f 736d 736d 7bee 7bee 7bee 630c 630c  .Osmsm{.{.{.c.c.
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/__init__.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from pathlib import Path
 
 from construct import Container
-from open_prime_rando.echoes.dock_lock_rando import dock_type
-from open_prime_rando.echoes.dock_lock_rando.dock_type_database import DOCK_TYPES
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.base_resource import AssetId, RawResource
 from retro_data_structures.formats.cmdl import Cmdl
 from retro_data_structures.game_check import Game
 
+from open_prime_rando.echoes.dock_lock_rando import dock_type
+from open_prime_rando.echoes.dock_lock_rando.dock_type_database import DOCK_TYPES
+from open_prime_rando.patcher_editor import PatcherEditor
+
 
 def add_custom_models(editor: PatcherEditor):
     assets = Path(__file__).parent.parent.joinpath("custom_assets", "doors")
-    def get_txtr(n: str) -> AssetId:
+    def get_txtr(n: str, must_exist: bool = True) -> AssetId:
+        f = assets.joinpath(n)
+        if not must_exist and not f.exists():
+            return None
         res = RawResource(
             type="TXTR",
-            data=assets.joinpath(f"{n}.TXTR").read_bytes()
+            data=f.read_bytes()
         )
-        return editor.add_file(f"{n}.TXTR", res, [])
+        return editor.add_file(n, res)
 
-    emissive = get_txtr("custom_door_lock_greyscale_emissive")
+    greyscale_emissive = get_txtr("custom_door_lock_greyscale_emissive.TXTR")
     template = editor.get_parsed_asset(0xF115F575, type_hint=Cmdl)
 
-    for name in ("darkburst", "sunburst", "sonicboom"):
-        txtr = get_txtr(f"custom_door_lock_{name}")
+    for name in ("darkburst", "sunburst", "sonicboom", "screwattack", "echo_visor"):
+        txtr = get_txtr(f"custom_door_lock_{name}.TXTR")
+        emissive = get_txtr(f"custom_door_lock_{name}_emissive.TXTR", must_exist=False)
+        if emissive is None:
+            emissive = greyscale_emissive
+
         cmdl = Container(template.raw)
         cmdl.material_sets[0].texture_file_ids[0] = txtr
         cmdl.material_sets[0].texture_file_ids[1] = emissive
         editor.add_file(f"custom_door_lock_{name}.CMDL", Cmdl(cmdl, Game.ECHOES, editor), [])
 
 
 def apply_door_rando(editor: PatcherEditor, world_name: str, area_name: str, dock_name: str,
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import dataclasses
-from typing import NamedTuple
 
-from open_prime_rando.echoes.asset_ids import world
-from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
-from open_prime_rando.echoes.vulnerabilities import resist_all_vuln
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.asset_manager import NameOrAssetId
 from retro_data_structures.base_resource import AssetId
 from retro_data_structures.enums.echoes import Message, State, VisorFlags
 from retro_data_structures.formats.mapa import Mapa
 from retro_data_structures.formats.mrea import Area
 from retro_data_structures.formats.scan import Scan
 from retro_data_structures.formats.script_object import ScriptInstance
@@ -30,21 +25,28 @@
 from retro_data_structures.properties.echoes.objects.CameraShaker import CameraShaker
 from retro_data_structures.properties.echoes.objects.Counter import Counter
 from retro_data_structures.properties.echoes.objects.DamageableTrigger import DamageableTrigger
 from retro_data_structures.properties.echoes.objects.DamageableTriggerOrientated import DamageableTriggerOrientated
 from retro_data_structures.properties.echoes.objects.Dock import Dock
 from retro_data_structures.properties.echoes.objects.Door import Door
 from retro_data_structures.properties.echoes.objects.Effect import Effect
+from retro_data_structures.properties.echoes.objects.HUDHint import HUDHint
 from retro_data_structures.properties.echoes.objects.MemoryRelay import MemoryRelay
+from retro_data_structures.properties.echoes.objects.PlayerController import PlayerController
 from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScannableObjectInfo import ScannableObjectInfo
 from retro_data_structures.properties.echoes.objects.Sound import Sound
 from retro_data_structures.properties.echoes.objects.StreamedAudio import StreamedAudio
 from retro_data_structures.properties.echoes.objects.Timer import Timer
 
+from open_prime_rando.echoes.asset_ids import world
+from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
+from open_prime_rando.echoes.vulnerabilities import resist_all_vuln
+from open_prime_rando.patcher_editor import PatcherEditor
+
 
 @dataclasses.dataclass(kw_only=True)
 class DoorType:
     name: str
 
     vulnerability: DamageVulnerability
 
@@ -148,16 +150,16 @@
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
         area = self.get_area(editor, world_name, area_name)
         door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
 
         with door.edit_properties(Door) as door_props:
             door_props.vulnerability = self.vulnerability
 
-
-class BlastShieldActors(NamedTuple):
+@dataclasses.dataclass
+class BlastShieldActors:
     door: ScriptInstance
     sound: ScriptInstance
     streamed: ScriptInstance
     lock: ScriptInstance
     relay: ScriptInstance
     gibs: ScriptInstance | None
 
@@ -182,14 +184,48 @@
 
     def get_spline(self) -> Spline:
         return Spline(
             data=b'\x00\x00\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x02'
                  b'\x02A \x00\x00?\x80\x00\x00\x02\x02\x01\x00\x00\x00\x00?\x80\x00\x00'
         )
 
+    def create_trigger(self,
+                       name: str,
+                       door_xfm: Transform,
+                       health: float,
+                       visor_flags: VisorFlags = VisorFlags.Combat | VisorFlags.Dark,
+                       active: bool = True,
+                       seeker_lock_on: bool = True,
+                       orbitable: bool = False,
+    ):
+        pos = Vector(
+            door_xfm.position.x,
+            door_xfm.position.y,
+            door_xfm.position.z + 1.8
+        )
+
+        return DamageableTriggerOrientated(
+            editor_properties=EditorProperties(
+                name=name,
+                transform=Transform(
+                    position=pos,
+                    rotation=door_xfm.rotation,
+                    scale=Vector(4.0, 4.0, 1.5)
+                ),
+                active=active
+            ),
+            health=HealthInfo(health=health),
+            vulnerability=self.vulnerability,
+            enable_seeker_lock_on=seeker_lock_on,
+            orbitable=orbitable,
+            visor=VisorParameters(
+                visor_flags=visor_flags
+            )
+        )
+
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         """
         blast shield connections:
             DEAD -> lock cleared MemoryRelay, ACTV
             DEAD -> lock breaking SoundEffect, PLAY
             DEAD -> lock explosion gibs, ACTV
             DEAD -> jingle streamedaudio, PLAY
@@ -316,38 +352,14 @@
         with actors.lock.edit_properties(Actor) as lock:
             lock.vulnerability = missile_immune
         with actors.door.edit_properties(Door) as door:
             door.vulnerability = missile_immune
 
         door_transform = actors.door.get_properties_as(Door).editor_properties.transform
 
-        def create_trigger(name: str, health: float, lock_on: bool = True) -> ScriptInstance:
-            pos = Vector(
-                door_transform.position.x,
-                door_transform.position.y,
-                door_transform.position.z + 1.8
-            )
-
-            return default.add_instance_with(DamageableTriggerOrientated(
-                editor_properties=EditorProperties(
-                    name=name,
-                    transform=Transform(
-                        position=pos,
-                        rotation=door_transform.rotation,
-                        scale=Vector(4.0, 4.0, 1.5)
-                    ),
-                ),
-                health=HealthInfo(health=health),
-                vulnerability=self.vulnerability,
-                enable_seeker_lock_on=lock_on,
-                visor=VisorParameters(
-                    visor_flags=VisorFlags.Combat | VisorFlags.Dark
-                )
-            ))
-
         timer = default.add_instance_with(Timer(
             editor_properties=EditorProperties(
                 name="Button Control",
                 transform=door_transform
             ),
             time=0.75
         ))
@@ -359,17 +371,27 @@
             ),
             time=0.01
         ))
 
         # create 5 triggers so that you can have 5 lock-ons
         # 30.01 health because splash damage is inconsistent. missiles do 30 damage
         # so this guarantees you need at least 2 missiles at once to break it
-        triggers = [create_trigger(f"Bridge Button {i}", 30.01) for i in range(5)]
+        triggers = [
+            default.add_instance_with(self.create_trigger(
+                f"Bridge Button {i}",
+                door_transform, 30.01)
+            ) for i in range(5)
+        ]
         main_trigger = triggers[0]
-        mini_trigger = create_trigger("Bridge Button Mini", 1.0, False)
+        mini_trigger = default.add_instance_with(self.create_trigger(
+            "Bridge Button Mini",
+            door_transform,
+            1.0,
+            seeker_lock_on=False
+        ))
 
         # start a timer when the tiny trigger dies. stop it if the main trigger dies
         mini_trigger.add_connection(State.Dead, Message.ResetAndStart, timer)
         main_trigger.add_connection(State.Dead, Message.Stop, timer)
         for trigger in triggers:
             timer.add_connection(State.Zero, Message.Deactivate, trigger)
 
@@ -381,15 +403,15 @@
 
         # move the lock's connections to the trigger, since it's the thing that dies now
         for connection in actors.lock.connections:
             actors.lock.remove_connection(connection)
             main_trigger.add_connection(
                 connection.state,
                 connection.message,
-                default.get_instance(connection.target)
+                connection.target
             )
 
         for trigger in triggers:
             actors.relay.add_connection(State.Active, Message.Deactivate, trigger)
         actors.relay.add_connection(State.Active, Message.Deactivate, mini_trigger)
         actors.relay.add_connection(State.Active, Message.Deactivate, timer)
         actors.relay.add_connection(State.Active, Message.Deactivate, timer_reset)
@@ -421,24 +443,191 @@
 
 @dataclasses.dataclass(kw_only=True)
 class GrappleDoorType(BlastShieldDoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         raise NotImplementedError()
 
 
+@dataclasses.dataclass
+class VisorBlastShieldActors(BlastShieldActors):
+    trigger: ScriptInstance
+    visor_detector: ScriptInstance
+
+
 @dataclasses.dataclass(kw_only=True)
-class DarkVisorDoorType(BlastShieldDoorType):
+class VisorDoorType(BlastShieldDoorType):
+    visor_flags: VisorFlags
+    player_controller_proxy: int
+
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
-        raise NotImplementedError()
+        actors = super().patch_door(editor, world_name, area_name, dock_name, low_memory)
+        area = self.get_area(editor, world_name, area_name)
+        default = area.get_layer("Default")
+
+        with actors.door.edit_properties(Door) as door:
+            door.vulnerability = resist_all_vuln
+            door_xfm = door.editor_properties.transform
+
+
+        with actors.lock.edit_properties(Actor) as lock:
+            lock.vulnerability = resist_all_vuln
+
+        trigger = default.add_instance_with(self.create_trigger(
+            "Door Button", door_xfm, 1.0, self.visor_flags,
+            active=False, seeker_lock_on=False, orbitable=True
+        ))
+
+        visor_detector = default.add_instance_with(PlayerController(
+            editor_properties=EditorProperties(
+                name="Detect Visor",
+                transform=door_xfm
+            ),
+            unknown_0xe71de331=1,
+            proxy_type=self.player_controller_proxy
+        ))
+
+        visor_detector.add_connection(State.Entered, Message.Activate, trigger)
+        visor_detector.add_connection(State.Exited, Message.Deactivate, trigger)
+
+        for connection in actors.lock.connections:
+            actors.lock.remove_connection(connection)
+            trigger.add_connection(
+                connection.state,
+                connection.message,
+                connection.target
+            )
+
+        actors.relay.add_connection(State.Active, Message.Deactivate, trigger)
+        actors.relay.add_connection(State.Active, Message.Deactivate, visor_detector)
+
+        return VisorBlastShieldActors(
+            actors.door, actors.sound, actors.streamed,
+            actors.lock, actors.relay, actors.gibs,
+            trigger, visor_detector
+        )
 
 
 @dataclasses.dataclass(kw_only=True)
-class EchoVisorDoorType(BlastShieldDoorType):
+class DarkVisorDoorType(VisorDoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
-        raise NotImplementedError()
+        actors = super().patch_door(editor, world_name, area_name, dock_name, low_memory)
+
+        with actors.lock.edit_properties(Actor) as lock:
+            # TODO: update the template
+            # this property makes the actor appear red in dark visor
+            lock.actor_information.unknown_0xcd4c81a1 = True
+
+
+@dataclasses.dataclass(kw_only=True)
+class EchoVisorDoorType(VisorDoorType):
+    def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
+        actors = super().patch_door(editor, world_name, area_name, dock_name, low_memory)
+        area = self.get_area(editor, world_name, area_name)
+        default = area.get_layer("Default")
+
+        door_xfm = actors.door.get_properties_as(Door).editor_properties.transform
+
+        center_pos = Vector(
+            door_xfm.position.x,
+            door_xfm.position.y,
+            door_xfm.position.z + 1.8
+        )
+
+        hud_hint = default.add_instance_with(HUDHint(
+            editor_properties=EditorProperties(
+                name="Echo Target Icon",
+                transform=Transform(
+                    center_pos,
+                    door_xfm.rotation,
+                ),
+                active=True
+            ),
+            hud_texture=0x36B1CB06,
+            unknown_0x6078a651=24.0,
+            unknown_0xf00bb6bb=128.0,
+            animation_time=0.5,
+            animation_frames=4,
+            unknown_0xd993f97b=2
+        ))
+
+        beacon_loop = default.add_instance_with(Sound(
+            editor_properties=EditorProperties(
+                name="Echo Beacon Sound Loop",
+                transform=Transform(
+                    position=center_pos
+                ),
+            ),
+            sound=1003,
+            max_audible_distance=75.0,
+            min_volume=0,
+            max_volume=60,
+            surround_pan=SurroundPan(
+                pan=0.0,
+                surround_pan=1.0
+            ),
+            loop=True,
+            play_always=True,
+            echo_visor_max_volume=127
+        ))
+
+        disrupted = default.add_instance_with(Sound(
+            editor_properties=EditorProperties(
+                name="Echo Particle Disrupted",
+                transform=Transform(
+                    position=center_pos
+                ),
+            ),
+            sound=1004,
+            max_audible_distance=75.0,
+            min_volume=20,
+            max_volume=120,
+            surround_pan=SurroundPan(
+                pan=0.0,
+                surround_pan=1.0
+            ),
+        ))
+
+        timer = default.add_instance_with(Timer(
+            editor_properties=EditorProperties(
+                name="Open Echo Door",
+                transform=door_xfm,
+            ),
+            time=1.0
+        ))
+        for connection in actors.trigger.connections:
+            actors.trigger.remove_connection(connection)
+            timer.add_connection(
+                State.Zero,
+                connection.message,
+                connection.target
+            )
+
+        with actors.lock.edit_properties(Actor) as lock:
+            lock.echo_information.is_echo_emitter = True
+
+        actors.trigger.add_connection(State.Dead, Message.ResetAndStart, timer)
+        actors.trigger.add_connection(State.Dead, Message.InternalMessage00, hud_hint)
+        actors.trigger.add_connection(State.Dead, Message.Stop, beacon_loop)
+        actors.trigger.add_connection(State.Dead, Message.Play, disrupted)
+
+        actors.visor_detector.add_connection(State.Entered, Message.Play, beacon_loop)
+        actors.visor_detector.add_connection(State.Exited, Message.Stop, beacon_loop)
+
+        actors.relay.add_connection(State.Active, Message.Deactivate, hud_hint)
+        actors.relay.add_connection(State.Active, Message.Deactivate, beacon_loop)
+        actors.relay.add_connection(State.Active, Message.Deactivate, timer)
+        actors.relay.add_connection(State.Active, Message.Deactivate, disrupted)
+
+        dependencies = (
+            0x36B1CB06, # hud hint TXTR
+            0x4FBCAC73 # DigitalGuardianBeacon.AGSC
+        )
+        for pak in self.get_paks(editor, world_name, area_name):
+            for asset in dependencies:
+                editor.ensure_present(pak, asset)
 
 
 @dataclasses.dataclass(kw_only=True)
 class ScanVisorDoorType(BlastShieldDoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         raise NotImplementedError()
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,247 +1,275 @@
 import dataclasses
 
-from open_prime_rando.echoes.dock_lock_rando import dock_type
-from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
-from open_prime_rando.echoes.vulnerabilities import resist_all_vuln, vulnerable
+from retro_data_structures.enums.echoes import VisorFlags
 from retro_data_structures.properties.echoes.core.Color import Color
 from retro_data_structures.properties.echoes.core.Vector import Vector
 
+from open_prime_rando.echoes.dock_lock_rando import dock_type
+from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
+from open_prime_rando.echoes.vulnerabilities import normal_vuln, resist_all_vuln, vulnerable, vulnerable_no_splash
+
 normal_door_model = 0x6B78FD92
 dark_door_model = 0xbbcf134d
 annihilator_door_model = 0xa50c7238
 
 blast_collision_box = Vector(0.35, 5.0, 4.0)
 blast_collision_offset = Vector(-2 / 3, 0, 2.0)
 
 DOCK_TYPES: dict[str, dock_type.DoorType] = {
     "Normal": dock_type.NormalDoorType(
         name="Normal",
-        vulnerability=dataclasses.replace(
-            resist_all_vuln,
-            power=vulnerable, dark=vulnerable, light=vulnerable, annihilator=vulnerable,
-            power_charge=vulnerable, entangler=vulnerable, light_blast=vulnerable, sonic_boom=vulnerable,
-            super_missle=vulnerable, black_hole=vulnerable, sunburst=vulnerable, imploder=vulnerable,
-
-            missile=vulnerable, bomb=vulnerable, power_bomb=vulnerable,
-
-        ),
-        shell_color=Color(r=0, g=1, b=1, a=1),
+        vulnerability=normal_vuln,
+        shell_color=Color(0, 1, 1, 1),
         map_icon=DoorMapIcon.Normal,
     ),
     "Dark": dock_type.NormalDoorType(
         name="Dark",
         vulnerability=dataclasses.replace(resist_all_vuln, dark=vulnerable, entangler=vulnerable,
                                           black_hole=vulnerable),
         shell_model=dark_door_model,
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. Dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Dark
     ),
     "Light": dock_type.NormalDoorType(
         name="Light",
         vulnerability=dataclasses.replace(resist_all_vuln, light=vulnerable, light_blast=vulnerable,
                                           sunburst=vulnerable),
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. Light energy may damage it."
         ),
         map_icon=DoorMapIcon.Light
     ),
     "Annihilator": dock_type.NormalDoorType(
         name="Annihilator",
         vulnerability=dataclasses.replace(resist_all_vuln, annihilator=vulnerable, sonic_boom=vulnerable,
                                           imploder=vulnerable),
         shell_model=annihilator_door_model,
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A mix of light and dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Annihilator
     ),
     "Disabled": dock_type.NormalDoorType(
         name="Disabled",
         vulnerability=resist_all_vuln,
-        shell_color=Color(r=0, g=0, b=0, a=0),
+        shell_color=Color(0, 0, 0, 0),
         scan_text=(
             "Door system access denied.",
             "Unable to bypass security codes. Seek an alternate exit."
         ),
         map_icon=DoorMapIcon.Disabled
     ),
     "Missile": dock_type.VanillaBlastShieldDoorType(
         name="Missile",
         vulnerability=dataclasses.replace(resist_all_vuln, missile=vulnerable),
-        shell_color=Color(r=1, g=0, b=0, a=1),
+        shell_color=Color(1, 0, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Missile blast may damage it."
         ),
         map_icon=DoorMapIcon.Missile,
         shield_model=0xBFB4A8EE,
     ),
     "SuperMissile": dock_type.VanillaBlastShieldDoorType(
         name="SuperMissile",
         vulnerability=dataclasses.replace(resist_all_vuln, super_missle=vulnerable),
-        shell_color=Color(r=0, g=1, b=0, a=1),
+        shell_color=Color(0, 1, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A Super Missile blast may damage it."
         ),
         map_icon=DoorMapIcon.SuperMissile,
         shield_model=0xF115F575,
     ),
     "PowerBomb": dock_type.VanillaBlastShieldDoorType(
         name="PowerBomb",
         vulnerability=dataclasses.replace(resist_all_vuln, power_bomb=vulnerable),
-        shell_color=Color(r=1, g=0.94, b=0, a=1),
+        shell_color=Color(1, 0.94, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Power Bomb may damage it."
         ),
         map_icon=DoorMapIcon.PowerBomb,
         shield_model=0xC2E4F075,
     ),
     "SeekerMissile": dock_type.SeekerBlastShieldDoorType(
         name="SeekerMissile",
         vulnerability=dataclasses.replace(resist_all_vuln, missile=vulnerable),
-        shell_color=Color(r=0.5, g=0, b=0.64, a=1),
+        shell_color=Color(0.5, 0, 0.64, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "Five simultaneous Missile blasts may damage it."
         ),
         map_icon=DoorMapIcon.SeekerMissile,
         shield_model=0x56F4208B,
     ),
     "ScrewAttack": dock_type.BlastShieldDoorType(
         name="ScrewAttack",
         vulnerability=dataclasses.replace(resist_all_vuln, screw_attack=vulnerable),
-        shell_model=annihilator_door_model,
-        shell_color=Color(r=0, g=0, b=1, a=1),
+        shell_model=normal_door_model,
+        shell_color=Color(0.93, 0.58, 0.83, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Screw Attack may damage it."
         ),
         map_icon=DoorMapIcon.ScrewAttack,
-        shield_model=0x56F4208B,
+        shield_model="custom_door_lock_screwattack.CMDL",
     ),
     "Bomb": dock_type.BlastShieldDoorType(
         name="Bomb",
         vulnerability=dataclasses.replace(resist_all_vuln, bomb=vulnerable),
-        shell_model=annihilator_door_model,
-        shell_color=Color(r=0, g=1, b=1, a=1),
+        shell_model=normal_door_model,
+        shell_color=Color(1/3, 1/3, 0.5, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A Morph Ball Bomb blast may damage it."
         ),
         map_icon=DoorMapIcon.Bomb,
-        shield_model=0x56F4208B,
+        shield_model="custom_door_lock_sonicboom.CMDL",
     ),
     "Boost": dock_type.BlastShieldDoorType(
         name="Boost",
-        vulnerability=dataclasses.replace(resist_all_vuln, boost_ball=vulnerable, cannon_ball=vulnerable),
-        shell_model=annihilator_door_model,
-        shell_color=Color(r=1, g=1, b=0, a=1),
+        vulnerability=dataclasses.replace(
+            resist_all_vuln,
+            boost_ball=vulnerable,
+            cannon_ball=vulnerable_no_splash
+        ),
+        shell_model=normal_door_model,
+        shell_color=Color(1, 1/3, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Boost Ball may damage it."
         ),
         map_icon=DoorMapIcon.Boost,
-        shield_model=0x56F4208B,
+        shield_model=0xBFB4A8EE,
     ),
     "Grapple": dock_type.GrappleDoorType(
         name="Grapple",
         vulnerability=resist_all_vuln,
         shell_model=annihilator_door_model,
-        shell_color=Color(r=1, g=0, b=0, a=1),
+        shell_color=Color(1, 0, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to weapon fire, but is weakly secured. "
             "The Grapple Beam may be able to remove it."
         ),
         map_icon=DoorMapIcon.Grapple,
         shield_model=0x56F4208B,
     ),
     "Darkburst": dock_type.BlastShieldDoorType(
         name="Darkburst",
         vulnerability=dataclasses.replace(resist_all_vuln, black_hole=vulnerable),
         shell_model=dark_door_model,
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Dark,
         shield_model="custom_door_lock_darkburst.CMDL",
     ),
     "Sunburst": dock_type.BlastShieldDoorType(
         name="Sunburst",
         vulnerability=dataclasses.replace(resist_all_vuln, sunburst=vulnerable),
         shell_model=normal_door_model,
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of light energy may damage it."
         ),
         map_icon=DoorMapIcon.Light,
         shield_model="custom_door_lock_sunburst.CMDL",
     ),
     "SonicBoom": dock_type.BlastShieldDoorType(
         name="SonicBoom",
         vulnerability=dataclasses.replace(resist_all_vuln, imploder=vulnerable),
         shell_model=annihilator_door_model,
-        shell_color=Color(r=1, g=1, b=1, a=1),
+        shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of light and dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Annihilator,
         shield_model="custom_door_lock_sonicboom.CMDL",
     ),
     "AgonEnergy": dock_type.PlanetaryEnergyDoorType(
         name="AgonEnergy",
         vulnerability=resist_all_vuln,
-        shell_color=Color(r=0.64, g=0.34, b=0, a=1),
+        shell_color=Color(0.64, 0.34, 0, 1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
             "Analysis indicates that the barrier is linked to the energy of Agon. Return the energy to the Agon Temple."
         ),
         map_icon=DoorMapIcon.AgonEnergy,
         planetary_energy_item_id=-1  # TODO
     ),
     "TorvusEnergy": dock_type.PlanetaryEnergyDoorType(
         name="TorvusEnergy",
         vulnerability=resist_all_vuln,
-        shell_color=Color(r=0.31, g=0.59, b=38, a=1),
+        shell_color=Color(0.31, 0.59, 38, 1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
             "Analysis indicates that the barrier is linked to the energy of Torvus. "
             "Return the energy to the Torvus Temple."
         ),
         map_icon=DoorMapIcon.TorvusEnergy,
         planetary_energy_item_id=-1  # TODO
     ),
     "SanctuaryEnergy": dock_type.PlanetaryEnergyDoorType(
         name="SanctuaryEnergy",
         vulnerability=resist_all_vuln,
-        shell_color=Color(r=0.64, g=0.34, b=0, a=1),
+        shell_color=Color(0.64, 0.34, 0, 1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
             "Analysis indicates that the barrier is linked to the energy of Sanctuary. "
             "Return the energy to the Sanctuary Temple."
         ),
         map_icon=DoorMapIcon.AgonEnergy,
         planetary_energy_item_id=-1  # TODO
     ),
+    "EchoVisor": dock_type.EchoVisorDoorType(
+        name="EchoVisor",
+        vulnerability=normal_vuln,
+        shell_model=dark_door_model,
+        shell_color=Color(1/16, 1/16, 1/16, 1),
+        scan_text=(
+            "There is a Blast Shield on the door blocking access. ",
+            "Sonic detection gear needed to interface with this system."
+            "Neutralizing the control emitter may disable it."
+        ),
+        map_icon=DoorMapIcon.EchoVisor,
+        shield_model="custom_door_lock_echo_visor.CMDL",
+        visor_flags=VisorFlags.Echo,
+        player_controller_proxy=8,
+    ),
+    "DarkVisor": dock_type.DarkVisorDoorType(
+        name="DarkVisor",
+        vulnerability=normal_vuln,
+        shell_model=dark_door_model,
+        shell_color=Color(1, 0, 0, 1),
+        scan_text=(
+            "There is a Blast Shield on the door blocking access. ",
+            "Scans indicate presence of a control system."
+            "Interface method unknown. Control units not present in the visible spectrum or current timespace. "
+        ),
+        map_icon=DoorMapIcon.DarkVisor,
+        shield_model=0xBFB4A8EE,
+        visor_flags=VisorFlags.Dark,
+        player_controller_proxy=7,
+    )
 }
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 
     DoorMapIcon.AgonEnergy: DoorIconColors(0xa45600ff),
     DoorMapIcon.TorvusEnergy: DoorIconColors(0x4e9761ff),
     DoorMapIcon.SanctuaryEnergy: DoorIconColors(0x56789dff),
 
     DoorMapIcon.ScanVisor: DoorIconColors(0x007f7fff),
     DoorMapIcon.DarkVisor: DoorIconColors(0x660000ff),
-    # DoorMapIcon.EchoVisor: None,
+    DoorMapIcon.EchoVisor: DoorIconColors(0xcc7a00ff),
 
-    # DoorMapIcon.ScrewAttack: None,
-    # DoorMapIcon.Bomb: None,
-    # DoorMapIcon.Boost: None,
+    DoorMapIcon.ScrewAttack: DoorIconColors(0xed94d4ff),
+    DoorMapIcon.Bomb: DoorIconColors(0x55557fff),
+    DoorMapIcon.Boost: DoorIconColors(0xff5500ff),
     # DoorMapIcon.Grapple: None,
 
     DoorMapIcon.Disabled: DoorIconColors(0x202020ff),
 }
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from retro_data_structures.enums.echoes import Message, State
+from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
+from retro_data_structures.properties.echoes.objects.Timer import Timer
+
 import open_prime_rando.echoes.asset_ids.agon_wastes as agon_wastes
 import open_prime_rando.echoes.asset_ids.great_temple as great_temple
 import open_prime_rando.echoes.asset_ids.sanctuary_fortress as sanctuary_fortress
 import open_prime_rando.echoes.asset_ids.temple_grounds as temple_grounds
 import open_prime_rando.echoes.asset_ids.torvus_bog as torvus_bog
 import open_prime_rando.echoes.asset_ids.world as world
 from open_prime_rando.patcher_editor import PatcherEditor
-from retro_data_structures.enums.echoes import Message, State
-from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
-from retro_data_structures.properties.echoes.objects.Timer import Timer
 
 ELEVATOR_MEMORY_RELAY_PER_MREA = {
     world.GREAT_TEMPLE_MLVL: {
         great_temple.TEMPLE_TRANSPORT_A_MREA: 0x00000107,
         great_temple.TEMPLE_TRANSPORT_B_MREA: 0x0008002f,
         great_temple.TEMPLE_TRANSPORT_C_MREA: 0x00060046,
     },
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/elevator_rando.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/elevator_rando.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.formats.mrea import Area
 from retro_data_structures.formats.strg import Strg
 from retro_data_structures.properties.echoes.objects.WorldTeleporter import WorldTeleporter
 
+from open_prime_rando.patcher_editor import PatcherEditor
+
 
 def patch_elevator(editor: PatcherEditor, area: Area, elevator_id: int,
                    target_mlvl: int, target_mrea: int, target_strg: int, target_name: str):
 
     elevator = area.get_instance(elevator_id)
     with elevator.edit_properties(WorldTeleporter) as props:
         props.world = target_mlvl
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import dataclasses
 
 import construct
-from open_prime_rando.echoes.asset_ids import world as world_ids
-from open_prime_rando.echoes.inverted import area_pairs
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.base_resource import Dependency, RawResource
 from retro_data_structures.dependencies import recursive_dependencies_for_editor
 from retro_data_structures.formats import Mlvl
 from retro_data_structures.formats.mrea import Area
 from retro_data_structures.formats.script_layer import ScriptLayer
 from retro_data_structures.formats.script_object import InstanceId, ScriptInstance
 from retro_data_structures.properties.echoes.objects.AreaAttributes import AreaAttributes
 from retro_data_structures.properties.echoes.objects.SafeZone import SafeZone
 from retro_data_structures.properties.echoes.objects.SafeZoneCrystal import SafeZoneCrystal
 
+from open_prime_rando.echoes.asset_ids import world as world_ids
+from open_prime_rando.echoes.inverted import area_pairs
+from open_prime_rando.patcher_editor import PatcherEditor
+
 _WORLDS = [
     world_ids.TEMPLE_GROUNDS_MLVL, world_ids.AGON_WASTES_MLVL, world_ids.TORVUS_BOG_MLVL,
     world_ids.SANCTUARY_FORTRESS_MLVL, world_ids.GREAT_TEMPLE_MLVL,
 ]
 _AREAS_TO_SKIP = {
     0x775664a5,  # 00_scandummy
     0x752b2850,  # game_end_part1
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998015873015872%*

 * *Differences: {"'$defs'": "{'dock_type': {'enum': {insert: [(19, 'DarkVisor'), (20, 'EchoVisor')]}}}"}*

```diff
@@ -126,15 +126,17 @@
                 "Boost",
                 "Grapple",
                 "Darkburst",
                 "Sunburst",
                 "SonicBoom",
                 "AgonEnergy",
                 "TorvusEnergy",
-                "SanctuaryEnergy"
+                "SanctuaryEnergy",
+                "DarkVisor",
+                "EchoVisor"
             ],
             "type": "string"
         },
         "world": {
             "$comment": "The list of areas is replaced in runtime with the existing areas of each specific world.",
             "additionalProperties": false,
             "properties": {
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/echo_locks.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import random
 
-from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA, SENTINELS_PATH_MREA
-from open_prime_rando.echoes.asset_ids.temple_grounds import PROFANE_PATH_MREA
-from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL, TEMPLE_GROUNDS_MLVL
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.enums.echoes import Message, ScanSpeed, State
 from retro_data_structures.formats.scan import Scan
 from retro_data_structures.formats.strg import Strg
 from retro_data_structures.properties.echoes.objects.PointOfInterest import PointOfInterest
 from retro_data_structures.properties.echoes.objects.ScannableObjectInfo import ScannableObjectInfo
 from retro_data_structures.properties.echoes.objects.Sound import Sound
 from retro_data_structures.properties.echoes.objects.Switch import Switch
 
+from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA, SENTINELS_PATH_MREA
+from open_prime_rando.echoes.asset_ids.temple_grounds import PROFANE_PATH_MREA
+from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL, TEMPLE_GROUNDS_MLVL
+from open_prime_rando.patcher_editor import PatcherEditor
+
 ECHO_LOCK_MREAS = [
     (SANCTUARY_FORTRESS_MLVL, MAIN_GYRO_CHAMBER_MREA),
     (SANCTUARY_FORTRESS_MLVL, SENTINELS_PATH_MREA),
     (TEMPLE_GROUNDS_MLVL, PROFANE_PATH_MREA)
 ]
 ECHO_LOCK_STATES = [State.Zero, State.InternalState00, State.InternalState01, State.InternalState02]
 ECHO_LOCK_SOUNDS = [1005, 1006, 1007]
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import random
 from enum import Enum
 
+from retro_data_structures.enums.echoes import Message, State
+from retro_data_structures.formats.strg import Strg
+
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MINIGYRO_CHAMBER_MREA
 from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
-from retro_data_structures.enums.echoes import Message, State
-from retro_data_structures.formats.strg import Strg
 
 
 class GyroColor(Enum):
     AMBER = 0
     COBALT = 1
     CRIMSON = 2
     EMERALD = 3
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/rubiks.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import random
 from dataclasses import dataclass
 from pathlib import Path
 
-from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA
-from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.base_resource import RawResource
 from retro_data_structures.enums.echoes import Message, State
 from retro_data_structures.formats.cmdl import Cmdl
 from retro_data_structures.properties.echoes.archetypes.Transform import Transform
 from retro_data_structures.properties.echoes.core.Vector import Vector
 from retro_data_structures.properties.echoes.objects.Actor import Actor
 from retro_data_structures.properties.echoes.objects.DamageableTrigger import DamageableTrigger
 from retro_data_structures.properties.echoes.objects.Waypoint import Waypoint
 
+from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA
+from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL
+from open_prime_rando.patcher_editor import PatcherEditor
+
 RUBIKS_CUBES = {
     "Puzzle 1": [
         0x240013, 0x2401A4, 0x240145,
         0x24010A, 0x24000E, 0x240192,
         0x240139, 0x24013A, 0x240148,
     ],
     "Puzzle 2": [
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/specific_area_patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 
 from construct import Container
-from open_prime_rando.echoes.asset_ids.agon_wastes import MINING_STATION_B_MREA, PORTAL_TERMINAL_MREA
-from open_prime_rando.echoes.asset_ids.torvus_bog import TORVUS_ENERGY_CONTROLLER_MREA, TORVUS_TEMPLE_MREA
-from open_prime_rando.echoes.asset_ids.world import TORVUS_BOG_MLVL
-from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.enums.echoes import Message, State
 from retro_data_structures.formats.script_object import ScriptInstance
 from retro_data_structures.game_check import Game
 from retro_data_structures.properties.echoes.objects.Counter import Counter
 from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScriptLayerController import ScriptLayerController
 
+from open_prime_rando.echoes.asset_ids.agon_wastes import MINING_STATION_B_MREA, PORTAL_TERMINAL_MREA
+from open_prime_rando.echoes.asset_ids.torvus_bog import TORVUS_ENERGY_CONTROLLER_MREA, TORVUS_TEMPLE_MREA
+from open_prime_rando.echoes.asset_ids.world import TORVUS_BOG_MLVL
+from open_prime_rando.patcher_editor import PatcherEditor
+
 LOG = logging.getLogger("echoes_patcher")
 
 
 def specific_patches(editor: PatcherEditor, area_patches: dict):
     # sand_mining(editor)
     # torvus_generator(editor)
     if area_patches["torvus_temple"]:
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes/vulnerabilities.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes/vulnerabilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+import dataclasses
+
 from retro_data_structures.enums import echoes
 from retro_data_structures.properties.echoes.archetypes.DamageVulnerability import DamageVulnerability
 from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
 
 reflect = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Reflect)
 vulnerable = WeaponVulnerability(damage_multiplier=100, effect=echoes.Effect.Normal)
 immune = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Normal, ignore_radius=True)
+vulnerable_no_splash = WeaponVulnerability(damage_multiplier=100.0, effect=echoes.Effect.Normal, ignore_radius=True)
 
 
 resist_all_vuln = DamageVulnerability(
     power=reflect, dark=reflect, light=reflect, annihilator=reflect,
     power_charge=reflect, entangler=reflect, light_blast=reflect, sonic_boom=reflect,
     super_missle=reflect, black_hole=reflect, sunburst=reflect, imploder=reflect,
 
     boost_ball=immune, cannon_ball=immune, screw_attack=immune, bomb=immune, power_bomb=immune,
-    missile=immune, phazon=reflect, ai=immune, poison_water=immune, dark_water=immune, lava=immune,
+    missile=reflect, phazon=reflect, ai=immune, poison_water=immune, dark_water=immune, lava=immune,
     area_damage_hot=immune, area_damage_cold=immune, area_damage_dark=immune, area_damage_light=immune,
     weapon_vulnerability=immune, normal_safe_zone=immune,
 )
+
+normal_vuln = dataclasses.replace(
+    resist_all_vuln,
+    power=vulnerable, dark=vulnerable, light=vulnerable, annihilator=vulnerable,
+    power_charge=vulnerable, entangler=vulnerable, light_blast=vulnerable, sonic_boom=vulnerable,
+    super_missle=vulnerable, black_hole=vulnerable, sunburst=vulnerable, imploder=vulnerable,
+
+    missile=vulnerable, bomb=vulnerable, power_bomb=vulnerable,
+)
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/echoes_patcher.py` & `open-prime-rando-0.8.0/src/open_prime_rando/echoes_patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 old_strg = area._raw.area_name_id
                 strg = editor.get_parsed_asset(old_strg, type_hint=Strg)
                 strg.set_string(0, area_config["new_name"])
                 paks = editor.find_paks(old_strg)
                 new_strg = editor.add_file(f"custom_name_for_{area.internal_name}.STRG", strg, paks)
                 area._raw.area_name_id = new_strg
 
-            area.build_mlvl_dependencies(only_modified=True)
+            area.update_all_dependencies(only_modified=True)
 
 
 def apply_corrupted_memory_card_change(editor: PatcherEditor):
     # STRG_MemoryCard_0
     table = editor.get_file(0x88E242D6, Strg)
 
     name_to_index = {
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.8.0/src/open_prime_rando/p1r_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.8.0/src/open_prime_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.8.0/src/open_prime_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.8.0/src/open_prime_rando.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.7.1
+Version: 0.8.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.7.1/src/open_prime_rando.egg-info/SOURCES.txt` & `open-prime-rando-0.8.0/src/open_prime_rando.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
-codecov.yml
 pyproject.toml
 setup.cfg
+.github/codecov.yml
 .github/dependabot.yml
 .github/workflows/python.yml
 src/open_prime_rando/__init__.py
 src/open_prime_rando/__main__.py
 src/open_prime_rando/cli.py
 src/open_prime_rando/dynamic_schema.py
 src/open_prime_rando/echoes_patcher.py
@@ -56,15 +56,20 @@
 src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
 src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
 src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
 src/open_prime_rando/echoes/asset_ids/temple_grounds.py
 src/open_prime_rando/echoes/asset_ids/torvus_bog.py
 src/open_prime_rando/echoes/asset_ids/world.py
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
 src/open_prime_rando/echoes/dock_lock_rando/__init__.py
@@ -77,14 +82,16 @@
 src/open_prime_rando/echoes/inverted/__init__.py
 src/open_prime_rando/echoes/inverted/area_pairs.py
 src/open_prime_rando/echoes/small_randomizations/__init__.py
 src/open_prime_rando/echoes/small_randomizations/echo_locks.py
 src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
 src/open_prime_rando/echoes/small_randomizations/rubiks.py
 src/open_prime_rando/prime_remastered/schema.json
+tests/conftest.py
 tests/test_echoes_custom_Assets.py
 tests/dol_patching/conftest.py
 tests/dol_patching/test_all_prime_dol_patches.py
 tests/dol_patching/test_dol_version.py
 tests/dol_patching/test_echoes_dol_patcher.py
 tests/dol_patching/test_echoes_dol_patches.py
+tests/echoes/test_echoes_dock_lock_rando.py
 tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.7.1/tests/dol_patching/conftest.py` & `open-prime-rando-0.8.0/tests/dol_patching/conftest.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/tests/dol_patching/test_all_prime_dol_patches.py` & `open-prime-rando-0.8.0/tests/dol_patching/test_all_prime_dol_patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 
 import pytest
-from open_prime_rando.dol_patching import all_prime_dol_patches
 from ppc_asm import assembler
 from retro_data_structures.game_check import Game
 
+from open_prime_rando.dol_patching import all_prime_dol_patches
+
 
 @pytest.fixture(name="string_display")
 def _string_display():
     return all_prime_dol_patches.StringDisplayPatchAddresses(
         update_hint_state=0x80038020,
         message_receiver_string_ref=0x9000,
         wstring_constructor=0x802ff3dc,
```

### Comparing `open-prime-rando-0.7.1/tests/dol_patching/test_dol_version.py` & `open-prime-rando-0.8.0/tests/dol_patching/test_dol_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest.mock import MagicMock
 
 import pytest
-from open_prime_rando.dol_patching import dol_version
 from retro_data_structures.game_check import Game
 
+from open_prime_rando.dol_patching import dol_version
+
 test_versions = [
     dol_version.DolVersion(
         game=Game.ECHOES,
         description="Gamecube NTSC",
         build_string_address=0x803ac3b0,
         build_string=b"!#$MetroidBuildInfo!#$Build v1.028 10/18/2004 10:44:32",
         sda2_base=0x804223c0,
```

### Comparing `open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patcher.py` & `open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest.mock import MagicMock
 
 import pytest_mock
-from open_prime_rando.dol_patching.echoes import dol_patcher, dol_versions
 from retro_data_structures.game_check import Game
 
+from open_prime_rando.dol_patching.echoes import dol_patcher, dol_versions
+
 
 def test_apply_patches(mocker: pytest_mock.MockerFixture):
     # Setup
     patches_data = MagicMock()
     version_patches = dol_versions.ALL_VERSIONS[0]
     mock_find_version_for_dol = mocker.patch(
         "open_prime_rando.dol_patching.dol_version.find_version_for_dol",
```

### Comparing `open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patches.py` & `open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
+from ppc_asm.dol_file import DolHeader, Section
+
 from open_prime_rando.dol_patching.echoes import dol_patches, dol_versions
 from open_prime_rando.dol_patching.echoes.beam_configuration import BeamAmmoConfiguration
 from open_prime_rando.dol_patching.echoes.dol_patches import StartingBeamVisorAddresses
 from open_prime_rando.dol_patching.echoes.user_preferences import OprEchoesUserPreferences
-from ppc_asm.dol_file import DolHeader, Section
 
 DOLS = [
     (DolHeader(sections=(Section(offset=256, base_address=2147496192, size=1344),
                          Section(offset=1600, base_address=2147498048, size=3808352),
                          Section(offset=3969024, base_address=2147491840, size=352),
                          Section(offset=0, base_address=0, size=0),
                          Section(offset=0, base_address=0, size=0),
```

### Comparing `open-prime-rando-0.7.1/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.8.0/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.1/tools/asset_id_files.py` & `open-prime-rando-0.8.0/tools/asset_id_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import argparse
 import os.path
 from pathlib import Path
 
 import retro_data_structures.exceptions
-from open_prime_rando.patcher_editor import PatcherEditor
-from open_prime_rando.unique_area_name import CUSTOM_AREA_NAMES
 from retro_data_structures.asset_manager import IsoFileProvider
 from retro_data_structures.formats import Mrea, Strg
 from retro_data_structures.game_check import Game
 from retro_data_structures.properties.shared_objects import Dock
 
+from open_prime_rando.patcher_editor import PatcherEditor
+from open_prime_rando.unique_area_name import CUSTOM_AREA_NAMES
+
 _CUSTOM_WORLD_NAMES = {
     Game.ECHOES: {
         0x69802220: "FrontEnd",
         0xA50A80CC: "M01_SidehopperStation",
         0xAE171602: "M02_Spires",
         0xE3B0C703: "M03_CrossfireChaos",
         0x233E42BE: "M04_Pipeline",
```

