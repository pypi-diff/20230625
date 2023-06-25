# Comparing `tmp/bluecast-0.4.2.tar.gz` & `tmp/bluecast-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.4.2.tar", max compression
+gzip compressed data, was "bluecast-0.5.tar", max compression
```

## Comparing `bluecast-0.4.2.tar` & `bluecast-0.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.4.2/LICENSE
--rw-r--r--   0        0        0    17251 2023-06-24 16:24:18.563305 bluecast-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.4.2/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4.2/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.4.2/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.4.2/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     9692 2023-06-24 16:24:24.659393 bluecast-0.4.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.4.2/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0    14358 2023-06-24 17:06:59.754761 bluecast-0.4.2/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4.2/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.4.2/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.4.2/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4479 2023-06-24 15:42:29.710840 bluecast-0.4.2/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.4.2/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0     3477 2023-06-24 15:42:22.702820 bluecast-0.4.2/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.4.2/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.4.2/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.4.2/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2037 2023-06-23 04:30:50.713477 bluecast-0.4.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.4.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.4.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.4.2/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     2478 2023-06-23 04:30:45.253379 bluecast-0.4.2/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.4.2/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.4.2/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.4.2/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.4.2/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.4.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.4.2/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.4.2/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4.2/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     8999 2023-06-24 15:42:30.258842 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.4.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.4.2/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    13523 2023-06-23 14:22:20.312328 bluecast-0.4.2/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4.2/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.4.2/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.4.2/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.4.2/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.4.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.4.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     1771 2023-06-24 15:42:30.438842 bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.4.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.4.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.4.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.4.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.4.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.4.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.4.2/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.4.2/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.4.2/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     1354 2023-06-23 13:12:42.063930 bluecast-0.4.2/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.4.2/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.4.2/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.4.2/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.4.2/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.4.2/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.4.2/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.4.2/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7689 2023-06-24 16:24:24.279387 bluecast-0.4.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.4.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.4.2/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.4.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.4.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.4.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.4.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.4.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.4.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.4.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4064 2023-06-24 15:55:25.448209 bluecast-0.4.2/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.4.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.4.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.4.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.4.2/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.4.2/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.4.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.4.2/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     5760 2023-06-24 16:22:59.698145 bluecast-0.4.2/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.4.2/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.4.2/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.4.2/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.4.2/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.4.2/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.4.2/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.4.2/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.4.2/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.4.2/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2295 2023-06-24 15:55:23.176162 bluecast-0.4.2/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.4.2/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.4.2/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.4.2/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1459 2023-06-24 17:11:26.510836 bluecast-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    18369 1970-01-01 00:00:00.000000 bluecast-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.5/LICENSE
+-rw-r--r--   0        0        0    18025 2023-06-25 05:34:18.251804 bluecast-0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.5/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.5/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.5/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    11452 2023-06-25 05:34:24.396073 bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0    16373 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.5/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.5/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3843 2023-06-25 05:34:24.400073 bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     2969 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.5/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.5/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.5/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1955 2023-06-25 05:34:24.432074 bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2212 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.5/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.5/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.5/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.5/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.5/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.5/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.5/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     8999 2023-06-25 05:34:25.660126 bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    13523 2023-06-25 05:33:45.141515 bluecast-0.5/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.5/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.5/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.5/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     2239 2023-06-25 05:34:26.012141 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.5/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1890 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.5/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.5/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.5/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.5/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8731 2023-06-25 05:34:23.192022 bluecast-0.5/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.5/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.5/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.5/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.5/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.5/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.5/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.5/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.5/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.5/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4064 2023-06-25 05:34:26.144146 bluecast-0.5/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.5/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.5/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.5/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     6604 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.5/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.5/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.5/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.5/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.5/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.5/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.5/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.5/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.5/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2296 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.5/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.5/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.5/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1457 2023-06-25 05:34:02.506980 bluecast-0.5/pyproject.toml
+-rw-r--r--   0        0        0    19141 1970-01-01 00:00:00.000000 bluecast-0.5/PKG-INFO
```

### Comparing `bluecast-0.4.2/LICENSE` & `bluecast-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/README.md` & `bluecast-0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
 BlueCast focuses on a few model architectures (on default Xgboost
 only) and a few preprocessing options (only what is
 needed for Xgboost). This allows for a much faster development
 cycle and a much more stable codebase while also having as few dependencies
 as possible for the library. Despite being lightweight in its core BlueCast
-offers high customization options for advanced users.
+offers high customization options for advanced users. Find
+the full documentation [here](https://bluecast.readthedocs.io/en/latest/).
 
 <!-- toc -->
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
@@ -263,49 +264,67 @@
         conf_training=train_config,
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
-Also this step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
-Otherwise the pipeline will fail. To surpass the `RFECV` limitation a custom feature
-selection algorithm can also be passed as part of a custom last mile computation.
-Here is an example adjusting the in-built solution via `RFECV`:
+Also this step can be customized. The following example shows how to:
 
 ```sh
 from bluecast.config.training_config import FeatureSelectionConfig
 from bluecast.config.training_config import TrainingConfig
+from bluecast.preprocessing.custom import CustomPreprocessing
 from sklearn.feature_selection import RFECV
 from sklearn.metrics import make_scorer, matthews_corrcoef
 from sklearn.model_selection import StratifiedKFold
+from typing import Optional, Tuple
 
 
 # Create a custom training config and adjust general training parameters
 train_config = TrainingConfig()
 train_config.enable_feature_selection = True
 
 # add custom feature selection
-custom_feat_sel = FeatureSelectionConfig()
-# custom_feat_sel.execute_selection = False
-custom_feat_sel.selection_strategy = RFECV(
-    estimator=xgb.XGBClassifier(),
-    step=1,
-    cv=StratifiedKFold(10, random_state=0, shuffle=True),
-    min_features_to_select=1,
-    scoring=make_scorer(matthews_corrcoef),
-    n_jobs=1,
-)
+class RFECVSelector(CustomPreprocessing):
+    def __init__(self, random_state: int = 0):
+        super().__init__()
+        self.selected_features = None
+        self.random_state = random_state
+        self.selection_strategy: RFECV = RFECV(
+            estimator=xgb.XGBClassifier(),
+            step=1,
+            cv=StratifiedKFold(5, random_state=random_state, shuffle=True),
+            min_features_to_select=1,
+            scoring=make_scorer(matthews_corrcoef),
+            n_jobs=2,
+        )
+
+    def fit_transform(self, df: pd.DataFrame, target: pd.Series) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        self.selection_strategy.fit(df, target)
+        self.selected_features = self.selection_strategy.support_
+        df = df.loc[:, self.selected_features]
+        return df, target
+
+    def transform(self,
+                  df: pd.DataFrame,
+                  target: Optional[pd.Series] = None,
+                  predicton_mode: bool = False) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        df = df.loc[:, self.selected_features]
+        return df, target
+
+custom_feature_selector = RFECVSelector()
 
 # Create an instance of the BlueCast class with the custom model
 bluecast = BlueCast(
     class_problem="binary",
     target_column="target",
     conf_feature_selection=custom_feat_sel,
     conf_training=train_config,
+    custom_feature_selector=custom_feature_selector,
 
 # Create some sample data for testing
 x_train = pd.DataFrame(
     {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
 )
 y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
 x_test = pd.DataFrame(
```

### Comparing `bluecast-0.4.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 24 16:24:16 2023 UTC, .py size: 14177 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,606 +1,716 @@
-00000000: 6f0d 0d0a 0000 0000 b018 9764 6137 0000  o..........da7..
+00000000: 6f0d 0d0a 0000 0000 cad1 9764 f53f 0000  o..........d.?..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
-00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
-00000060: 6402 6c0a 5a0b 6401 6402 6c0c 5a0d 6401  d.l.Z.d.d.l.Z.d.
-00000070: 6404 6c0e 6d0f 5a0f 6d10 5a10 6d11 5a11  d.l.m.Z.m.Z.m.Z.
-00000080: 6d12 5a12 0100 6401 6405 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-00000090: 0100 6401 6406 6c15 6d16 5a16 0100 6401  ..d.d.l.m.Z...d.
-000000a0: 6407 6c17 6d18 5a18 0100 6401 6408 6c19  d.l.m.Z...d.d.l.
-000000b0: 6d1a 5a1a 0100 6401 6409 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
-000000c0: 0100 6401 640a 6c1d 6d1e 5a1e 0100 6401  ..d.d.l.m.Z...d.
-000000d0: 640b 6c1f 6d20 5a20 0100 6401 640c 6c21  d.l.m Z ..d.d.l!
-000000e0: 6d22 5a22 0100 6401 640d 6c23 6d24 5a24  m"Z"..d.d.l#m$Z$
-000000f0: 0100 6401 640e 6c25 6d26 5a26 0100 6401  ..d.d.l%m&Z&..d.
-00000100: 640f 6c27 6d28 5a28 0100 6401 6410 6c29  d.l'm(Z(..d.d.l)
-00000110: 6d2a 5a2a 6d2b 5a2b 0100 6401 6411 6c2c  m*Z*m+Z+..d.d.l,
-00000120: 6d2d 5a2d 0100 4700 6412 6413 8400 6413  m-Z-..G.d.d...d.
-00000130: 8302 5a2e 6402 5300 2914 61f9 0100 0052  ..Z.d.S.).a....R
-00000140: 756e 2066 756c 6c79 2063 6f6e 6669 6775  un fully configu
-00000150: 7265 6420 636c 6173 7369 6669 6361 7469  red classificati
-00000160: 6f6e 2062 6c75 6570 7269 6e74 2e0a 0a43  on blueprint...C
-00000170: 7573 746f 6d69 7a61 7469 6f6e 2076 6961  ustomization via
-00000180: 2063 6c61 7373 2061 7474 7269 6275 7465   class attribute
-00000190: 7320 6973 2070 6f73 7369 626c 652e 2043  s is possible. C
-000001a0: 6f6e 6669 6773 2063 616e 2062 6520 696e  onfigs can be in
-000001b0: 7374 616e 7469 6174 6564 2061 6e64 2070  stantiated and p
-000001c0: 726f 7669 6465 6420 746f 2063 6861 6e67  rovided to chang
-000001d0: 6520 5867 626f 6f73 7420 7472 6169 6e69  e Xgboost traini
-000001e0: 6e67 2e0a 4465 6661 756c 7420 6879 7065  ng..Default hype
-000001f0: 7270 6172 616d 6574 6572 2073 6561 7263  rparameter searc
-00000200: 6820 7370 6163 6520 6973 2072 656c 6174  h space is relat
-00000210: 6976 656c 7920 6c69 6768 742d 7765 6967  ively light-weig
-00000220: 6874 2074 6f20 7370 6565 6420 7570 2074  ht to speed up t
-00000230: 6865 2070 726f 746f 7479 7069 6e67 2e0a  he prototyping..
-00000240: 4361 6e20 6465 616c 2077 6974 6820 6269  Can deal with bi
-00000250: 6e61 7279 2061 6e64 206d 756c 7469 2d63  nary and multi-c
-00000260: 6c61 7373 2063 6c61 7373 6966 6963 6174  lass classificat
-00000270: 696f 6e20 7072 6f62 6c65 6d73 2e0a 4879  ion problems..Hy
-00000280: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
-00000290: 696e 6720 6361 6e20 6265 2073 7769 7463  ing can be switc
-000002a0: 6865 6420 6f66 6620 6f72 2065 7665 6e20  hed off or even 
-000002b0: 7374 7265 6e67 7468 656e 6564 2076 6961  strengthened via
-000002c0: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
-000002d0: 6e2e 2054 6869 7320 6265 6861 7669 6f75  n. This behaviou
-000002e0: 7220 6361 6e20 6265 2063 6f6e 7472 6f6c  r can be control
-000002f0: 6c65 640a 7669 6120 7468 6520 636f 6e66  led.via the conf
-00000300: 6967 2063 6c61 7373 2061 7474 7269 6275  ig class attribu
-00000310: 7465 7320 6672 6f6d 2063 6f6e 6669 672e  tes from config.
-00000320: 7472 6169 6e69 6e67 5f63 6f6e 6669 6720  training_config 
-00000330: 6d6f 6475 6c65 2e0a e900 0000 004e 2907  module.......N).
-00000340: da03 416e 79da 0444 6963 74da 044c 6973  ..Any..Dict..Lis
-00000350: 74da 074c 6974 6572 616c da08 4f70 7469  t..Literal..Opti
-00000360: 6f6e 616c da05 5475 706c 65da 0555 6e69  onal..Tuple..Uni
-00000370: 6f6e 2904 da16 4665 6174 7572 6553 656c  on)...FeatureSel
-00000380: 6563 7469 6f6e 436f 6e66 6967 da0e 5472  ectionConfig..Tr
+00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
+00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6402 6c0b  m.Z.m.Z...d.d.l.
+00000070: 5a0c 6401 6402 6c0d 5a0e 6401 6405 6c0f  Z.d.d.l.Z.d.d.l.
+00000080: 6d10 5a10 6d11 5a11 6d12 5a12 0100 6401  m.Z.m.Z.m.Z...d.
+00000090: 6406 6c13 6d14 5a14 0100 6401 6407 6c15  d.l.m.Z...d.d.l.
+000000a0: 6d16 5a16 0100 6401 6408 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
+000000b0: 6d19 5a19 0100 6401 6409 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
+000000c0: 0100 6401 640a 6c1c 6d1d 5a1d 0100 6401  ..d.d.l.m.Z...d.
+000000d0: 640b 6c1e 6d1f 5a1f 0100 6401 640c 6c20  d.l.m.Z...d.d.l 
+000000e0: 6d21 5a21 0100 6401 640d 6c22 6d23 5a23  m!Z!..d.d.l"m#Z#
+000000f0: 0100 6401 640e 6c24 6d25 5a25 0100 6401  ..d.d.l$m%Z%..d.
+00000100: 640f 6c26 6d27 5a27 0100 6401 6410 6c28  d.l&m'Z'..d.d.l(
+00000110: 6d29 5a29 0100 6401 6411 6c2a 6d2b 5a2b  m)Z)..d.d.l*m+Z+
+00000120: 6d2c 5a2c 0100 6401 6412 6c2d 6d2e 5a2e  m,Z,..d.d.l-m.Z.
+00000130: 0100 4700 6413 6414 8400 6414 8302 5a2f  ..G.d.d...d...Z/
+00000140: 6402 5300 2915 61f9 0100 0052 756e 2066  d.S.).a....Run f
+00000150: 756c 6c79 2063 6f6e 6669 6775 7265 6420  ully configured 
+00000160: 636c 6173 7369 6669 6361 7469 6f6e 2062  classification b
+00000170: 6c75 6570 7269 6e74 2e0a 0a43 7573 746f  lueprint...Custo
+00000180: 6d69 7a61 7469 6f6e 2076 6961 2063 6c61  mization via cla
+00000190: 7373 2061 7474 7269 6275 7465 7320 6973  ss attributes is
+000001a0: 2070 6f73 7369 626c 652e 2043 6f6e 6669   possible. Confi
+000001b0: 6773 2063 616e 2062 6520 696e 7374 616e  gs can be instan
+000001c0: 7469 6174 6564 2061 6e64 2070 726f 7669  tiated and provi
+000001d0: 6465 6420 746f 2063 6861 6e67 6520 5867  ded to change Xg
+000001e0: 626f 6f73 7420 7472 6169 6e69 6e67 2e0a  boost training..
+000001f0: 4465 6661 756c 7420 6879 7065 7270 6172  Default hyperpar
+00000200: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
+00000210: 6163 6520 6973 2072 656c 6174 6976 656c  ace is relativel
+00000220: 7920 6c69 6768 742d 7765 6967 6874 2074  y light-weight t
+00000230: 6f20 7370 6565 6420 7570 2074 6865 2070  o speed up the p
+00000240: 726f 746f 7479 7069 6e67 2e0a 4361 6e20  rototyping..Can 
+00000250: 6465 616c 2077 6974 6820 6269 6e61 7279  deal with binary
+00000260: 2061 6e64 206d 756c 7469 2d63 6c61 7373   and multi-class
+00000270: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00000280: 7072 6f62 6c65 6d73 2e0a 4879 7065 7270  problems..Hyperp
+00000290: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
+000002a0: 6361 6e20 6265 2073 7769 7463 6865 6420  can be switched 
+000002b0: 6f66 6620 6f72 2065 7665 6e20 7374 7265  off or even stre
+000002c0: 6e67 7468 656e 6564 2076 6961 2063 726f  ngthened via cro
+000002d0: 7373 2d76 616c 6964 6174 696f 6e2e 2054  ss-validation. T
+000002e0: 6869 7320 6265 6861 7669 6f75 7220 6361  his behaviour ca
+000002f0: 6e20 6265 2063 6f6e 7472 6f6c 6c65 640a  n be controlled.
+00000300: 7669 6120 7468 6520 636f 6e66 6967 2063  via the config c
+00000310: 6c61 7373 2061 7474 7269 6275 7465 7320  lass attributes 
+00000320: 6672 6f6d 2063 6f6e 6669 672e 7472 6169  from config.trai
+00000330: 6e69 6e67 5f63 6f6e 6669 6720 6d6f 6475  ning_config modu
+00000340: 6c65 2e0a e900 0000 004e 2901 da08 6461  le.......N)...da
+00000350: 7465 7469 6d65 2907 da03 416e 79da 0444  tetime)...Any..D
+00000360: 6963 74da 044c 6973 74da 074c 6974 6572  ict..List..Liter
+00000370: 616c da08 4f70 7469 6f6e 616c da05 5475  al..Optional..Tu
+00000380: 706c 65da 0555 6e69 6f6e 2903 da0e 5472  ple..Union)...Tr
 00000390: 6169 6e69 6e67 436f 6e66 6967 da17 5867  ainingConfig..Xg
 000003a0: 626f 6f73 7446 696e 616c 5061 7261 6d43  boostFinalParamC
 000003b0: 6f6e 6669 67da 1758 6762 6f6f 7374 5475  onfig..XgboostTu
 000003c0: 6e65 5061 7261 6d73 436f 6e66 6967 2901  neParamsConfig).
 000003d0: da0f 6576 616c 5f63 6c61 7373 6966 6965  ..eval_classifie
 000003e0: 7229 01da 1173 6861 705f 6578 706c 616e  r)...shap_explan
-000003f0: 6174 696f 6e73 2901 da11 6368 6563 6b5f  ations)...check_
-00000400: 6770 755f 7375 7070 6f72 7429 01da 0c58  gpu_support)...X
-00000410: 6762 6f6f 7374 4d6f 6465 6c29 01da 1343  gboostModel)...C
-00000420: 7573 746f 6d50 7265 7072 6f63 6573 7369  ustomPreprocessi
-00000430: 6e67 2901 da0e 6461 7465 5f63 6f6e 7665  ng)...date_conve
-00000440: 7274 6572 2901 da12 5461 7267 6574 4c61  rter)...TargetLa
-00000450: 6265 6c45 6e63 6f64 6572 2901 da0f 4665  belEncoder)...Fe
-00000460: 6174 7572 6553 656c 6563 746f 7229 01da  atureSelector)..
-00000470: 1346 6561 7475 7265 5479 7065 4465 7465  .FeatureTypeDete
-00000480: 6374 6f72 2901 da14 6669 6c6c 5f69 6e66  ctor)...fill_inf
-00000490: 696e 6974 655f 7661 6c75 6573 2901 da0e  inite_values)...
-000004a0: 5363 6865 6d61 4465 7465 6374 6f72 2902  SchemaDetector).
-000004b0: da18 4269 6e61 7279 436c 6173 7354 6172  ..BinaryClassTar
-000004c0: 6765 7445 6e63 6f64 6572 da17 4d75 6c74  getEncoder..Mult
-000004d0: 6943 6c61 7373 5461 7267 6574 456e 636f  iClassTargetEnco
-000004e0: 6465 7229 01da 1074 7261 696e 5f74 6573  der)...train_tes
-000004f0: 745f 7370 6c69 7463 0000 0000 0000 0000  t_splitc........
-00000500: 0000 0000 0000 0000 1a00 0000 4000 0000  ............@...
-00000510: 7334 0100 0065 005a 0164 005a 0264 015a  s4...e.Z.d.Z.d.Z
-00000520: 0309 0209 0209 0209 0209 0209 0209 0209  ................
-00000530: 0209 0209 0264 1f64 0365 0464 0419 0064  .....d.d.e.d...d
-00000540: 0565 0565 0665 0765 0866 0319 0064 0665  .e.e.e.e.f...d.e
-00000550: 0965 0a65 0565 0665 0765 0866 0319 0019  .e.e.e.e.e.f....
-00000560: 0019 0064 0765 0965 0a65 0565 0665 0765  ...d.e.e.e.e.e.e
-00000570: 0866 0319 0019 0019 0064 0865 0965 0619  .f.......d.e.e..
-00000580: 0064 0965 0965 0565 0b65 0c66 0219 0019  .d.e.e.e.e.f....
-00000590: 0064 0a65 0965 0d19 0064 0b65 0965 0d19  .d.e.e...d.e.e..
-000005a0: 0064 0c65 0965 0e19 0064 0d65 0965 0f19  .d.e.e...d.e.e..
-000005b0: 0064 0e65 0965 1019 0064 0f65 0965 1119  .d.e.e...d.e.e..
-000005c0: 0066 1864 1064 1184 055a 1264 1265 136a  .f.d.d...Z.d.e.j
-000005d0: 1464 1365 0664 1464 0266 0664 1564 1684  .d.e.d.d.f.d.d..
-000005e0: 045a 1564 1265 136a 1464 1765 136a 1464  .Z.d.e.j.d.e.j.d
-000005f0: 1865 136a 1664 1365 0664 1465 1765 0665  .e.j.d.e.d.e.e.e
-00000600: 0c66 0219 0066 0a64 1964 1a84 045a 1864  .f...f.d.d...Z.d
-00000610: 1265 136a 1464 1465 136a 1466 0464 1b64  .e.j.d.e.j.f.d.d
-00000620: 1c84 045a 1964 1265 136a 1464 1465 1a65  ...Z.d.e.j.d.e.e
-00000630: 1b6a 1c65 1b6a 1c66 0219 0066 0464 1d64  .j.e.j.f...f.d.d
-00000640: 1e84 045a 1d64 0253 0029 20da 0842 6c75  ...Z.d.S.) ..Blu
-00000650: 6543 6173 7461 2206 0000 5275 6e20 6675  eCasta"...Run fu
-00000660: 6c6c 7920 636f 6e66 6967 7572 6564 2063  lly configured c
-00000670: 6c61 7373 6966 6963 6174 696f 6e20 626c  lassification bl
-00000680: 7565 7072 696e 742e 0a0a 2020 2020 4375  ueprint...    Cu
-00000690: 7374 6f6d 697a 6174 696f 6e20 7669 6120  stomization via 
-000006a0: 636c 6173 7320 6174 7472 6962 7574 6573  class attributes
-000006b0: 2069 7320 706f 7373 6962 6c65 2e20 436f   is possible. Co
-000006c0: 6e66 6967 7320 6361 6e20 6265 2069 6e73  nfigs can be ins
-000006d0: 7461 6e74 6961 7465 6420 616e 6420 7072  tantiated and pr
-000006e0: 6f76 6964 6564 2074 6f20 6368 616e 6765  ovided to change
-000006f0: 2058 6762 6f6f 7374 2074 7261 696e 696e   Xgboost trainin
-00000700: 672e 0a20 2020 2044 6566 6175 6c74 2068  g..    Default h
-00000710: 7970 6572 7061 7261 6d65 7465 7220 7365  yperparameter se
-00000720: 6172 6368 2073 7061 6365 2069 7320 7265  arch space is re
-00000730: 6c61 7469 7665 6c79 206c 6967 6874 2d77  latively light-w
-00000740: 6569 6768 7420 746f 2073 7065 6564 2075  eight to speed u
-00000750: 7020 7468 6520 7072 6f74 6f74 7970 696e  p the prototypin
-00000760: 672e 0a20 2020 203a 7061 7261 6d20 3a63  g..    :param :c
-00000770: 6c61 7373 5f70 726f 626c 656d 3a20 5461  lass_problem: Ta
-00000780: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-00000790: 7461 696e 696e 6720 7468 6520 636c 6173  taining the clas
-000007a0: 7320 7072 6f62 6c65 6d20 7479 7065 2e20  s problem type. 
-000007b0: 4569 7468 6572 2022 6269 6e61 7279 2220  Either "binary" 
-000007c0: 6f72 2022 6d75 6c74 6963 6c61 7373 222e  or "multiclass".
-000007d0: 0a20 2020 203a 7061 7261 6d20 3a74 6172  .    :param :tar
-000007e0: 6765 745f 636f 6c75 6d6e 3a20 5461 6b65  get_column: Take
-000007f0: 7320 6120 7374 7269 6e67 2063 6f6e 7461  s a string conta
-00000800: 696e 696e 6720 7468 6520 6e61 6d65 206f  ining the name o
-00000810: 6620 7468 6520 7461 7267 6574 2063 6f6c  f the target col
-00000820: 756d 6e2e 0a20 2020 203a 7061 7261 6d20  umn..    :param 
-00000830: 3a63 6174 5f63 6f6c 756d 6e73 3a20 5461  :cat_columns: Ta
-00000840: 6b65 7320 6120 6c69 7374 206f 6620 7374  kes a list of st
-00000850: 7269 6e67 7320 636f 6e74 6169 6e69 6e67  rings containing
-00000860: 2074 6865 206e 616d 6573 206f 6620 7468   the names of th
-00000870: 6520 6361 7465 676f 7269 6361 6c20 636f  e categorical co
-00000880: 6c75 6d6e 732e 2049 6620 6e6f 7420 7072  lumns. If not pr
-00000890: 6f76 6964 6564 2c0a 2020 2020 426c 7565  ovided,.    Blue
-000008a0: 4361 7374 2077 696c 6c20 696e 6665 7220  Cast will infer 
-000008b0: 7468 6573 6520 6175 746f 6d61 6963 616c  these automaical
-000008c0: 6c79 2e0a 2020 2020 3a70 6172 616d 203a  ly..    :param :
-000008d0: 6461 7465 5f63 6f6c 756d 6e73 3a20 5461  date_columns: Ta
-000008e0: 6b65 7320 6120 6c69 7374 206f 6620 7374  kes a list of st
-000008f0: 7269 6e67 7320 636f 6e74 6169 6e69 6e67  rings containing
-00000900: 2074 6865 206e 616d 6573 206f 6620 7468   the names of th
-00000910: 6520 6461 7465 2063 6f6c 756d 6e73 2e20  e date columns. 
-00000920: 4966 206e 6f74 2070 726f 7669 6465 642c  If not provided,
-00000930: 0a20 2020 2042 6c75 6543 6173 7420 7769  .    BlueCast wi
-00000940: 6c6c 2069 6e66 6572 2074 6865 7365 2061  ll infer these a
-00000950: 7574 6f6d 6169 6361 6c6c 792e 0a20 2020  utomaically..   
-00000960: 203a 7061 7261 6d20 3a74 696d 655f 7370   :param :time_sp
-00000970: 6c69 745f 636f 6c75 6d6e 3a20 5461 6b65  lit_column: Take
-00000980: 7320 6120 7374 7269 6e67 2063 6f6e 7461  s a string conta
-00000990: 696e 696e 6720 7468 6520 6e61 6d65 206f  ining the name o
-000009a0: 6620 7468 6520 7469 6d65 2073 706c 6974  f the time split
-000009b0: 2063 6f6c 756d 6e2e 2049 6620 6e6f 7420   column. If not 
-000009c0: 7072 6f76 6964 6564 2c0a 2020 2020 426c  provided,.    Bl
-000009d0: 7565 4361 7374 2077 696c 6c20 6e6f 7420  ueCast will not 
-000009e0: 7370 6c69 7420 7468 6520 6461 7461 2062  split the data b
-000009f0: 7920 7469 6d65 206f 7220 6f72 6465 722c  y time or order,
-00000a00: 2062 7574 2064 6f20 6120 7261 6e64 6f6d   but do a random
-00000a10: 2073 706c 6974 2069 6e73 7465 6164 2e0a   split instead..
-00000a20: 2020 2020 3a70 6172 616d 203a 6d6c 5f6d      :param :ml_m
-00000a30: 6f64 656c 3a20 5461 6b65 7320 616e 2069  odel: Takes an i
-00000a40: 6e73 7461 6e63 6520 6f66 2061 2058 6762  nstance of a Xgb
-00000a50: 6f6f 7374 4d6f 6465 6c20 636c 6173 732e  oostModel class.
-00000a60: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
-00000a70: 2c20 426c 7565 4361 7374 2077 696c 6c20  , BlueCast will 
-00000a80: 696e 7374 616e 7469 6174 6520 6f6e 652e  instantiate one.
-00000a90: 0a20 2020 2054 6869 7320 6973 2061 6e20  .    This is an 
-00000aa0: 4150 4920 746f 2070 6173 7320 616e 7920  API to pass any 
-00000ab0: 6d6f 6465 6c20 636c 6173 732e 2049 6e68  model class. Inh
-00000ac0: 6572 6974 2074 6865 2062 6173 6563 6c61  erit the basecla
-00000ad0: 7373 2066 726f 6d20 6d6c 5f6d 6f64 656c  ss from ml_model
-00000ae0: 6c69 6e67 2e62 6173 655f 6d6f 6465 6c2e  ling.base_model.
-00000af0: 4261 7365 4d6f 6465 6c2e 0a20 2020 203a  BaseModel..    :
-00000b00: 7061 7261 6d20 6375 7374 6f6d 5f70 7265  param custom_pre
-00000b10: 7072 6f63 6573 736f 723a 2054 616b 6573  processor: Takes
-00000b20: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
-00000b30: 6120 4375 7374 6f6d 5072 6570 726f 6365  a CustomPreproce
-00000b40: 7373 696e 6720 636c 6173 732e 2041 6c6c  ssing class. All
-00000b50: 6f77 7320 7573 6572 7320 746f 2069 6e6a  ows users to inj
-00000b60: 6563 7420 6375 7374 6f6d 0a20 2020 2070  ect custom.    p
-00000b70: 7265 7072 6f63 6573 7369 6e67 2073 7465  reprocessing ste
-00000b80: 7073 2077 6869 6368 2074 616b 6520 706c  ps which take pl
-00000b90: 6163 6520 7269 6768 7420 6166 7465 7220  ace right after 
-00000ba0: 7468 6520 7472 6169 6e20 7465 7374 2073  the train test s
-00000bb0: 7069 742e 0a20 2020 203a 7061 7261 6d20  pit..    :param 
-00000bc0: 6375 7374 6f6d 5f6c 6173 745f 6d69 6c65  custom_last_mile
-00000bd0: 5f63 6f6d 7075 7461 7469 6f6e 3a20 5461  _computation: Ta
-00000be0: 6b65 7320 616e 2069 6e73 7461 6e63 6520  kes an instance 
-00000bf0: 6f66 2061 2043 7573 746f 6d50 7265 7072  of a CustomPrepr
-00000c00: 6f63 6573 7369 6e67 2063 6c61 7373 2e20  ocessing class. 
-00000c10: 416c 6c6f 7773 2075 7365 7273 2074 6f20  Allows users to 
-00000c20: 696e 6a65 6374 2063 7573 746f 6d0a 2020  inject custom.  
-00000c30: 2020 7072 6570 726f 6365 7373 696e 6720    preprocessing 
-00000c40: 7374 6570 7320 7768 6963 6820 7461 6b65  steps which take
-00000c50: 2070 6c61 6365 2072 6967 6874 2062 6566   place right bef
-00000c60: 6f72 6520 7468 6520 6d6f 6465 6c20 7472  ore the model tr
-00000c70: 6169 6e69 6e67 2e0a 2020 2020 4eda 0d63  aining..    N..c
-00000c80: 6c61 7373 5f70 726f 626c 656d 2902 da06  lass_problem)...
-00000c90: 6269 6e61 7279 da0a 6d75 6c74 6963 6c61  binary..multicla
-00000ca0: 7373 da0d 7461 7267 6574 5f63 6f6c 756d  ss..target_colum
-00000cb0: 6eda 0b63 6174 5f63 6f6c 756d 6e73 da0c  n..cat_columns..
-00000cc0: 6461 7465 5f63 6f6c 756d 6e73 da11 7469  date_columns..ti
-00000cd0: 6d65 5f73 706c 6974 5f63 6f6c 756d 6eda  me_split_column.
-00000ce0: 086d 6c5f 6d6f 6465 6cda 1c63 7573 746f  .ml_model..custo
-00000cf0: 6d5f 6c61 7374 5f6d 696c 655f 636f 6d70  m_last_mile_comp
-00000d00: 7574 6174 696f 6eda 1363 7573 746f 6d5f  utation..custom_
-00000d10: 7072 6570 726f 6365 7373 6f72 da0d 636f  preprocessor..co
-00000d20: 6e66 5f74 7261 696e 696e 67da 0c63 6f6e  nf_training..con
-00000d30: 665f 7867 626f 6f73 74da 1363 6f6e 665f  f_xgboost..conf_
-00000d40: 7061 7261 6d73 5f78 6762 6f6f 7374 da16  params_xgboost..
-00000d50: 636f 6e66 5f66 6561 7475 7265 5f73 656c  conf_feature_sel
-00000d60: 6563 7469 6f6e 630d 0000 0000 0000 0000  ectionc.........
-00000d70: 0000 000d 0000 0002 0000 0043 0000 0073  ...........C...s
-00000d80: 7600 0000 7c01 7c00 5f00 6401 7c00 5f01  v...|.|._.d.|._.
-00000d90: 7c03 7c00 5f02 7c04 7c00 5f03 7c05 7c00  |.|._.|.|._.|.|.
-00000da0: 5f04 7c02 7c00 5f05 7c09 7c00 5f06 7c0a  _.|.|._.|.|._.|.
-00000db0: 7c00 5f07 7c0b 7c00 5f08 7c0c 7c00 5f09  |._.|.|._.|.|._.
-00000dc0: 6400 7c00 5f0a 6400 7c00 5f0b 6400 7c00  d.|._.d.|._.d.|.
-00000dd0: 5f0c 6400 7c00 5f0d 6400 7c00 5f0e 7c06  _.d.|._.d.|._.|.
-00000de0: 7c00 5f0f 7c07 7c00 5f10 7c08 7c00 5f11  |._.|.|._.|.|._.
-00000df0: 6400 7c00 5f12 6400 5300 2902 4e46 2913  d.|._.d.S.).NF).
-00000e00: 721c 0000 00da 0f70 7265 6469 6374 696f  r......predictio
-00000e10: 6e5f 6d6f 6465 7220 0000 0072 2100 0000  n_moder ...r!...
-00000e20: 7222 0000 0072 1f00 0000 7226 0000 0072  r"...r....r&...r
-00000e30: 2700 0000 7228 0000 0072 2900 0000 da10  '...r(...r).....
-00000e40: 6665 6174 7572 655f 7365 6c65 6374 6f72  feature_selector
-00000e50: da12 6665 6174 5f74 7970 655f 6465 7465  ..feat_type_dete
-00000e60: 6374 6f72 da0b 6361 745f 656e 636f 6465  ctor..cat_encode
-00000e70: 72da 1474 6172 6765 745f 6c61 6265 6c5f  r..target_label_
-00000e80: 656e 636f 6465 72da 0f73 6368 656d 615f  encoder..schema_
-00000e90: 6465 7465 6374 6f72 7223 0000 0072 2400  detectorr#...r$.
-00000ea0: 0000 7225 0000 00da 0b73 6861 705f 7661  ..r%.....shap_va
-00000eb0: 6c75 6573 290d da04 7365 6c66 721c 0000  lues)...selfr...
-00000ec0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000ed0: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
-00000ee0: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
-00000ef0: 0000 0072 2900 0000 a900 7232 0000 00fa  ...r).....r2....
-00000f00: 3e2f 686f 6d65 2f74 686f 6d61 732f 4964  >/home/thomas/Id
-00000f10: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
-00000f20: 6173 742f 626c 7565 6361 7374 2f62 6c75  ast/bluecast/blu
-00000f30: 6570 7269 6e74 732f 6361 7374 2e70 79da  eprints/cast.py.
-00000f40: 085f 5f69 6e69 745f 5f3c 0000 0073 2800  .__init__<...s(.
-00000f50: 0000 060f 0601 0601 0601 0601 0601 0601  ................
-00000f60: 0601 0601 0601 0601 0601 0203 04fe 0603  ................
-00000f70: 0601 0601 0601 0601 0a01 7a11 426c 7565  ..........z.Blue
-00000f80: 4361 7374 2e5f 5f69 6e69 745f 5fda 0264  Cast.__init__..d
-00000f90: 66da 0a74 6172 6765 745f 636f 6cda 0672  f..target_col..r
-00000fa0: 6574 7572 6e63 0300 0000 0000 0000 0000  eturnc..........
-00000fb0: 0000 0a00 0000 0700 0000 4300 0000 730e  ..........C...s.
-00000fc0: 0300 0074 0083 0001 0074 0183 007d 037c  ...t.....t...}.|
-00000fd0: 03a0 027c 01a1 017d 017c 037c 005f 037c  ...|...}.|.|._.|
-00000fe0: 006a 036a 0472 297c 006a 057c 006a 036a  .j.j.r)|.j.|.j.j
-00000ff0: 0476 0072 2974 0683 007c 005f 077c 006a  .v.r)t...|._.|.j
-00001000: 07a0 087c 017c 006a 0519 00a1 017c 017c  ...|.|.j.....|.|
-00001010: 006a 053c 007c 006a 036a 047c 005f 047c  .j.<.|.j.j.|._.|
-00001020: 006a 036a 097c 005f 097c 006a 0a73 3a74  .j.j.|._.|.j.s:t
-00001030: 0b83 007c 005f 0a7c 006a 0a6a 0c73 4864  ...|._.|.j.j.sHd
-00001040: 017d 0474 0d6a 0e7c 0474 0f64 0264 038d  .}.t.j.|.t.d.d..
-00001050: 0301 007c 006a 0a6a 1064 046b 0272 5864  ...|.j.j.d.k.rXd
-00001060: 057d 0474 0d6a 0e7c 0474 0f64 0264 038d  .}.t.j.|.t.d.d..
-00001070: 0301 0074 117c 017c 027c 006a 127c 006a  ...t.|.|.|.j.|.j
-00001080: 0a6a 137c 006a 0a6a 147c 006a 0a6a 1583  .j.|.j.j.|.j.j..
-00001090: 065c 047d 057d 067d 077d 087c 006a 1672  .\.}.}.}.}.|.j.r
-000010a0: b07c 006a 16a0 177c 057c 07a1 025c 027d  .|.j...|.|...\.}
-000010b0: 057d 077c 006a 166a 187c 067c 0864 0664  .}.|.j.j.|.|.d.d
-000010c0: 078d 035c 027d 067d 0874 0183 007d 037c  ...\.}.}.t...}.|
-000010d0: 03a0 027c 05a1 017d 097c 056a 1964 0864  ...|...}.|.j.d.d
-000010e0: 098d 017c 076a 1964 0864 098d 0102 027d  ...|.j.d.d.....}
-000010f0: 057d 077c 066a 1964 0864 098d 017c 086a  .}.|.j.d.d...|.j
-00001100: 1964 0864 098d 0102 027d 067d 087c 027c  .d.d.....}.}.|.|
-00001110: 036a 0476 0072 b07c 036a 04a0 1a7c 02a1  .j.v.r.|.j...|..
-00001120: 0101 0074 1b7c 0583 0174 1b7c 0683 0102  ...t.|...t.|....
-00001130: 027d 057d 0674 1c7c 057c 006a 0983 0274  .}.}.t.|.|.j...t
-00001140: 1c7c 067c 006a 0983 0202 027d 057d 0674  .|.|.j.....}.}.t
-00001150: 1d83 007c 005f 1e7c 006a 1ea0 1f7c 05a1  ...|._.|.j...|..
-00001160: 0101 007c 006a 1ea0 187c 06a1 017d 067c  ...|.j...|...}.|
-00001170: 006a 0464 0a75 0172 f47c 006a 2064 0b6b  .j.d.u.r.|.j d.k
-00001180: 0272 f474 217c 036a 0483 017c 005f 227c  .r.t!|.j...|._"|
-00001190: 006a 22a0 237c 057c 07a1 027d 057c 006a  .j".#|.|...}.|.j
-000011a0: 22a0 247c 06a1 017d 066e 1f7c 006a 0464  ".$|...}.n.|.j.d
-000011b0: 0a75 0190 0172 137c 006a 2064 0c6b 0290  .u...r.|.j d.k..
-000011c0: 0172 1374 257c 036a 0483 017c 005f 227c  .r.t%|.j...|._"|
-000011d0: 006a 22a0 267c 057c 07a1 027d 057c 006a  .j".&|.|...}.|.j
-000011e0: 22a0 277c 06a1 017d 067c 006a 2890 0172  ".'|...}.|.j(..r
-000011f0: 2b7c 006a 28a0 177c 057c 07a1 025c 027d  +|.j(..|.|...\.}
-00001200: 057d 077c 006a 286a 187c 067c 0864 0664  .}.|.j(j.|.|.d.d
-00001210: 078d 035c 027d 067d 087c 006a 2990 0173  ...\.}.}.|.j)..s
-00001220: 3374 2a83 007c 005f 297c 006a 0a6a 0c90  3t*..|._)|.j.j..
-00001230: 0172 4074 2b7c 006a 296a 2c64 0d8d 017c  .r@t+|.j)j,d...|
-00001240: 005f 2d7c 006a 2d90 0172 567c 006a 0a6a  ._-|.j-..rV|.j.j
-00001250: 0c90 0172 567c 006a 2da0 177c 057c 07a1  ...rV|.j-..|.|..
-00001260: 027d 057c 006a 2da0 187c 06a1 017d 067c  .}.|.j-..|...}.|
-00001270: 006a 2e90 0173 6774 2f7c 006a 207c 006a  .j...sgt/|.j |.j
-00001280: 0a7c 006a 307c 006a 3164 0e8d 047c 005f  .|.j0|.j1d...|._
-00001290: 2e7c 006a 2ea0 1f7c 057c 067c 077c 08a1  .|.j...|.|.|.|..
-000012a0: 0401 007c 006a 0a90 0172 827c 006a 0a6a  ...|.j...r.|.j.j
-000012b0: 3290 0172 8274 337c 006a 2e6a 347c 0664  2..r.t3|.j.j4|.d
-000012c0: 0f83 037c 005f 3564 087c 005f 3664 0a53  ...|._5d.|._6d.S
-000012d0: 0029 107a 1954 7261 696e 2061 2066 756c  .).z.Train a ful
-000012e0: 6c20 4d4c 2070 6970 656c 696e 652e 7ade  l ML pipeline.z.
-000012f0: 4665 6174 7572 6520 7365 6c65 6374 696f  Feature selectio
-00001300: 6e20 6973 2064 6973 6162 6c65 642e 2055  n is disabled. U
-00001310: 7064 6174 6520 7468 6520 5472 6169 6e69  pdate the Traini
-00001320: 6e67 436f 6e66 6967 2070 6172 616d 2027  ngConfig param '
-00001330: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
-00001340: 656c 6563 7469 6f6e 270a 2020 2020 2020  election'.      
-00001350: 2020 2020 2020 746f 2065 6e61 626c 6520        to enable 
-00001360: 6974 206f 7220 6d61 6b65 2075 7365 206f  it or make use o
-00001370: 6620 6120 6375 7374 6f6d 2070 7265 7072  f a custom prepr
-00001380: 6f63 6573 736f 7220 746f 2064 6f20 6974  ocessor to do it
-00001390: 206d 616e 7561 6c6c 7920 6475 7269 6e67   manually during
-000013a0: 2074 6865 206c 6173 7420 6d69 6c65 2063   the last mile c
-000013b0: 6f6d 7075 7461 7469 6f6e 7320 7374 6570  omputations step
-000013c0: 2e0a 2020 2020 2020 2020 2020 2020 e902  ..            ..
-000013d0: 0000 0029 01da 0a73 7461 636b 6c65 7665  ...)...stackleve
-000013e0: 6ce9 0100 0000 6105 0100 0043 726f 7373  l.....a....Cross
-000013f0: 2076 616c 6964 6174 696f 6e20 6973 2064   validation is d
-00001400: 6973 6162 6c65 642e 2055 7064 6174 6520  isabled. Update 
-00001410: 7468 6520 5472 6169 6e69 6e67 436f 6e66  the TrainingConf
-00001420: 6967 2070 6172 616d 2027 6879 7065 7274  ig param 'hypert
-00001430: 756e 696e 675f 6376 5f66 6f6c 6473 270a  uning_cv_folds'.
-00001440: 2020 2020 2020 2020 2020 2020 746f 2065              to e
-00001450: 6e61 626c 6520 6974 2e20 4372 6f73 7320  nable it. Cross 
-00001460: 7661 6c69 6461 7469 6f6e 2069 7320 6469  validation is di
-00001470: 7361 626c 6564 206f 6e20 6465 6661 796c  sabled on defayl
-00001480: 7420 746f 2061 6c6c 6f77 2066 6173 7420  t to allow fast 
-00001490: 7072 6f74 6f74 7970 696e 672e 2046 6f72  prototyping. For
-000014a0: 2072 6f62 7573 7420 6879 7065 7270 6172   robust hyperpar
-000014b0: 616d 6574 6572 0a20 2020 2020 2020 2020  ameter.         
-000014c0: 2020 2074 756e 696e 6720 7573 696e 6720     tuning using 
-000014d0: 6174 206c 6561 7374 2035 2066 6f6c 6473  at least 5 folds
-000014e0: 2069 7320 7265 636f 6d6d 656e 6465 642e   is recommended.
-000014f0: 46a9 01da 0e70 7265 6469 6374 6f6e 5f6d  F....predicton_m
-00001500: 6f64 6554 a901 da04 6472 6f70 4e72 1d00  odeT....dropNr..
-00001510: 0000 721e 0000 0029 01da 1273 656c 6563  ..r....)...selec
-00001520: 7469 6f6e 5f73 7472 6174 6567 7929 0372  tion_strategy).r
-00001530: 2600 0000 7227 0000 0072 2800 0000 da04  &...r'...r(.....
-00001540: 7472 6565 2937 720f 0000 0072 1500 0000  tree)7r....r....
-00001550: 5a1b 6669 745f 7472 616e 7366 6f72 6d5f  Z.fit_transform_
-00001560: 6665 6174 7572 655f 7479 7065 7372 2c00  feature_typesr,.
-00001570: 0000 7220 0000 0072 1f00 0000 7213 0000  ..r ...r....r...
-00001580: 0072 2e00 0000 5a1b 6669 745f 7472 616e  .r....Z.fit_tran
-00001590: 7366 6f72 6d5f 7461 7267 6574 5f6c 6162  sform_target_lab
-000015a0: 656c 7372 2100 0000 7226 0000 0072 0a00  elsr!...r&...r..
-000015b0: 0000 da18 656e 6162 6c65 5f66 6561 7475  ....enable_featu
-000015c0: 7265 5f73 656c 6563 7469 6f6e da08 7761  re_selection..wa
-000015d0: 726e 696e 6773 da04 7761 726e da0b 5573  rnings..warn..Us
-000015e0: 6572 5761 726e 696e 67da 1468 7970 6572  erWarning..hyper
-000015f0: 7475 6e69 6e67 5f63 765f 666f 6c64 7372  tuning_cv_foldsr
-00001600: 1a00 0000 7222 0000 00da 0a74 7261 696e  ....r".....train
-00001610: 5f73 697a 655a 1367 6c6f 6261 6c5f 7261  _sizeZ.global_ra
-00001620: 6e64 6f6d 5f73 7461 7465 5a14 7472 6169  ndom_stateZ.trai
-00001630: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
-00001640: 7225 0000 00da 0d66 6974 5f74 7261 6e73  r%.....fit_trans
-00001650: 666f 726d da09 7472 616e 7366 6f72 6dda  form..transform.
-00001660: 0b72 6573 6574 5f69 6e64 6578 da06 7265  .reset_index..re
-00001670: 6d6f 7665 7216 0000 0072 1200 0000 7217  mover....r....r.
-00001680: 0000 0072 2f00 0000 da03 6669 7472 1c00  ...r/.....fitr..
-00001690: 0000 7218 0000 0072 2d00 0000 5a1e 6669  ..r....r-...Z.fi
-000016a0: 745f 7461 7267 6574 5f65 6e63 6f64 655f  t_target_encode_
-000016b0: 6269 6e61 7279 5f63 6c61 7373 da24 7472  binary_class.$tr
-000016c0: 616e 7366 6f72 6d5f 7461 7267 6574 5f65  ansform_target_e
-000016d0: 6e63 6f64 655f 6269 6e61 7279 5f63 6c61  ncode_binary_cla
-000016e0: 7373 7219 0000 005a 1c66 6974 5f74 6172  ssr....Z.fit_tar
-000016f0: 6765 745f 656e 636f 6465 5f6d 756c 7469  get_encode_multi
-00001700: 636c 6173 73da 2274 7261 6e73 666f 726d  class."transform
-00001710: 5f74 6172 6765 745f 656e 636f 6465 5f6d  _target_encode_m
-00001720: 756c 7469 636c 6173 7372 2400 0000 7229  ulticlassr$...r)
-00001730: 0000 0072 0900 0000 7214 0000 0072 3f00  ...r....r....r?.
-00001740: 0000 722b 0000 0072 2300 0000 7210 0000  ..r+...r#...r...
-00001750: 0072 2700 0000 7228 0000 005a 1563 616c  .r'...r(...Z.cal
-00001760: 6375 6c61 7465 5f73 6861 705f 7661 6c75  culate_shap_valu
-00001770: 6573 720e 0000 00da 056d 6f64 656c 7230  esr......modelr0
-00001780: 0000 0072 2a00 0000 290a 7231 0000 0072  ...r*...).r1...r
-00001790: 3500 0000 7236 0000 0072 2c00 0000 da07  5...r6...r,.....
-000017a0: 6d65 7373 6167 65da 0778 5f74 7261 696e  message..x_train
-000017b0: da06 785f 7465 7374 da07 795f 7472 6169  ..x_test..y_trai
-000017c0: 6eda 0679 5f74 6573 74da 015f 7232 0000  n..y_test.._r2..
-000017d0: 0072 3200 0000 7233 0000 0072 4b00 0000  .r2...r3...rK...
-000017e0: 6100 0000 73b0 0000 0006 0206 010a 0106  a...s...........
-000017f0: 0108 020e 0108 0106 0308 0102 ff02 fe04  ................
-00001800: 0102 ff0a 060a 0106 0208 0108 0204 0110  ................
-00001810: 030c 0204 0110 0302 0202 0102 0104 0106  ................
-00001820: 0106 0106 010c fa06 0912 0106 0106 010a  ................
-00001830: ff06 030a 010e 0102 010a ff0e 0302 010a  ................
-00001840: ff0a 030c 0112 020c 0106 0108 ff08 040c  ................
-00001850: 010c 0114 020c 010e 010e 0118 010c 010e  ................
-00001860: 010c 0108 0206 0104 0108 ff06 0306 010a  ................
-00001870: ff08 0408 010a 0202 0106 0108 ff12 040e  ................
-00001880: 010c 0108 0202 0104 0104 0104 0104 0108  ................
-00001890: fc12 0612 0112 010a 017a 0c42 6c75 6543  .........z.BlueC
-000018a0: 6173 742e 6669 74da 0764 665f 6576 616c  ast.fit..df_eval
-000018b0: da0b 7461 7267 6574 5f65 7661 6c63 0500  ..target_evalc..
-000018c0: 0000 0000 0000 0000 0000 0800 0000 0400  ................
-000018d0: 0000 4300 0000 732a 0000 007c 00a0 007c  ..C...s*...|...|
-000018e0: 017c 04a1 0201 007c 00a0 017c 02a1 015c  .|.....|...|...\
-000018f0: 027d 057d 0674 027c 036a 037c 0683 027d  .}.}.t.|.j.|...}
-00001900: 077c 0753 0029 0161 8e02 0000 5472 6169  .|.S.).a....Trai
-00001910: 6e20 6120 6675 6c6c 204d 4c20 7069 7065  n a full ML pipe
-00001920: 6c69 6e65 2061 6e64 2065 7661 6c75 6174  line and evaluat
-00001930: 6520 6f6e 2061 2068 6f6c 646f 7574 2073  e on a holdout s
-00001940: 6574 2e0a 0a20 2020 2020 2020 2054 6869  et...        Thi
-00001950: 7320 6973 2061 2063 6f6e 7665 6e69 656e  s is a convenien
-00001960: 6365 2066 756e 6374 696f 6e20 746f 2074  ce function to t
-00001970: 7261 696e 2061 6e64 2065 7661 6c75 6174  rain and evaluat
-00001980: 6520 6f6e 2061 2068 6f6c 646f 7574 2073  e on a holdout s
-00001990: 6574 2e20 4974 2069 7320 7265 636f 6d6d  et. It is recomm
-000019a0: 656e 6465 6420 746f 2075 7365 2074 6869  ended to use thi
-000019b0: 7320 666f 7220 6d6f 6465 6c0a 2020 2020  s for model.    
-000019c0: 2020 2020 6578 706c 6f72 6174 696f 6e2e      exploration.
-000019d0: 204f 6e20 7072 6f64 7563 7469 6f6e 2074   On production t
-000019e0: 6865 2073 696d 706c 6520 6669 7428 2920  he simple fit() 
-000019f0: 6675 6e63 7469 6f6e 2073 686f 756c 6420  function should 
-00001a00: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
-00001a10: 203a 7061 7261 6d20 3a64 663a 2054 616b   :param :df: Tak
-00001a20: 6573 2061 2070 616e 6461 7320 4461 7461  es a pandas Data
-00001a30: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
-00001a40: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001a50: 7461 2061 6e64 2074 6865 2074 6172 6765  ta and the targe
-00001a60: 7473 2e0a 2020 2020 2020 2020 3a70 6172  ts..        :par
-00001a70: 616d 203a 6466 5f65 7661 6c3a 2054 616b  am :df_eval: Tak
-00001a80: 6573 2061 2070 616e 6461 7320 4461 7461  es a pandas Data
-00001a90: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
-00001aa0: 2074 6865 2065 7661 6c75 6174 696f 6e20   the evaluation 
-00001ab0: 6461 7461 2c20 6275 7420 6e6f 7420 7468  data, but not th
-00001ac0: 6520 7461 7267 6574 732e 0a20 2020 2020  e targets..     
-00001ad0: 2020 203a 7061 7261 6d20 3a74 6172 6765     :param :targe
-00001ae0: 745f 6576 616c 3a20 5461 6b65 7320 6120  t_eval: Takes a 
-00001af0: 7061 6e64 6173 2053 6572 6965 7320 636f  pandas Series co
-00001b00: 6e74 6169 6e69 6e67 2074 6865 2065 7661  ntaining the eva
-00001b10: 6c75 6174 696f 6e20 7461 7267 6574 732e  luation targets.
-00001b20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001b30: 3a74 6172 6765 745f 636f 6c3a 2054 616b  :target_col: Tak
-00001b40: 6573 2061 2073 7472 696e 6720 636f 6e74  es a string cont
-00001b50: 6169 6e69 6e67 2074 6865 206e 616d 6520  aining the name 
-00001b60: 6f66 2074 6865 2074 6172 6765 7420 636f  of the target co
-00001b70: 6c75 6d6e 2069 6e73 6964 6520 7468 6520  lumn inside the 
-00001b80: 7472 6169 6e69 6e67 2064 6174 6120 6466  training data df
-00001b90: 2e0a 2020 2020 2020 2020 2904 724b 0000  ..        ).rK..
-00001ba0: 00da 0770 7265 6469 6374 720d 0000 00da  ...predictr.....
-00001bb0: 0676 616c 7565 7329 0872 3100 0000 7235  .values).r1...r5
-00001bc0: 0000 0072 5500 0000 7256 0000 0072 3600  ...rU...rV...r6.
-00001bd0: 0000 da07 795f 7072 6f62 73da 0979 5f63  ....y_probs..y_c
-00001be0: 6c61 7373 6573 5a09 6576 616c 5f64 6963  lassesZ.eval_dic
-00001bf0: 7472 3200 0000 7232 0000 0072 3300 0000  tr2...r2...r3...
-00001c00: da08 6669 745f 6576 616c ce00 0000 7308  ..fit_eval....s.
-00001c10: 0000 000c 100e 010c 0104 017a 1142 6c75  ...........z.Blu
-00001c20: 6543 6173 742e 6669 745f 6576 616c 6302  eCast.fit_evalc.
-00001c30: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00001c40: 0000 0043 0000 0073 2601 0000 7400 8300  ...C...s&...t...
-00001c50: 0100 7c00 6a01 730a 7402 6401 8301 8201  ..|.j.s.t.d.....
-00001c60: 7c00 6a01 6a03 7c01 7c00 6a04 6701 6402  |.j.j.|.|.j.g.d.
-00001c70: 8d02 7d01 7c00 6a05 7227 7c00 6a05 6a06  ..}.|.j.r'|.j.j.
-00001c80: 7c01 6403 6404 8d02 5c02 7d01 7d02 7c01  |.d.d...\.}.}.|.
-00001c90: 6a07 6403 6405 8d01 7d01 7408 7c01 8301  j.d.d...}.t.|...
-00001ca0: 7d01 7409 7c01 7c00 6a0a 8302 7d01 7c00  }.t.|.|.j...}.|.
-00001cb0: 6a0b 723a 7c00 6a0b a006 7c01 a101 7d01  j.r:|.j...|...}.
-00001cc0: 7c00 6a0c 7252 7c00 6a0d 7252 7c00 6a0e  |.j.rR|.j.rR|.j.
-00001cd0: 6406 6b02 7252 740f 7c00 6a0d 7410 8302  d.k.rRt.|.j.t...
-00001ce0: 7252 7c00 6a0d a011 7c01 a101 7d01 6e17  rR|.j...|...}.n.
-00001cf0: 7c00 6a0c 7269 7c00 6a0d 7269 7c00 6a0e  |.j.ri|.j.ri|.j.
-00001d00: 6407 6b02 7269 740f 7c00 6a0d 7412 8302  d.k.rit.|.j.t...
-00001d10: 7269 7c00 6a0d a013 7c01 a101 7d01 7c00  ri|.j...|...}.|.
-00001d20: 6a14 7276 7c00 6a14 6a06 7c01 6403 6404  j.rv|.j.j.|.d.d.
-00001d30: 8d02 5c02 7d01 7d02 7c00 6a15 737d 7416  ..\.}.}.|.j.s}t.
-00001d40: 8300 7c00 5f15 7c00 6a17 7384 7418 8300  ..|._.|.j.s.t...
-00001d50: 7c00 5f17 7c00 6a19 7291 7c00 6a17 6a1a  |._.|.j.r.|.j.j.
-00001d60: 7291 7c00 6a19 a006 7c01 a101 7d01 7c01  r.|.j...|...}.|.
-00001d70: 5300 2908 7a37 5472 616e 7366 6f72 6d20  S.).z7Transform 
-00001d80: 6e65 7720 6461 7461 2061 6363 6f72 6469  new data accordi
-00001d90: 6e67 2074 6f20 7072 6570 726f 6365 7373  ng to preprocess
-00001da0: 696e 6720 7069 7065 6c69 6e65 2efa 2a46  ing pipeline..*F
-00001db0: 6561 7475 7265 2074 7970 6520 636f 6e76  eature type conv
-00001dc0: 6572 7465 7220 636f 756c 6420 6e6f 7420  erter could not 
-00001dd0: 6265 2066 6f75 6e64 2e29 015a 0b69 676e  be found.).Z.ign
-00001de0: 6f72 655f 636f 6c73 5472 3b00 0000 723d  ore_colsTr;...r=
-00001df0: 0000 0072 1d00 0000 721e 0000 0029 1b72  ...r....r....).r
-00001e00: 0f00 0000 722c 0000 00da 0945 7863 6570  ....r,.....Excep
-00001e10: 7469 6f6e 5a17 7472 616e 7366 6f72 6d5f  tionZ.transform_
-00001e20: 6665 6174 7572 655f 7479 7065 7372 1f00  feature_typesr..
-00001e30: 0000 7225 0000 0072 4800 0000 7249 0000  ..r%...rH...rI..
-00001e40: 0072 1600 0000 7212 0000 0072 2100 0000  .r....r....r!...
-00001e50: 722f 0000 0072 2000 0000 722d 0000 0072  r/...r ...r-...r
-00001e60: 1c00 0000 da0a 6973 696e 7374 616e 6365  ......isinstance
-00001e70: 7218 0000 0072 4c00 0000 7219 0000 0072  r....rL...r....r
-00001e80: 4d00 0000 7224 0000 0072 2900 0000 7209  M...r$...r)...r.
-00001e90: 0000 0072 2600 0000 720a 0000 0072 2b00  ...r&...r....r+.
-00001ea0: 0000 7241 0000 0029 0372 3100 0000 7235  ..rA...).r1...r5
-00001eb0: 0000 0072 5400 0000 7232 0000 0072 3200  ...rT...r2...r2.
-00001ec0: 0000 7233 0000 00da 1274 7261 6e73 666f  ..r3.....transfo
-00001ed0: 726d 5f6e 6577 5f64 6174 61e3 0000 0073  rm_new_data....s
-00001ee0: 4c00 0000 0602 0601 0801 0602 0801 06ff  L...............
-00001ef0: 0604 1401 0c01 0802 0c01 0602 0c01 0403  ................
-00001f00: 02ff 0402 02fe 0a03 0a01 02ff 0e03 0402  ................
-00001f10: 02ff 0402 02fe 0a03 0a01 02ff 0c03 0602  ................
-00001f20: 1401 0602 0801 0602 0801 0e02 0c01 0402  ................
-00001f30: 7a1b 426c 7565 4361 7374 2e74 7261 6e73  z.BlueCast.trans
-00001f40: 666f 726d 5f6e 6577 5f64 6174 6163 0200  form_new_datac..
-00001f50: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00001f60: 0000 4300 0000 7380 0000 007c 006a 0073  ..C...s....|.j.s
-00001f70: 0774 0164 0183 0182 017c 006a 0273 0e74  .t.d.....|.j.s.t
-00001f80: 0164 0283 0182 0174 0383 0001 007c 00a0  .d.....t.....|..
-00001f90: 047c 01a1 017d 0174 0564 0383 0101 007c  .|...}.t.d.....|
-00001fa0: 006a 00a0 067c 01a1 015c 027d 027d 037c  .j...|...\.}.}.|
-00001fb0: 006a 026a 0772 3c7c 006a 087c 006a 026a  .j.j.r<|.j.|.j.j
-00001fc0: 0776 0072 3c7c 006a 0972 3c7c 006a 0272  .v.r<|.j.r<|.j.r
-00001fd0: 3c7c 006a 09a0 0a74 0ba0 0c7c 03a1 01a1  <|.j...t...|....
-00001fe0: 017d 037c 027c 0366 0253 0029 047a 9050  .}.|.|.f.S.).z.P
-00001ff0: 7265 6469 6374 206f 6e20 756e 7365 656e  redict on unseen
-00002000: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
-00002010: 5265 7475 726e 2074 6865 2070 7265 6469  Return the predi
-00002020: 6374 6564 2070 726f 6261 6269 6c69 7469  cted probabiliti
-00002030: 6573 2061 6e64 2074 6865 2070 7265 6469  es and the predi
-00002040: 6374 6564 2063 6c61 7373 6573 3a0a 2020  cted classes:.  
-00002050: 2020 2020 2020 795f 7072 6f62 732c 2079        y_probs, y
-00002060: 5f63 6c61 7373 6573 203d 2070 7265 6469  _classes = predi
-00002070: 6374 2864 6629 0a20 2020 2020 2020 207a  ct(df).        z
-00002080: 1b4d 6c20 6d6f 6465 6c20 636f 756c 6420  .Ml model could 
-00002090: 6e6f 7420 6265 2066 6f75 6e64 725c 0000  not be foundr\..
-000020a0: 007a 0d50 7265 6469 6374 696e 672e 2e2e  .z.Predicting...
-000020b0: 290d 7223 0000 0072 5d00 0000 722c 0000  ).r#...r]...r,..
-000020c0: 0072 0f00 0000 725f 0000 00da 0570 7269  .r....r_.....pri
-000020d0: 6e74 7257 0000 0072 2000 0000 721f 0000  ntrW...r ...r...
-000020e0: 0072 2e00 0000 5a1f 6c61 6265 6c5f 656e  .r....Z.label_en
-000020f0: 636f 6465 725f 7265 7665 7273 655f 7472  coder_reverse_tr
-00002100: 616e 7366 6f72 6dda 0270 64da 0653 6572  ansform..pd..Ser
-00002110: 6965 7329 0472 3100 0000 7235 0000 0072  ies).r1...r5...r
-00002120: 5900 0000 725a 0000 0072 3200 0000 7232  Y...rZ...r2...r2
-00002130: 0000 0072 3300 0000 7257 0000 0014 0100  ...r3...rW......
-00002140: 0073 2400 0000 0606 0801 0602 0801 0602  .s$.............
-00002150: 0a01 0802 1001 0802 0e02 0401 02ff 0402  ................
-00002160: 02fe 0604 0801 04ff 0804 7a10 426c 7565  ..........z.Blue
-00002170: 4361 7374 2e70 7265 6469 6374 290a 4e4e  Cast.predict).NN
-00002180: 4e4e 4e4e 4e4e 4e4e 291e da08 5f5f 6e61  NNNNNNNN)...__na
-00002190: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000021a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000021b0: 5f5f 646f 635f 5f72 0500 0000 7208 0000  __doc__r....r...
-000021c0: 00da 0373 7472 da05 666c 6f61 74da 0369  ...str..float..i
-000021d0: 6e74 7206 0000 0072 0400 0000 7210 0000  ntr....r....r...
-000021e0: 0072 0200 0000 7211 0000 0072 0a00 0000  .r....r....r....
-000021f0: 720c 0000 0072 0b00 0000 7209 0000 0072  r....r....r....r
-00002200: 3400 0000 7261 0000 00da 0944 6174 6146  4...ra.....DataF
-00002210: 7261 6d65 724b 0000 0072 6200 0000 7203  ramerK...rb...r.
-00002220: 0000 0072 5b00 0000 725f 0000 0072 0700  ...r[...r_...r..
-00002230: 0000 da02 6e70 da07 6e64 6172 7261 7972  ....np..ndarrayr
-00002240: 5700 0000 7232 0000 0072 3200 0000 7232  W...r2...r2...r2
-00002250: 0000 0072 3300 0000 721b 0000 0027 0000  ...r3...r....'..
-00002260: 0073 6600 0000 0800 0401 0218 0201 0201  .sf.............
-00002270: 0201 0201 0201 0201 0201 0201 0201 04f3  ................
-00002280: 0602 02fe 0c03 02fd 1404 02fc 1405 02fb  ................
-00002290: 0606 02fa 0e07 02f9 0608 02f8 0609 02f7  ................
-000022a0: 060a 02f6 060b 02f5 060c 02f4 060d 0af3  ................
-000022b0: 1825 026d 0402 02fe 0403 02fd 0404 02fc  .%.m............
-000022c0: 0205 02fb 0a06 0afa 1615 2431 721b 0000  ..........$1r...
-000022d0: 0029 2f72 6600 0000 7242 0000 00da 0674  .)/rf...rB.....t
-000022e0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-000022f0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00002300: 0000 0072 0800 0000 da05 6e75 6d70 7972  ...r......numpyr
-00002310: 6b00 0000 da06 7061 6e64 6173 7261 0000  k.....pandasra..
-00002320: 00da 1f62 6c75 6563 6173 742e 636f 6e66  ...bluecast.conf
-00002330: 6967 2e74 7261 696e 696e 675f 636f 6e66  ig.training_conf
-00002340: 6967 7209 0000 0072 0a00 0000 720b 0000  igr....r....r...
-00002350: 0072 0c00 0000 5a20 626c 7565 6361 7374  .r....Z bluecast
-00002360: 2e65 7661 6c75 6174 696f 6e2e 6576 616c  .evaluation.eval
-00002370: 5f6d 6574 7269 6373 720d 0000 005a 1f62  _metricsr....Z.b
-00002380: 6c75 6563 6173 742e 6576 616c 7561 7469  luecast.evaluati
-00002390: 6f6e 2e73 6861 705f 7661 6c75 6573 720e  on.shap_valuesr.
-000023a0: 0000 005a 2462 6c75 6563 6173 742e 6765  ...Z$bluecast.ge
-000023b0: 6e65 7261 6c5f 7574 696c 732e 6765 6e65  neral_utils.gene
-000023c0: 7261 6c5f 7574 696c 7372 0f00 0000 5a1d  ral_utilsr....Z.
-000023d0: 626c 7565 6361 7374 2e6d 6c5f 6d6f 6465  bluecast.ml_mode
-000023e0: 6c6c 696e 672e 7867 626f 6f73 7472 1000  lling.xgboostr..
-000023f0: 0000 da1d 626c 7565 6361 7374 2e70 7265  ....bluecast.pre
-00002400: 7072 6f63 6573 7369 6e67 2e63 7573 746f  processing.custo
-00002410: 6d72 1100 0000 5a28 626c 7565 6361 7374  mr....Z(bluecast
-00002420: 2e70 7265 7072 6f63 6573 7369 6e67 2e64  .preprocessing.d
-00002430: 6174 6574 696d 655f 6665 6174 7572 6573  atetime_features
-00002440: 7212 0000 005a 2b62 6c75 6563 6173 742e  r....Z+bluecast.
-00002450: 7072 6570 726f 6365 7373 696e 672e 656e  preprocessing.en
-00002460: 636f 6465 5f74 6172 6765 745f 6c61 6265  code_target_labe
-00002470: 6c73 7213 0000 005a 2862 6c75 6563 6173  lsr....Z(bluecas
-00002480: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
-00002490: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
-000024a0: 6e72 1400 0000 5a24 626c 7565 6361 7374  nr....Z$bluecast
-000024b0: 2e70 7265 7072 6f63 6573 7369 6e67 2e66  .preprocessing.f
-000024c0: 6561 7475 7265 5f74 7970 6573 7215 0000  eature_typesr...
-000024d0: 005a 2562 6c75 6563 6173 742e 7072 6570  .Z%bluecast.prep
-000024e0: 726f 6365 7373 696e 672e 6e75 6c6c 735f  rocessing.nulls_
-000024f0: 616e 645f 696e 6673 7216 0000 005a 2462  and_infsr....Z$b
-00002500: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00002510: 7373 696e 672e 7363 6865 6d61 5f63 6865  ssing.schema_che
-00002520: 636b 7372 1700 0000 5a26 626c 7565 6361  cksr....Z&blueca
-00002530: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00002540: 2e74 6172 6765 745f 656e 636f 6469 6e67  .target_encoding
-00002550: 7218 0000 0072 1900 0000 5a27 626c 7565  r....r....Z'blue
-00002560: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
-00002570: 6e67 2e74 7261 696e 5f74 6573 745f 7370  ng.train_test_sp
-00002580: 6c69 7472 1a00 0000 721b 0000 0072 3200  litr....r....r2.
-00002590: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
-000025a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000025b0: 2800 0000 0400 0808 2401 0802 0801 1802  (.......$.......
-000025c0: 0c06 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000025d0: 0c01 0c01 0c01 1001 0c04 1203            ............
+000003f0: 6174 696f 6e73 2902 da11 6368 6563 6b5f  ations)...check_
+00000400: 6770 755f 7375 7070 6f72 74da 066c 6f67  gpu_support..log
+00000410: 6765 7229 01da 0c58 6762 6f6f 7374 4d6f  ger)...XgboostMo
+00000420: 6465 6c29 01da 1343 7573 746f 6d50 7265  del)...CustomPre
+00000430: 7072 6f63 6573 7369 6e67 2901 da0e 6461  processing)...da
+00000440: 7465 5f63 6f6e 7665 7274 6572 2901 da12  te_converter)...
+00000450: 5461 7267 6574 4c61 6265 6c45 6e63 6f64  TargetLabelEncod
+00000460: 6572 2901 da0d 5246 4543 5653 656c 6563  er)...RFECVSelec
+00000470: 746f 7229 01da 1346 6561 7475 7265 5479  tor)...FeatureTy
+00000480: 7065 4465 7465 6374 6f72 2901 da14 6669  peDetector)...fi
+00000490: 6c6c 5f69 6e66 696e 6974 655f 7661 6c75  ll_infinite_valu
+000004a0: 6573 2901 da0e 5363 6865 6d61 4465 7465  es)...SchemaDete
+000004b0: 6374 6f72 2902 da18 4269 6e61 7279 436c  ctor)...BinaryCl
+000004c0: 6173 7354 6172 6765 7445 6e63 6f64 6572  assTargetEncoder
+000004d0: da17 4d75 6c74 6943 6c61 7373 5461 7267  ..MultiClassTarg
+000004e0: 6574 456e 636f 6465 7229 01da 1074 7261  etEncoder)...tra
+000004f0: 696e 5f74 6573 745f 7370 6c69 7463 0000  in_test_splitc..
+00000500: 0000 0000 0000 0000 0000 0000 0000 1a00  ................
+00000510: 0000 4000 0000 7350 0100 0065 005a 0164  ..@...sP...e.Z.d
+00000520: 005a 0264 015a 0309 0209 0209 0209 0209  .Z.d.Z..........
+00000530: 0209 0209 0209 0209 0209 0264 2164 0365  ...........d!d.e
+00000540: 0464 0419 0064 0565 0565 0665 0765 0866  .d...d.e.e.e.e.f
+00000550: 0319 0064 0665 0965 0a65 0565 0665 0765  ...d.e.e.e.e.e.e
+00000560: 0866 0319 0019 0019 0064 0765 0965 0a65  .f.......d.e.e.e
+00000570: 0565 0665 0765 0866 0319 0019 0019 0064  .e.e.e.f.......d
+00000580: 0865 0965 0619 0064 0965 0965 0565 0b65  .e.e...d.e.e.e.e
+00000590: 0c66 0219 0019 0064 0a65 0965 0d19 0064  .f.....d.e.e...d
+000005a0: 0b65 0965 0d19 0064 0c65 0965 0565 0e65  .e.e...d.e.e.e.e
+000005b0: 0d66 0219 0019 0064 0d65 0965 0f19 0064  .f.....d.e.e...d
+000005c0: 0e65 0965 1019 0064 0f65 0965 1119 0066  .e.e...d.e.e...f
+000005d0: 1864 1064 1184 055a 1264 1265 136a 1464  .d.d...Z.d.e.j.d
+000005e0: 1364 0266 0464 1464 1584 045a 1564 1265  .d.f.d.d...Z.d.e
+000005f0: 136a 1464 1665 0664 1364 0266 0664 1764  .j.d.e.d.d.f.d.d
+00000600: 1884 045a 1664 1265 136a 1464 1965 136a  ...Z.d.e.j.d.e.j
+00000610: 1464 1a65 136a 1764 1665 0664 1365 1865  .d.e.j.d.e.d.e.e
+00000620: 0665 0c66 0219 0066 0a64 1b64 1c84 045a  .e.f...f.d.d...Z
+00000630: 1964 1265 136a 1464 1365 136a 1466 0464  .d.e.j.d.e.j.f.d
+00000640: 1d64 1e84 045a 1a64 1265 136a 1464 1365  .d...Z.d.e.j.d.e
+00000650: 1b65 1c6a 1d65 1c6a 1d66 0219 0066 0464  .e.j.e.j.f...f.d
+00000660: 1f64 2084 045a 1e64 0253 0029 22da 0842  .d ..Z.d.S.)"..B
+00000670: 6c75 6543 6173 7461 2206 0000 5275 6e20  lueCasta"...Run 
+00000680: 6675 6c6c 7920 636f 6e66 6967 7572 6564  fully configured
+00000690: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+000006a0: 626c 7565 7072 696e 742e 0a0a 2020 2020  blueprint...    
+000006b0: 4375 7374 6f6d 697a 6174 696f 6e20 7669  Customization vi
+000006c0: 6120 636c 6173 7320 6174 7472 6962 7574  a class attribut
+000006d0: 6573 2069 7320 706f 7373 6962 6c65 2e20  es is possible. 
+000006e0: 436f 6e66 6967 7320 6361 6e20 6265 2069  Configs can be i
+000006f0: 6e73 7461 6e74 6961 7465 6420 616e 6420  nstantiated and 
+00000700: 7072 6f76 6964 6564 2074 6f20 6368 616e  provided to chan
+00000710: 6765 2058 6762 6f6f 7374 2074 7261 696e  ge Xgboost train
+00000720: 696e 672e 0a20 2020 2044 6566 6175 6c74  ing..    Default
+00000730: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
+00000740: 7365 6172 6368 2073 7061 6365 2069 7320  search space is 
+00000750: 7265 6c61 7469 7665 6c79 206c 6967 6874  relatively light
+00000760: 2d77 6569 6768 7420 746f 2073 7065 6564  -weight to speed
+00000770: 2075 7020 7468 6520 7072 6f74 6f74 7970   up the prototyp
+00000780: 696e 672e 0a20 2020 203a 7061 7261 6d20  ing..    :param 
+00000790: 3a63 6c61 7373 5f70 726f 626c 656d 3a20  :class_problem: 
+000007a0: 5461 6b65 7320 6120 7374 7269 6e67 2063  Takes a string c
+000007b0: 6f6e 7461 696e 696e 6720 7468 6520 636c  ontaining the cl
+000007c0: 6173 7320 7072 6f62 6c65 6d20 7479 7065  ass problem type
+000007d0: 2e20 4569 7468 6572 2022 6269 6e61 7279  . Either "binary
+000007e0: 2220 6f72 2022 6d75 6c74 6963 6c61 7373  " or "multiclass
+000007f0: 222e 0a20 2020 203a 7061 7261 6d20 3a74  "..    :param :t
+00000800: 6172 6765 745f 636f 6c75 6d6e 3a20 5461  arget_column: Ta
+00000810: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
+00000820: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
+00000830: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
+00000840: 6f6c 756d 6e2e 0a20 2020 203a 7061 7261  olumn..    :para
+00000850: 6d20 3a63 6174 5f63 6f6c 756d 6e73 3a20  m :cat_columns: 
+00000860: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
+00000870: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
+00000880: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
+00000890: 7468 6520 6361 7465 676f 7269 6361 6c20  the categorical 
+000008a0: 636f 6c75 6d6e 732e 2049 6620 6e6f 7420  columns. If not 
+000008b0: 7072 6f76 6964 6564 2c0a 2020 2020 426c  provided,.    Bl
+000008c0: 7565 4361 7374 2077 696c 6c20 696e 6665  ueCast will infe
+000008d0: 7220 7468 6573 6520 6175 746f 6d61 6963  r these automaic
+000008e0: 616c 6c79 2e0a 2020 2020 3a70 6172 616d  ally..    :param
+000008f0: 203a 6461 7465 5f63 6f6c 756d 6e73 3a20   :date_columns: 
+00000900: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
+00000910: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
+00000920: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
+00000930: 7468 6520 6461 7465 2063 6f6c 756d 6e73  the date columns
+00000940: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
+00000950: 642c 0a20 2020 2042 6c75 6543 6173 7420  d,.    BlueCast 
+00000960: 7769 6c6c 2069 6e66 6572 2074 6865 7365  will infer these
+00000970: 2061 7574 6f6d 6169 6361 6c6c 792e 0a20   automaically.. 
+00000980: 2020 203a 7061 7261 6d20 3a74 696d 655f     :param :time_
+00000990: 7370 6c69 745f 636f 6c75 6d6e 3a20 5461  split_column: Ta
+000009a0: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
+000009b0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
+000009c0: 206f 6620 7468 6520 7469 6d65 2073 706c   of the time spl
+000009d0: 6974 2063 6f6c 756d 6e2e 2049 6620 6e6f  it column. If no
+000009e0: 7420 7072 6f76 6964 6564 2c0a 2020 2020  t provided,.    
+000009f0: 426c 7565 4361 7374 2077 696c 6c20 6e6f  BlueCast will no
+00000a00: 7420 7370 6c69 7420 7468 6520 6461 7461  t split the data
+00000a10: 2062 7920 7469 6d65 206f 7220 6f72 6465   by time or orde
+00000a20: 722c 2062 7574 2064 6f20 6120 7261 6e64  r, but do a rand
+00000a30: 6f6d 2073 706c 6974 2069 6e73 7465 6164  om split instead
+00000a40: 2e0a 2020 2020 3a70 6172 616d 203a 6d6c  ..    :param :ml
+00000a50: 5f6d 6f64 656c 3a20 5461 6b65 7320 616e  _model: Takes an
+00000a60: 2069 6e73 7461 6e63 6520 6f66 2061 2058   instance of a X
+00000a70: 6762 6f6f 7374 4d6f 6465 6c20 636c 6173  gboostModel clas
+00000a80: 732e 2049 6620 6e6f 7420 7072 6f76 6964  s. If not provid
+00000a90: 6564 2c20 426c 7565 4361 7374 2077 696c  ed, BlueCast wil
+00000aa0: 6c20 696e 7374 616e 7469 6174 6520 6f6e  l instantiate on
+00000ab0: 652e 0a20 2020 2054 6869 7320 6973 2061  e..    This is a
+00000ac0: 6e20 4150 4920 746f 2070 6173 7320 616e  n API to pass an
+00000ad0: 7920 6d6f 6465 6c20 636c 6173 732e 2049  y model class. I
+00000ae0: 6e68 6572 6974 2074 6865 2062 6173 6563  nherit the basec
+00000af0: 6c61 7373 2066 726f 6d20 6d6c 5f6d 6f64  lass from ml_mod
+00000b00: 656c 6c69 6e67 2e62 6173 655f 6d6f 6465  elling.base_mode
+00000b10: 6c2e 4261 7365 4d6f 6465 6c2e 0a20 2020  l.BaseModel..   
+00000b20: 203a 7061 7261 6d20 6375 7374 6f6d 5f70   :param custom_p
+00000b30: 7265 7072 6f63 6573 736f 723a 2054 616b  reprocessor: Tak
+00000b40: 6573 2061 6e20 696e 7374 616e 6365 206f  es an instance o
+00000b50: 6620 6120 4375 7374 6f6d 5072 6570 726f  f a CustomPrepro
+00000b60: 6365 7373 696e 6720 636c 6173 732e 2041  cessing class. A
+00000b70: 6c6c 6f77 7320 7573 6572 7320 746f 2069  llows users to i
+00000b80: 6e6a 6563 7420 6375 7374 6f6d 0a20 2020  nject custom.   
+00000b90: 2070 7265 7072 6f63 6573 7369 6e67 2073   preprocessing s
+00000ba0: 7465 7073 2077 6869 6368 2074 616b 6520  teps which take 
+00000bb0: 706c 6163 6520 7269 6768 7420 6166 7465  place right afte
+00000bc0: 7220 7468 6520 7472 6169 6e20 7465 7374  r the train test
+00000bd0: 2073 7069 742e 0a20 2020 203a 7061 7261   spit..    :para
+00000be0: 6d20 6375 7374 6f6d 5f6c 6173 745f 6d69  m custom_last_mi
+00000bf0: 6c65 5f63 6f6d 7075 7461 7469 6f6e 3a20  le_computation: 
+00000c00: 5461 6b65 7320 616e 2069 6e73 7461 6e63  Takes an instanc
+00000c10: 6520 6f66 2061 2043 7573 746f 6d50 7265  e of a CustomPre
+00000c20: 7072 6f63 6573 7369 6e67 2063 6c61 7373  processing class
+00000c30: 2e20 416c 6c6f 7773 2075 7365 7273 2074  . Allows users t
+00000c40: 6f20 696e 6a65 6374 2063 7573 746f 6d0a  o inject custom.
+00000c50: 2020 2020 7072 6570 726f 6365 7373 696e      preprocessin
+00000c60: 6720 7374 6570 7320 7768 6963 6820 7461  g steps which ta
+00000c70: 6b65 2070 6c61 6365 2072 6967 6874 2062  ke place right b
+00000c80: 6566 6f72 6520 7468 6520 6d6f 6465 6c20  efore the model 
+00000c90: 7472 6169 6e69 6e67 2e0a 2020 2020 4eda  training..    N.
+00000ca0: 0d63 6c61 7373 5f70 726f 626c 656d 2902  .class_problem).
+00000cb0: da06 6269 6e61 7279 da0a 6d75 6c74 6963  ..binary..multic
+00000cc0: 6c61 7373 da0d 7461 7267 6574 5f63 6f6c  lass..target_col
+00000cd0: 756d 6eda 0b63 6174 5f63 6f6c 756d 6e73  umn..cat_columns
+00000ce0: da0c 6461 7465 5f63 6f6c 756d 6e73 da11  ..date_columns..
+00000cf0: 7469 6d65 5f73 706c 6974 5f63 6f6c 756d  time_split_colum
+00000d00: 6eda 086d 6c5f 6d6f 6465 6cda 1c63 7573  n..ml_model..cus
+00000d10: 746f 6d5f 6c61 7374 5f6d 696c 655f 636f  tom_last_mile_co
+00000d20: 6d70 7574 6174 696f 6eda 1363 7573 746f  mputation..custo
+00000d30: 6d5f 7072 6570 726f 6365 7373 6f72 da17  m_preprocessor..
+00000d40: 6375 7374 6f6d 5f66 6561 7475 7265 5f73  custom_feature_s
+00000d50: 656c 6563 746f 72da 0d63 6f6e 665f 7472  elector..conf_tr
+00000d60: 6169 6e69 6e67 da0c 636f 6e66 5f78 6762  aining..conf_xgb
+00000d70: 6f6f 7374 da13 636f 6e66 5f70 6172 616d  oost..conf_param
+00000d80: 735f 7867 626f 6f73 7463 0d00 0000 0000  s_xgboostc......
+00000d90: 0000 0000 0000 0d00 0000 0200 0000 4300  ..............C.
+00000da0: 0000 7370 0000 007c 017c 005f 0064 017c  ..sp...|.|._.d.|
+00000db0: 005f 017c 037c 005f 027c 047c 005f 037c  ._.|.|._.|.|._.|
+00000dc0: 057c 005f 047c 027c 005f 057c 0a7c 005f  .|._.|.|._.|.|._
+00000dd0: 067c 0b7c 005f 077c 0c7c 005f 0864 007c  .|.|._.|.|._.d.|
+00000de0: 005f 0964 007c 005f 0a64 007c 005f 0b64  ._.d.|._.d.|._.d
+00000df0: 007c 005f 0c7c 067c 005f 0d7c 077c 005f  .|._.|.|._.|.|._
+00000e00: 0e7c 087c 005f 0f7c 097c 005f 1064 007c  .|.|._.|.|._.d.|
+00000e10: 005f 1164 0053 0029 024e 4629 1272 1d00  ._.d.S.).NF).r..
+00000e20: 0000 da0f 7072 6564 6963 7469 6f6e 5f6d  ....prediction_m
+00000e30: 6f64 6572 2100 0000 7222 0000 0072 2300  oder!...r"...r#.
+00000e40: 0000 7220 0000 0072 2800 0000 7229 0000  ..r ...r(...r)..
+00000e50: 0072 2a00 0000 da12 6665 6174 5f74 7970  .r*.....feat_typ
+00000e60: 655f 6465 7465 6374 6f72 da0b 6361 745f  e_detector..cat_
+00000e70: 656e 636f 6465 72da 1474 6172 6765 745f  encoder..target_
+00000e80: 6c61 6265 6c5f 656e 636f 6465 72da 0f73  label_encoder..s
+00000e90: 6368 656d 615f 6465 7465 6374 6f72 7224  chema_detectorr$
+00000ea0: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
+00000eb0: 0000 da0b 7368 6170 5f76 616c 7565 7329  ....shap_values)
+00000ec0: 0dda 0473 656c 6672 1d00 0000 7220 0000  ...selfr....r ..
+00000ed0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+00000ee0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00000ef0: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
+00000f00: 0000 00a9 0072 3200 0000 fa3e 2f68 6f6d  .....r2....>/hom
+00000f10: 652f 7468 6f6d 6173 2f49 6465 6150 726f  e/thomas/IdeaPro
+00000f20: 6a65 6374 732f 426c 7565 4361 7374 2f62  jects/BlueCast/b
+00000f30: 6c75 6563 6173 742f 626c 7565 7072 696e  luecast/blueprin
+00000f40: 7473 2f63 6173 742e 7079 da08 5f5f 696e  ts/cast.py..__in
+00000f50: 6974 5f5f 3c00 0000 7326 0000 0006 1106  it__<...s&......
+00000f60: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000f70: 0102 0304 fe06 0306 0106 0106 0106 0106  ................
+00000f80: 010a 017a 1142 6c75 6543 6173 742e 5f5f  ...z.BlueCast.__
+00000f90: 696e 6974 5f5f da02 6466 da06 7265 7475  init__..df..retu
+00000fa0: 726e 6302 0000 0000 0000 0000 0000 0003  rnc.............
+00000fb0: 0000 0005 0000 0043 0000 0073 dc00 0000  .......C...s....
+00000fc0: 7c00 6a00 7307 7401 8300 7c00 5f00 7c00  |.j.s.t...|._.|.
+00000fd0: 6a00 6a02 7315 6401 7d02 7403 6a04 7c02  j.j.s.d.}.t.j.|.
+00000fe0: 7405 6402 6403 8d03 0100 7c00 6a00 6a06  t.d.d.....|.j.j.
+00000ff0: 6404 6b02 7225 6405 7d02 7403 6a04 7c02  d.k.r%d.}.t.j.|.
+00001000: 7405 6402 6403 8d03 0100 7c00 6a00 6a02  t.d.d.....|.j.j.
+00001010: 7236 7c00 6a07 7336 6406 7d02 7403 6a04  r6|.j.s6d.}.t.j.
+00001020: 7c02 7405 6402 6403 8d03 0100 7c00 6a08  |.t.d.d.....|.j.
+00001030: 7343 6407 7d02 7403 6a04 7c02 7405 6402  sCd.}.t.j.|.t.d.
+00001040: 6403 8d03 0100 7c00 6a00 6a09 740a 7c01  d.....|.j.j.t.|.
+00001050: 6a0b 8301 6b05 725a 7c00 6a00 6a02 725a  j...k.rZ|.j.j.rZ
+00001060: 6408 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+00001070: 8d03 0100 7c00 6a0c 7c01 6a0b 7600 726c  ....|.j.|.j.v.rl
+00001080: 6409 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+00001090: 8d03 0100 6400 5300 6400 5300 290a 4e61  ....d.S.d.S.).Na
+000010a0: 9301 0000 4665 6174 7572 6520 7365 6c65  ....Feature sele
+000010b0: 6374 696f 6e20 6973 2064 6973 6162 6c65  ction is disable
+000010c0: 642e 2055 7064 6174 6520 7468 6520 5472  d. Update the Tr
+000010d0: 6169 6e69 6e67 436f 6e66 6967 2070 6172  ainingConfig par
+000010e0: 616d 2027 656e 6162 6c65 5f66 6561 7475  am 'enable_featu
+000010f0: 7265 5f73 656c 6563 7469 6f6e 270a 2020  re_selection'.  
+00001100: 2020 2020 2020 2020 2020 746f 2065 6e61            to ena
+00001110: 626c 6520 6974 206f 7220 6d61 6b65 2075  ble it or make u
+00001120: 7365 206f 6620 6120 6375 7374 6f6d 2070  se of a custom p
+00001130: 7265 7072 6f63 6573 736f 7220 746f 2064  reprocessor to d
+00001140: 6f20 6974 206d 616e 7561 6c6c 7920 6475  o it manually du
+00001150: 7269 6e67 2074 6865 206c 6173 7420 6d69  ring the last mi
+00001160: 6c65 2063 6f6d 7075 7461 7469 6f6e 7320  le computations 
+00001170: 7374 6570 2e0a 2020 2020 2020 2020 2020  step..          
+00001180: 2020 4665 6174 7572 6520 7365 6c65 6374    Feature select
+00001190: 696f 6e20 6973 2072 6563 6f6d 6d65 6e64  ion is recommend
+000011a0: 6564 2066 6f72 2064 6174 6173 6574 7320  ed for datasets 
+000011b0: 7769 7468 206d 616e 7920 6665 6174 7572  with many featur
+000011c0: 6573 2028 3e31 3030 3029 2e20 466f 7220  es (>1000). For 
+000011d0: 6461 7461 7365 7473 2077 6974 6820 6120  datasets with a 
+000011e0: 736d 616c 6c20 616d 6f75 6e74 0a20 2020  small amount.   
+000011f0: 2020 2020 2020 2020 206f 6620 6665 6174           of feat
+00001200: 7572 6573 2066 6561 7475 7265 2073 656c  ures feature sel
+00001210: 6563 7469 6f6e 2069 7320 6e6f 7420 7265  ection is not re
+00001220: 636f 6d6d 656e 6465 642e 0a20 2020 2020  commended..     
+00001230: 2020 2020 2020 20e9 0200 0000 2901 da0a         .....)...
+00001240: 7374 6163 6b6c 6576 656c e901 0000 0061  stacklevel.....a
+00001250: 0501 0000 4372 6f73 7320 7661 6c69 6461  ....Cross valida
+00001260: 7469 6f6e 2069 7320 6469 7361 626c 6564  tion is disabled
+00001270: 2e20 5570 6461 7465 2074 6865 2054 7261  . Update the Tra
+00001280: 696e 696e 6743 6f6e 6669 6720 7061 7261  iningConfig para
+00001290: 6d20 2768 7970 6572 7475 6e69 6e67 5f63  m 'hypertuning_c
+000012a0: 765f 666f 6c64 7327 0a20 2020 2020 2020  v_folds'.       
+000012b0: 2020 2020 2074 6f20 656e 6162 6c65 2069       to enable i
+000012c0: 742e 2043 726f 7373 2076 616c 6964 6174  t. Cross validat
+000012d0: 696f 6e20 6973 2064 6973 6162 6c65 6420  ion is disabled 
+000012e0: 6f6e 2064 6566 6175 6c74 2074 6f20 616c  on default to al
+000012f0: 6c6f 7720 6661 7374 2070 726f 746f 7479  low fast prototy
+00001300: 7069 6e67 2e20 466f 7220 726f 6275 7374  ping. For robust
+00001310: 2068 7970 6572 7061 7261 6d65 7465 720a   hyperparameter.
+00001320: 2020 2020 2020 2020 2020 2020 7475 6e69              tuni
+00001330: 6e67 2075 7369 6e67 2061 7420 6c65 6173  ng using at leas
+00001340: 7420 3520 666f 6c64 7320 6973 2072 6563  t 5 folds is rec
+00001350: 6f6d 6d65 6e64 6564 2e61 5f01 0000 4665  ommended.a_...Fe
+00001360: 6174 7572 6520 7365 6c65 6374 696f 6e20  ature selection 
+00001370: 6973 2065 6e61 626c 6564 2062 7574 206e  is enabled but n
+00001380: 6f20 6665 6174 7572 6520 7365 6c65 6374  o feature select
+00001390: 6f72 2068 6173 2062 6565 6e20 7072 6f76  or has been prov
+000013a0: 6964 6564 2e20 4661 6c6c 696e 6720 6261  ided. Falling ba
+000013b0: 636b 2074 6f0a 2020 2020 2020 2020 2020  ck to.          
+000013c0: 2020 6372 6f73 732d 7661 6c69 6461 7465    cross-validate
+000013d0: 6420 6665 6174 7572 6520 656c 696d 696e  d feature elimin
+000013e0: 6174 696f 6e2e 2053 7065 6369 6669 6361  ation. Specifica
+000013f0: 6c6c 7920 666f 7220 736d 616c 6c20 6461  lly for small da
+00001400: 7461 7365 7473 2063 6865 636b 2074 6865  tasets check the
+00001410: 206c 6f67 7320 746f 2076 6572 6966 7920   logs to verify 
+00001420: 7468 6174 206e 6f74 2074 6f6f 0a20 2020  that not too.   
+00001430: 2020 2020 2020 2020 206d 616e 7920 6665           many fe
+00001440: 6174 7572 6573 2068 6176 6520 6265 656e  atures have been
+00001450: 2072 656d 6f76 6564 2e20 4f74 6865 7277   removed. Otherw
+00001460: 6973 652c 2063 6f6e 7369 6465 7220 6469  ise, consider di
+00001470: 7361 626c 696e 6720 6665 6174 7572 6520  sabling feature 
+00001480: 7365 6c65 6374 696f 6e20 6f72 2070 726f  selection or pro
+00001490: 7669 6469 6e67 2061 2063 7573 746f 6d0a  viding a custom.
+000014a0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+000014b0: 7572 6520 7365 6c65 6374 6f72 2e61 6501  ure selector.ae.
+000014c0: 0000 4e6f 2058 6762 6f6f 7374 5475 6e65  ..No XgboostTune
+000014d0: 5061 7261 6d73 436f 6e66 6967 2068 6173  ParamsConfig has
+000014e0: 2062 6565 6e20 7072 6f76 6964 6564 2e20   been provided. 
+000014f0: 4661 6c6c 696e 6720 6261 636b 2074 6f20  Falling back to 
+00001500: 6465 6661 756c 7420 7661 6c75 6573 2e20  default values. 
+00001510: 4465 6661 756c 7420 7661 6c75 6573 0a20  Default values. 
+00001520: 2020 2020 2020 2020 2020 2068 6176 6520             have 
+00001530: 6265 656e 2063 686f 7365 6e20 746f 2073  been chosen to s
+00001540: 7065 6564 2075 7020 7468 6520 7072 6f74  peed up the prot
+00001550: 6f74 7970 696e 672e 2046 6f72 2072 6f62  otyping. For rob
+00001560: 7573 7420 6879 7065 7270 6172 616d 6574  ust hyperparamet
+00001570: 6572 2074 756e 696e 6720 636f 6e73 6964  er tuning consid
+00001580: 6572 2070 726f 7669 6469 6e67 2061 2063  er providing a c
+00001590: 7573 746f 6d0a 2020 2020 2020 2020 2020  ustom.          
+000015a0: 2020 5867 626f 6f73 7454 756e 6550 6172    XgboostTunePar
+000015b0: 616d 7343 6f6e 6669 6720 7769 7468 2061  amsConfig with a
+000015c0: 2064 6565 7065 7220 6879 7065 7270 6172   deeper hyperpar
+000015d0: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
+000015e0: 6163 6520 616e 6420 6120 6375 7374 6f6d  ace and a custom
+000015f0: 2054 7261 696e 696e 6743 6f6e 6669 6720   TrainingConfig 
+00001600: 746f 2065 6e61 626c 650a 2020 2020 2020  to enable.      
+00001610: 2020 2020 2020 6372 6f73 732d 7661 6c69        cross-vali
+00001620: 6461 7469 6f6e 2e61 0f01 0000 5468 6520  dation.a....The 
+00001630: 6d69 6e69 6d75 6d20 6e75 6d62 6572 206f  minimum number o
+00001640: 6620 6665 6174 7572 6573 2074 6f20 7365  f features to se
+00001650: 6c65 6374 2069 7320 6772 6561 7465 7220  lect is greater 
+00001660: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
+00001670: 6e75 6d62 6572 206f 6620 6665 6174 7572  number of featur
+00001680: 6573 2069 6e0a 2020 2020 2020 2020 2020  es in.          
+00001690: 2020 7468 6520 6461 7461 7365 7420 7768    the dataset wh
+000016a0: 696c 6520 6665 6174 7572 6520 7365 6c65  ile feature sele
+000016b0: 6374 696f 6e20 6973 2065 6e61 626c 6564  ction is enabled
+000016c0: 2e20 436f 6e73 6964 6572 2072 6564 7563  . Consider reduc
+000016d0: 696e 6720 7468 6520 6d69 6e69 6d75 6d20  ing the minimum 
+000016e0: 6e75 6d62 6572 206f 6620 6665 6174 7572  number of featur
+000016f0: 6573 2074 6f0a 2020 2020 2020 2020 2020  es to.          
+00001700: 2020 7365 6c65 6374 206f 7220 6469 7361    select or disa
+00001710: 626c 696e 6720 6665 6174 7572 6520 7365  bling feature se
+00001720: 6c65 6374 696f 6e20 7669 6120 5472 6169  lection via Trai
+00001730: 6e69 6e67 436f 6e66 6967 2e7a 8154 6865  ningConfig.z.The
+00001740: 2074 6172 6765 7420 636f 6c75 6d6e 2069   target column i
+00001750: 7320 7072 6573 656e 7420 696e 2074 6865  s present in the
+00001760: 2064 6174 6173 6574 2e20 436f 6e73 6964   dataset. Consid
+00001770: 6572 2072 656d 6f76 696e 6720 7468 6520  er removing the 
+00001780: 7461 7267 6574 2063 6f6c 756d 6e20 6672  target column fr
+00001790: 6f6d 2074 6865 0a20 2020 2020 2020 2020  om the.         
+000017a0: 2020 2064 6174 6173 6574 2074 6f20 7072     dataset to pr
+000017b0: 6576 656e 7420 6c65 616b 6167 652e 290d  event leakage.).
+000017c0: 7228 0000 0072 0a00 0000 da18 656e 6162  r(...r......enab
+000017d0: 6c65 5f66 6561 7475 7265 5f73 656c 6563  le_feature_selec
+000017e0: 7469 6f6e da08 7761 726e 696e 6773 da04  tion..warnings..
+000017f0: 7761 726e da0b 5573 6572 5761 726e 696e  warn..UserWarnin
+00001800: 67da 1468 7970 6572 7475 6e69 6e67 5f63  g..hypertuning_c
+00001810: 765f 666f 6c64 7372 2700 0000 7229 0000  v_foldsr'...r)..
+00001820: 00da 166d 696e 5f66 6561 7475 7265 735f  ...min_features_
+00001830: 746f 5f73 656c 6563 74da 036c 656e da07  to_select..len..
+00001840: 636f 6c75 6d6e 7372 2000 0000 2903 7231  columnsr ...).r1
+00001850: 0000 0072 3500 0000 da07 6d65 7373 6167  ...r5.....messag
+00001860: 6572 3200 0000 7232 0000 0072 3300 0000  er2...r2...r3...
+00001870: da0e 696e 6974 6961 6c5f 6368 6563 6b73  ..initial_checks
+00001880: 6200 0000 7334 0000 0006 0108 0108 0104  b...s4..........
+00001890: 0110 050c 0204 0110 0306 0302 ff04 0202  ................
+000018a0: fe04 0410 0406 0104 0110 0412 0206 0102  ................
+000018b0: ff04 0310 030c 0104 0114 0204 fd7a 1742  .............z.B
+000018c0: 6c75 6543 6173 742e 696e 6974 6961 6c5f  lueCast.initial_
+000018d0: 6368 6563 6b73 da0a 7461 7267 6574 5f63  checks..target_c
+000018e0: 6f6c 6303 0000 0000 0000 0000 0000 0009  olc.............
+000018f0: 0000 0007 0000 0043 0000 0073 d002 0000  .......C...s....
+00001900: 7400 8300 0100 7401 8300 7d03 7c03 a002  t.....t...}.|...
+00001910: 7c01 a101 7d01 7c03 7c00 5f03 7c00 6a03  |...}.|.|._.|.j.
+00001920: 6a04 7229 7c00 6a05 7c00 6a03 6a04 7600  j.r)|.j.|.j.j.v.
+00001930: 7229 7406 8300 7c00 5f07 7c00 6a07 a008  r)t...|._.|.j...
+00001940: 7c01 7c00 6a05 1900 a101 7c01 7c00 6a05  |.|.j.....|.|.j.
+00001950: 3c00 7c00 6a03 6a04 7c00 5f04 7c00 6a03  <.|.j.j.|._.|.j.
+00001960: 6a09 7c00 5f09 7c00 6a0a 733a 740b 8300  j.|._.|.j.s:t...
+00001970: 7c00 5f0a 7c00 a00c 7c01 a101 0100 740d  |._.|...|.....t.
+00001980: 7c01 7c02 7c00 6a0e 7c00 6a0a 6a0f 7c00  |.|.|.j.|.j.j.|.
+00001990: 6a0a 6a10 7c00 6a0a 6a11 8306 5c04 7d04  j.j.|.j.j...\.}.
+000019a0: 7d05 7d06 7d07 7c00 6a12 7297 7c00 6a12  }.}.}.|.j.r.|.j.
+000019b0: a013 7c04 7c06 a102 5c02 7d04 7d06 7c00  ..|.|...\.}.}.|.
+000019c0: 6a12 6a14 7c05 7c07 6401 6402 8d03 5c02  j.j.|.|.d.d...\.
+000019d0: 7d05 7d07 7401 8300 7d03 7c03 a002 7c04  }.}.t...}.|...|.
+000019e0: a101 7d08 7c04 6a15 6403 6404 8d01 7c06  ..}.|.j.d.d...|.
+000019f0: 6a15 6403 6404 8d01 0202 7d04 7d06 7c05  j.d.d.....}.}.|.
+00001a00: 6a15 6403 6404 8d01 7c07 6a15 6403 6404  j.d.d...|.j.d.d.
+00001a10: 8d01 0202 7d05 7d07 7c02 7c03 6a04 7600  ....}.}.|.|.j.v.
+00001a20: 7297 7c03 6a04 a016 7c02 a101 0100 7417  r.|.j...|.....t.
+00001a30: 7c04 8301 7417 7c05 8301 0202 7d04 7d05  |...t.|.....}.}.
+00001a40: 7418 7c04 7c00 6a09 8302 7418 7c05 7c00  t.|.|.j...t.|.|.
+00001a50: 6a09 8302 0202 7d04 7d05 7419 8300 7c00  j.....}.}.t...|.
+00001a60: 5f1a 7c00 6a1a a01b 7c04 a101 0100 7c00  _.|.j...|.....|.
+00001a70: 6a1a a014 7c05 a101 7d05 7c00 6a04 6405  j...|...}.|.j.d.
+00001a80: 7501 72db 7c00 6a1c 6406 6b02 72db 741d  u.r.|.j.d.k.r.t.
+00001a90: 7c03 6a04 8301 7c00 5f1e 7c00 6a1e a01f  |.j...|._.|.j...
+00001aa0: 7c04 7c06 a102 7d04 7c00 6a1e a020 7c05  |.|...}.|.j.. |.
+00001ab0: a101 7d05 6e1d 7c00 6a04 6405 7501 72f8  ..}.n.|.j.d.u.r.
+00001ac0: 7c00 6a1c 6407 6b02 72f8 7421 7c03 6a04  |.j.d.k.r.t!|.j.
+00001ad0: 8301 7c00 5f1e 7c00 6a1e a022 7c04 7c06  ..|._.|.j.."|.|.
+00001ae0: a102 7d04 7c00 6a1e a023 7c05 a101 7d05  ..}.|.j..#|...}.
+00001af0: 7c00 6a24 9001 7210 7c00 6a24 a013 7c04  |.j$..r.|.j$..|.
+00001b00: 7c06 a102 5c02 7d04 7d06 7c00 6a24 6a14  |...\.}.}.|.j$j.
+00001b10: 7c05 7c07 6401 6402 8d03 5c02 7d05 7d07  |.|.d.d...\.}.}.
+00001b20: 7c00 6a25 9001 731f 7426 7c00 6a0a 6a10  |.j%..s.t&|.j.j.
+00001b30: 7c00 6a0a 6a27 6408 8d02 7c00 5f25 7c00  |.j.j'd...|._%|.
+00001b40: 6a0a 6a28 9001 7237 7c00 6a25 a013 7c04  j.j(..r7|.j%..|.
+00001b50: 7c06 a102 5c02 7d04 7d06 7c00 6a25 6a14  |...\.}.}.|.j%j.
+00001b60: 7c05 6401 6402 8d02 5c02 7d05 7d08 7c00  |.d.d...\.}.}.|.
+00001b70: 6a29 9001 7348 742a 7c00 6a1c 7c00 6a0a  j)..sHt*|.j.|.j.
+00001b80: 7c00 6a2b 7c00 6a2c 6409 8d04 7c00 5f29  |.j+|.j,d...|._)
+00001b90: 7c00 6a29 a01b 7c04 7c05 7c06 7c07 a104  |.j)..|.|.|.|...
+00001ba0: 0100 7c00 6a0a 9001 7263 7c00 6a0a 6a2d  ..|.j...rc|.j.j-
+00001bb0: 9001 7263 742e 7c00 6a29 6a2f 7c05 640a  ..rct.|.j)j/|.d.
+00001bc0: 8303 7c00 5f30 6403 7c00 5f31 6405 5300  ..|._0d.|._1d.S.
+00001bd0: 290b 7a19 5472 6169 6e20 6120 6675 6c6c  ).z.Train a full
+00001be0: 204d 4c20 7069 7065 6c69 6e65 2e46 a901   ML pipeline.F..
+00001bf0: da0e 7072 6564 6963 746f 6e5f 6d6f 6465  ..predicton_mode
+00001c00: 54a9 01da 0464 726f 704e 721e 0000 0072  T....dropNr....r
+00001c10: 1f00 0000 2902 da0c 7261 6e64 6f6d 5f73  ....)...random_s
+00001c20: 7461 7465 723f 0000 0029 0372 2800 0000  tater?...).r(...
+00001c30: 7229 0000 0072 2a00 0000 da04 7472 6565  r)...r*.....tree
+00001c40: 2932 720f 0000 0072 1600 0000 5a1b 6669  )2r....r....Z.fi
+00001c50: 745f 7472 616e 7366 6f72 6d5f 6665 6174  t_transform_feat
+00001c60: 7572 655f 7479 7065 7372 2c00 0000 7221  ure_typesr,...r!
+00001c70: 0000 0072 2000 0000 7214 0000 0072 2e00  ...r ...r....r..
+00001c80: 0000 5a1b 6669 745f 7472 616e 7366 6f72  ..Z.fit_transfor
+00001c90: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
+00001ca0: 2200 0000 7228 0000 0072 0a00 0000 7243  "...r(...r....rC
+00001cb0: 0000 0072 1b00 0000 7223 0000 00da 0a74  ...r....r#.....t
+00001cc0: 7261 696e 5f73 697a 655a 1367 6c6f 6261  rain_sizeZ.globa
+00001cd0: 6c5f 7261 6e64 6f6d 5f73 7461 7465 5a14  l_random_stateZ.
+00001ce0: 7472 6169 6e5f 7370 6c69 745f 7374 7261  train_split_stra
+00001cf0: 7469 6679 7226 0000 00da 0d66 6974 5f74  tifyr&.....fit_t
+00001d00: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
+00001d10: 6f72 6dda 0b72 6573 6574 5f69 6e64 6578  orm..reset_index
+00001d20: da06 7265 6d6f 7665 7217 0000 0072 1300  ..remover....r..
+00001d30: 0000 7218 0000 0072 2f00 0000 da03 6669  ..r....r/.....fi
+00001d40: 7472 1d00 0000 7219 0000 0072 2d00 0000  tr....r....r-...
+00001d50: 5a1e 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
+00001d60: 6f64 655f 6269 6e61 7279 5f63 6c61 7373  ode_binary_class
+00001d70: da24 7472 616e 7366 6f72 6d5f 7461 7267  .$transform_targ
+00001d80: 6574 5f65 6e63 6f64 655f 6269 6e61 7279  et_encode_binary
+00001d90: 5f63 6c61 7373 721a 0000 005a 1c66 6974  _classr....Z.fit
+00001da0: 5f74 6172 6765 745f 656e 636f 6465 5f6d  _target_encode_m
+00001db0: 756c 7469 636c 6173 73da 2274 7261 6e73  ulticlass."trans
+00001dc0: 666f 726d 5f74 6172 6765 745f 656e 636f  form_target_enco
+00001dd0: 6465 5f6d 756c 7469 636c 6173 7372 2500  de_multiclassr%.
+00001de0: 0000 7227 0000 0072 1500 0000 723f 0000  ..r'...r....r?..
+00001df0: 0072 3a00 0000 7224 0000 0072 1100 0000  .r:...r$...r....
+00001e00: 7229 0000 0072 2a00 0000 5a15 6361 6c63  r)...r*...Z.calc
+00001e10: 756c 6174 655f 7368 6170 5f76 616c 7565  ulate_shap_value
+00001e20: 7372 0e00 0000 da05 6d6f 6465 6c72 3000  sr......modelr0.
+00001e30: 0000 722b 0000 0029 0972 3100 0000 7235  ..r+...).r1...r5
+00001e40: 0000 0072 4400 0000 722c 0000 00da 0778  ...rD...r,.....x
+00001e50: 5f74 7261 696e da06 785f 7465 7374 da07  _train..x_test..
+00001e60: 795f 7472 6169 6eda 0679 5f74 6573 74da  y_train..y_test.
+00001e70: 015f 7232 0000 0072 3200 0000 7233 0000  ._r2...r2...r3..
+00001e80: 0072 5000 0000 8f00 0000 73ac 0000 0006  .rP.......s.....
+00001e90: 0206 010a 0106 0108 020e 0108 0106 0308  ................
+00001ea0: 0102 ff02 fe04 0102 ff0a 060a 0106 0208  ................
+00001eb0: 010a 0202 0202 0102 0104 0106 0106 0106  ................
+00001ec0: 010c fa06 0912 0106 0106 010a ff06 030a  ................
+00001ed0: 010e 0102 010a ff0e 0302 010a ff0a 030c  ................
+00001ee0: 0112 020c 0106 0108 ff08 040c 010c 0114  ................
+00001ef0: 020c 010e 010e 0114 010c 010e 010c 0108  ................
+00001f00: 0206 0104 0108 ff06 0306 010a ff08 0402  ................
+00001f10: 0106 0106 0108 fe0a 0506 0104 0108 ff06  ................
+00001f20: 0304 010a ff08 0402 0104 0104 0104 0104  ................
+00001f30: 0108 fc12 0612 0112 010a 017a 0c42 6c75  ...........z.Blu
+00001f40: 6543 6173 742e 6669 74da 0764 665f 6576  eCast.fit..df_ev
+00001f50: 616c da0b 7461 7267 6574 5f65 7661 6c63  al..target_evalc
+00001f60: 0500 0000 0000 0000 0000 0000 0800 0000  ................
+00001f70: 0400 0000 4300 0000 732c 0000 007c 00a0  ....C...s,...|..
+00001f80: 007c 017c 04a1 0201 007c 00a0 017c 02a1  .|.|.....|...|..
+00001f90: 015c 027d 057d 0674 027c 036a 037c 057c  .\.}.}.t.|.j.|.|
+00001fa0: 0683 037d 077c 0753 0029 0161 8e02 0000  ...}.|.S.).a....
+00001fb0: 5472 6169 6e20 6120 6675 6c6c 204d 4c20  Train a full ML 
+00001fc0: 7069 7065 6c69 6e65 2061 6e64 2065 7661  pipeline and eva
+00001fd0: 6c75 6174 6520 6f6e 2061 2068 6f6c 646f  luate on a holdo
+00001fe0: 7574 2073 6574 2e0a 0a20 2020 2020 2020  ut set...       
+00001ff0: 2054 6869 7320 6973 2061 2063 6f6e 7665   This is a conve
+00002000: 6e69 656e 6365 2066 756e 6374 696f 6e20  nience function 
+00002010: 746f 2074 7261 696e 2061 6e64 2065 7661  to train and eva
+00002020: 6c75 6174 6520 6f6e 2061 2068 6f6c 646f  luate on a holdo
+00002030: 7574 2073 6574 2e20 4974 2069 7320 7265  ut set. It is re
+00002040: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
+00002050: 2074 6869 7320 666f 7220 6d6f 6465 6c0a   this for model.
+00002060: 2020 2020 2020 2020 6578 706c 6f72 6174          explorat
+00002070: 696f 6e2e 204f 6e20 7072 6f64 7563 7469  ion. On producti
+00002080: 6f6e 2074 6865 2073 696d 706c 6520 6669  on the simple fi
+00002090: 7428 2920 6675 6e63 7469 6f6e 2073 686f  t() function sho
+000020a0: 756c 6420 6265 2075 7365 642e 0a20 2020  uld be used..   
+000020b0: 2020 2020 203a 7061 7261 6d20 3a64 663a       :param :df:
+000020c0: 2054 616b 6573 2061 2070 616e 6461 7320   Takes a pandas 
+000020d0: 4461 7461 4672 616d 6520 636f 6e74 6169  DataFrame contai
+000020e0: 6e69 6e67 2074 6865 2074 7261 696e 696e  ning the trainin
+000020f0: 6720 6461 7461 2061 6e64 2074 6865 2074  g data and the t
+00002100: 6172 6765 7473 2e0a 2020 2020 2020 2020  argets..        
+00002110: 3a70 6172 616d 203a 6466 5f65 7661 6c3a  :param :df_eval:
+00002120: 2054 616b 6573 2061 2070 616e 6461 7320   Takes a pandas 
+00002130: 4461 7461 4672 616d 6520 636f 6e74 6169  DataFrame contai
+00002140: 6e69 6e67 2074 6865 2065 7661 6c75 6174  ning the evaluat
+00002150: 696f 6e20 6461 7461 2c20 6275 7420 6e6f  ion data, but no
+00002160: 7420 7468 6520 7461 7267 6574 732e 0a20  t the targets.. 
+00002170: 2020 2020 2020 203a 7061 7261 6d20 3a74         :param :t
+00002180: 6172 6765 745f 6576 616c 3a20 5461 6b65  arget_eval: Take
+00002190: 7320 6120 7061 6e64 6173 2053 6572 6965  s a pandas Serie
+000021a0: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
+000021b0: 2065 7661 6c75 6174 696f 6e20 7461 7267   evaluation targ
+000021c0: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
+000021d0: 7261 6d20 3a74 6172 6765 745f 636f 6c3a  ram :target_col:
+000021e0: 2054 616b 6573 2061 2073 7472 696e 6720   Takes a string 
+000021f0: 636f 6e74 6169 6e69 6e67 2074 6865 206e  containing the n
+00002200: 616d 6520 6f66 2074 6865 2074 6172 6765  ame of the targe
+00002210: 7420 636f 6c75 6d6e 2069 6e73 6964 6520  t column inside 
+00002220: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
+00002230: 6120 6466 2e0a 2020 2020 2020 2020 2904  a df..        ).
+00002240: 7250 0000 00da 0770 7265 6469 6374 720d  rP.....predictr.
+00002250: 0000 00da 0676 616c 7565 7329 0872 3100  .....values).r1.
+00002260: 0000 7235 0000 0072 5900 0000 725a 0000  ..r5...rY...rZ..
+00002270: 0072 4400 0000 da07 795f 7072 6f62 73da  .rD.....y_probs.
+00002280: 0979 5f63 6c61 7373 6573 5a09 6576 616c  .y_classesZ.eval
+00002290: 5f64 6963 7472 3200 0000 7232 0000 0072  _dictr2...r2...r
+000022a0: 3300 0000 da08 6669 745f 6576 616c f400  3.....fit_eval..
+000022b0: 0000 7308 0000 000c 100e 010e 0104 017a  ..s............z
+000022c0: 1142 6c75 6543 6173 742e 6669 745f 6576  .BlueCast.fit_ev
+000022d0: 616c 6302 0000 0000 0000 0000 0000 0003  alc.............
+000022e0: 0000 0004 0000 0043 0000 0073 2001 0000  .......C...s ...
+000022f0: 7400 8300 0100 7c00 6a01 730a 7402 6401  t.....|.j.s.t.d.
+00002300: 8301 8201 7c00 6a03 7311 7402 6402 8301  ....|.j.s.t.d...
+00002310: 8201 7c00 6a01 6a04 7c01 7c00 6a05 6701  ..|.j.j.|.|.j.g.
+00002320: 6403 8d02 7d01 7c00 6a06 722e 7c00 6a06  d...}.|.j.r.|.j.
+00002330: 6a07 7c01 6404 6405 8d02 5c02 7d01 7d02  j.|.d.d...\.}.}.
+00002340: 7c01 6a08 6404 6406 8d01 7d01 7409 7c01  |.j.d.d...}.t.|.
+00002350: 8301 7d01 740a 7c01 7c00 6a0b 8302 7d01  ..}.t.|.|.j...}.
+00002360: 7c00 6a0c 7241 7c00 6a0c a007 7c01 a101  |.j.rA|.j...|...
+00002370: 7d01 7c00 6a0d 7259 7c00 6a0e 7259 7c00  }.|.j.rY|.j.rY|.
+00002380: 6a0f 6407 6b02 7259 7410 7c00 6a0e 7411  j.d.k.rYt.|.j.t.
+00002390: 8302 7259 7c00 6a0e a012 7c01 a101 7d01  ..rY|.j...|...}.
+000023a0: 6e17 7c00 6a0d 7270 7c00 6a0e 7270 7c00  n.|.j.rp|.j.rp|.
+000023b0: 6a0f 6408 6b02 7270 7410 7c00 6a0e 7413  j.d.k.rpt.|.j.t.
+000023c0: 8302 7270 7c00 6a0e a014 7c01 a101 7d01  ..rp|.j...|...}.
+000023d0: 7c00 6a15 727d 7c00 6a15 6a07 7c01 6404  |.j.r}|.j.j.|.d.
+000023e0: 6405 8d02 5c02 7d01 7d02 7c00 6a16 728e  d...\.}.}.|.j.r.
+000023f0: 7c00 6a03 6a17 728e 7c00 6a16 6a07 7c01  |.j.j.r.|.j.j.|.
+00002400: 6404 6405 8d02 5c02 7d01 7d02 7c01 5300  d.d...\.}.}.|.S.
+00002410: 2909 7a37 5472 616e 7366 6f72 6d20 6e65  ).z7Transform ne
+00002420: 7720 6461 7461 2061 6363 6f72 6469 6e67  w data according
+00002430: 2074 6f20 7072 6570 726f 6365 7373 696e   to preprocessin
+00002440: 6720 7069 7065 6c69 6e65 2efa 2a46 6561  g pipeline..*Fea
+00002450: 7475 7265 2074 7970 6520 636f 6e76 6572  ture type conver
+00002460: 7465 7220 636f 756c 6420 6e6f 7420 6265  ter could not be
+00002470: 2066 6f75 6e64 2e7a 2a54 7261 696e 696e   found.z*Trainin
+00002480: 6720 636f 6e66 6967 7572 6174 696f 6e20  g configuration 
+00002490: 636f 756c 6420 6e6f 7420 6265 2066 6f75  could not be fou
+000024a0: 6e64 2e29 015a 0b69 676e 6f72 655f 636f  nd.).Z.ignore_co
+000024b0: 6c73 5472 4500 0000 7247 0000 0072 1e00  lsTrE...rG...r..
+000024c0: 0000 721f 0000 0029 1872 0f00 0000 722c  ..r....).r....r,
+000024d0: 0000 00da 0945 7863 6570 7469 6f6e 7228  .....Exceptionr(
+000024e0: 0000 005a 1774 7261 6e73 666f 726d 5f66  ...Z.transform_f
+000024f0: 6561 7475 7265 5f74 7970 6573 7220 0000  eature_typesr ..
+00002500: 0072 2600 0000 724d 0000 0072 4e00 0000  .r&...rM...rN...
+00002510: 7217 0000 0072 1300 0000 7222 0000 0072  r....r....r"...r
+00002520: 2f00 0000 7221 0000 0072 2d00 0000 721d  /...r!...r-...r.
+00002530: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
+00002540: 1900 0000 7251 0000 0072 1a00 0000 7252  ....rQ...r....rR
+00002550: 0000 0072 2500 0000 7227 0000 0072 3a00  ...r%...r'...r:.
+00002560: 0000 2903 7231 0000 0072 3500 0000 7258  ..).r1...r5...rX
+00002570: 0000 0072 3200 0000 7232 0000 0072 3300  ...r2...r2...r3.
+00002580: 0000 da12 7472 616e 7366 6f72 6d5f 6e65  ....transform_ne
+00002590: 775f 6461 7461 0901 0000 7348 0000 0006  w_data....sH....
+000025a0: 0206 0108 0106 0208 0106 0208 0106 ff06  ................
+000025b0: 0414 010c 0108 020c 0106 020c 0104 0302  ................
+000025c0: ff04 0202 fe0a 030a 0102 ff0e 0304 0202  ................
+000025d0: ff04 0202 fe0a 030a 0102 ff0c 0306 0214  ................
+000025e0: 010e 0214 0104 027a 1b42 6c75 6543 6173  .......z.BlueCas
+000025f0: 742e 7472 616e 7366 6f72 6d5f 6e65 775f  t.transform_new_
+00002600: 6461 7461 6302 0000 0000 0000 0000 0000  datac...........
+00002610: 0004 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
+00002620: 0000 7c00 6a00 7307 7401 6401 8301 8201  ..|.j.s.t.d.....
+00002630: 7c00 6a02 730e 7401 6402 8301 8201 7403  |.j.s.t.d.....t.
+00002640: 8300 0100 7c00 a004 7c01 a101 7d01 7405  ....|...|...}.t.
+00002650: 7406 a007 a100 9b00 6403 9d02 8301 0100  t.......d.......
+00002660: 7c00 6a00 a008 7c01 a101 5c02 7d02 7d03  |.j...|...\.}.}.
+00002670: 7c00 6a02 6a09 7241 7c00 6a0a 7c00 6a02  |.j.j.rA|.j.|.j.
+00002680: 6a09 7600 7241 7c00 6a0b 7241 7c00 6a02  j.v.rA|.j.rA|.j.
+00002690: 7241 7c00 6a0b a00c 740d a00e 7c03 a101  rA|.j...t...|...
+000026a0: a101 7d03 7c02 7c03 6602 5300 2904 7a90  ..}.|.|.f.S.).z.
+000026b0: 5072 6564 6963 7420 6f6e 2075 6e73 6565  Predict on unsee
+000026c0: 6e20 6461 7461 2e0a 0a20 2020 2020 2020  n data...       
+000026d0: 2052 6574 7572 6e20 7468 6520 7072 6564   Return the pred
+000026e0: 6963 7465 6420 7072 6f62 6162 696c 6974  icted probabilit
+000026f0: 6965 7320 616e 6420 7468 6520 7072 6564  ies and the pred
+00002700: 6963 7465 6420 636c 6173 7365 733a 0a20  icted classes:. 
+00002710: 2020 2020 2020 2079 5f70 726f 6273 2c20         y_probs, 
+00002720: 795f 636c 6173 7365 7320 3d20 7072 6564  y_classes = pred
+00002730: 6963 7428 6466 290a 2020 2020 2020 2020  ict(df).        
+00002740: 7a1b 4d6c 206d 6f64 656c 2063 6f75 6c64  z.Ml model could
+00002750: 206e 6f74 2062 6520 666f 756e 6472 6000   not be foundr`.
+00002760: 0000 7a0f 3a20 5072 6564 6963 7469 6e67  ..z.: Predicting
+00002770: 2e2e 2e29 0f72 2400 0000 7261 0000 0072  ...).r$...ra...r
+00002780: 2c00 0000 720f 0000 0072 6300 0000 7210  ,...r....rc...r.
+00002790: 0000 0072 0200 0000 da06 7574 636e 6f77  ...r......utcnow
+000027a0: 725b 0000 0072 2100 0000 7220 0000 0072  r[...r!...r ...r
+000027b0: 2e00 0000 5a1f 6c61 6265 6c5f 656e 636f  ....Z.label_enco
+000027c0: 6465 725f 7265 7665 7273 655f 7472 616e  der_reverse_tran
+000027d0: 7366 6f72 6dda 0270 64da 0653 6572 6965  sform..pd..Serie
+000027e0: 7329 0472 3100 0000 7235 0000 0072 5d00  s).r1...r5...r].
+000027f0: 0000 725e 0000 0072 3200 0000 7232 0000  ..r^...r2...r2..
+00002800: 0072 3300 0000 725b 0000 0037 0100 0073  .r3...r[...7...s
+00002810: 2400 0000 0606 0801 0602 0801 0602 0a01  $...............
+00002820: 1202 1001 0802 0e02 0401 02ff 0402 02fe  ................
+00002830: 0604 0801 04ff 0804 7a10 426c 7565 4361  ........z.BlueCa
+00002840: 7374 2e70 7265 6469 6374 290a 4e4e 4e4e  st.predict).NNNN
+00002850: 4e4e 4e4e 4e4e 291f da08 5f5f 6e61 6d65  NNNNNN)...__name
+00002860: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00002870: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00002880: 646f 635f 5f72 0600 0000 7209 0000 00da  doc__r....r.....
+00002890: 0373 7472 da05 666c 6f61 74da 0369 6e74  .str..float..int
+000028a0: 7207 0000 0072 0500 0000 7211 0000 0072  r....r....r....r
+000028b0: 0300 0000 7212 0000 0072 1500 0000 720a  ....r....r....r.
+000028c0: 0000 0072 0c00 0000 720b 0000 0072 3400  ...r....r....r4.
+000028d0: 0000 7265 0000 00da 0944 6174 6146 7261  ..re.....DataFra
+000028e0: 6d65 7243 0000 0072 5000 0000 7266 0000  merC...rP...rf..
+000028f0: 0072 0400 0000 725f 0000 0072 6300 0000  .r....r_...rc...
+00002900: 7208 0000 00da 026e 70da 076e 6461 7272  r......np..ndarr
+00002910: 6179 725b 0000 0072 3200 0000 7232 0000  ayr[...r2...r2..
+00002920: 0072 3200 0000 7233 0000 0072 1c00 0000  .r2...r3...r....
+00002930: 2700 0000 736c 0000 0008 0004 0102 1802  '...sl..........
+00002940: 0102 0102 0102 0102 0102 0302 0102 0102  ................
+00002950: 0104 f106 0202 fe0c 0302 fd14 0402 fc14  ................
+00002960: 0502 fb06 0602 fa0e 0702 f906 0802 f806  ................
+00002970: 0902 f702 0a0a 0102 ff02 f606 0d02 f306  ................
+00002980: 0e02 f206 0f0a f114 2618 2d02 6504 0202  ........&.-.e...
+00002990: fe04 0302 fd04 0402 fc02 0502 fb0a 060a  ................
+000029a0: fa16 1524 2e72 1c00 0000 2930 726a 0000  ...$.r....)0rj..
+000029b0: 0072 3b00 0000 7202 0000 00da 0674 7970  .r;...r......typ
+000029c0: 696e 6772 0300 0000 7204 0000 0072 0500  ingr....r....r..
+000029d0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+000029e0: 0072 0900 0000 da05 6e75 6d70 7972 6f00  .r......numpyro.
+000029f0: 0000 da06 7061 6e64 6173 7265 0000 00da  ....pandasre....
+00002a00: 1f62 6c75 6563 6173 742e 636f 6e66 6967  .bluecast.config
+00002a10: 2e74 7261 696e 696e 675f 636f 6e66 6967  .training_config
+00002a20: 720a 0000 0072 0b00 0000 720c 0000 005a  r....r....r....Z
+00002a30: 2062 6c75 6563 6173 742e 6576 616c 7561   bluecast.evalua
+00002a40: 7469 6f6e 2e65 7661 6c5f 6d65 7472 6963  tion.eval_metric
+00002a50: 7372 0d00 0000 5a1f 626c 7565 6361 7374  sr....Z.bluecast
+00002a60: 2e65 7661 6c75 6174 696f 6e2e 7368 6170  .evaluation.shap
+00002a70: 5f76 616c 7565 7372 0e00 0000 5a24 626c  _valuesr....Z$bl
+00002a80: 7565 6361 7374 2e67 656e 6572 616c 5f75  uecast.general_u
+00002a90: 7469 6c73 2e67 656e 6572 616c 5f75 7469  tils.general_uti
+00002aa0: 6c73 720f 0000 0072 1000 0000 5a1d 626c  lsr....r....Z.bl
+00002ab0: 7565 6361 7374 2e6d 6c5f 6d6f 6465 6c6c  uecast.ml_modell
+00002ac0: 696e 672e 7867 626f 6f73 7472 1100 0000  ing.xgboostr....
+00002ad0: da1d 626c 7565 6361 7374 2e70 7265 7072  ..bluecast.prepr
+00002ae0: 6f63 6573 7369 6e67 2e63 7573 746f 6d72  ocessing.customr
+00002af0: 1200 0000 5a28 626c 7565 6361 7374 2e70  ....Z(bluecast.p
+00002b00: 7265 7072 6f63 6573 7369 6e67 2e64 6174  reprocessing.dat
+00002b10: 6574 696d 655f 6665 6174 7572 6573 7213  etime_featuresr.
+00002b20: 0000 005a 2b62 6c75 6563 6173 742e 7072  ...Z+bluecast.pr
+00002b30: 6570 726f 6365 7373 696e 672e 656e 636f  eprocessing.enco
+00002b40: 6465 5f74 6172 6765 745f 6c61 6265 6c73  de_target_labels
+00002b50: 7214 0000 005a 2862 6c75 6563 6173 742e  r....Z(bluecast.
+00002b60: 7072 6570 726f 6365 7373 696e 672e 6665  preprocessing.fe
+00002b70: 6174 7572 655f 7365 6c65 6374 696f 6e72  ature_selectionr
+00002b80: 1500 0000 5a24 626c 7565 6361 7374 2e70  ....Z$bluecast.p
+00002b90: 7265 7072 6f63 6573 7369 6e67 2e66 6561  reprocessing.fea
+00002ba0: 7475 7265 5f74 7970 6573 7216 0000 005a  ture_typesr....Z
+00002bb0: 2562 6c75 6563 6173 742e 7072 6570 726f  %bluecast.prepro
+00002bc0: 6365 7373 696e 672e 6e75 6c6c 735f 616e  cessing.nulls_an
+00002bd0: 645f 696e 6673 7217 0000 005a 2462 6c75  d_infsr....Z$blu
+00002be0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
+00002bf0: 696e 672e 7363 6865 6d61 5f63 6865 636b  ing.schema_check
+00002c00: 7372 1800 0000 5a26 626c 7565 6361 7374  sr....Z&bluecast
+00002c10: 2e70 7265 7072 6f63 6573 7369 6e67 2e74  .preprocessing.t
+00002c20: 6172 6765 745f 656e 636f 6469 6e67 7219  arget_encodingr.
+00002c30: 0000 0072 1a00 0000 5a27 626c 7565 6361  ...r....Z'blueca
+00002c40: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00002c50: 2e74 7261 696e 5f74 6573 745f 7370 6c69  .train_test_spli
+00002c60: 7472 1b00 0000 721c 0000 0072 3200 0000  tr....r....r2...
+00002c70: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00002c80: 083c 6d6f 6475 6c65 3e01 0000 0073 2a00  .<module>....s*.
+00002c90: 0000 0400 0808 0c01 2401 0802 0801 1402  ........$.......
+00002ca0: 0c05 0c01 1001 0c01 0c01 0c01 0c01 0c01  ................
+00002cb0: 0c01 0c01 0c01 1001 0c04 1203            ............
```

### Comparing `bluecast-0.4.2/bluecast/blueprints/__pycache__/cast.cpython-38.pyc` & `bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/blueprints/cast.py` & `bluecast-0.5/bluecast/blueprints/cast.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 Customization via class attributes is possible. Configs can be instantiated and provided to change Xgboost training.
 Default hyperparameter search space is relatively light-weight to speed up the prototyping.
 Can deal with binary and multi-class classification problems.
 Hyperparameter tuning can be switched off or even strengthened via cross-validation. This behaviour can be controlled
 via the config class attributes from config.training_config module.
 """
 import warnings
+from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from bluecast.config.training_config import (
-    FeatureSelectionConfig,
     TrainingConfig,
     XgboostFinalParamConfig,
     XgboostTuneParamsConfig,
 )
 from bluecast.evaluation.eval_metrics import eval_classifier
 from bluecast.evaluation.shap_values import shap_explanations
-from bluecast.general_utils.general_utils import check_gpu_support
+from bluecast.general_utils.general_utils import check_gpu_support, logger
 from bluecast.ml_modelling.xgboost import XgboostModel
 from bluecast.preprocessing.custom import CustomPreprocessing
 from bluecast.preprocessing.datetime_features import date_converter
 from bluecast.preprocessing.encode_target_labels import TargetLabelEncoder
-from bluecast.preprocessing.feature_selection import FeatureSelector
+from bluecast.preprocessing.feature_selection import RFECVSelector
 from bluecast.preprocessing.feature_types import FeatureTypeDetector
 from bluecast.preprocessing.nulls_and_infs import fill_infinite_values
 from bluecast.preprocessing.schema_checks import SchemaDetector
 from bluecast.preprocessing.target_encoding import (
     BinaryClassTargetEncoder,
     MultiClassTargetEncoder,
 )
@@ -63,41 +63,87 @@
         target_column: Union[str, float, int],
         cat_columns: Optional[List[Union[str, float, int]]] = None,
         date_columns: Optional[List[Union[str, float, int]]] = None,
         time_split_column: Optional[str] = None,
         ml_model: Optional[Union[XgboostModel, Any]] = None,
         custom_last_mile_computation: Optional[CustomPreprocessing] = None,
         custom_preprocessor: Optional[CustomPreprocessing] = None,
+        custom_feature_selector: Optional[
+            Union[RFECVSelector, CustomPreprocessing]
+        ] = None,
         conf_training: Optional[TrainingConfig] = None,
         conf_xgboost: Optional[XgboostTuneParamsConfig] = None,
         conf_params_xgboost: Optional[XgboostFinalParamConfig] = None,
-        conf_feature_selection: Optional[FeatureSelectionConfig] = None,
     ):
         self.class_problem = class_problem
         self.prediction_mode: bool = False
         self.cat_columns = cat_columns
         self.date_columns = date_columns
         self.time_split_column = time_split_column
         self.target_column = target_column
         self.conf_training = conf_training
         self.conf_xgboost = conf_xgboost
         self.conf_params_xgboost = conf_params_xgboost
-        self.conf_feature_selection = conf_feature_selection
-        self.feature_selector: Optional[FeatureSelector] = None
         self.feat_type_detector: Optional[FeatureTypeDetector] = None
         self.cat_encoder: Optional[
             Union[BinaryClassTargetEncoder, MultiClassTargetEncoder]
         ] = None
         self.target_label_encoder: Optional[TargetLabelEncoder] = None
         self.schema_detector: Optional[SchemaDetector] = None
         self.ml_model: Optional[XgboostModel] = ml_model
         self.custom_last_mile_computation = custom_last_mile_computation
         self.custom_preprocessor = custom_preprocessor
+        self.custom_feature_selector = custom_feature_selector
         self.shap_values: Optional[np.ndarray] = None
 
+    def initial_checks(self, df: pd.DataFrame) -> None:
+        if not self.conf_training:
+            self.conf_training = TrainingConfig()
+        if not self.conf_training.enable_feature_selection:
+            message = """Feature selection is disabled. Update the TrainingConfig param 'enable_feature_selection'
+            to enable it or make use of a custom preprocessor to do it manually during the last mile computations step.
+            Feature selection is recommended for datasets with many features (>1000). For datasets with a small amount
+            of features feature selection is not recommended.
+            """
+            warnings.warn(message, UserWarning, stacklevel=2)
+
+        if self.conf_training.hypertuning_cv_folds == 1:
+            message = """Cross validation is disabled. Update the TrainingConfig param 'hypertuning_cv_folds'
+            to enable it. Cross validation is disabled on default to allow fast prototyping. For robust hyperparameter
+            tuning using at least 5 folds is recommended."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+
+        if (
+            self.conf_training.enable_feature_selection
+            and not self.custom_feature_selector
+        ):
+            message = """Feature selection is enabled but no feature selector has been provided. Falling back to
+            cross-validated feature elimination. Specifically for small datasets check the logs to verify that not too
+            many features have been removed. Otherwise, consider disabling feature selection or providing a custom
+            feature selector."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+        if not self.conf_xgboost:
+            message = """No XgboostTuneParamsConfig has been provided. Falling back to default values. Default values
+            have been chosen to speed up the prototyping. For robust hyperparameter tuning consider providing a custom
+            XgboostTuneParamsConfig with a deeper hyperparameter search space and a custom TrainingConfig to enable
+            cross-validation."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+        if (
+            self.conf_training.min_features_to_select >= len(df.columns)
+            and self.conf_training.enable_feature_selection
+        ):
+            message = """The minimum number of features to select is greater or equal to the number of features in
+            the dataset while feature selection is enabled. Consider reducing the minimum number of features to
+            select or disabling feature selection via TrainingConfig."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+        if self.target_column in df.columns:
+            message = """The target column is present in the dataset. Consider removing the target column from the
+            dataset to prevent leakage."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+
     def fit(self, df: pd.DataFrame, target_col: str) -> None:
         """Train a full ML pipeline."""
         check_gpu_support()
         feat_type_detector = FeatureTypeDetector()
         df = feat_type_detector.fit_transform_feature_types(df)
         self.feat_type_detector = feat_type_detector
 
@@ -112,27 +158,15 @@
 
         self.cat_columns = self.feat_type_detector.cat_columns
         self.date_columns = self.feat_type_detector.date_columns
 
         if not self.conf_training:
             self.conf_training = TrainingConfig()
 
-        if not self.conf_training.enable_feature_selection:
-            message = """Feature selection is disabled. Update the TrainingConfig param 'enable_feature_selection'
-            to enable it or make use of a custom preprocessor to do it manually during the last mile computations step.
-            Feature selection is recommended for datasets with many features (>1000). For datasets with a small amount
-            of features feature selection is not recommended.
-            """
-            warnings.warn(message, UserWarning, stacklevel=2)
-
-        if self.conf_training.hypertuning_cv_folds == 1:
-            message = """Cross validation is disabled. Update the TrainingConfig param 'hypertuning_cv_folds'
-            to enable it. Cross validation is disabled on default to allow fast prototyping. For robust hyperparameter
-            tuning using at least 5 folds is recommended."""
-            warnings.warn(message, UserWarning, stacklevel=2)
+        self.initial_checks(df)
 
         x_train, x_test, y_train, y_test = train_test_split(
             df,
             target_col,
             self.time_split_column,
             self.conf_training.train_size,
             self.conf_training.global_random_state,
@@ -177,25 +211,27 @@
             x_train, y_train = self.custom_last_mile_computation.fit_transform(
                 x_train, y_train
             )
             x_test, y_test = self.custom_last_mile_computation.transform(
                 x_test, y_test, predicton_mode=False
             )
 
-        if not self.conf_feature_selection:
-            self.conf_feature_selection = FeatureSelectionConfig()
+        if not self.custom_feature_selector:
+            self.custom_feature_selector = RFECVSelector(
+                random_state=self.conf_training.global_random_state,
+                min_features_to_select=self.conf_training.min_features_to_select,
+            )
 
         if self.conf_training.enable_feature_selection:
-            self.feature_selector = FeatureSelector(
-                selection_strategy=self.conf_feature_selection.selection_strategy
+            x_train, y_train = self.custom_feature_selector.fit_transform(
+                x_train, y_train
+            )
+            x_test, _ = self.custom_feature_selector.transform(
+                x_test, predicton_mode=False
             )
-
-        if self.feature_selector and self.conf_training.enable_feature_selection:
-            x_train = self.feature_selector.fit_transform(x_train, y_train)
-            x_test = self.feature_selector.transform(x_test)
 
         if not self.ml_model:
             self.ml_model = XgboostModel(
                 self.class_problem,
                 conf_training=self.conf_training,
                 conf_xgboost=self.conf_xgboost,
                 conf_params_xgboost=self.conf_params_xgboost,
@@ -219,23 +255,26 @@
         :param :df: Takes a pandas DataFrame containing the training data and the targets.
         :param :df_eval: Takes a pandas DataFrame containing the evaluation data, but not the targets.
         :param :target_eval: Takes a pandas Series containing the evaluation targets.
         :param :target_col: Takes a string containing the name of the target column inside the training data df.
         """
         self.fit(df, target_col)
         y_probs, y_classes = self.predict(df_eval)
-        eval_dict = eval_classifier(target_eval.values, y_classes)
+        eval_dict = eval_classifier(target_eval.values, y_probs, y_classes)
         return eval_dict
 
     def transform_new_data(self, df: pd.DataFrame) -> pd.DataFrame:
         """Transform new data according to preprocessing pipeline."""
         check_gpu_support()
         if not self.feat_type_detector:
             raise Exception("Feature type converter could not be found.")
 
+        if not self.conf_training:
+            raise Exception("Training configuration could not be found.")
+
         df = self.feat_type_detector.transform_feature_types(
             df, ignore_cols=[self.target_column]
         )
 
         if self.custom_preprocessor:
             df, _ = self.custom_preprocessor.transform(df, predicton_mode=True)
             df = df.reset_index(drop=True)
@@ -260,22 +299,16 @@
             and isinstance(self.cat_encoder, MultiClassTargetEncoder)
         ):
             df = self.cat_encoder.transform_target_encode_multiclass(df)
 
         if self.custom_last_mile_computation:
             df, _ = self.custom_last_mile_computation.transform(df, predicton_mode=True)
 
-        if not self.conf_feature_selection:
-            self.conf_feature_selection = FeatureSelectionConfig()
-
-        if not self.conf_training:
-            self.conf_training = TrainingConfig()
-
-        if self.feature_selector and self.conf_training.enable_feature_selection:
-            df = self.feature_selector.transform(df)
+        if self.custom_feature_selector and self.conf_training.enable_feature_selection:
+            df, _ = self.custom_feature_selector.transform(df, predicton_mode=True)
 
         return df
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data.
 
         Return the predicted probabilities and the predicted classes:
@@ -286,15 +319,15 @@
 
         if not self.feat_type_detector:
             raise Exception("Feature type converter could not be found.")
 
         check_gpu_support()
         df = self.transform_new_data(df)
 
-        print("Predicting...")
+        logger(f"{datetime.utcnow()}: Predicting...")
         y_probs, y_classes = self.ml_model.predict(df)
 
         if self.feat_type_detector.cat_columns:
             if (
                 self.target_column in self.feat_type_detector.cat_columns
                 and self.target_label_encoder
                 and self.feat_type_detector
```

### Comparing `bluecast-0.4.2/bluecast/config/__pycache__/training_config.cpython-38.pyc` & `bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/config/training_config.py` & `bluecast-0.5/bluecast/config/training_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 Pydantic dataclasses are used to define the configuration parameters. This allows for type checking and validation of
 the configuration parameters. The configuration parameters are used in the training pipeline and in the evaluation
 pipeline. Pydantic dataclasses are used to allow users a pythonic way to define the configuration parameters.
 Default configurations can be loaded, adjusted and passed into the blueprints.
 """
 from typing import Dict, Optional
 
-import xgboost as xgb
 from pydantic.dataclasses import dataclass
-from sklearn.feature_selection import RFECV
-from sklearn.metrics import make_scorer, matthews_corrcoef
-from sklearn.model_selection import StratifiedKFold
 
 
 class Config:
     arbitrary_types_allowed = True
 
 
 @dataclass
@@ -30,28 +26,15 @@
     early_stopping_rounds: int = 10
     autotune_model: bool = True
     enable_feature_selection: bool = False
     calculate_shap_values: bool = True
     train_size: float = 0.8
     train_split_stratify: bool = True
     use_full_data_for_final_model: bool = True
-
-
-@dataclass(config=Config)
-class FeatureSelectionConfig:
-    """Define feature selection parameters."""
-
-    selection_strategy: RFECV = RFECV(
-        estimator=xgb.XGBClassifier(),
-        step=1,
-        cv=StratifiedKFold(5, random_state=0, shuffle=True),
-        min_features_to_select=1,
-        scoring=make_scorer(matthews_corrcoef),
-        n_jobs=4,
-    )
+    min_features_to_select: int = 5
 
 
 @dataclass
 class XgboostTuneParamsConfig:
     """Define hyperparameter tuning search space."""
 
     max_depth_min: int = 2
```

### Comparing `bluecast-0.4.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 04:30:45 2023 UTC, .py size: 2478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,123 @@
-00000000: 6f0d 0d0a 0000 0000 f51f 9564 ae09 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 cad1 9764 a408 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
+00000020: 000a 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a05 6401 6404 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 0100 6406 6407 8400 5a0f 6408  m.Z...d.d...Z.d.
-00000080: 6505 6a10 6409 6505 6a10 640a 6503 6511  e.j.d.e.j.d.e.e.
-00000090: 6502 6602 1900 6606 640b 640c 8404 5a12  e.f...f.d.d...Z.
-000000a0: 6403 5300 290d 7a51 4d6f 6475 6c65 2066  d.S.).zQModule f
-000000b0: 6f72 2065 7661 6c75 6174 696f 6e20 6d65  or evaluation me
-000000c0: 7472 6963 732e 0a0a 5468 6973 2069 7320  trics...This is 
-000000d0: 6361 6c6c 6564 2061 7320 7061 7274 206f  called as part o
-000000e0: 6620 7468 6520 6669 745f 6576 616c 2066  f the fit_eval f
-000000f0: 756e 6374 696f 6e2e 0ae9 0000 0000 2902  unction.......).
-00000100: da03 416e 79da 0444 6963 744e 2906 da0e  ..Any..DictN)...
-00000110: 6163 6375 7261 6379 5f73 636f 7265 da15  accuracy_score..
-00000120: 636c 6173 7369 6669 6361 7469 6f6e 5f72  classification_r
-00000130: 6570 6f72 74da 1063 6f6e 6675 7369 6f6e  eport..confusion
-00000140: 5f6d 6174 7269 78da 0866 315f 7363 6f72  _matrix..f1_scor
-00000150: 65da 116d 6174 7468 6577 735f 636f 7272  e..matthews_corr
-00000160: 636f 6566 da0c 7265 6361 6c6c 5f73 636f  coef..recall_sco
-00000170: 7265 2901 da06 6c6f 6767 6572 6302 0000  re)...loggerc...
-00000180: 0000 0000 0000 0000 0005 0000 0006 0000  ................
-00000190: 0043 0000 0073 8e00 0000 7c00 6401 6b02  .C...s....|.d.k.
-000001a0: 7c00 6402 6b02 4200 a000 a100 730c 4a00  |.d.k.B.....s.J.
-000001b0: 8201 7401 7c00 8301 7401 7c01 8301 6b02  ..t.|...t.|...k.
-000001c0: 7316 4a00 8201 7c01 6a02 6402 6b02 731d  s.J...|.j.d.k.s.
-000001d0: 4a00 8201 6403 7d02 7c01 a003 7c02 6402  J...d.}.|...|.d.
-000001e0: 7c02 1800 a102 7d01 7404 a005 6402 7c01  |.....}.t...d.|.
-000001f0: 7c00 6401 6b02 1900 1800 a101 0b00 7d03  |.d.k.........}.
-00000200: 7404 a005 7c01 7c00 6401 6b03 1900 a101  t...|.|.d.k.....
-00000210: 0b00 7d04 7c03 a006 a100 7c04 a006 a100  ..}.|.....|.....
-00000220: 1700 6404 1b00 5300 2905 4e72 0100 0000  ..d...S.).Nr....
-00000230: e901 0000 0067 1656 e79e af03 d23c e902  .....g.V.....<..
-00000240: 0000 0029 07da 0361 6c6c da03 6c65 6eda  ...)...all..len.
-00000250: 046e 6469 6dda 0463 6c69 70da 026e 70da  .ndim..clip..np.
-00000260: 036c 6f67 da04 6d65 616e 2905 da06 795f  .log..mean)...y_
-00000270: 7472 7565 da06 795f 7072 6564 da03 6570  true..y_pred..ep
-00000280: 735a 026c 30da 026c 31a9 0072 1800 0000  sZ.l0..l1..r....
-00000290: fa46 2f68 6f6d 652f 7468 6f6d 6173 2f49  .F/home/thomas/I
-000002a0: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
-000002b0: 4361 7374 2f62 6c75 6563 6173 742f 6576  Cast/bluecast/ev
-000002c0: 616c 7561 7469 6f6e 2f65 7661 6c5f 6d65  aluation/eval_me
-000002d0: 7472 6963 732e 7079 da11 6261 6c61 6e63  trics.py..balanc
-000002e0: 6564 5f6c 6f67 5f6c 6f73 7314 0000 0073  ed_log_loss....s
-000002f0: 1000 0000 1801 1401 0e01 0401 1001 1801  ................
-00000300: 1401 1401 721a 0000 0072 1400 0000 da09  ....r....r......
-00000310: 795f 636c 6173 7365 73da 0672 6574 7572  y_classes..retur
-00000320: 6e63 0200 0000 0000 0000 0000 0000 0b00  nc..............
-00000330: 0000 0b00 0000 4300 0000 735c 0100 007a  ......C...s\...z
-00000340: 0774 007c 007c 0183 027d 0257 006e 0b04  .t.|.|...}.W.n..
-00000350: 0074 0179 1201 0001 0001 0064 017d 0259  .t.y.......d.}.Y
-00000360: 006e 0177 0074 0264 027c 029b 009d 0283  .n.w.t.d.|......
-00000370: 0101 0074 0364 027c 029b 009d 0283 0101  ...t.d.|........
-00000380: 0074 0264 0383 0101 0074 047c 007c 0183  .t.d.....t.|.|..
-00000390: 027d 0374 0264 047c 039b 009d 0283 0101  .}.t.d.|........
-000003a0: 0074 057c 007c 0164 0564 068d 037d 0474  .t.|.|.d.d...}.t
-000003b0: 0264 077c 049b 009d 0283 0101 0074 067c  .d.|.........t.|
-000003c0: 007c 0164 0864 0164 098d 047d 0574 0264  .|.d.d.d...}.t.d
-000003d0: 0a7c 059b 009d 0283 0101 0074 0364 0a7c  .|.........t.d.|
-000003e0: 059b 009d 0283 0101 0074 067c 007c 0164  .........t.|.|.d
-000003f0: 0b64 0164 098d 047d 0674 0264 0c7c 069b  .d.d...}.t.d.|..
-00000400: 009d 0283 0101 0074 0364 0c7c 069b 009d  .......t.d.|....
-00000410: 0283 0101 0074 067c 007c 0164 0564 0164  .....t.|.|.d.d.d
-00000420: 098d 047d 0774 0264 0d7c 079b 009d 0283  ...}.t.d.|......
-00000430: 0101 0074 0364 0d7c 079b 009d 0283 0101  ...t.d.|........
-00000440: 0074 077c 007c 0183 027d 0874 0264 0e7c  .t.|.|...}.t.d.|
-00000450: 089b 009d 0283 0101 0074 0364 0e7c 089b  .........t.d.|..
-00000460: 009d 0283 0101 0074 087c 007c 0183 027d  .......t.|.|...}
-00000470: 0974 027c 0983 0101 007c 027c 037c 047c  .t.|.....|.|.|.|
-00000480: 057c 067c 077c 087c 0974 097c 007c 0183  .|.|.|.|.t.|.|..
-00000490: 0264 0f9c 097d 0a7c 0a53 0029 104e 7201  .d...}.|.S.).Nr.
-000004a0: 0000 007a 1b54 6865 204d 6174 7468 6577  ...z.The Matthew
-000004b0: 2063 6f72 7265 6c61 7469 6f6e 2069 7320   correlation is 
-000004c0: 7a13 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  z.--------------
-000004d0: 2d2d 2d2d 2d7a 1054 6865 2061 6363 7572  -----z.The accur
-000004e0: 6163 7920 6973 20da 0877 6569 6768 7465  acy is ..weighte
-000004f0: 6429 01da 0761 7665 7261 6765 7a0e 5468  d)...averagez.Th
-00000500: 6520 7265 6361 6c6c 2069 7320 da05 6d61  e recall is ..ma
-00000510: 6372 6f29 0272 1e00 0000 da0d 7a65 726f  cro).r......zero
-00000520: 5f64 6976 6973 696f 6e7a 1654 6865 206d  _divisionz.The m
-00000530: 6163 726f 2046 3120 7363 6f72 6520 6973  acro F1 score is
-00000540: 20da 056d 6963 726f 7a16 5468 6520 6d69   ..microz.The mi
-00000550: 6372 6f20 4631 2073 636f 7265 2069 7320  cro F1 score is 
-00000560: 7a19 5468 6520 7765 6967 6874 6564 2046  z.The weighted F
-00000570: 3120 7363 6f72 6520 6973 207a 1854 6865  1 score is z.The
-00000580: 2062 616c 616e 6365 6420 6c6f 676c 6f73   balanced loglos
-00000590: 7320 6973 2029 09da 086d 6174 7468 6577  s is )...matthew
-000005a0: 73da 0861 6363 7572 6163 79da 0672 6563  s..accuracy..rec
-000005b0: 616c 6cda 0e66 315f 7363 6f72 655f 6d61  all..f1_score_ma
-000005c0: 6372 6fda 0e66 315f 7363 6f72 655f 6d69  cro..f1_score_mi
-000005d0: 6372 6fda 1166 315f 7363 6f72 655f 7765  cro..f1_score_we
-000005e0: 6967 6874 6564 5a10 6261 6c61 6e63 6564  ightedZ.balanced
-000005f0: 5f6c 6f67 6c6f 7373 5a14 636c 6173 7366  _loglossZ.classf
-00000600: 6963 6174 696f 6e5f 7265 706f 7274 7206  ication_reportr.
-00000610: 0000 0029 0a72 0800 0000 da09 4578 6365  ...).r......Exce
-00000620: 7074 696f 6eda 0570 7269 6e74 720a 0000  ption..printr...
-00000630: 0072 0400 0000 7209 0000 0072 0700 0000  .r....r....r....
-00000640: 721a 0000 0072 0500 0000 7206 0000 0029  r....r....r....)
-00000650: 0b72 1400 0000 721b 0000 0072 2200 0000  .r....r....r"...
-00000660: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
-00000670: 2600 0000 7227 0000 005a 0362 6c6c 5a1a  &...r'...Z.bllZ.
-00000680: 6675 6c6c 5f63 6c61 7373 6966 6963 6174  full_classificat
-00000690: 696f 6e5f 7265 706f 7274 5a11 6576 616c  ion_reportZ.eval
-000006a0: 7561 7469 6f6e 5f73 636f 7265 7372 1800  uation_scoresr..
-000006b0: 0000 7218 0000 0072 1900 0000 da0f 6576  ..r....r......ev
-000006c0: 616c 5f63 6c61 7373 6966 6965 721f 0000  al_classifier...
-000006d0: 0073 4a00 0000 0201 0e01 0c01 0801 02ff  .sJ.............
-000006e0: 0e03 0e01 0801 0a01 0e01 0e01 0e01 1001  ................
-000006f0: 0e01 0e01 1001 0e01 0e01 1001 0e01 0e01  ................
-00000700: 0a01 0e01 0e01 0a02 0801 0203 0201 0201  ................
-00000710: 0201 0201 0201 0201 0201 0801 06f7 040b  ................
-00000720: 722a 0000 0029 13da 075f 5f64 6f63 5f5f  r*...)...__doc__
-00000730: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000740: 0000 da05 6e75 6d70 7972 1100 0000 5a0f  ....numpyr....Z.
-00000750: 736b 6c65 6172 6e2e 6d65 7472 6963 7372  sklearn.metricsr
-00000760: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000770: 0000 0072 0800 0000 7209 0000 00da 2462  ...r....r.....$b
-00000780: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
-00000790: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
-000007a0: 696c 7372 0a00 0000 721a 0000 00da 076e  ilsr....r......n
-000007b0: 6461 7272 6179 da03 7374 7272 2a00 0000  darray..strr*...
-000007c0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-000007d0: 1900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000007e0: 0000 730e 0000 0004 0010 0408 0220 010c  ..s.......... ..
-000007f0: 0908 0326 0b                             ...&.
+00000080: 6505 6a10 6409 6505 6a10 640a 6505 6a10  e.j.d.e.j.d.e.j.
+00000090: 640b 6503 6511 6502 6602 1900 6608 640c  d.e.e.e.f...f.d.
+000000a0: 640d 8404 5a12 6403 5300 290e 7a51 4d6f  d...Z.d.S.).zQMo
+000000b0: 6475 6c65 2066 6f72 2065 7661 6c75 6174  dule for evaluat
+000000c0: 696f 6e20 6d65 7472 6963 732e 0a0a 5468  ion metrics...Th
+000000d0: 6973 2069 7320 6361 6c6c 6564 2061 7320  is is called as 
+000000e0: 7061 7274 206f 6620 7468 6520 6669 745f  part of the fit_
+000000f0: 6576 616c 2066 756e 6374 696f 6e2e 0ae9  eval function...
+00000100: 0000 0000 2902 da03 416e 79da 0444 6963  ....)...Any..Dic
+00000110: 744e 2906 da0e 6163 6375 7261 6379 5f73  tN)...accuracy_s
+00000120: 636f 7265 da15 636c 6173 7369 6669 6361  core..classifica
+00000130: 7469 6f6e 5f72 6570 6f72 74da 1063 6f6e  tion_report..con
+00000140: 6675 7369 6f6e 5f6d 6174 7269 78da 0866  fusion_matrix..f
+00000150: 315f 7363 6f72 65da 116d 6174 7468 6577  1_score..matthew
+00000160: 735f 636f 7272 636f 6566 da0c 7265 6361  s_corrcoef..reca
+00000170: 6c6c 5f73 636f 7265 2901 da06 6c6f 6767  ll_score)...logg
+00000180: 6572 6302 0000 0000 0000 0000 0000 0005  erc.............
+00000190: 0000 0006 0000 0043 0000 0073 8e00 0000  .......C...s....
+000001a0: 7c00 6401 6b02 7c00 6402 6b02 4200 a000  |.d.k.|.d.k.B...
+000001b0: a100 730c 4a00 8201 7401 7c00 8301 7401  ..s.J...t.|...t.
+000001c0: 7c01 8301 6b02 7316 4a00 8201 7c01 6a02  |...k.s.J...|.j.
+000001d0: 6402 6b02 731d 4a00 8201 6403 7d02 7c01  d.k.s.J...d.}.|.
+000001e0: a003 7c02 6402 7c02 1800 a102 7d01 7404  ..|.d.|.....}.t.
+000001f0: a005 6402 7c01 7c00 6401 6b02 1900 1800  ..d.|.|.d.k.....
+00000200: a101 0b00 7d03 7404 a005 7c01 7c00 6401  ....}.t...|.|.d.
+00000210: 6b03 1900 a101 0b00 7d04 7c03 a006 a100  k.......}.|.....
+00000220: 7c04 a006 a100 1700 6404 1b00 5300 2905  |.......d...S.).
+00000230: 4e72 0100 0000 e901 0000 0067 1656 e79e  Nr.........g.V..
+00000240: af03 d23c e902 0000 0029 07da 0361 6c6c  ...<.....)...all
+00000250: da03 6c65 6eda 046e 6469 6dda 0463 6c69  ..len..ndim..cli
+00000260: 70da 026e 70da 036c 6f67 da04 6d65 616e  p..np..log..mean
+00000270: 2905 da06 795f 7472 7565 da06 795f 7072  )...y_true..y_pr
+00000280: 6564 da03 6570 735a 026c 30da 026c 31a9  ed..epsZ.l0..l1.
+00000290: 0072 1800 0000 fa46 2f68 6f6d 652f 7468  .r.....F/home/th
+000002a0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
+000002b0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
+000002c0: 6173 742f 6576 616c 7561 7469 6f6e 2f65  ast/evaluation/e
+000002d0: 7661 6c5f 6d65 7472 6963 732e 7079 da11  val_metrics.py..
+000002e0: 6261 6c61 6e63 6564 5f6c 6f67 5f6c 6f73  balanced_log_los
+000002f0: 7314 0000 0073 1000 0000 1801 1401 0e01  s....s..........
+00000300: 0401 1001 1801 1401 1401 721a 0000 0072  ..........r....r
+00000310: 1400 0000 da07 795f 7072 6f62 73da 0979  ......y_probs..y
+00000320: 5f63 6c61 7373 6573 da06 7265 7475 726e  _classes..return
+00000330: 6303 0000 0000 0000 0000 0000 000c 0000  c...............
+00000340: 000b 0000 0043 0000 0073 0e01 0000 7a07  .....C...s....z.
+00000350: 7400 7c00 7c02 8302 7d03 5700 6e0b 0400  t.|.|...}.W.n...
+00000360: 7401 7912 0100 0100 0100 6401 7d03 5900  t.y.......d.}.Y.
+00000370: 6e01 7700 7402 6402 7c03 9b00 9d02 8301  n.w.t.d.|.......
+00000380: 0100 7403 7c00 7c02 8302 7d04 7402 6403  ..t.|.|...}.t.d.
+00000390: 7c04 9b00 9d02 8301 0100 7404 7c00 7c02  |.........t.|.|.
+000003a0: 6404 6405 8d03 7d05 7402 6406 7c05 9b00  d.d...}.t.d.|...
+000003b0: 9d02 8301 0100 7405 7c00 7c02 6407 6401  ......t.|.|.d.d.
+000003c0: 6408 8d04 7d06 7402 6409 7c06 9b00 9d02  d...}.t.d.|.....
+000003d0: 8301 0100 7405 7c00 7c02 640a 6401 6408  ....t.|.|.d.d.d.
+000003e0: 8d04 7d07 7402 640b 7c07 9b00 9d02 8301  ..}.t.d.|.......
+000003f0: 0100 7405 7c00 7c02 6404 6401 6408 8d04  ..t.|.|.d.d.d...
+00000400: 7d08 7402 640c 7c08 9b00 9d02 8301 0100  }.t.d.|.........
+00000410: 7406 7c00 7c01 8302 7d09 7402 640d 7c09  t.|.|...}.t.d.|.
+00000420: 9b00 9d02 8301 0100 7407 7c00 7c02 8302  ........t.|.|...
+00000430: 7d0a 7402 7c0a 8301 0100 7c03 7c04 7c05  }.t.|.....|.|.|.
+00000440: 7c06 7c07 7c08 7c09 7c0a 7408 7c00 7c02  |.|.|.|.|.t.|.|.
+00000450: 8302 640e 9c09 7d0b 7c0b 5300 290f 4e72  ..d...}.|.S.).Nr
+00000460: 0100 0000 7a1b 5468 6520 4d61 7474 6865  ....z.The Matthe
+00000470: 7720 636f 7272 656c 6174 696f 6e20 6973  w correlation is
+00000480: 207a 1054 6865 2061 6363 7572 6163 7920   z.The accuracy 
+00000490: 6973 20da 0877 6569 6768 7465 6429 01da  is ..weighted)..
+000004a0: 0761 7665 7261 6765 7a0e 5468 6520 7265  .averagez.The re
+000004b0: 6361 6c6c 2069 7320 da05 6d61 6372 6f29  call is ..macro)
+000004c0: 0272 1f00 0000 da0d 7a65 726f 5f64 6976  .r......zero_div
+000004d0: 6973 696f 6e7a 1654 6865 206d 6163 726f  isionz.The macro
+000004e0: 2046 3120 7363 6f72 6520 6973 20da 056d   F1 score is ..m
+000004f0: 6963 726f 7a16 5468 6520 6d69 6372 6f20  icroz.The micro 
+00000500: 4631 2073 636f 7265 2069 7320 7a19 5468  F1 score is z.Th
+00000510: 6520 7765 6967 6874 6564 2046 3120 7363  e weighted F1 sc
+00000520: 6f72 6520 6973 207a 1854 6865 2062 616c  ore is z.The bal
+00000530: 616e 6365 6420 6c6f 676c 6f73 7320 6973  anced logloss is
+00000540: 2029 09da 086d 6174 7468 6577 73da 0861   )...matthews..a
+00000550: 6363 7572 6163 79da 0672 6563 616c 6cda  ccuracy..recall.
+00000560: 0e66 315f 7363 6f72 655f 6d61 6372 6fda  .f1_score_macro.
+00000570: 0e66 315f 7363 6f72 655f 6d69 6372 6fda  .f1_score_micro.
+00000580: 1166 315f 7363 6f72 655f 7765 6967 6874  .f1_score_weight
+00000590: 6564 5a10 6261 6c61 6e63 6564 5f6c 6f67  edZ.balanced_log
+000005a0: 6c6f 7373 5a14 636c 6173 7366 6963 6174  lossZ.classficat
+000005b0: 696f 6e5f 7265 706f 7274 7206 0000 0029  ion_reportr....)
+000005c0: 0972 0800 0000 da09 4578 6365 7074 696f  .r......Exceptio
+000005d0: 6e72 0a00 0000 7204 0000 0072 0900 0000  nr....r....r....
+000005e0: 7207 0000 0072 1a00 0000 7205 0000 0072  r....r....r....r
+000005f0: 0600 0000 290c 7214 0000 0072 1b00 0000  ....).r....r....
+00000600: 721c 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
+00000610: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
+00000620: 0000 005a 0362 6c6c 5a1a 6675 6c6c 5f63  ...Z.bllZ.full_c
+00000630: 6c61 7373 6966 6963 6174 696f 6e5f 7265  lassification_re
+00000640: 706f 7274 5a11 6576 616c 7561 7469 6f6e  portZ.evaluation
+00000650: 5f73 636f 7265 7372 1800 0000 7218 0000  _scoresr....r...
+00000660: 0072 1900 0000 da0f 6576 616c 5f63 6c61  .r......eval_cla
+00000670: 7373 6966 6965 721f 0000 0073 3e00 0000  ssifier....s>...
+00000680: 0203 0e01 0c01 0801 02ff 0e03 0a01 0e01  ................
+00000690: 0e01 0e01 1001 0e01 1001 0e01 1001 0e01  ................
+000006a0: 0a01 0e01 0a02 0801 0203 0201 0201 0201  ................
+000006b0: 0201 0201 0201 0201 0801 06f7 040b 722a  ..............r*
+000006c0: 0000 0029 13da 075f 5f64 6f63 5f5f da06  ...)...__doc__..
+000006d0: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
+000006e0: da05 6e75 6d70 7972 1100 0000 da0f 736b  ..numpyr......sk
+000006f0: 6c65 6172 6e2e 6d65 7472 6963 7372 0400  learn.metricsr..
+00000700: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000710: 0072 0800 0000 7209 0000 00da 2462 6c75  .r....r.....$blu
+00000720: 6563 6173 742e 6765 6e65 7261 6c5f 7574  ecast.general_ut
+00000730: 696c 732e 6765 6e65 7261 6c5f 7574 696c  ils.general_util
+00000740: 7372 0a00 0000 721a 0000 00da 076e 6461  sr....r......nda
+00000750: 7272 6179 da03 7374 7272 2a00 0000 7218  rray..strr*...r.
+00000760: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000770: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000780: 731e 0000 0004 0010 0408 0220 010c 0908  s.......... ....
+00000790: 0302 0b04 0102 ff04 0102 ff04 0102 ff0a  ................
+000007a0: 020e fe                                  ...
```

### Comparing `bluecast-0.4.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc` & `bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/evaluation/eval_metrics.py` & `bluecast-0.5/bluecast/evaluation/eval_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,42 +24,38 @@
     eps = 1e-15
     y_pred = y_pred.clip(eps, 1 - eps)
     l0 = -np.log(1 - y_pred[y_true == 0])
     l1 = -np.log(y_pred[y_true != 0])
     return (l0.mean() + l1.mean()) / 2
 
 
-def eval_classifier(y_true: np.ndarray, y_classes: np.ndarray) -> Dict[str, Any]:
+def eval_classifier(
+    y_true: np.ndarray, y_probs: np.ndarray, y_classes: np.ndarray
+) -> Dict[str, Any]:
     try:
         matthews = matthews_corrcoef(y_true, y_classes)
     except Exception:
         matthews = 0
 
-    print(f"The Matthew correlation is {matthews}")
     logger(f"The Matthew correlation is {matthews}")
-    print("-------------------")
     accuracy = accuracy_score(y_true, y_classes)
-    print(f"The accuracy is {accuracy}")
+    logger(f"The accuracy is {accuracy}")
     recall = recall_score(y_true, y_classes, average="weighted")
-    print(f"The recall is {recall}")
+    logger(f"The recall is {recall}")
     f1_score_macro = f1_score(y_true, y_classes, average="macro", zero_division=0)
-    print(f"The macro F1 score is {f1_score_macro}")
     logger(f"The macro F1 score is {f1_score_macro}")
     f1_score_micro = f1_score(y_true, y_classes, average="micro", zero_division=0)
-    print(f"The micro F1 score is {f1_score_micro}")
     logger(f"The micro F1 score is {f1_score_micro}")
     f1_score_weighted = f1_score(y_true, y_classes, average="weighted", zero_division=0)
-    print(f"The weighted F1 score is {f1_score_weighted}")
     logger(f"The weighted F1 score is {f1_score_weighted}")
-    bll = balanced_log_loss(y_true, y_classes)
-    print(f"The balanced logloss is {bll}")
+    bll = balanced_log_loss(y_true, y_probs)
     logger(f"The balanced logloss is {bll}")
 
     full_classification_report = classification_report(y_true, y_classes)
-    print(full_classification_report)
+    logger(full_classification_report)
 
     evaluation_scores = {
         "matthews": matthews,
         "accuracy": accuracy,
         "recall": recall,
         "f1_score_macro": f1_score_macro,
         "f1_score_micro": f1_score_micro,
```

### Comparing `bluecast-0.4.2/bluecast/evaluation/shap_values.py` & `bluecast-0.5/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/general_utils/general_utils.py` & `bluecast-0.5/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 14:22:20 2023 UTC, .py size: 13523 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9caa 9564 d334 0000  o..........d.4..
+00000000: 6f0d 0d0a 0000 0000 b9d1 9764 d334 0000  o..........d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/base_classes.py` & `bluecast-0.5/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/ml_modelling/xgboost.py` & `bluecast-0.5/bluecast/ml_modelling/xgboost.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 13:12:42 2023 UTC, .py size: 1354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,140 @@
-00000000: 6f0d 0d0a 0000 0000 4a9a 9564 4a05 0000  o.......J..dJ...
+00000000: 6f0d 0d0a 0000 0000 cad1 9764 6207 0000  o..........db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
+00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000060: 8400 6406 8302 5a07 6402 5300 2907 e900  ..d...Z.d.S.)...
-00000070: 0000 0029 01da 0864 6174 6574 696d 654e  ...)...datetimeN
-00000080: 2901 da16 4665 6174 7572 6553 656c 6563  )...FeatureSelec
-00000090: 7469 6f6e 436f 6e66 6967 2901 da06 6c6f  tionConfig)...lo
-000000a0: 6767 6572 6300 0000 0000 0000 0000 0000  ggerc...........
-000000b0: 0000 0000 0006 0000 0040 0000 0073 5200  .........@...sR.
-000000c0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000000d0: 6504 6a05 6602 6403 6404 8404 5a06 6405  e.j.f.d.d...Z.d.
-000000e0: 6507 6a08 6406 6507 6a09 6407 6507 6a08  e.j.d.e.j.d.e.j.
-000000f0: 6606 6408 6409 8404 5a0a 6405 6507 6a08  f.d.d...Z.d.e.j.
-00000100: 6407 6507 6a08 6604 640a 640b 8404 5a0b  d.e.j.f.d.d...Z.
-00000110: 640c 5300 290d da0f 4665 6174 7572 6553  d.S.)...FeatureS
-00000120: 656c 6563 746f 7261 7901 0000 5365 6c65  electoray...Sele
-00000130: 6374 2074 6f70 2066 6561 7475 7265 7320  ct top features 
-00000140: 6261 7365 6420 6f6e 2073 656c 6563 7469  based on selecti
-00000150: 6f6e 5f73 7472 6174 6567 7920 6465 6669  on_strategy defi
-00000160: 6e65 6420 696e 2046 6561 7475 7265 5365  ned in FeatureSe
-00000170: 6c65 6374 696f 6e43 6f6e 6669 672e 0a0a  lectionConfig...
-00000180: 2020 2020 4f6e 2064 6566 6175 6c74 2063      On default c
-00000190: 726f 7373 2d76 616c 6964 6174 6564 2072  ross-validated r
-000001a0: 6563 7572 7369 7665 2066 6561 7475 7265  ecursive feature
-000001b0: 2065 6c69 6d69 6e61 7469 6f6e 2069 7320   elimination is 
-000001c0: 7573 6564 2e20 496e 2074 6865 2063 6f6e  used. In the con
-000001d0: 6669 6720 6669 6c65 2061 2064 6966 6665  fig file a diffe
-000001e0: 7265 6e74 0a20 2020 2052 4645 4356 2069  rent.    RFECV i
-000001f0: 6e73 7461 6e63 6520 6361 6e20 6265 2064  nstance can be d
-00000200: 6566 696e 6564 2028 7573 696e 6720 6120  efined (using a 
-00000210: 2064 6966 6665 7265 6e74 2063 6c61 7373   different class
-00000220: 6966 6965 722c 2073 636f 7269 6e67 2066  ifier, scoring f
-00000230: 756e 6374 696f 6e2c 2072 616e 646f 6d20  unction, random 
-00000240: 7365 6564 2065 7463 2e29 2e0a 2020 2020  seed etc.)..    
-00000250: 3a70 6172 616d 2073 656c 6563 7469 6f6e  :param selection
-00000260: 5f73 7472 6174 6567 793a 2049 6e73 7461  _strategy: Insta
-00000270: 6e63 6520 6f66 2046 6561 7475 7265 5365  nce of FeatureSe
-00000280: 6c65 6374 696f 6e43 6f6e 6669 672e 7365  lectionConfig.se
-00000290: 6c65 6374 696f 6e5f 7374 7261 7465 6779  lection_strategy
-000002a0: 0a20 2020 20da 1273 656c 6563 7469 6f6e  .    ..selection
-000002b0: 5f73 7472 6174 6567 7963 0200 0000 0000  _strategyc......
-000002c0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-000002d0: 0000 7310 0000 0064 007c 005f 007c 017c  ..s....d.|._.|.|
-000002e0: 005f 0164 0053 00a9 014e 2902 da11 7365  ._.d.S...N)...se
-000002f0: 6c65 6374 6564 5f66 6561 7475 7265 7372  lected_featuresr
-00000300: 0600 0000 2902 da04 7365 6c66 7206 0000  ....)...selfr...
-00000310: 00a9 0072 0a00 0000 fa4e 2f68 6f6d 652f  ...r.....N/home/
-00000320: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
-00000330: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
-00000340: 6563 6173 742f 7072 6570 726f 6365 7373  ecast/preprocess
-00000350: 696e 672f 6665 6174 7572 655f 7365 6c65  ing/feature_sele
-00000360: 6374 696f 6e2e 7079 da08 5f5f 696e 6974  ction.py..__init
-00000370: 5f5f 1100 0000 7304 0000 0006 010a 017a  __....s........z
-00000380: 1846 6561 7475 7265 5365 6c65 6374 6f72  .FeatureSelector
-00000390: 2e5f 5f69 6e69 745f 5fda 0264 66da 0674  .__init__..df..t
-000003a0: 6172 6765 74da 0672 6574 7572 6e63 0300  arget..returnc..
-000003b0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-000003c0: 0000 4300 0000 735c 0000 0074 0074 01a0  ..C...s\...t.t..
-000003d0: 02a1 009b 0064 019d 0283 0101 007c 006a  .....d.......|.j
-000003e0: 03a0 047c 017c 02a1 0201 007c 006a 036a  ...|.|.....|.j.j
-000003f0: 057c 005f 067c 016a 0764 0064 0085 027c  .|._.|.j.d.d...|
-00000400: 006a 0666 0219 007d 0174 0074 01a0 02a1  .j.f...}.t.t....
-00000410: 009b 0064 027c 016a 089b 0064 039d 0483  ...d.|.j...d....
-00000420: 0101 007c 0153 0029 044e 7a3f 3a20 5374  ...|.S.).Nz?: St
-00000430: 6172 7420 6665 6174 7572 6520 7365 6c65  art feature sele
-00000440: 6374 696f 6e20 6173 2064 6566 696e 6564  ction as defined
-00000450: 2069 6e20 4665 6174 7572 6553 656c 6563   in FeatureSelec
-00000460: 7469 6f6e 436f 6e66 6967 2e7a 183a 2053  tionConfig.z.: S
-00000470: 656c 6563 7465 6420 6665 6174 7572 6573  elected features
-00000480: 2061 7265 20da 012e 2909 7204 0000 0072   are ...).r....r
-00000490: 0200 0000 da06 7574 636e 6f77 7206 0000  ......utcnowr...
-000004a0: 00da 0366 6974 da08 7375 7070 6f72 745f  ...fit..support_
-000004b0: 7208 0000 00da 036c 6f63 da07 636f 6c75  r......loc..colu
-000004c0: 6d6e 7329 0372 0900 0000 720d 0000 0072  mns).r....r....r
-000004d0: 0e00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-000004e0: 0000 00da 0d66 6974 5f74 7261 6e73 666f  .....fit_transfo
-000004f0: 726d 1500 0000 7310 0000 0002 010c 0104  rm....s.........
-00000500: ff0e 030a 0114 011a 0104 017a 1d46 6561  ...........z.Fea
-00000510: 7475 7265 5365 6c65 6374 6f72 2e66 6974  tureSelector.fit
-00000520: 5f74 7261 6e73 666f 726d 6302 0000 0000  _transformc.....
-00000530: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000540: 0000 0073 1800 0000 7c01 6a00 6400 6400  ...s....|.j.d.d.
-00000550: 8502 7c00 6a01 6602 1900 7d01 7c01 5300  ..|.j.f...}.|.S.
-00000560: 7207 0000 0029 0272 1400 0000 7208 0000  r....).r....r...
-00000570: 0029 0272 0900 0000 720d 0000 0072 0a00  .).r....r....r..
-00000580: 0000 720a 0000 0072 0b00 0000 da09 7472  ..r....r......tr
-00000590: 616e 7366 6f72 6d1f 0000 0073 0400 0000  ansform....s....
-000005a0: 1401 0401 7a19 4665 6174 7572 6553 656c  ....z.FeatureSel
-000005b0: 6563 746f 722e 7472 616e 7366 6f72 6d4e  ector.transformN
-000005c0: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000005d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000005e0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000005f0: 0300 0000 7206 0000 0072 0c00 0000 da02  ....r....r......
-00000600: 7064 da09 4461 7461 4672 616d 65da 0653  pd..DataFrame..S
-00000610: 6572 6965 7372 1600 0000 7217 0000 0072  eriesr....r....r
-00000620: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-00000630: 0000 0072 0500 0000 0900 0000 730a 0000  ...r........s...
-00000640: 0008 0004 0110 071c 041a 0a72 0500 0000  ...........r....
-00000650: 2908 7202 0000 00da 0670 616e 6461 7372  ).r......pandasr
-00000660: 1c00 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
-00000670: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
-00000680: 6f6e 6669 6772 0300 0000 da24 626c 7565  onfigr.....$blue
-00000690: 6361 7374 2e67 656e 6572 616c 5f75 7469  cast.general_uti
-000006a0: 6c73 2e67 656e 6572 616c 5f75 7469 6c73  ls.general_utils
-000006b0: 7204 0000 0072 0500 0000 720a 0000 0072  r....r....r....r
-000006c0: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-000006d0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-000006e0: 000c 0008 020c 020c 0112 03              ...........
+00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
+00000050: 5a05 6400 6403 6c06 5a07 6400 6404 6c08  Z.d.d.l.Z.d.d.l.
+00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6407 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6408 6c11 6d12 5a12 0100 4700 6409 640a  d.l.m.Z...G.d.d.
+000000a0: 8400 640a 6512 8303 5a13 6403 5300 290b  ..d.e...Z.d.S.).
+000000b0: e900 0000 0029 01da 0864 6174 6574 696d  .....)...datetim
+000000c0: 6529 02da 084f 7074 696f 6e61 6cda 0554  e)...Optional..T
+000000d0: 7570 6c65 4e29 01da 0552 4645 4356 2902  upleN)...RFECV).
+000000e0: da0b 6d61 6b65 5f73 636f 7265 72da 116d  ..make_scorer..m
+000000f0: 6174 7468 6577 735f 636f 7272 636f 6566  atthews_corrcoef
+00000100: 2901 da0f 5374 7261 7469 6669 6564 4b46  )...StratifiedKF
+00000110: 6f6c 6429 01da 066c 6f67 6765 7229 01da  old)...logger)..
+00000120: 1343 7573 746f 6d50 7265 7072 6f63 6573  .CustomPreproces
+00000130: 7369 6e67 6300 0000 0000 0000 0000 0000  singc...........
+00000140: 0000 0000 000c 0000 0000 0000 0073 8e00  .............s..
+00000150: 0000 6500 5a01 6400 5a02 6401 5a03 6412  ..e.Z.d.Z.d.Z.d.
+00000160: 6404 6504 6405 6504 6604 8700 6601 6406  d.e.d.e.f...f.d.
+00000170: 6407 840d 5a05 6408 6506 6a07 6409 6506  d...Z.d.e.j.d.e.
+00000180: 6a08 640a 6509 6506 6a07 650a 6506 6a08  j.d.e.e.j.e.e.j.
+00000190: 1900 6602 1900 6606 640b 640c 8404 5a0b  ..f...f.d.d...Z.
+000001a0: 090d 090e 6413 6408 6506 6a07 6409 650a  ....d.d.e.j.d.e.
+000001b0: 6506 6a08 1900 640f 650c 640a 6509 6506  e.j...d.e.d.e.e.
+000001c0: 6a07 650a 6506 6a08 1900 6602 1900 6608  j.e.e.j...f...f.
+000001d0: 6410 6411 8405 5a0d 8700 0400 5a0e 5300  d.d...Z.....Z.S.
+000001e0: 2914 da0d 5246 4543 5653 656c 6563 746f  )...RFECVSelecto
+000001f0: 727a 9e53 656c 6563 7420 746f 7020 6665  rz.Select top fe
+00000200: 6174 7572 6573 2062 6173 6564 206f 6e20  atures based on 
+00000210: 7365 6c65 6374 696f 6e5f 7374 7261 7465  selection_strate
+00000220: 6779 2064 6566 696e 6564 2069 6e20 4665  gy defined in Fe
+00000230: 6174 7572 6553 656c 6563 7469 6f6e 436f  atureSelectionCo
+00000240: 6e66 6967 2e0a 0a20 2020 204f 6e20 6465  nfig...    On de
+00000250: 6661 756c 7420 6372 6f73 732d 7661 6c69  fault cross-vali
+00000260: 6461 7465 6420 7265 6375 7273 6976 6520  dated recursive 
+00000270: 6665 6174 7572 6520 656c 696d 696e 6174  feature eliminat
+00000280: 696f 6e20 6973 2075 7365 642e 0a20 2020  ion is used..   
+00000290: 2072 0100 0000 e905 0000 00da 0c72 616e   r...........ran
+000002a0: 646f 6d5f 7374 6174 65da 166d 696e 5f66  dom_state..min_f
+000002b0: 6561 7475 7265 735f 746f 5f73 656c 6563  eatures_to_selec
+000002c0: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
+000002d0: 0000 0800 0000 0300 0000 7342 0000 0074  ..........sB...t
+000002e0: 0083 00a0 01a1 0001 0064 007c 005f 027c  .........d.|._.|
+000002f0: 017c 005f 0374 0474 05a0 06a1 0064 0174  .|._.t.t.....d.t
+00000300: 0764 027c 0164 0364 048d 037c 0274 0874  .d.|.d.d...|.t.t
+00000310: 0983 0164 0564 068d 067c 005f 0a64 0053  ...d.d...|._.d.S
+00000320: 0029 074e e901 0000 0072 0c00 0000 5429  .).N.....r....T)
+00000330: 0272 0d00 0000 da07 7368 7566 666c 65e9  .r......shuffle.
+00000340: 0200 0000 2906 da09 6573 7469 6d61 746f  ....)...estimato
+00000350: 72da 0473 7465 70da 0263 7672 0e00 0000  r..step..cvr....
+00000360: da07 7363 6f72 696e 67da 066e 5f6a 6f62  ..scoring..n_job
+00000370: 7329 0bda 0573 7570 6572 da08 5f5f 696e  s)...super..__in
+00000380: 6974 5f5f da11 7365 6c65 6374 6564 5f66  it__..selected_f
+00000390: 6561 7475 7265 7372 0d00 0000 7205 0000  eaturesr....r...
+000003a0: 00da 0378 6762 da0d 5847 4243 6c61 7373  ...xgb..XGBClass
+000003b0: 6966 6965 7272 0800 0000 7206 0000 0072  ifierr....r....r
+000003c0: 0700 0000 da12 7365 6c65 6374 696f 6e5f  ......selection_
+000003d0: 7374 7261 7465 6779 2903 da04 7365 6c66  strategy)...self
+000003e0: 720d 0000 0072 0e00 0000 a901 da09 5f5f  r....r........__
+000003f0: 636c 6173 735f 5fa9 00fa 4e2f 686f 6d65  class__...N/home
+00000400: 2f74 686f 6d61 732f 4964 6561 5072 6f6a  /thomas/IdeaProj
+00000410: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
+00000420: 7565 6361 7374 2f70 7265 7072 6f63 6573  uecast/preproces
+00000430: 7369 6e67 2f66 6561 7475 7265 5f73 656c  sing/feature_sel
+00000440: 6563 7469 6f6e 2e70 7972 1800 0000 1400  ection.pyr......
+00000450: 0000 7316 0000 000a 0106 0106 0102 0106  ..s.............
+00000460: 0102 010c 0102 0106 0102 010c fa7a 1652  .............z.R
+00000470: 4645 4356 5365 6c65 6374 6f72 2e5f 5f69  FECVSelector.__i
+00000480: 6e69 745f 5fda 0264 66da 0674 6172 6765  nit__..df..targe
+00000490: 74da 0672 6574 7572 6e63 0300 0000 0000  t..returnc......
+000004a0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
+000004b0: 0000 7360 0000 0074 0074 01a0 02a1 009b  ..s`...t.t......
+000004c0: 0064 019d 0283 0101 007c 006a 03a0 047c  .d.......|.j...|
+000004d0: 017c 02a1 0201 007c 006a 036a 057c 005f  .|.....|.j.j.|._
+000004e0: 067c 016a 0764 0064 0085 027c 006a 0666  .|.j.d.d...|.j.f
+000004f0: 0219 007d 0174 0074 01a0 02a1 009b 0064  ...}.t.t.......d
+00000500: 027c 016a 089b 0064 039d 0483 0101 007c  .|.j...d.......|
+00000510: 017c 0266 0253 0029 044e 7a3f 3a20 5374  .|.f.S.).Nz?: St
+00000520: 6172 7420 6665 6174 7572 6520 7365 6c65  art feature sele
+00000530: 6374 696f 6e20 6173 2064 6566 696e 6564  ction as defined
+00000540: 2069 6e20 4665 6174 7572 6553 656c 6563   in FeatureSelec
+00000550: 7469 6f6e 436f 6e66 6967 2e7a 183a 2053  tionConfig.z.: S
+00000560: 656c 6563 7465 6420 6665 6174 7572 6573  elected features
+00000570: 2061 7265 20da 012e 2909 7209 0000 0072   are ...).r....r
+00000580: 0200 0000 da06 7574 636e 6f77 721c 0000  ......utcnowr...
+00000590: 00da 0366 6974 da08 7375 7070 6f72 745f  ...fit..support_
+000005a0: 7219 0000 00da 036c 6f63 da07 636f 6c75  r......loc..colu
+000005b0: 6d6e 7329 0372 1d00 0000 7222 0000 0072  mns).r....r"...r
+000005c0: 2300 0000 7220 0000 0072 2000 0000 7221  #...r ...r ...r!
+000005d0: 0000 00da 0d66 6974 5f74 7261 6e73 666f  .....fit_transfo
+000005e0: 726d 2100 0000 7310 0000 0002 030c 0104  rm!...s.........
+000005f0: ff0e 030a 0114 011a 0108 017a 1b52 4645  ...........z.RFE
+00000600: 4356 5365 6c65 6374 6f72 2e66 6974 5f74  CVSelector.fit_t
+00000610: 7261 6e73 666f 726d 4e46 da0e 7072 6564  ransformNF..pred
+00000620: 6963 746f 6e5f 6d6f 6465 6304 0000 0000  icton_modec.....
+00000630: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00000640: 0000 0073 1c00 0000 7c01 6a00 6400 6400  ...s....|.j.d.d.
+00000650: 8502 7c00 6a01 6602 1900 7d01 7c01 7c02  ..|.j.f...}.|.|.
+00000660: 6602 5300 2901 4e29 0272 2900 0000 7219  f.S.).N).r)...r.
+00000670: 0000 0029 0472 1d00 0000 7222 0000 0072  ...).r....r"...r
+00000680: 2300 0000 722c 0000 0072 2000 0000 7220  #...r,...r ...r 
+00000690: 0000 0072 2100 0000 da09 7472 616e 7366  ...r!.....transf
+000006a0: 6f72 6d2d 0000 0073 0400 0000 1406 0801  orm-...s........
+000006b0: 7a17 5246 4543 5653 656c 6563 746f 722e  z.RFECVSelector.
+000006c0: 7472 616e 7366 6f72 6d29 0272 0100 0000  transform).r....
+000006d0: 720c 0000 0029 024e 4629 0fda 085f 5f6e  r....).NF)...__n
+000006e0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000006f0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000700: 075f 5f64 6f63 5f5f da03 696e 7472 1800  .__doc__..intr..
+00000710: 0000 da02 7064 da09 4461 7461 4672 616d  ....pd..DataFram
+00000720: 65da 0653 6572 6965 7372 0400 0000 7203  e..Seriesr....r.
+00000730: 0000 0072 2b00 0000 da04 626f 6f6c 722d  ...r+.....boolr-
+00000740: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00000750: 5f5f 7220 0000 0072 2000 0000 721e 0000  __r ...r ...r...
+00000760: 0072 2100 0000 720b 0000 000e 0000 0073  .r!...r........s
+00000770: 2a00 0000 0800 0401 1805 020d 0401 02ff  *...............
+00000780: 0401 02ff 1202 0afe 020f 0201 04fc 0402  ................
+00000790: 02fe 0803 02fd 0204 02fc 1205 12fb 720b  ..............r.
+000007a0: 0000 0029 1472 0200 0000 da06 7479 7069  ...).r......typi
+000007b0: 6e67 7203 0000 0072 0400 0000 da06 7061  ngr....r......pa
+000007c0: 6e64 6173 7233 0000 00da 0778 6762 6f6f  ndasr3.....xgboo
+000007d0: 7374 721a 0000 00da 1973 6b6c 6561 726e  str......sklearn
+000007e0: 2e66 6561 7475 7265 5f73 656c 6563 7469  .feature_selecti
+000007f0: 6f6e 7205 0000 00da 0f73 6b6c 6561 726e  onr......sklearn
+00000800: 2e6d 6574 7269 6373 7206 0000 0072 0700  .metricsr....r..
+00000810: 0000 da17 736b 6c65 6172 6e2e 6d6f 6465  ....sklearn.mode
+00000820: 6c5f 7365 6c65 6374 696f 6e72 0800 0000  l_selectionr....
+00000830: da24 626c 7565 6361 7374 2e67 656e 6572  .$bluecast.gener
+00000840: 616c 5f75 7469 6c73 2e67 656e 6572 616c  al_utils.general
+00000850: 5f75 7469 6c73 7209 0000 00da 1d62 6c75  _utilsr......blu
+00000860: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
+00000870: 696e 672e 6375 7374 6f6d 720a 0000 0072  ing.customr....r
+00000880: 0b00 0000 7220 0000 0072 2000 0000 7220  ....r ...r ...r 
+00000890: 0000 0072 2100 0000 da08 3c6d 6f64 756c  ...r!.....<modul
+000008a0: 653e 0100 0000 7314 0000 000c 0010 0108  e>....s.........
+000008b0: 0208 010c 0110 010c 010c 020c 0114 03    ...............
```

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/custom.py` & `bluecast-0.5/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/datetime_features.py` & `bluecast-0.5/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.5/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/feature_types.py` & `bluecast-0.5/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.5/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/schema_checks.py` & `bluecast-0.5/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/target_encoding.py` & `bluecast-0.5/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/preprocessing/train_test_split.py` & `bluecast-0.5/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 24 16:22:59 2023 UTC, .py size: 5760 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,481 +1,546 @@
-00000000: 6f0d 0d0a 0000 0000 6318 9764 8016 0000  o.......c..d....
+00000000: 6f0d 0d0a 0000 0000 cad1 9764 cc19 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
 00000060: 6400 6401 6c0b 5a0c 6400 6401 6c0d 5a0d  d.d.l.Z.d.d.l.Z.
 00000070: 6400 6401 6c0e 5a0f 6400 6403 6c10 6d11  d.d.l.Z.d.d.l.m.
 00000080: 5a11 0100 6400 6404 6c12 6d13 5a13 0100  Z...d.d.l.m.Z...
 00000090: 6400 6405 6c14 6d15 5a15 6d16 5a16 0100  d.d.l.m.Z.m.Z...
 000000a0: 6400 6406 6c17 6d18 5a18 0100 6400 6407  d.d.l.m.Z...d.d.
 000000b0: 6c19 6d1a 5a1a 0100 6400 6408 6c1b 6d1c  l.m.Z...d.d.l.m.
-000000c0: 5a1c 6d1d 5a1d 6d1e 5a1e 0100 6400 6409  Z.m.Z.m.Z...d.d.
-000000d0: 6c1f 6d20 5a20 6d21 5a21 6d22 5a22 0100  l.m Z m!Z!m"Z"..
-000000e0: 6400 640a 6c23 6d24 5a24 0100 6400 640b  d.d.l#m$Z$..d.d.
-000000f0: 6c25 6d26 5a26 0100 650d 6a27 640c 6508  l%m&Z&..e.j'd.e.
-00000100: 650c 6a28 650c 6a28 6602 1900 6602 640d  e.j(e.j(f...f.d.
-00000110: 640e 8404 8301 5a29 640f 6410 8400 5a2a  d.....Z)d.d...Z*
-00000120: 4700 6411 6412 8400 6412 6520 8303 5a2b  G.d.d...d.e ..Z+
-00000130: 6413 6414 8400 5a2c 6401 5300 2915 e900  d.d...Z,d.S.)...
-00000140: 0000 004e 2902 da08 4f70 7469 6f6e 616c  ...N)...Optional
-00000150: da05 5475 706c 6529 01da 1652 616e 646f  ..Tuple)...Rando
-00000160: 6d46 6f72 6573 7443 6c61 7373 6966 6965  mForestClassifie
-00000170: 7229 01da 0552 4645 4356 2902 da0b 6d61  r)...RFECV)...ma
-00000180: 6b65 5f73 636f 7265 72da 116d 6174 7468  ke_scorer..matth
-00000190: 6577 735f 636f 7272 636f 6566 2901 da0f  ews_corrcoef)...
-000001a0: 5374 7261 7469 6669 6564 4b46 6f6c 6429  StratifiedKFold)
-000001b0: 01da 0842 6c75 6543 6173 7429 03da 1646  ...BlueCast)...F
-000001c0: 6561 7475 7265 5365 6c65 6374 696f 6e43  eatureSelectionC
-000001d0: 6f6e 6669 67da 0e54 7261 696e 696e 6743  onfig..TrainingC
-000001e0: 6f6e 6669 67da 1758 6762 6f6f 7374 5475  onfig..XgboostTu
-000001f0: 6e65 5061 7261 6d73 436f 6e66 6967 2903  neParamsConfig).
-00000200: da10 4261 7365 436c 6173 734d 6c4d 6f64  ..BaseClassMlMod
-00000210: 656c da10 5072 6564 6963 7465 6443 6c61  el..PredictedCla
-00000220: 7373 6573 da0f 5072 6564 6963 7465 6450  sses..PredictedP
-00000230: 726f 6261 7329 01da 1343 7573 746f 6d50  robas)...CustomP
-00000240: 7265 7072 6f63 6573 7369 6e67 a901 da1a  reprocessing....
-00000250: 6372 6561 7465 5f73 796e 7468 6574 6963  create_synthetic
-00000260: 5f64 6174 6166 7261 6d65 da06 7265 7475  _dataframe..retu
-00000270: 726e 6300 0000 0000 0000 0000 0000 0002  rnc.............
-00000280: 0000 0004 0000 0043 0000 0073 2000 0000  .......C...s ...
-00000290: 7400 6401 6402 6403 8d02 7d00 7400 6401  t.d.d.d...}.t.d.
-000002a0: 6404 6403 8d02 7d01 7c00 7c01 6602 5300  d.d...}.|.|.f.S.
-000002b0: 2905 4e69 d007 0000 e914 0000 0029 01da  ).Ni.........)..
-000002c0: 0c72 616e 646f 6d5f 7374 6174 65e9 c800  .random_state...
-000002d0: 0000 7211 0000 0029 02da 0864 665f 7472  ..r....)...df_tr
-000002e0: 6169 6eda 0664 665f 7661 6ca9 0072 1900  ain..df_val..r..
-000002f0: 0000 fa3e 2f68 6f6d 652f 7468 6f6d 6173  ...>/home/thomas
-00000300: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-00000310: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-00000320: 7465 7374 732f 7465 7374 5f63 6173 742e  tests/test_cast.
-00000330: 7079 da19 7379 6e74 6865 7469 635f 7472  py..synthetic_tr
-00000340: 6169 6e5f 7465 7374 5f64 6174 611b 0000  ain_test_data...
-00000350: 0073 0600 0000 0c02 0c01 0801 721b 0000  .s..........r...
-00000360: 0063 0100 0000 0000 0000 0000 0000 1000  .c..............
-00000370: 0000 0a00 0000 4300 0000 73ba 0200 007c  ......C...s....|
-00000380: 0064 0119 007d 017c 0064 0219 007d 0274  .d...}.|.d...}.t
-00000390: 0083 007d 0364 037c 035f 0164 047c 035f  ...}.d.|._.d.|._
-000003a0: 0274 0383 007d 0464 057c 045f 0464 067c  .t...}.d.|._.d.|
-000003b0: 045f 0564 027c 045f 0647 0064 0764 0884  ._.d.|._.G.d.d..
-000003c0: 0064 0874 0783 037d 057c 0583 007d 0674  .d.t...}.|...}.t
-000003d0: 0864 0964 0a7c 047c 037c 0664 0b8d 057d  .d.d.|.|.|.d...}
-000003e0: 077c 076a 097c 0164 0a64 0c8d 0201 0074  .|.j.|.d.d.....t
-000003f0: 0a64 0d83 0101 007c 07a0 0b7c 026a 0c64  .d.....|...|.j.d
-00000400: 0a64 0264 0e8d 02a1 015c 027d 087d 0974  .d.d.....\.}.}.t
-00000410: 0a64 0f83 0101 0074 0d7c 0883 017d 0a7c  .d.....t.|...}.|
-00000420: 026a 0e7d 0b74 0d7c 0b83 017d 0c7c 0a7c  .j.}.t.|...}.|.|
-00000430: 0c6b 027d 0d7c 0d73 c874 0fa0 1064 107c  .k.}.|.s.t...d.|
-00000440: 0d66 0164 117c 0a7c 0c66 02a1 0464 1274  .f.d.|.|.f...d.t
-00000450: 11a0 12a1 0076 0073 7274 0fa0 1374 0da1  .....v.srt...t..
-00000460: 0172 7774 0fa0 1474 0da1 016e 0164 1264  .rwt...t...n.d.d
-00000470: 1374 11a0 12a1 0076 0073 8374 0fa0 137c  .t.....v.s.t...|
-00000480: 08a1 0172 8874 0fa0 147c 08a1 016e 0164  ...r.t...|...n.d
-00000490: 1374 0fa0 147c 0aa1 0164 1274 11a0 12a1  .t...|...d.t....
-000004a0: 0076 0073 9874 0fa0 1374 0da1 0172 9d74  .v.s.t...t...r.t
-000004b0: 0fa0 1474 0da1 016e 0164 1264 1474 11a0  ...t...n.d.d.t..
-000004c0: 12a1 0076 0073 a974 0fa0 137c 02a1 0172  ...v.s.t...|...r
-000004d0: ae74 0fa0 147c 02a1 016e 0164 1474 0fa0  .t...|...n.d.t..
-000004e0: 147c 0ba1 0174 0fa0 147c 0ca1 0164 159c  .|...t...|...d..
-000004f0: 0716 007d 0e64 1664 177c 0e69 0116 007d  ...}.d.d.|.i...}
-00000500: 0f74 1574 0fa0 167c 0fa1 0183 0182 0164  .t.t...|.......d
-00000510: 1804 007d 0a04 007d 0d04 007d 0b7d 0c74  ...}...}...}.}.t
-00000520: 0d7c 0983 017d 0a7c 026a 0e7d 0b74 0d7c  .|...}.|.j.}.t.|
-00000530: 0b83 017d 0c7c 0a7c 0c6b 027d 0d7c 0d90  ...}.|.|.k.}.|..
-00000540: 0173 5374 0fa0 1064 107c 0d66 0164 117c  .sSt...d.|.f.d.|
-00000550: 0a7c 0c66 02a1 0464 1274 11a0 12a1 0076  .|.f...d.t.....v
-00000560: 0073 f774 0fa0 1374 0da1 0172 fc74 0fa0  .s.t...t...r.t..
-00000570: 1474 0da1 016e 0164 1264 1974 11a0 12a1  .t...n.d.d.t....
-00000580: 0076 0090 0173 0a74 0fa0 137c 09a1 0190  .v...s.t...|....
-00000590: 0172 0f74 0fa0 147c 09a1 016e 0164 1974  .r.t...|...n.d.t
-000005a0: 0fa0 147c 0aa1 0164 1274 11a0 12a1 0076  ...|...d.t.....v
-000005b0: 0090 0173 2174 0fa0 1374 0da1 0190 0172  ...s!t...t.....r
-000005c0: 2674 0fa0 1474 0da1 016e 0164 1264 1474  &t...t...n.d.d.t
-000005d0: 11a0 12a1 0076 0090 0173 3474 0fa0 137c  .....v...s4t...|
-000005e0: 02a1 0190 0172 3974 0fa0 147c 02a1 016e  .....r9t...|...n
-000005f0: 0164 1474 0fa0 147c 0ba1 0174 0fa0 147c  .d.t...|...t...|
-00000600: 0ca1 0164 159c 0716 007d 0e64 1664 177c  ...d.....}.d.d.|
-00000610: 0e69 0116 007d 0f74 1574 0fa0 167c 0fa1  .i...}.t.t...|..
-00000620: 0183 0182 0164 1804 007d 0a04 007d 0d04  .....d...}...}..
-00000630: 007d 0b7d 0c64 1853 0029 1a7a 2254 6573  .}.}.d.S.).z"Tes
-00000640: 7420 7468 6174 2074 6573 7473 2074 6865  t that tests the
-00000650: 2042 6c75 6543 6173 7420 636c 6173 7372   BlueCast classr
-00000660: 0100 0000 e901 0000 00e9 6400 0000 e910  ..........d.....
-00000670: 0000 00e9 0a00 0000 4663 0000 0000 0000  ........Fc......
-00000680: 0000 0000 0000 0000 0000 0c00 0000 4000  ..............@.
-00000690: 0000 7380 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000006a0: 0165 036a 0464 0265 036a 0466 0464 0364  .e.j.d.e.j.f.d.d
-000006b0: 0484 045a 0564 0165 036a 0464 0565 036a  ...Z.d.e.j.d.e.j
-000006c0: 0664 0265 0765 036a 0465 036a 0666 0219  .d.e.e.j.e.j.f..
-000006d0: 0066 0664 0664 0784 045a 0809 0809 0964  .f.d.d...Z.....d
-000006e0: 0d64 0165 036a 0464 0565 0965 036a 0619  .d.e.j.d.e.e.j..
-000006f0: 0064 0a65 0a64 0265 0765 036a 0465 0965  .d.e.d.e.e.j.e.e
-00000700: 036a 0619 0066 0219 0066 0864 0b64 0c84  .j...f...f.d.d..
-00000710: 055a 0b64 0853 0029 0e7a 3d74 6573 745f  .Z.d.S.).z=test_
-00000720: 626c 7565 7072 696e 745f 7867 626f 6f73  blueprint_xgboos
-00000730: 742e 3c6c 6f63 616c 733e 2e4d 7943 7573  t.<locals>.MyCus
-00000740: 746f 6d4c 6173 744d 696c 6550 7265 7072  tomLastMilePrepr
-00000750: 6f63 6573 7369 6e67 da02 6466 7213 0000  ocessing..dfr...
-00000760: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00000770: 0000 0300 0000 5300 0000 7314 0000 007c  ......S...s....|
-00000780: 0164 011b 007d 0164 027c 0164 033c 007c  .d...}.d.|.d.<.|
-00000790: 0153 0029 044e e902 0000 00e9 0500 0000  .S.).N..........
-000007a0: 5a0a 6375 7374 6f6d 5f63 6f6c 7219 0000  Z.custom_colr...
-000007b0: 0029 02da 0473 656c 6672 2000 0000 7219  .)...selfr ...r.
-000007c0: 0000 0072 1900 0000 721a 0000 00da 0f63  ...r....r......c
-000007d0: 7573 746f 6d5f 6675 6e63 7469 6f6e 3000  ustom_function0.
-000007e0: 0000 7306 0000 0008 0108 0104 017a 4d74  ..s..........zMt
-000007f0: 6573 745f 626c 7565 7072 696e 745f 7867  est_blueprint_xg
-00000800: 626f 6f73 742e 3c6c 6f63 616c 733e 2e4d  boost.<locals>.M
-00000810: 7943 7573 746f 6d4c 6173 744d 696c 6550  yCustomLastMileP
-00000820: 7265 7072 6f63 6573 7369 6e67 2e63 7573  reprocessing.cus
-00000830: 746f 6d5f 6675 6e63 7469 6f6e da06 7461  tom_function..ta
-00000840: 7267 6574 6303 0000 0000 0000 0000 0000  rgetc...........
-00000850: 0003 0000 0003 0000 0053 0000 0073 2600  .........S...s&.
-00000860: 0000 7c00 a000 7c01 a101 7d01 7c01 a001  ..|...|...}.|...
-00000870: 6401 a101 7d01 7c02 a001 6401 a101 7d02  d...}.|...d...}.
-00000880: 7c01 7c02 6602 5300 2902 4e69 e803 0000  |.|.f.S.).Ni....
-00000890: 2902 7224 0000 00da 0468 6561 6429 0372  ).r$.....head).r
-000008a0: 2300 0000 7220 0000 0072 2500 0000 7219  #...r ...r%...r.
-000008b0: 0000 0072 1900 0000 721a 0000 00da 0d66  ...r....r......f
-000008c0: 6974 5f74 7261 6e73 666f 726d 3500 0000  it_transform5...
-000008d0: 7308 0000 000a 030a 010a 0108 017a 4b74  s............zKt
-000008e0: 6573 745f 626c 7565 7072 696e 745f 7867  est_blueprint_xg
-000008f0: 626f 6f73 742e 3c6c 6f63 616c 733e 2e4d  boost.<locals>.M
-00000900: 7943 7573 746f 6d4c 6173 744d 696c 6550  yCustomLastMileP
-00000910: 7265 7072 6f63 6573 7369 6e67 2e66 6974  reprocessing.fit
-00000920: 5f74 7261 6e73 666f 726d 4e46 da0e 7072  _transformNF..pr
-00000930: 6564 6963 746f 6e5f 6d6f 6465 6304 0000  edicton_modec...
-00000940: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000950: 0053 0000 0073 3600 0000 7c00 a000 7c01  .S...s6...|...|.
-00000960: a101 7d01 7c03 7317 7401 7c02 7402 6a03  ..}.|.s.t.|.t.j.
-00000970: 8302 7217 7c01 a004 6401 a101 7d01 7c02  ..r.|...d...}.|.
-00000980: a004 6401 a101 7d02 7c01 7c02 6602 5300  ..d...}.|.|.f.S.
-00000990: 2902 4e72 1d00 0000 2905 7224 0000 00da  ).Nr....).r$....
-000009a0: 0a69 7369 6e73 7461 6e63 65da 0270 64da  .isinstance..pd.
-000009b0: 0653 6572 6965 7372 2600 0000 2904 7223  .Seriesr&...).r#
-000009c0: 0000 0072 2000 0000 7225 0000 0072 2800  ...r ...r%...r(.
-000009d0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000009e0: 00da 0974 7261 6e73 666f 726d 3d00 0000  ...transform=...
-000009f0: 730a 0000 000a 0610 010a 010a 0108 017a  s..............z
-00000a00: 4774 6573 745f 626c 7565 7072 696e 745f  Gtest_blueprint_
-00000a10: 7867 626f 6f73 742e 3c6c 6f63 616c 733e  xgboost.<locals>
-00000a20: 2e4d 7943 7573 746f 6d4c 6173 744d 696c  .MyCustomLastMil
-00000a30: 6550 7265 7072 6f63 6573 7369 6e67 2e74  ePreprocessing.t
-00000a40: 7261 6e73 666f 726d 2902 4e46 290c da08  ransform).NF)...
-00000a50: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000a60: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000a70: 5f5f 722a 0000 00da 0944 6174 6146 7261  __r*.....DataFra
-00000a80: 6d65 7224 0000 0072 2b00 0000 7203 0000  mer$...r+...r...
-00000a90: 0072 2700 0000 7202 0000 00da 0462 6f6f  .r'...r......boo
-00000aa0: 6c72 2c00 0000 7219 0000 0072 1900 0000  lr,...r....r....
-00000ab0: 7219 0000 0072 1a00 0000 da1d 4d79 4375  r....r......MyCu
-00000ac0: 7374 6f6d 4c61 7374 4d69 6c65 5072 6570  stomLastMilePrep
-00000ad0: 726f 6365 7373 696e 672f 0000 0073 2800  rocessing/...s(.
-00000ae0: 0000 0800 1601 0205 0401 02ff 0401 02ff  ................
-00000af0: 0e02 0afe 020b 0201 04fc 0402 02fe 0803  ................
-00000b00: 02fd 0204 02fc 1205 0efb 7232 0000 00da  ..........r2....
-00000b10: 0662 696e 6172 7972 2500 0000 2905 da0d  .binaryr%...)...
-00000b20: 636c 6173 735f 7072 6f62 6c65 6dda 0d74  class_problem..t
-00000b30: 6172 6765 745f 636f 6c75 6d6e da0d 636f  arget_column..co
-00000b40: 6e66 5f74 7261 696e 696e 675a 0c63 6f6e  nf_trainingZ.con
-00000b50: 665f 7867 626f 6f73 74da 1c63 7573 746f  f_xgboost..custo
-00000b60: 6d5f 6c61 7374 5f6d 696c 655f 636f 6d70  m_last_mile_comp
-00000b70: 7574 6174 696f 6e29 015a 0a74 6172 6765  utation).Z.targe
-00000b80: 745f 636f 6c7a 1641 7574 6f74 756e 696e  t_colz.Autotunin
-00000b90: 6720 7375 6363 6573 7366 756c 2e29 015a  g successful.).Z
-00000ba0: 0461 7869 737a 1650 7265 6469 6374 696e  .axisz.Predictin
-00000bb0: 6720 7375 6363 6573 7366 756c 2e29 01fa  g successful.)..
-00000bc0: 023d 3d29 017a 6b25 2870 7933 2973 0a7b  .==).zk%(py3)s.{
-00000bd0: 2528 7079 3329 7320 3d20 2528 7079 3029  %(py3)s = %(py0)
-00000be0: 7328 2528 7079 3129 7329 0a7d 203d 3d20  s(%(py1)s).} == 
-00000bf0: 2528 7079 3130 2973 0a7b 2528 7079 3130  %(py10)s.{%(py10
-00000c00: 2973 203d 2025 2870 7935 2973 2825 2870  )s = %(py5)s(%(p
-00000c10: 7938 2973 0a7b 2528 7079 3829 7320 3d20  y8)s.{%(py8)s = 
-00000c20: 2528 7079 3629 732e 696e 6465 780a 7d29  %(py6)s.index.})
-00000c30: 0a7d da03 6c65 6eda 0779 5f70 726f 6273  .}..len..y_probs
-00000c40: 7218 0000 0029 07da 0370 7930 da03 7079  r....)...py0..py
-00000c50: 315a 0370 7933 5a03 7079 35da 0370 7936  1Z.py3Z.py5..py6
-00000c60: 5a03 7079 385a 0470 7931 307a 0f61 7373  Z.py8Z.py10z.ass
-00000c70: 6572 7420 2528 7079 3132 2973 5a04 7079  ert %(py12)sZ.py
-00000c80: 3132 4eda 0979 5f63 6c61 7373 6573 2917  12N..y_classes).
-00000c90: 720c 0000 005a 0973 7465 7073 5f6d 6178  r....Z.steps_max
-00000ca0: 5a0e 6e75 6d5f 6c65 6176 6573 5f6d 6178  Z.num_leaves_max
-00000cb0: 720b 0000 00da 1c68 7970 6572 7061 7261  r......hyperpara
-00000cc0: 6d65 7465 725f 7475 6e69 6e67 5f72 6f75  meter_tuning_rou
-00000cd0: 6e64 73da 1865 6e61 626c 655f 6665 6174  nds..enable_feat
-00000ce0: 7572 655f 7365 6c65 6374 696f 6eda 1468  ure_selection..h
-00000cf0: 7970 6572 7475 6e69 6e67 5f63 765f 666f  ypertuning_cv_fo
-00000d00: 6c64 7372 1000 0000 7209 0000 00da 0366  ldsr....r......f
-00000d10: 6974 da05 7072 696e 74da 0770 7265 6469  it..print..predi
-00000d20: 6374 5a04 6472 6f70 7239 0000 00da 0569  ctZ.dropr9.....i
-00000d30: 6e64 6578 da0a 4070 7974 6573 745f 6172  ndex..@pytest_ar
-00000d40: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
-00000d50: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
-00000d60: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
-00000d70: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
-00000d80: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
-00000d90: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
-00000da0: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
-00000db0: 696f 6e29 1072 1b00 0000 7217 0000 0072  ion).r....r....r
-00000dc0: 1800 0000 5a14 7867 626f 6f73 745f 7061  ....Z.xgboost_pa
-00000dd0: 7261 6d5f 636f 6e66 6967 da0c 7472 6169  ram_config..trai
-00000de0: 6e5f 636f 6e66 6967 7232 0000 0072 3700  n_configr2...r7.
-00000df0: 0000 5a06 6175 746f 6d6c 723a 0000 0072  ..Z.automlr:...r
-00000e00: 3e00 0000 5a0b 4070 795f 6173 7365 7274  >...Z.@py_assert
-00000e10: 325a 0b40 7079 5f61 7373 6572 7437 5a0b  2Z.@py_assert7Z.
-00000e20: 4070 795f 6173 7365 7274 395a 0b40 7079  @py_assert9Z.@py
-00000e30: 5f61 7373 6572 7434 5a0c 4070 795f 666f  _assert4Z.@py_fo
-00000e40: 726d 6174 3131 5a0c 4070 795f 666f 726d  rmat11Z.@py_form
-00000e50: 6174 3133 7219 0000 0072 1900 0000 721a  at13r....r....r.
-00000e60: 0000 00da 1674 6573 745f 626c 7565 7072  .....test_bluepr
-00000e70: 696e 745f 7867 626f 6f73 7422 0000 0073  int_xgboost"...s
-00000e80: 3400 0000 0802 0801 0601 0601 0601 0601  4...............
-00000e90: 0601 0601 0601 1003 061a 0202 0201 0201  ................
-00000ea0: 0201 0201 0201 06fb 0e07 0801 1801 0801  ................
-00000eb0: fe01 0a00 fe01 1c00 724f 0000 0063 0000  ........rO...c..
-00000ec0: 0000 0000 0000 0000 0000 0000 0000 0a00  ................
-00000ed0: 0000 4000 0000 7356 0000 0065 005a 0164  ..@...sV...e.Z.d
-00000ee0: 005a 0264 0164 0284 005a 0364 0365 046a  .Z.d.d...Z.d.e.j
-00000ef0: 0564 0465 046a 0564 0565 046a 0664 0665  .d.e.j.d.e.j.d.e
-00000f00: 046a 0664 0764 0866 0a64 0964 0a84 045a  .j.d.d.f.d.d...Z
-00000f10: 0764 0b65 046a 0564 0765 0865 0965 0a66  .d.e.j.d.e.e.e.f
-00000f20: 0219 0066 0464 0c64 0d84 045a 0b64 0853  ...f.d.d...Z.d.S
-00000f30: 0029 0eda 0b43 7573 746f 6d4d 6f64 656c  .)...CustomModel
-00000f40: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000f50: 0002 0000 0043 0000 0073 0a00 0000 6400  .....C...s....d.
-00000f60: 7c00 5f00 6400 5300 a901 4e29 01da 056d  |._.d.S...N)...m
-00000f70: 6f64 656c 2901 7223 0000 0072 1900 0000  odel).r#...r....
-00000f80: 7219 0000 0072 1a00 0000 da08 5f5f 696e  r....r......__in
-00000f90: 6974 5f5f 5b00 0000 7302 0000 000a 017a  it__[...s......z
-00000fa0: 1443 7573 746f 6d4d 6f64 656c 2e5f 5f69  .CustomModel.__i
-00000fb0: 6e69 745f 5fda 0778 5f74 7261 696e da06  nit__..x_train..
-00000fc0: 785f 7465 7374 da07 795f 7472 6169 6eda  x_test..y_train.
-00000fd0: 0679 5f74 6573 7472 1300 0000 4e63 0500  .y_testr....Nc..
-00000fe0: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00000ff0: 0000 4300 0000 731a 0000 0074 0083 007c  ..C...s....t...|
-00001000: 005f 017c 006a 01a0 027c 017c 03a1 0201  ._.|.j...|.|....
-00001010: 0064 0053 0072 5100 0000 2903 7204 0000  .d.S.rQ...).r...
-00001020: 0072 5200 0000 7242 0000 0029 0572 2300  .rR...rB...).r#.
-00001030: 0000 7254 0000 0072 5500 0000 7256 0000  ..rT...rU...rV..
-00001040: 0072 5700 0000 7219 0000 0072 1900 0000  .rW...r....r....
-00001050: 721a 0000 0072 4200 0000 5e00 0000 7304  r....rB...^...s.
-00001060: 0000 0008 0712 017a 0f43 7573 746f 6d4d  .......z.CustomM
-00001070: 6f64 656c 2e66 6974 7220 0000 0063 0200  odel.fitr ...c..
-00001080: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00001090: 0000 4300 0000 7320 0000 007c 006a 00a0  ..C...s ...|.j..
-000010a0: 017c 01a1 017d 027c 006a 00a0 027c 01a1  .|...}.|.j...|..
-000010b0: 017d 037c 027c 0366 0253 0072 5100 0000  .}.|.|.f.S.rQ...
-000010c0: 2903 7252 0000 005a 0d70 7265 6469 6374  ).rR...Z.predict
-000010d0: 5f70 726f 6261 7244 0000 0029 0472 2300  _probarD...).r#.
-000010e0: 0000 7220 0000 00da 1070 7265 6469 6374  ..r .....predict
-000010f0: 6564 5f70 726f 6261 73da 1170 7265 6469  ed_probas..predi
-00001100: 6374 6564 5f63 6c61 7373 6573 7219 0000  cted_classesr...
-00001110: 0072 1900 0000 721a 0000 0072 4400 0000  .r....r....rD...
-00001120: 6800 0000 7306 0000 000c 010c 0108 017a  h...s..........z
-00001130: 1343 7573 746f 6d4d 6f64 656c 2e70 7265  .CustomModel.pre
-00001140: 6469 6374 290c 722d 0000 0072 2e00 0000  dict).r-...r....
-00001150: 722f 0000 0072 5300 0000 722a 0000 0072  r/...rS...r*...r
-00001160: 3000 0000 722b 0000 0072 4200 0000 7203  0...r+...rB...r.
-00001170: 0000 0072 0f00 0000 720e 0000 0072 4400  ...r....r....rD.
-00001180: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00001190: 0072 1a00 0000 7250 0000 005a 0000 0073  .r....rP...Z...s
-000011a0: 1c00 0000 0800 0801 0203 0402 02fe 0403  ................
-000011b0: 02fd 0404 02fc 0405 02fb 0206 0afa 200a  .............. .
-000011c0: 7250 0000 0063 0000 0000 0000 0000 0000  rP...c..........
-000011d0: 0000 0c00 0000 0a00 0000 4300 0000 73ce  ..........C...s.
-000011e0: 0200 0074 0083 007d 0074 0183 007d 0164  ...t...}.t...}.d
-000011f0: 017c 015f 0264 027c 015f 0364 037c 015f  .|._.d.|._.d.|._
-00001200: 0474 0583 007d 0274 0674 07a0 08a1 0064  .t...}.t.t.....d
-00001210: 0474 0964 0364 0564 0264 068d 0364 0474  .t.d.d.d.d...d.t
-00001220: 0a74 0b83 0164 0464 078d 067c 025f 0c74  .t...d.d...|._.t
-00001230: 0d64 0864 097c 007c 017c 0264 0a8d 057d  .d.d.|.|.|.d...}
-00001240: 0374 0ea0 0f64 0b64 0c84 0074 1064 0183  .t...d.d...t.d..
-00001250: 0144 0083 0164 0d64 0c84 0074 1064 0183  .D...d.d...t.d..
-00001260: 0144 0083 0164 0e64 0c84 0074 1064 0183  .D...d.d...t.d..
-00001270: 0144 0083 0164 0f64 0c84 0074 1064 0183  .D...d.d...t.d..
-00001280: 0144 0083 0164 1064 0c84 0074 1064 0183  .D...d.d...t.d..
-00001290: 0144 0083 0164 1164 0c84 0074 1064 0183  .D...d.d...t.d..
-000012a0: 0144 0083 0164 129c 06a1 017d 0474 0ea0  .D...d.....}.t..
-000012b0: 1167 0064 13a2 01a1 017d 0574 0ea0 0f64  .g.d.....}.t...d
-000012c0: 1464 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-000012d0: 1564 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-000012e0: 1664 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-000012f0: 1764 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-00001300: 1864 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-00001310: 1964 0c84 0074 1064 0183 0144 0083 0164  .d...t.d...D...d
-00001320: 129c 06a1 017d 067c 057c 0464 093c 007c  .....}.|.|.d.<.|
-00001330: 03a0 127c 0464 09a1 0201 007c 03a0 137c  ...|.d.....|...|
-00001340: 06a1 015c 027d 077d 0874 146a 157d 0974  ...\.}.}.t.j.}.t
-00001350: 167c 077c 0983 027d 0a7c 0a90 0173 0564  .|.|...}.|...s.d
-00001360: 1a64 1b74 17a0 18a1 0076 0073 ca74 19a0  .d.t.....v.s.t..
-00001370: 1a74 16a1 0172 cf74 19a0 1b74 16a1 016e  .t...r.t...t...n
-00001380: 0164 1b64 1c74 17a0 18a1 0076 0073 db74  .d.d.t.....v.s.t
-00001390: 19a0 1a7c 07a1 0172 e074 19a0 1b7c 07a1  ...|...r.t...|..
-000013a0: 016e 0164 1c64 1d74 17a0 18a1 0076 0073  .n.d.d.t.....v.s
-000013b0: ec74 19a0 1a74 14a1 0172 f174 19a0 1b74  .t...t...r.t...t
-000013c0: 14a1 016e 0164 1d74 19a0 1b7c 09a1 0174  ...n.d.t...|...t
-000013d0: 19a0 1b7c 0aa1 0164 1e9c 0516 007d 0b74  ...|...d.....}.t
-000013e0: 1c74 19a0 1d7c 0ba1 0183 0182 0164 0004  .t...|.......d..
-000013f0: 007d 097d 0a74 146a 157d 0974 167c 087c  .}.}.t.j.}.t.|.|
-00001400: 0983 027d 0a7c 0a90 0173 6164 1a64 1b74  ...}.|...sad.d.t
-00001410: 17a0 18a1 0076 0090 0173 2274 19a0 1a74  .....v...s"t...t
-00001420: 16a1 0190 0172 2774 19a0 1b74 16a1 016e  .....r't...t...n
-00001430: 0164 1b64 1f74 17a0 18a1 0076 0090 0173  .d.d.t.....v...s
-00001440: 3574 19a0 1a7c 08a1 0190 0172 3a74 19a0  5t...|.....r:t..
-00001450: 1b7c 08a1 016e 0164 1f64 1d74 17a0 18a1  .|...n.d.d.t....
-00001460: 0076 0090 0173 4874 19a0 1a74 14a1 0190  .v...sHt...t....
-00001470: 0172 4d74 19a0 1b74 14a1 016e 0164 1d74  .rMt...t...n.d.t
-00001480: 19a0 1b7c 09a1 0174 19a0 1b7c 0aa1 0164  ...|...t...|...d
-00001490: 1e9c 0516 007d 0b74 1c74 19a0 1d7c 0ba1  .....}.t.t...|..
-000014a0: 0183 0182 0164 0004 007d 097d 0a64 0053  .....d...}.}.d.S
-000014b0: 0029 204e 721f 0000 0054 7221 0000 0072  .) Nr....Tr!...r
-000014c0: 1c00 0000 7201 0000 0029 0272 1500 0000  ....r....).r....
-000014d0: da07 7368 7566 666c 6529 065a 0965 7374  ..shuffle).Z.est
-000014e0: 696d 6174 6f72 da04 7374 6570 5a02 6376  imator..stepZ.cv
-000014f0: 5a16 6d69 6e5f 6665 6174 7572 6573 5f74  Z.min_features_t
-00001500: 6f5f 7365 6c65 6374 5a07 7363 6f72 696e  o_selectZ.scorin
-00001510: 675a 066e 5f6a 6f62 7372 3300 0000 7225  gZ.n_jobsr3...r%
-00001520: 0000 0029 0572 3400 0000 7235 0000 005a  ...).r4...r5...Z
-00001530: 086d 6c5f 6d6f 6465 6c72 3600 0000 5a16  .ml_modelr6...Z.
-00001540: 636f 6e66 5f66 6561 7475 7265 5f73 656c  conf_feature_sel
-00001550: 6563 7469 6f6e 6301 0000 0000 0000 0000  ectionc.........
-00001560: 0000 0002 0000 0003 0000 0053 0000 00f3  ...........S....
-00001570: 1000 0000 6700 7c00 5d04 7d01 7c01 9102  ....g.|.].}.|...
-00001580: 7102 5300 7219 0000 0072 1900 0000 a902  q.S.r....r......
-00001590: da02 2e30 da01 6972 1900 0000 7219 0000  ...0..ir....r...
-000015a0: 0072 1a00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-000015b0: 703e 8e00 0000 f302 0000 0010 007a 3374  p>...........z3t
-000015c0: 6573 745f 626c 7565 6361 7374 5f77 6974  est_bluecast_wit
-000015d0: 685f 6375 7374 6f6d 5f6d 6f64 656c 2e3c  h_custom_model.<
-000015e0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000015f0: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-00001600: 0000 0003 0000 0053 0000 0072 5c00 0000  .......S...r\...
-00001610: 7219 0000 0072 1900 0000 725d 0000 0072  r....r....r]...r
-00001620: 1900 0000 7219 0000 0072 1a00 0000 7260  ....r....r....r`
-00001630: 0000 008f 0000 0072 6100 0000 6301 0000  .......ra...c...
-00001640: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001650: 0053 0000 0072 5c00 0000 7219 0000 0072  .S...r\...r....r
-00001660: 1900 0000 725d 0000 0072 1900 0000 7219  ....r]...r....r.
-00001670: 0000 0072 1a00 0000 7260 0000 0090 0000  ...r....r`......
-00001680: 0072 6100 0000 6301 0000 0000 0000 0000  .ra...c.........
-00001690: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-000016a0: 5c00 0000 7219 0000 0072 1900 0000 725d  \...r....r....r]
-000016b0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-000016c0: 0000 7260 0000 0091 0000 0072 6100 0000  ..r`.......ra...
-000016d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000016e0: 0003 0000 0053 0000 0072 5c00 0000 7219  .....S...r\...r.
-000016f0: 0000 0072 1900 0000 725d 0000 0072 1900  ...r....r]...r..
-00001700: 0000 7219 0000 0072 1a00 0000 7260 0000  ..r....r....r`..
-00001710: 0092 0000 0072 6100 0000 6301 0000 0000  .....ra...c.....
-00001720: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001730: 0000 0072 5c00 0000 7219 0000 0072 1900  ...r\...r....r..
-00001740: 0000 725d 0000 0072 1900 0000 7219 0000  ..r]...r....r...
-00001750: 0072 1a00 0000 7260 0000 0093 0000 0072  .r....r`.......r
-00001760: 6100 0000 2906 5a08 6665 6174 7572 6531  a...).Z.feature1
-00001770: 5a08 6665 6174 7572 6532 5a08 6665 6174  Z.feature2Z.feat
-00001780: 7572 6533 5a08 6665 6174 7572 6534 5a08  ure3Z.feature4Z.
-00001790: 6665 6174 7572 6535 5a08 6665 6174 7572  feature5Z.featur
-000017a0: 6536 290a 7201 0000 0072 1c00 0000 7201  e6).r....r....r.
-000017b0: 0000 0072 1c00 0000 7201 0000 0072 1c00  ...r....r....r..
-000017c0: 0000 7201 0000 0072 1c00 0000 7201 0000  ..r....r....r...
-000017d0: 0072 1c00 0000 6301 0000 0000 0000 0000  .r....c.........
-000017e0: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-000017f0: 5c00 0000 7219 0000 0072 1900 0000 725d  \...r....r....r]
-00001800: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001810: 0000 7260 0000 0099 0000 0072 6100 0000  ..r`.......ra...
-00001820: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001830: 0003 0000 0053 0000 0072 5c00 0000 7219  .....S...r\...r.
-00001840: 0000 0072 1900 0000 725d 0000 0072 1900  ...r....r]...r..
-00001850: 0000 7219 0000 0072 1a00 0000 7260 0000  ..r....r....r`..
-00001860: 009a 0000 0072 6100 0000 6301 0000 0000  .....ra...c.....
-00001870: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001880: 0000 0072 5c00 0000 7219 0000 0072 1900  ...r\...r....r..
-00001890: 0000 725d 0000 0072 1900 0000 7219 0000  ..r]...r....r...
-000018a0: 0072 1a00 0000 7260 0000 009b 0000 0072  .r....r`.......r
-000018b0: 6100 0000 6301 0000 0000 0000 0000 0000  a...c...........
-000018c0: 0002 0000 0003 0000 0053 0000 0072 5c00  .........S...r\.
-000018d0: 0000 7219 0000 0072 1900 0000 725d 0000  ..r....r....r]..
-000018e0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-000018f0: 7260 0000 009c 0000 0072 6100 0000 6301  r`.......ra...c.
-00001900: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001910: 0000 0053 0000 0072 5c00 0000 7219 0000  ...S...r\...r...
-00001920: 0072 1900 0000 725d 0000 0072 1900 0000  .r....r]...r....
-00001930: 7219 0000 0072 1a00 0000 7260 0000 009d  r....r....r`....
-00001940: 0000 0072 6100 0000 6301 0000 0000 0000  ...ra...c.......
-00001950: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001960: 0072 5c00 0000 7219 0000 0072 1900 0000  .r\...r....r....
-00001970: 725d 0000 0072 1900 0000 7219 0000 0072  r]...r....r....r
-00001980: 1a00 0000 7260 0000 009e 0000 0072 6100  ....r`.......ra.
-00001990: 0000 7a52 6173 7365 7274 2025 2870 7936  ..zRassert %(py6
-000019a0: 2973 0a7b 2528 7079 3629 7320 3d20 2528  )s.{%(py6)s = %(
-000019b0: 7079 3029 7328 2528 7079 3129 732c 2025  py0)s(%(py1)s, %
-000019c0: 2870 7934 2973 0a7b 2528 7079 3429 7320  (py4)s.{%(py4)s 
-000019d0: 3d20 2528 7079 3229 732e 6e64 6172 7261  = %(py2)s.ndarra
-000019e0: 790a 7d29 0a7d 7229 0000 0072 5800 0000  y.}).}r)...rX...
-000019f0: da02 6e70 2905 723b 0000 0072 3c00 0000  ..np).r;...r<...
-00001a00: 5a03 7079 325a 0370 7934 723d 0000 0072  Z.py2Z.py4r=...r
-00001a10: 5900 0000 291e 7250 0000 0072 0b00 0000  Y...).rP...r....
-00001a20: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
-00001a30: 0a00 0000 7205 0000 00da 0378 6762 5a0d  ....r......xgbZ.
-00001a40: 5847 4243 6c61 7373 6966 6965 7272 0800  XGBClassifierr..
-00001a50: 0000 7206 0000 0072 0700 0000 5a12 7365  ..r....r....Z.se
-00001a60: 6c65 6374 696f 6e5f 7374 7261 7465 6779  lection_strategy
-00001a70: 7209 0000 0072 2a00 0000 7230 0000 00da  r....r*...r0....
-00001a80: 0572 616e 6765 722b 0000 0072 4200 0000  .ranger+...rB...
-00001a90: 7244 0000 0072 6200 0000 da07 6e64 6172  rD...rb.....ndar
-00001aa0: 7261 7972 2900 0000 7248 0000 0072 4900  rayr)...rH...rI.
-00001ab0: 0000 7246 0000 0072 4a00 0000 724b 0000  ..rF...rJ...rK..
-00001ac0: 0072 4c00 0000 724d 0000 0029 0c5a 0c63  .rL...rM...).Z.c
-00001ad0: 7573 746f 6d5f 6d6f 6465 6c72 4e00 0000  ustom_modelrN...
-00001ae0: 5a0f 6375 7374 6f6d 5f66 6561 745f 7365  Z.custom_feat_se
-00001af0: 6cda 0862 6c75 6563 6173 7472 5400 0000  l..bluecastrT...
-00001b00: 7256 0000 0072 5500 0000 7258 0000 0072  rV...rU...rX...r
-00001b10: 5900 0000 5a0b 4070 795f 6173 7365 7274  Y...Z.@py_assert
-00001b20: 335a 0b40 7079 5f61 7373 6572 7435 5a0b  3Z.@py_assert5Z.
-00001b30: 4070 795f 666f 726d 6174 3772 1900 0000  @py_format7r....
-00001b40: 7219 0000 0072 1a00 0000 da1f 7465 7374  r....r......test
-00001b50: 5f62 6c75 6563 6173 745f 7769 7468 5f63  _bluecast_with_c
-00001b60: 7573 746f 6d5f 6d6f 6465 6c6e 0000 0073  ustom_modeln...s
-00001b70: 5a00 0000 0602 0601 0601 0601 0601 0603  Z...............
-00001b80: 0202 0601 0201 0c01 0201 0601 0201 08fa  ................
-00001b90: 020a 0201 0201 0201 0201 0201 06fb 0409  ................
-00001ba0: 1002 1001 1001 1001 1001 1001 04fa 04ff  ................
-00001bb0: 0e0a 0401 1002 1001 1001 1001 1001 1001  ................
-00001bc0: 04fa 04ff 080b 0c03 0e03 ac03 bc01 7267  ..............rg
-00001bd0: 0000 0029 2dda 0862 7569 6c74 696e 7372  ...)-..builtinsr
-00001be0: 4800 0000 da19 5f70 7974 6573 742e 6173  H....._pytest.as
-00001bf0: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
-00001c00: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
-00001c10: 6974 6572 4600 0000 da06 7479 7069 6e67  iterF.....typing
-00001c20: 7202 0000 0072 0300 0000 da05 6e75 6d70  r....r......nump
-00001c30: 7972 6200 0000 5a06 7061 6e64 6173 722a  yrb...Z.pandasr*
-00001c40: 0000 00da 0670 7974 6573 745a 0778 6762  .....pytestZ.xgb
-00001c50: 6f6f 7374 7263 0000 005a 1073 6b6c 6561  oostrc...Z.sklea
-00001c60: 726e 2e65 6e73 656d 626c 6572 0400 0000  rn.ensembler....
-00001c70: 5a19 736b 6c65 6172 6e2e 6665 6174 7572  Z.sklearn.featur
-00001c80: 655f 7365 6c65 6374 696f 6e72 0500 0000  e_selectionr....
-00001c90: 5a0f 736b 6c65 6172 6e2e 6d65 7472 6963  Z.sklearn.metric
-00001ca0: 7372 0600 0000 7207 0000 005a 1773 6b6c  sr....r....Z.skl
-00001cb0: 6561 726e 2e6d 6f64 656c 5f73 656c 6563  earn.model_selec
-00001cc0: 7469 6f6e 7208 0000 005a 1862 6c75 6563  tionr....Z.bluec
-00001cd0: 6173 742e 626c 7565 7072 696e 7473 2e63  ast.blueprints.c
-00001ce0: 6173 7472 0900 0000 5a1f 626c 7565 6361  astr....Z.blueca
-00001cf0: 7374 2e63 6f6e 6669 672e 7472 6169 6e69  st.config.traini
-00001d00: 6e67 5f63 6f6e 6669 6772 0a00 0000 720b  ng_configr....r.
-00001d10: 0000 0072 0c00 0000 5a22 626c 7565 6361  ...r....Z"blueca
-00001d20: 7374 2e6d 6c5f 6d6f 6465 6c6c 696e 672e  st.ml_modelling.
-00001d30: 6261 7365 5f63 6c61 7373 6573 720d 0000  base_classesr...
-00001d40: 0072 0e00 0000 720f 0000 005a 1d62 6c75  .r....r....Z.blu
-00001d50: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-00001d60: 696e 672e 6375 7374 6f6d 7210 0000 005a  ing.customr....Z
-00001d70: 2462 6c75 6563 6173 742e 7465 7374 732e  $bluecast.tests.
-00001d80: 6d61 6b65 5f64 6174 612e 6372 6561 7465  make_data.create
-00001d90: 5f64 6174 6172 1200 0000 da07 6669 7874  _datar......fixt
-00001da0: 7572 6572 3000 0000 721b 0000 0072 4f00  urer0...r....rO.
-00001db0: 0000 7250 0000 0072 6700 0000 7219 0000  ..rP...rg...r...
-00001dc0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001dd0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
-00001de0: 0000 002a 0008 0208 0108 0108 010c 010c  ...*............
-00001df0: 0110 010c 010c 0214 0114 050c 050c 0104  ................
-00001e00: 031c 0108 0610 380c 14                   ......8..
+000000c0: 5a1c 6d1d 5a1d 0100 6400 6409 6c1e 6d1f  Z.m.Z...d.d.l.m.
+000000d0: 5a1f 6d20 5a20 6d21 5a21 0100 6400 640a  Z.m Z m!Z!..d.d.
+000000e0: 6c22 6d23 5a23 0100 6400 640b 6c24 6d25  l"m#Z#..d.d.l$m%
+000000f0: 5a25 0100 650d 6a26 640c 6508 650c 6a27  Z%..e.j&d.e.e.j'
+00000100: 650c 6a27 6602 1900 6602 640d 640e 8404  e.j'f...f.d.d...
+00000110: 8301 5a28 640f 6410 8400 5a29 4700 6411  ..Z(d.d...Z)G.d.
+00000120: 6412 8400 6412 651f 8303 5a2a 6413 6414  d...d.e...Z*d.d.
+00000130: 8400 5a2b 6401 5300 2915 e900 0000 004e  ..Z+d.S.)......N
+00000140: 2902 da08 4f70 7469 6f6e 616c da05 5475  )...Optional..Tu
+00000150: 706c 6529 01da 1652 616e 646f 6d46 6f72  ple)...RandomFor
+00000160: 6573 7443 6c61 7373 6966 6965 7229 01da  estClassifier)..
+00000170: 0552 4645 4356 2902 da0b 6d61 6b65 5f73  .RFECV)...make_s
+00000180: 636f 7265 72da 116d 6174 7468 6577 735f  corer..matthews_
+00000190: 636f 7272 636f 6566 2901 da0f 5374 7261  corrcoef)...Stra
+000001a0: 7469 6669 6564 4b46 6f6c 6429 01da 0842  tifiedKFold)...B
+000001b0: 6c75 6543 6173 7429 02da 0e54 7261 696e  lueCast)...Train
+000001c0: 696e 6743 6f6e 6669 67da 1758 6762 6f6f  ingConfig..Xgboo
+000001d0: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
+000001e0: 6967 2903 da10 4261 7365 436c 6173 734d  ig)...BaseClassM
+000001f0: 6c4d 6f64 656c da10 5072 6564 6963 7465  lModel..Predicte
+00000200: 6443 6c61 7373 6573 da0f 5072 6564 6963  dClasses..Predic
+00000210: 7465 6450 726f 6261 7329 01da 1343 7573  tedProbas)...Cus
+00000220: 746f 6d50 7265 7072 6f63 6573 7369 6e67  tomPreprocessing
+00000230: a901 da1a 6372 6561 7465 5f73 796e 7468  ....create_synth
+00000240: 6574 6963 5f64 6174 6166 7261 6d65 da06  etic_dataframe..
+00000250: 7265 7475 726e 6300 0000 0000 0000 0000  returnc.........
+00000260: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000270: 2000 0000 7400 6401 6402 6403 8d02 7d00   ...t.d.d.d...}.
+00000280: 7400 6401 6404 6403 8d02 7d01 7c00 7c01  t.d.d.d...}.|.|.
+00000290: 6602 5300 2905 4e69 d007 0000 e914 0000  f.S.).Ni........
+000002a0: 0029 01da 0c72 616e 646f 6d5f 7374 6174  .)...random_stat
+000002b0: 65e9 c800 0000 7210 0000 0029 02da 0864  e.....r....)...d
+000002c0: 665f 7472 6169 6eda 0664 665f 7661 6ca9  f_train..df_val.
+000002d0: 0072 1800 0000 fa3e 2f68 6f6d 652f 7468  .r.....>/home/th
+000002e0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
+000002f0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
+00000300: 6173 742f 7465 7374 732f 7465 7374 5f63  ast/tests/test_c
+00000310: 6173 742e 7079 da19 7379 6e74 6865 7469  ast.py..syntheti
+00000320: 635f 7472 6169 6e5f 7465 7374 5f64 6174  c_train_test_dat
+00000330: 6117 0000 0073 0600 0000 0c02 0c01 0801  a....s..........
+00000340: 721a 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000350: 0000 1000 0000 0a00 0000 4300 0000 73ba  ..........C...s.
+00000360: 0200 007c 0064 0119 007d 017c 0064 0219  ...|.d...}.|.d..
+00000370: 007d 0274 0083 007d 0364 037c 035f 0164  .}.t...}.d.|._.d
+00000380: 047c 035f 0274 0383 007d 0464 057c 045f  .|._.t...}.d.|._
+00000390: 0464 067c 045f 0564 027c 045f 0647 0064  .d.|._.d.|._.G.d
+000003a0: 0764 0884 0064 0874 0783 037d 057c 0583  .d...d.t...}.|..
+000003b0: 007d 0674 0864 0964 0a7c 047c 037c 0664  .}.t.d.d.|.|.|.d
+000003c0: 0b8d 057d 077c 076a 097c 0164 0a64 0c8d  ...}.|.j.|.d.d..
+000003d0: 0201 0074 0a64 0d83 0101 007c 07a0 0b7c  ...t.d.....|...|
+000003e0: 026a 0c64 0a64 0264 0e8d 02a1 015c 027d  .j.d.d.d.....\.}
+000003f0: 087d 0974 0a64 0f83 0101 0074 0d7c 0883  .}.t.d.....t.|..
+00000400: 017d 0a7c 026a 0e7d 0b74 0d7c 0b83 017d  .}.|.j.}.t.|...}
+00000410: 0c7c 0a7c 0c6b 027d 0d7c 0d73 c874 0fa0  .|.|.k.}.|.s.t..
+00000420: 1064 107c 0d66 0164 117c 0a7c 0c66 02a1  .d.|.f.d.|.|.f..
+00000430: 0464 1274 11a0 12a1 0076 0073 7274 0fa0  .d.t.....v.srt..
+00000440: 1374 0da1 0172 7774 0fa0 1474 0da1 016e  .t...rwt...t...n
+00000450: 0164 1264 1374 11a0 12a1 0076 0073 8374  .d.d.t.....v.s.t
+00000460: 0fa0 137c 08a1 0172 8874 0fa0 147c 08a1  ...|...r.t...|..
+00000470: 016e 0164 1374 0fa0 147c 0aa1 0164 1274  .n.d.t...|...d.t
+00000480: 11a0 12a1 0076 0073 9874 0fa0 1374 0da1  .....v.s.t...t..
+00000490: 0172 9d74 0fa0 1474 0da1 016e 0164 1264  .r.t...t...n.d.d
+000004a0: 1474 11a0 12a1 0076 0073 a974 0fa0 137c  .t.....v.s.t...|
+000004b0: 02a1 0172 ae74 0fa0 147c 02a1 016e 0164  ...r.t...|...n.d
+000004c0: 1474 0fa0 147c 0ba1 0174 0fa0 147c 0ca1  .t...|...t...|..
+000004d0: 0164 159c 0716 007d 0e64 1664 177c 0e69  .d.....}.d.d.|.i
+000004e0: 0116 007d 0f74 1574 0fa0 167c 0fa1 0183  ...}.t.t...|....
+000004f0: 0182 0164 1804 007d 0a04 007d 0d04 007d  ...d...}...}...}
+00000500: 0b7d 0c74 0d7c 0983 017d 0a7c 026a 0e7d  .}.t.|...}.|.j.}
+00000510: 0b74 0d7c 0b83 017d 0c7c 0a7c 0c6b 027d  .t.|...}.|.|.k.}
+00000520: 0d7c 0d90 0173 5374 0fa0 1064 107c 0d66  .|...sSt...d.|.f
+00000530: 0164 117c 0a7c 0c66 02a1 0464 1274 11a0  .d.|.|.f...d.t..
+00000540: 12a1 0076 0073 f774 0fa0 1374 0da1 0172  ...v.s.t...t...r
+00000550: fc74 0fa0 1474 0da1 016e 0164 1264 1974  .t...t...n.d.d.t
+00000560: 11a0 12a1 0076 0090 0173 0a74 0fa0 137c  .....v...s.t...|
+00000570: 09a1 0190 0172 0f74 0fa0 147c 09a1 016e  .....r.t...|...n
+00000580: 0164 1974 0fa0 147c 0aa1 0164 1274 11a0  .d.t...|...d.t..
+00000590: 12a1 0076 0090 0173 2174 0fa0 1374 0da1  ...v...s!t...t..
+000005a0: 0190 0172 2674 0fa0 1474 0da1 016e 0164  ...r&t...t...n.d
+000005b0: 1264 1474 11a0 12a1 0076 0090 0173 3474  .d.t.....v...s4t
+000005c0: 0fa0 137c 02a1 0190 0172 3974 0fa0 147c  ...|.....r9t...|
+000005d0: 02a1 016e 0164 1474 0fa0 147c 0ba1 0174  ...n.d.t...|...t
+000005e0: 0fa0 147c 0ca1 0164 159c 0716 007d 0e64  ...|...d.....}.d
+000005f0: 1664 177c 0e69 0116 007d 0f74 1574 0fa0  .d.|.i...}.t.t..
+00000600: 167c 0fa1 0183 0182 0164 1804 007d 0a04  .|.......d...}..
+00000610: 007d 0d04 007d 0b7d 0c64 1853 0029 1a7a  .}...}.}.d.S.).z
+00000620: 2254 6573 7420 7468 6174 2074 6573 7473  "Test that tests
+00000630: 2074 6865 2042 6c75 6543 6173 7420 636c   the BlueCast cl
+00000640: 6173 7372 0100 0000 e901 0000 00e9 6400  assr..........d.
+00000650: 0000 e910 0000 00e9 0a00 0000 4663 0000  ............Fc..
+00000660: 0000 0000 0000 0000 0000 0000 0000 0c00  ................
+00000670: 0000 4000 0000 7380 0000 0065 005a 0164  ..@...s....e.Z.d
+00000680: 005a 0264 0165 036a 0464 0265 036a 0466  .Z.d.e.j.d.e.j.f
+00000690: 0464 0364 0484 045a 0564 0165 036a 0464  .d.d...Z.d.e.j.d
+000006a0: 0565 036a 0664 0265 0765 036a 0465 036a  .e.j.d.e.e.j.e.j
+000006b0: 0666 0219 0066 0664 0664 0784 045a 0809  .f...f.d.d...Z..
+000006c0: 0809 0964 0d64 0165 036a 0464 0565 0965  ...d.d.e.j.d.e.e
+000006d0: 036a 0619 0064 0a65 0a64 0265 0765 036a  .j...d.e.d.e.e.j
+000006e0: 0465 0965 036a 0619 0066 0219 0066 0864  .e.e.j...f...f.d
+000006f0: 0b64 0c84 055a 0b64 0853 0029 0e7a 3d74  .d...Z.d.S.).z=t
+00000700: 6573 745f 626c 7565 7072 696e 745f 7867  est_blueprint_xg
+00000710: 626f 6f73 742e 3c6c 6f63 616c 733e 2e4d  boost.<locals>.M
+00000720: 7943 7573 746f 6d4c 6173 744d 696c 6550  yCustomLastMileP
+00000730: 7265 7072 6f63 6573 7369 6e67 da02 6466  reprocessing..df
+00000740: 7212 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00000750: 0000 0200 0000 0300 0000 5300 0000 7314  ..........S...s.
+00000760: 0000 007c 0164 011b 007d 0164 027c 0164  ...|.d...}.d.|.d
+00000770: 033c 007c 0153 0029 044e e902 0000 00e9  .<.|.S.).N......
+00000780: 0500 0000 5a0a 6375 7374 6f6d 5f63 6f6c  ....Z.custom_col
+00000790: 7218 0000 0029 02da 0473 656c 6672 1f00  r....)...selfr..
+000007a0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000007b0: 00da 0f63 7573 746f 6d5f 6675 6e63 7469  ...custom_functi
+000007c0: 6f6e 2c00 0000 7306 0000 0008 0108 0104  on,...s.........
+000007d0: 017a 4d74 6573 745f 626c 7565 7072 696e  .zMtest_blueprin
+000007e0: 745f 7867 626f 6f73 742e 3c6c 6f63 616c  t_xgboost.<local
+000007f0: 733e 2e4d 7943 7573 746f 6d4c 6173 744d  s>.MyCustomLastM
+00000800: 696c 6550 7265 7072 6f63 6573 7369 6e67  ilePreprocessing
+00000810: 2e63 7573 746f 6d5f 6675 6e63 7469 6f6e  .custom_function
+00000820: da06 7461 7267 6574 6303 0000 0000 0000  ..targetc.......
+00000830: 0000 0000 0003 0000 0003 0000 0053 0000  .............S..
+00000840: 0073 2600 0000 7c00 a000 7c01 a101 7d01  .s&...|...|...}.
+00000850: 7c01 a001 6401 a101 7d01 7c02 a001 6401  |...d...}.|...d.
+00000860: a101 7d02 7c01 7c02 6602 5300 2902 4e69  ..}.|.|.f.S.).Ni
+00000870: e803 0000 2902 7223 0000 00da 0468 6561  ....).r#.....hea
+00000880: 64a9 0372 2200 0000 721f 0000 0072 2400  d..r"...r....r$.
+00000890: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000008a0: 00da 0d66 6974 5f74 7261 6e73 666f 726d  ...fit_transform
+000008b0: 3100 0000 7308 0000 000a 030a 010a 0108  1...s...........
+000008c0: 017a 4b74 6573 745f 626c 7565 7072 696e  .zKtest_blueprin
+000008d0: 745f 7867 626f 6f73 742e 3c6c 6f63 616c  t_xgboost.<local
+000008e0: 733e 2e4d 7943 7573 746f 6d4c 6173 744d  s>.MyCustomLastM
+000008f0: 696c 6550 7265 7072 6f63 6573 7369 6e67  ilePreprocessing
+00000900: 2e66 6974 5f74 7261 6e73 666f 726d 4e46  .fit_transformNF
+00000910: da0e 7072 6564 6963 746f 6e5f 6d6f 6465  ..predicton_mode
+00000920: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00000930: 0003 0000 0053 0000 0073 3600 0000 7c00  .....S...s6...|.
+00000940: a000 7c01 a101 7d01 7c03 7317 7401 7c02  ..|...}.|.s.t.|.
+00000950: 7402 6a03 8302 7217 7c01 a004 6401 a101  t.j...r.|...d...
+00000960: 7d01 7c02 a004 6401 a101 7d02 7c01 7c02  }.|...d...}.|.|.
+00000970: 6602 5300 2902 4e72 1c00 0000 2905 7223  f.S.).Nr....).r#
+00000980: 0000 00da 0a69 7369 6e73 7461 6e63 65da  .....isinstance.
+00000990: 0270 64da 0653 6572 6965 7372 2500 0000  .pd..Seriesr%...
+000009a0: a904 7222 0000 0072 1f00 0000 7224 0000  ..r"...r....r$..
+000009b0: 0072 2800 0000 7218 0000 0072 1800 0000  .r(...r....r....
+000009c0: 7219 0000 00da 0974 7261 6e73 666f 726d  r......transform
+000009d0: 3900 0000 730a 0000 000a 0610 010a 010a  9...s...........
+000009e0: 0108 017a 4774 6573 745f 626c 7565 7072  ...zGtest_bluepr
+000009f0: 696e 745f 7867 626f 6f73 742e 3c6c 6f63  int_xgboost.<loc
+00000a00: 616c 733e 2e4d 7943 7573 746f 6d4c 6173  als>.MyCustomLas
+00000a10: 744d 696c 6550 7265 7072 6f63 6573 7369  tMilePreprocessi
+00000a20: 6e67 2e74 7261 6e73 666f 726d a902 4e46  ng.transform..NF
+00000a30: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000a40: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000a50: 6e61 6d65 5f5f 722a 0000 00da 0944 6174  name__r*.....Dat
+00000a60: 6146 7261 6d65 7223 0000 0072 2b00 0000  aFramer#...r+...
+00000a70: 7203 0000 0072 2700 0000 7202 0000 00da  r....r'...r.....
+00000a80: 0462 6f6f 6c72 2d00 0000 7218 0000 0072  .boolr-...r....r
+00000a90: 1800 0000 7218 0000 0072 1900 0000 da1d  ....r....r......
+00000aa0: 4d79 4375 7374 6f6d 4c61 7374 4d69 6c65  MyCustomLastMile
+00000ab0: 5072 6570 726f 6365 7373 696e 672b 0000  Preprocessing+..
+00000ac0: 0073 2800 0000 0800 1601 0205 0401 02ff  .s(.............
+00000ad0: 0401 02ff 0e02 0afe 020b 0201 04fc 0402  ................
+00000ae0: 02fe 0803 02fd 0204 02fc 1205 0efb 7234  ..............r4
+00000af0: 0000 00da 0662 696e 6172 7972 2400 0000  .....binaryr$...
+00000b00: 2905 da0d 636c 6173 735f 7072 6f62 6c65  )...class_proble
+00000b10: 6dda 0d74 6172 6765 745f 636f 6c75 6d6e  m..target_column
+00000b20: da0d 636f 6e66 5f74 7261 696e 696e 675a  ..conf_trainingZ
+00000b30: 0c63 6f6e 665f 7867 626f 6f73 74da 1c63  .conf_xgboost..c
+00000b40: 7573 746f 6d5f 6c61 7374 5f6d 696c 655f  ustom_last_mile_
+00000b50: 636f 6d70 7574 6174 696f 6e29 015a 0a74  computation).Z.t
+00000b60: 6172 6765 745f 636f 6c7a 1641 7574 6f74  arget_colz.Autot
+00000b70: 756e 696e 6720 7375 6363 6573 7366 756c  uning successful
+00000b80: 2e29 015a 0461 7869 737a 1650 7265 6469  .).Z.axisz.Predi
+00000b90: 6374 696e 6720 7375 6363 6573 7366 756c  cting successful
+00000ba0: 2e29 01fa 023d 3d29 017a 6b25 2870 7933  .)...==).zk%(py3
+00000bb0: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
+00000bc0: 7079 3029 7328 2528 7079 3129 7329 0a7d  py0)s(%(py1)s).}
+00000bd0: 203d 3d20 2528 7079 3130 2973 0a7b 2528   == %(py10)s.{%(
+00000be0: 7079 3130 2973 203d 2025 2870 7935 2973  py10)s = %(py5)s
+00000bf0: 2825 2870 7938 2973 0a7b 2528 7079 3829  (%(py8)s.{%(py8)
+00000c00: 7320 3d20 2528 7079 3629 732e 696e 6465  s = %(py6)s.inde
+00000c10: 780a 7d29 0a7d da03 6c65 6eda 0779 5f70  x.}).}..len..y_p
+00000c20: 726f 6273 7217 0000 0029 07da 0370 7930  robsr....)...py0
+00000c30: da03 7079 315a 0370 7933 5a03 7079 35da  ..py1Z.py3Z.py5.
+00000c40: 0370 7936 5a03 7079 385a 0470 7931 307a  .py6Z.py8Z.py10z
+00000c50: 0f61 7373 6572 7420 2528 7079 3132 2973  .assert %(py12)s
+00000c60: 5a04 7079 3132 4eda 0979 5f63 6c61 7373  Z.py12N..y_class
+00000c70: 6573 2917 720b 0000 005a 0973 7465 7073  es).r....Z.steps
+00000c80: 5f6d 6178 5a0e 6e75 6d5f 6c65 6176 6573  _maxZ.num_leaves
+00000c90: 5f6d 6178 720a 0000 00da 1c68 7970 6572  _maxr......hyper
+00000ca0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+00000cb0: 5f72 6f75 6e64 73da 1865 6e61 626c 655f  _rounds..enable_
+00000cc0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
+00000cd0: 6eda 1468 7970 6572 7475 6e69 6e67 5f63  n..hypertuning_c
+00000ce0: 765f 666f 6c64 7372 0f00 0000 7209 0000  v_foldsr....r...
+00000cf0: 00da 0366 6974 da05 7072 696e 74da 0770  ...fit..print..p
+00000d00: 7265 6469 6374 5a04 6472 6f70 723b 0000  redictZ.dropr;..
+00000d10: 00da 0569 6e64 6578 da0a 4070 7974 6573  ...index..@pytes
+00000d20: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
+00000d30: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
+00000d40: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
+00000d50: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
+00000d60: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
+00000d70: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
+00000d80: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
+00000d90: 616e 6174 696f 6e29 1072 1a00 0000 7216  anation).r....r.
+00000da0: 0000 0072 1700 0000 5a14 7867 626f 6f73  ...r....Z.xgboos
+00000db0: 745f 7061 7261 6d5f 636f 6e66 6967 da0c  t_param_config..
+00000dc0: 7472 6169 6e5f 636f 6e66 6967 7234 0000  train_configr4..
+00000dd0: 0072 3900 0000 5a06 6175 746f 6d6c 723c  .r9...Z.automlr<
+00000de0: 0000 0072 4000 0000 5a0b 4070 795f 6173  ...r@...Z.@py_as
+00000df0: 7365 7274 325a 0b40 7079 5f61 7373 6572  sert2Z.@py_asser
+00000e00: 7437 5a0b 4070 795f 6173 7365 7274 395a  t7Z.@py_assert9Z
+00000e10: 0b40 7079 5f61 7373 6572 7434 5a0c 4070  .@py_assert4Z.@p
+00000e20: 795f 666f 726d 6174 3131 5a0c 4070 795f  y_format11Z.@py_
+00000e30: 666f 726d 6174 3133 7218 0000 0072 1800  format13r....r..
+00000e40: 0000 7219 0000 00da 1674 6573 745f 626c  ..r......test_bl
+00000e50: 7565 7072 696e 745f 7867 626f 6f73 741e  ueprint_xgboost.
+00000e60: 0000 0073 3400 0000 0802 0801 0601 0601  ...s4...........
+00000e70: 0601 0601 0601 0601 0601 1003 061a 0202  ................
+00000e80: 0201 0201 0201 0201 0201 06fb 0e07 0801  ................
+00000e90: 1801 0801 fe01 0a00 fe01 1c00 7251 0000  ............rQ..
+00000ea0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000eb0: 0000 0a00 0000 4000 0000 7356 0000 0065  ......@...sV...e
+00000ec0: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00000ed0: 0365 046a 0564 0465 046a 0564 0565 046a  .e.j.d.e.j.d.e.j
+00000ee0: 0664 0665 046a 0664 0764 0866 0a64 0964  .d.e.j.d.d.f.d.d
+00000ef0: 0a84 045a 0764 0b65 046a 0564 0765 0865  ...Z.d.e.j.d.e.e
+00000f00: 0965 0a66 0219 0066 0464 0c64 0d84 045a  .e.f...f.d.d...Z
+00000f10: 0b64 0853 0029 0eda 0b43 7573 746f 6d4d  .d.S.)...CustomM
+00000f20: 6f64 656c 6301 0000 0000 0000 0000 0000  odelc...........
+00000f30: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000f40: 0000 6400 7c00 5f00 6400 5300 a901 4e29  ..d.|._.d.S...N)
+00000f50: 01da 056d 6f64 656c 2901 7222 0000 0072  ...model).r"...r
+00000f60: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+00000f70: 5f5f 696e 6974 5f5f 5700 0000 7302 0000  __init__W...s...
+00000f80: 000a 017a 1443 7573 746f 6d4d 6f64 656c  ...z.CustomModel
+00000f90: 2e5f 5f69 6e69 745f 5fda 0778 5f74 7261  .__init__..x_tra
+00000fa0: 696e da06 785f 7465 7374 da07 795f 7472  in..x_test..y_tr
+00000fb0: 6169 6eda 0679 5f74 6573 7472 1200 0000  ain..y_testr....
+00000fc0: 4e63 0500 0000 0000 0000 0000 0000 0500  Nc..............
+00000fd0: 0000 0400 0000 4300 0000 731a 0000 0074  ......C...s....t
+00000fe0: 0083 007c 005f 017c 006a 01a0 027c 017c  ...|._.|.j...|.|
+00000ff0: 03a1 0201 0064 0053 0072 5300 0000 2903  .....d.S.rS...).
+00001000: 7204 0000 0072 5400 0000 7244 0000 0029  r....rT...rD...)
+00001010: 0572 2200 0000 7256 0000 0072 5700 0000  .r"...rV...rW...
+00001020: 7258 0000 0072 5900 0000 7218 0000 0072  rX...rY...r....r
+00001030: 1800 0000 7219 0000 0072 4400 0000 5a00  ....r....rD...Z.
+00001040: 0000 7304 0000 0008 0712 017a 0f43 7573  ..s........z.Cus
+00001050: 746f 6d4d 6f64 656c 2e66 6974 721f 0000  tomModel.fitr...
+00001060: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
+00001070: 0000 0300 0000 4300 0000 7320 0000 007c  ......C...s ...|
+00001080: 006a 00a0 017c 01a1 017d 027c 006a 00a0  .j...|...}.|.j..
+00001090: 027c 01a1 017d 037c 027c 0366 0253 0072  .|...}.|.|.f.S.r
+000010a0: 5300 0000 2903 7254 0000 005a 0d70 7265  S...).rT...Z.pre
+000010b0: 6469 6374 5f70 726f 6261 7246 0000 0029  dict_probarF...)
+000010c0: 0472 2200 0000 721f 0000 00da 1070 7265  .r"...r......pre
+000010d0: 6469 6374 6564 5f70 726f 6261 73da 1170  dicted_probas..p
+000010e0: 7265 6469 6374 6564 5f63 6c61 7373 6573  redicted_classes
+000010f0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00001100: 4600 0000 6400 0000 7306 0000 000c 010c  F...d...s.......
+00001110: 0108 017a 1343 7573 746f 6d4d 6f64 656c  ...z.CustomModel
+00001120: 2e70 7265 6469 6374 290c 722f 0000 0072  .predict).r/...r
+00001130: 3000 0000 7231 0000 0072 5500 0000 722a  0...r1...rU...r*
+00001140: 0000 0072 3200 0000 722b 0000 0072 4400  ...r2...r+...rD.
+00001150: 0000 7203 0000 0072 0e00 0000 720d 0000  ..r....r....r...
+00001160: 0072 4600 0000 7218 0000 0072 1800 0000  .rF...r....r....
+00001170: 7218 0000 0072 1900 0000 7252 0000 0056  r....r....rR...V
+00001180: 0000 0073 1c00 0000 0800 0801 0203 0402  ...s............
+00001190: 02fe 0403 02fd 0404 02fc 0405 02fb 0206  ................
+000011a0: 0afa 200a 7252 0000 0063 0000 0000 0000  .. .rR...c......
+000011b0: 0000 0000 0000 0d00 0000 0a00 0000 4300  ..............C.
+000011c0: 0000 73b4 0200 0074 0083 007d 0074 0183  ..s....t...}.t..
+000011d0: 007d 0164 017c 015f 0264 027c 015f 0364  .}.d.|._.d.|._.d
+000011e0: 037c 015f 0447 0064 0464 0584 0064 0574  .|._.G.d.d...d.t
+000011f0: 0583 037d 027c 0283 007d 0374 0664 0664  ...}.|...}.t.d.d
+00001200: 077c 007c 017c 0364 088d 057d 0474 07a0  .|.|.|.d...}.t..
+00001210: 0864 0964 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001220: 0164 0b64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001230: 0164 0c64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001240: 0164 0d64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001250: 0164 0e64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001260: 0164 0f64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001270: 0164 109c 06a1 017d 0574 07a0 0a67 0064  .d.....}.t...g.d
+00001280: 11a2 01a1 017d 0674 07a0 0864 1264 0a84  .....}.t...d.d..
+00001290: 0074 0964 0183 0144 0083 0164 1364 0a84  .t.d...D...d.d..
+000012a0: 0074 0964 0183 0144 0083 0164 1464 0a84  .t.d...D...d.d..
+000012b0: 0074 0964 0183 0144 0083 0164 1564 0a84  .t.d...D...d.d..
+000012c0: 0074 0964 0183 0144 0083 0164 1664 0a84  .t.d...D...d.d..
+000012d0: 0074 0964 0183 0144 0083 0164 1764 0a84  .t.d...D...d.d..
+000012e0: 0074 0964 0183 0144 0083 0164 109c 06a1  .t.d...D...d....
+000012f0: 017d 077c 067c 0564 073c 007c 04a0 0b7c  .}.|.|.d.<.|...|
+00001300: 0564 07a1 0201 007c 04a0 0c7c 07a1 015c  .d.....|...|...\
+00001310: 027d 087d 0974 0d6a 0e7d 0a74 0f7c 087c  .}.}.t.j.}.t.|.|
+00001320: 0a83 027d 0b7c 0b73 f864 1864 1974 10a0  ...}.|.s.d.d.t..
+00001330: 11a1 0076 0073 bd74 12a0 1374 0fa1 0172  ...v.s.t...t...r
+00001340: c274 12a0 1474 0fa1 016e 0164 1964 1a74  .t...t...n.d.d.t
+00001350: 10a0 11a1 0076 0073 ce74 12a0 137c 08a1  .....v.s.t...|..
+00001360: 0172 d374 12a0 147c 08a1 016e 0164 1a64  .r.t...|...n.d.d
+00001370: 1b74 10a0 11a1 0076 0073 df74 12a0 1374  .t.....v.s.t...t
+00001380: 0da1 0172 e474 12a0 1474 0da1 016e 0164  ...r.t...t...n.d
+00001390: 1b74 12a0 147c 0aa1 0174 12a0 147c 0ba1  .t...|...t...|..
+000013a0: 0164 1c9c 0516 007d 0c74 1574 12a0 167c  .d.....}.t.t...|
+000013b0: 0ca1 0183 0182 0164 0004 007d 0a7d 0b74  .......d...}.}.t
+000013c0: 0d6a 0e7d 0a74 0f7c 097c 0a83 027d 0b7c  .j.}.t.|.|...}.|
+000013d0: 0b90 0173 5464 1864 1974 10a0 11a1 0076  ...sTd.d.t.....v
+000013e0: 0090 0173 1574 12a0 1374 0fa1 0190 0172  ...s.t...t.....r
+000013f0: 1a74 12a0 1474 0fa1 016e 0164 1964 1d74  .t...t...n.d.d.t
+00001400: 10a0 11a1 0076 0090 0173 2874 12a0 137c  .....v...s(t...|
+00001410: 09a1 0190 0172 2d74 12a0 147c 09a1 016e  .....r-t...|...n
+00001420: 0164 1d64 1b74 10a0 11a1 0076 0090 0173  .d.d.t.....v...s
+00001430: 3b74 12a0 1374 0da1 0190 0172 4074 12a0  ;t...t.....r@t..
+00001440: 1474 0da1 016e 0164 1b74 12a0 147c 0aa1  .t...n.d.t...|..
+00001450: 0174 12a0 147c 0ba1 0164 1c9c 0516 007d  .t...|...d.....}
+00001460: 0c74 1574 12a0 167c 0ca1 0183 0182 0164  .t.t...|.......d
+00001470: 0004 007d 0a7d 0b64 0053 0029 1e4e 721e  ...}.}.d.S.).Nr.
+00001480: 0000 0054 7220 0000 0063 0000 0000 0000  ...Tr ...c......
+00001490: 0000 0000 0000 0000 0000 0c00 0000 0000  ................
+000014a0: 0000 7386 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000014b0: 0f64 0265 0366 0287 0066 0164 0364 0484  .d.e.f...f.d.d..
+000014c0: 0d5a 0464 0565 056a 0664 0665 056a 0764  .Z.d.e.j.d.e.j.d
+000014d0: 0765 0865 056a 0665 0965 056a 0719 0066  .e.e.j.e.e.j...f
+000014e0: 0219 0066 0664 0864 0984 045a 0a09 0a09  ...f.d.d...Z....
+000014f0: 0b64 1064 0565 056a 0664 0665 0965 056a  .d.d.e.j.d.e.e.j
+00001500: 0719 0064 0c65 0b64 0765 0865 056a 0665  ...d.e.d.e.e.j.e
+00001510: 0965 056a 0719 0066 0219 0066 0864 0d64  .e.j...f...f.d.d
+00001520: 0e84 055a 0c87 0004 005a 0d53 0029 117a  ...Z.....Z.S.).z
+00001530: 3674 6573 745f 626c 7565 6361 7374 5f77  6test_bluecast_w
+00001540: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
+00001550: 2e3c 6c6f 6361 6c73 3e2e 5246 4543 5653  .<locals>.RFECVS
+00001560: 656c 6563 746f 7272 0100 0000 7214 0000  electorr....r...
+00001570: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00001580: 0000 0800 0000 1300 0000 7342 0000 0074  ..........sB...t
+00001590: 0083 00a0 01a1 0001 0064 007c 005f 027c  .........d.|._.|
+000015a0: 017c 005f 0374 0474 05a0 06a1 0064 0174  .|._.t.t.....d.t
+000015b0: 0764 027c 0164 0364 048d 0364 0174 0874  .d.|.d.d...d.t.t
+000015c0: 0983 0164 0264 058d 067c 005f 0a64 0053  ...d.d...|._.d.S
+000015d0: 0029 064e 721b 0000 0072 2000 0000 5429  .).Nr....r ...T)
+000015e0: 0272 1400 0000 da07 7368 7566 666c 6529  .r......shuffle)
+000015f0: 065a 0965 7374 696d 6174 6f72 da04 7374  .Z.estimator..st
+00001600: 6570 5a02 6376 5a16 6d69 6e5f 6665 6174  epZ.cvZ.min_feat
+00001610: 7572 6573 5f74 6f5f 7365 6c65 6374 5a07  ures_to_selectZ.
+00001620: 7363 6f72 696e 675a 066e 5f6a 6f62 7329  scoringZ.n_jobs)
+00001630: 0bda 0573 7570 6572 7255 0000 00da 1173  ...superrU.....s
+00001640: 656c 6563 7465 645f 6665 6174 7572 6573  elected_features
+00001650: 7214 0000 0072 0500 0000 da03 7867 625a  r....r......xgbZ
+00001660: 0d58 4742 436c 6173 7369 6669 6572 7208  .XGBClassifierr.
+00001670: 0000 0072 0600 0000 7207 0000 00da 1273  ...r....r......s
+00001680: 656c 6563 7469 6f6e 5f73 7472 6174 6567  election_strateg
+00001690: 7929 0272 2200 0000 7214 0000 00a9 01da  y).r"...r.......
+000016a0: 095f 5f63 6c61 7373 5f5f 7218 0000 0072  .__class__r....r
+000016b0: 1900 0000 7255 0000 0074 0000 0073 1600  ....rU...t...s..
+000016c0: 0000 0a01 0601 0601 0201 0601 0201 0c01  ................
+000016d0: 0201 0601 0201 0cfa 7a3f 7465 7374 5f62  ........z?test_b
+000016e0: 6c75 6563 6173 745f 7769 7468 5f63 7573  luecast_with_cus
+000016f0: 746f 6d5f 6d6f 6465 6c2e 3c6c 6f63 616c  tom_model.<local
+00001700: 733e 2e52 4645 4356 5365 6c65 6374 6f72  s>.RFECVSelector
+00001710: 2e5f 5f69 6e69 745f 5f72 1f00 0000 7224  .__init__r....r$
+00001720: 0000 0072 1200 0000 6303 0000 0000 0000  ...r....c.......
+00001730: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00001740: 0073 3400 0000 7c00 6a00 a001 7c01 7c02  .s4...|.j...|.|.
+00001750: a102 0100 7c00 6a00 6a02 7c00 5f03 7c01  ....|.j.j.|._.|.
+00001760: 6a04 6400 6400 8502 7c00 6a03 6602 1900  j.d.d...|.j.f...
+00001770: 7d01 7c01 7c02 6602 5300 7253 0000 0029  }.|.|.f.S.rS...)
+00001780: 0572 6100 0000 7244 0000 005a 0873 7570  .ra...rD...Z.sup
+00001790: 706f 7274 5f72 5f00 0000 da03 6c6f 6372  port_r_.....locr
+000017a0: 2600 0000 7218 0000 0072 1800 0000 7219  &...r....r....r.
+000017b0: 0000 0072 2700 0000 8100 0000 7308 0000  ...r'.......s...
+000017c0: 000e 030a 0114 0108 017a 4474 6573 745f  .........zDtest_
+000017d0: 626c 7565 6361 7374 5f77 6974 685f 6375  bluecast_with_cu
+000017e0: 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f 6361  stom_model.<loca
+000017f0: 6c73 3e2e 5246 4543 5653 656c 6563 746f  ls>.RFECVSelecto
+00001800: 722e 6669 745f 7472 616e 7366 6f72 6d4e  r.fit_transformN
+00001810: 4672 2800 0000 6304 0000 0000 0000 0000  Fr(...c.........
+00001820: 0000 0004 0000 0003 0000 0053 0000 0073  ...........S...s
+00001830: 1c00 0000 7c01 6a00 6400 6400 8502 7c00  ....|.j.d.d...|.
+00001840: 6a01 6602 1900 7d01 7c01 7c02 6602 5300  j.f...}.|.|.f.S.
+00001850: 7253 0000 0029 0272 6400 0000 725f 0000  rS...).rd...r_..
+00001860: 0072 2c00 0000 7218 0000 0072 1800 0000  .r,...r....r....
+00001870: 7219 0000 0072 2d00 0000 8900 0000 7304  r....r-.......s.
+00001880: 0000 0014 0608 017a 4074 6573 745f 626c  .......z@test_bl
+00001890: 7565 6361 7374 5f77 6974 685f 6375 7374  uecast_with_cust
+000018a0: 6f6d 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  om_model.<locals
+000018b0: 3e2e 5246 4543 5653 656c 6563 746f 722e  >.RFECVSelector.
+000018c0: 7472 616e 7366 6f72 6d29 0172 0100 0000  transform).r....
+000018d0: 722e 0000 0029 0e72 2f00 0000 7230 0000  r....).r/...r0..
+000018e0: 0072 3100 0000 da03 696e 7472 5500 0000  .r1.....intrU...
+000018f0: 722a 0000 0072 3200 0000 722b 0000 0072  r*...r2...r+...r
+00001900: 0300 0000 7202 0000 0072 2700 0000 7233  ....r....r'...r3
+00001910: 0000 0072 2d00 0000 da0d 5f5f 636c 6173  ...r-.....__clas
+00001920: 7363 656c 6c5f 5f72 1800 0000 7218 0000  scell__r....r...
+00001930: 0072 6200 0000 7219 0000 00da 0d52 4645  .rb...r......RFE
+00001940: 4356 5365 6c65 6374 6f72 7300 0000 7328  CVSelectors...s(
+00001950: 0000 0008 0014 0102 0d04 0102 ff04 0102  ................
+00001960: ff12 020a fe02 0b02 0104 fc04 0202 fe08  ................
+00001970: 0302 fd02 0402 fc12 0512 fb72 6700 0000  ...........rg...
+00001980: 7235 0000 0072 2400 0000 2905 7236 0000  r5...r$...).r6..
+00001990: 0072 3700 0000 5a08 6d6c 5f6d 6f64 656c  .r7...Z.ml_model
+000019a0: 7238 0000 00da 1763 7573 746f 6d5f 6665  r8.....custom_fe
+000019b0: 6174 7572 655f 7365 6c65 6374 6f72 6301  ature_selectorc.
+000019c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000019d0: 0000 0053 0000 00f3 1000 0000 6700 7c00  ...S........g.|.
+000019e0: 5d04 7d01 7c01 9102 7102 5300 7218 0000  ].}.|...q.S.r...
+000019f0: 0072 1800 0000 a902 da02 2e30 da01 6972  .r.........0..ir
+00001a00: 1800 0000 7218 0000 0072 1900 0000 da0a  ....r....r......
+00001a10: 3c6c 6973 7463 6f6d 703e a000 0000 f302  <listcomp>......
+00001a20: 0000 0010 007a 3374 6573 745f 626c 7565  .....z3test_blue
+00001a30: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
+00001a40: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
+00001a50: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+00001a60: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
+00001a70: 0000 0072 6900 0000 7218 0000 0072 1800  ...ri...r....r..
+00001a80: 0000 726a 0000 0072 1800 0000 7218 0000  ..rj...r....r...
+00001a90: 0072 1900 0000 726d 0000 00a1 0000 0072  .r....rm.......r
+00001aa0: 6e00 0000 6301 0000 0000 0000 0000 0000  n...c...........
+00001ab0: 0002 0000 0003 0000 0053 0000 0072 6900  .........S...ri.
+00001ac0: 0000 7218 0000 0072 1800 0000 726a 0000  ..r....r....rj..
+00001ad0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001ae0: 726d 0000 00a2 0000 0072 6e00 0000 6301  rm.......rn...c.
+00001af0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001b00: 0000 0053 0000 0072 6900 0000 7218 0000  ...S...ri...r...
+00001b10: 0072 1800 0000 726a 0000 0072 1800 0000  .r....rj...r....
+00001b20: 7218 0000 0072 1900 0000 726d 0000 00a3  r....r....rm....
+00001b30: 0000 0072 6e00 0000 6301 0000 0000 0000  ...rn...c.......
+00001b40: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00001b50: 0072 6900 0000 7218 0000 0072 1800 0000  .ri...r....r....
+00001b60: 726a 0000 0072 1800 0000 7218 0000 0072  rj...r....r....r
+00001b70: 1900 0000 726d 0000 00a4 0000 0072 6e00  ....rm.......rn.
+00001b80: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001b90: 0000 0003 0000 0053 0000 0072 6900 0000  .......S...ri...
+00001ba0: 7218 0000 0072 1800 0000 726a 0000 0072  r....r....rj...r
+00001bb0: 1800 0000 7218 0000 0072 1900 0000 726d  ....r....r....rm
+00001bc0: 0000 00a5 0000 0072 6e00 0000 2906 5a08  .......rn...).Z.
+00001bd0: 6665 6174 7572 6531 5a08 6665 6174 7572  feature1Z.featur
+00001be0: 6532 5a08 6665 6174 7572 6533 5a08 6665  e2Z.feature3Z.fe
+00001bf0: 6174 7572 6534 5a08 6665 6174 7572 6535  ature4Z.feature5
+00001c00: 5a08 6665 6174 7572 6536 290a 7201 0000  Z.feature6).r...
+00001c10: 0072 1b00 0000 7201 0000 0072 1b00 0000  .r....r....r....
+00001c20: 7201 0000 0072 1b00 0000 7201 0000 0072  r....r....r....r
+00001c30: 1b00 0000 7201 0000 0072 1b00 0000 6301  ....r....r....c.
+00001c40: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001c50: 0000 0053 0000 0072 6900 0000 7218 0000  ...S...ri...r...
+00001c60: 0072 1800 0000 726a 0000 0072 1800 0000  .r....rj...r....
+00001c70: 7218 0000 0072 1900 0000 726d 0000 00ab  r....r....rm....
+00001c80: 0000 0072 6e00 0000 6301 0000 0000 0000  ...rn...c.......
+00001c90: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00001ca0: 0072 6900 0000 7218 0000 0072 1800 0000  .ri...r....r....
+00001cb0: 726a 0000 0072 1800 0000 7218 0000 0072  rj...r....r....r
+00001cc0: 1900 0000 726d 0000 00ac 0000 0072 6e00  ....rm.......rn.
+00001cd0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001ce0: 0000 0003 0000 0053 0000 0072 6900 0000  .......S...ri...
+00001cf0: 7218 0000 0072 1800 0000 726a 0000 0072  r....r....rj...r
+00001d00: 1800 0000 7218 0000 0072 1900 0000 726d  ....r....r....rm
+00001d10: 0000 00ad 0000 0072 6e00 0000 6301 0000  .......rn...c...
+00001d20: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00001d30: 0053 0000 0072 6900 0000 7218 0000 0072  .S...ri...r....r
+00001d40: 1800 0000 726a 0000 0072 1800 0000 7218  ....rj...r....r.
+00001d50: 0000 0072 1900 0000 726d 0000 00ae 0000  ...r....rm......
+00001d60: 0072 6e00 0000 6301 0000 0000 0000 0000  .rn...c.........
+00001d70: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
+00001d80: 6900 0000 7218 0000 0072 1800 0000 726a  i...r....r....rj
+00001d90: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00001da0: 0000 726d 0000 00af 0000 0072 6e00 0000  ..rm.......rn...
+00001db0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001dc0: 0003 0000 0053 0000 0072 6900 0000 7218  .....S...ri...r.
+00001dd0: 0000 0072 1800 0000 726a 0000 0072 1800  ...r....rj...r..
+00001de0: 0000 7218 0000 0072 1900 0000 726d 0000  ..r....r....rm..
+00001df0: 00b0 0000 0072 6e00 0000 7a52 6173 7365  .....rn...zRasse
+00001e00: 7274 2025 2870 7936 2973 0a7b 2528 7079  rt %(py6)s.{%(py
+00001e10: 3629 7320 3d20 2528 7079 3029 7328 2528  6)s = %(py0)s(%(
+00001e20: 7079 3129 732c 2025 2870 7934 2973 0a7b  py1)s, %(py4)s.{
+00001e30: 2528 7079 3429 7320 3d20 2528 7079 3229  %(py4)s = %(py2)
+00001e40: 732e 6e64 6172 7261 790a 7d29 0a7d 7229  s.ndarray.}).}r)
+00001e50: 0000 0072 5a00 0000 da02 6e70 2905 723d  ...rZ.....np).r=
+00001e60: 0000 0072 3e00 0000 5a03 7079 325a 0370  ...r>...Z.py2Z.p
+00001e70: 7934 723f 0000 0072 5b00 0000 2917 7252  y4r?...r[...).rR
+00001e80: 0000 0072 0a00 0000 7241 0000 0072 4200  ...r....rA...rB.
+00001e90: 0000 7243 0000 0072 0f00 0000 7209 0000  ..rC...r....r...
+00001ea0: 0072 2a00 0000 7232 0000 00da 0572 616e  .r*...r2.....ran
+00001eb0: 6765 722b 0000 0072 4400 0000 7246 0000  ger+...rD...rF..
+00001ec0: 0072 6f00 0000 da07 6e64 6172 7261 7972  .ro.....ndarrayr
+00001ed0: 2900 0000 724a 0000 0072 4b00 0000 7248  )...rJ...rK...rH
+00001ee0: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
+00001ef0: 0000 724f 0000 0029 0d5a 0c63 7573 746f  ..rO...).Z.custo
+00001f00: 6d5f 6d6f 6465 6c72 5000 0000 7267 0000  m_modelrP...rg..
+00001f10: 0072 6800 0000 da08 626c 7565 6361 7374  .rh.....bluecast
+00001f20: 7256 0000 0072 5800 0000 7257 0000 0072  rV...rX...rW...r
+00001f30: 5a00 0000 725b 0000 005a 0b40 7079 5f61  Z...r[...Z.@py_a
+00001f40: 7373 6572 7433 5a0b 4070 795f 6173 7365  ssert3Z.@py_asse
+00001f50: 7274 355a 0b40 7079 5f66 6f72 6d61 7437  rt5Z.@py_format7
+00001f60: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00001f70: 1f74 6573 745f 626c 7565 6361 7374 5f77  .test_bluecast_w
+00001f80: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
+00001f90: 6a00 0000 734c 0000 0006 0206 0106 0106  j...sL..........
+00001fa0: 0106 0110 0306 1f02 0302 0102 0102 0102  ................
+00001fb0: 0102 0106 fb04 0910 0210 0110 0110 0110  ................
+00001fc0: 0110 0104 fa04 ff0e 0a04 0110 0210 0110  ................
+00001fd0: 0110 0110 0110 0104 fa04 ff08 0b0c 030e  ................
+00001fe0: 03aa 03bc 0172 7300 0000 292c da08 6275  .....rs...),..bu
+00001ff0: 696c 7469 6e73 724a 0000 00da 195f 7079  iltinsrJ....._py
+00002000: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00002010: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00002020: 6eda 0772 6577 7269 7465 7248 0000 00da  n..rewriterH....
+00002030: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00002040: 00da 056e 756d 7079 726f 0000 005a 0670  ...numpyro...Z.p
+00002050: 616e 6461 7372 2a00 0000 da06 7079 7465  andasr*.....pyte
+00002060: 7374 5a07 7867 626f 6f73 7472 6000 0000  stZ.xgboostr`...
+00002070: 5a10 736b 6c65 6172 6e2e 656e 7365 6d62  Z.sklearn.ensemb
+00002080: 6c65 7204 0000 005a 1973 6b6c 6561 726e  ler....Z.sklearn
+00002090: 2e66 6561 7475 7265 5f73 656c 6563 7469  .feature_selecti
+000020a0: 6f6e 7205 0000 005a 0f73 6b6c 6561 726e  onr....Z.sklearn
+000020b0: 2e6d 6574 7269 6373 7206 0000 0072 0700  .metricsr....r..
+000020c0: 0000 5a17 736b 6c65 6172 6e2e 6d6f 6465  ..Z.sklearn.mode
+000020d0: 6c5f 7365 6c65 6374 696f 6e72 0800 0000  l_selectionr....
+000020e0: 5a18 626c 7565 6361 7374 2e62 6c75 6570  Z.bluecast.bluep
+000020f0: 7269 6e74 732e 6361 7374 7209 0000 005a  rints.castr....Z
+00002100: 1f62 6c75 6563 6173 742e 636f 6e66 6967  .bluecast.config
+00002110: 2e74 7261 696e 696e 675f 636f 6e66 6967  .training_config
+00002120: 720a 0000 0072 0b00 0000 5a22 626c 7565  r....r....Z"blue
+00002130: 6361 7374 2e6d 6c5f 6d6f 6465 6c6c 696e  cast.ml_modellin
+00002140: 672e 6261 7365 5f63 6c61 7373 6573 720c  g.base_classesr.
+00002150: 0000 0072 0d00 0000 720e 0000 005a 1d62  ...r....r....Z.b
+00002160: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
+00002170: 7373 696e 672e 6375 7374 6f6d 720f 0000  ssing.customr...
+00002180: 005a 2462 6c75 6563 6173 742e 7465 7374  .Z$bluecast.test
+00002190: 732e 6d61 6b65 5f64 6174 612e 6372 6561  s.make_data.crea
+000021a0: 7465 5f64 6174 6172 1100 0000 da07 6669  te_datar......fi
+000021b0: 7874 7572 6572 3200 0000 721a 0000 0072  xturer2...r....r
+000021c0: 5100 0000 7252 0000 0072 7300 0000 7218  Q...rR...rs...r.
+000021d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+000021e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000021f0: 7326 0000 002a 0008 0208 0108 0108 010c  s&...*..........
+00002200: 010c 0110 010c 010c 0210 0114 010c 050c  ................
+00002210: 0104 031c 0108 0610 380c 14              ........8..
```

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 24 15:55:23 2023 UTC, .py size: 2295 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 eb11 9764 f708 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 cad1 9764 f808 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
 00000060: 6c0a 5a0b 6400 6401 6c0c 5a0c 6400 6403  l.Z.d.d.l.Z.d.d.
 00000070: 6c0d 6d0e 5a0e 0100 6400 6404 6c0f 6d10  l.m.Z...d.d.l.m.
@@ -63,15 +63,15 @@
 000003e0: 127c 06a1 0164 149c 0416 007d 0774 1374  .|...d.....}.t.t
 000003f0: 10a0 147c 07a1 0183 0182 0164 157d 0664  ...|.......d.}.d
 00000400: 1553 0029 167a 2254 6573 7420 7468 6174  .S.).z"Test that
 00000410: 2074 6573 7473 2074 6865 2042 6c75 6543   tests the BlueC
 00000420: 6173 7420 636c 6173 73e9 c800 0000 e914  ast class.......
 00000430: 0000 0029 01da 0c72 616e 646f 6d5f 7374  ...)...random_st
 00000440: 6174 65e9 6400 0000 e915 0000 00e9 1000  ate.d...........
-00000450: 0000 e90a 0000 0054 720d 0000 00da 0662  .......Tr......b
+00000450: 0000 e90a 0000 0046 720d 0000 00da 0662  .......Fr......b
 00000460: 696e 6172 79da 0674 6172 6765 7429 04da  inary..target)..
 00000470: 0d63 6c61 7373 5f70 726f 626c 656d da0d  .class_problem..
 00000480: 7461 7267 6574 5f63 6f6c 756d 6eda 0d63  target_column..c
 00000490: 6f6e 665f 7472 6169 6e69 6e67 da0c 636f  onf_training..co
 000004a0: 6e66 5f78 6762 6f6f 7374 720c 0000 0029  nf_xgboostr....)
 000004b0: 01da 0461 7869 7329 01da 0a74 6172 6765  ...axis)...targe
 000004c0: 745f 636f 6c7a 3561 7373 6572 7420 2528  t_colz5assert %(
```

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.5/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.5/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/make_data/create_data.py` & `bluecast-0.5/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_cast.py` & `bluecast-0.5/bluecast/tests/test_cast.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 import xgboost as xgb
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_selection import RFECV
 from sklearn.metrics import make_scorer, matthews_corrcoef
 from sklearn.model_selection import StratifiedKFold
 
 from bluecast.blueprints.cast import BlueCast
-from bluecast.config.training_config import (
-    FeatureSelectionConfig,
-    TrainingConfig,
-    XgboostTuneParamsConfig,
-)
+from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
 from bluecast.ml_modelling.base_classes import (
     BaseClassMlModel,
     PredictedClasses,
     PredictedProbas,
 )
 from bluecast.preprocessing.custom import CustomPreprocessing
 from bluecast.tests.make_data.create_data import create_synthetic_dataframe
@@ -112,32 +108,54 @@
     custom_model = CustomModel()
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
     train_config.enable_feature_selection = True
     train_config.hypertuning_cv_folds = 2
 
     # add custom feature selection
-    custom_feat_sel = FeatureSelectionConfig()
-    # custom_feat_sel.execute_selection = False
-    custom_feat_sel.selection_strategy = RFECV(
-        estimator=xgb.XGBClassifier(),
-        step=1,
-        cv=StratifiedKFold(2, random_state=0, shuffle=True),
-        min_features_to_select=1,
-        scoring=make_scorer(matthews_corrcoef),
-        n_jobs=1,
-    )
+    class RFECVSelector(CustomPreprocessing):
+        def __init__(self, random_state: int = 0):
+            super().__init__()
+            self.selected_features = None
+            self.random_state = random_state
+            self.selection_strategy: RFECV = RFECV(
+                estimator=xgb.XGBClassifier(),
+                step=1,
+                cv=StratifiedKFold(2, random_state=random_state, shuffle=True),
+                min_features_to_select=1,
+                scoring=make_scorer(matthews_corrcoef),
+                n_jobs=2,
+            )
+
+        def fit_transform(
+            self, df: pd.DataFrame, target: pd.Series
+        ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+            self.selection_strategy.fit(df, target)
+            self.selected_features = self.selection_strategy.support_
+            df = df.loc[:, self.selected_features]
+            return df, target
+
+        def transform(
+            self,
+            df: pd.DataFrame,
+            target: Optional[pd.Series] = None,
+            predicton_mode: bool = False,
+        ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+            df = df.loc[:, self.selected_features]
+            return df, target
+
+    custom_feature_selector = RFECVSelector()
 
     # Create an instance of the BlueCast class with the custom model
     bluecast = BlueCast(
         class_problem="binary",
         target_column="target",
         ml_model=custom_model,
         conf_training=train_config,
-        conf_feature_selection=custom_feat_sel,
+        custom_feature_selector=custom_feature_selector,
     )
 
     # Create some sample data for testing
     x_train = pd.DataFrame(
         {
             "feature1": [i for i in range(10)],
             "feature2": [i for i in range(10)],
```

### Comparing `bluecast-0.4.2/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.5/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.5/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_datetime_features.py` & `bluecast-0.5/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.5/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.5/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_load_for_production.py` & `bluecast-0.5/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.5/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_save_to_production.py` & `bluecast-0.5/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_schema_checks.py` & `bluecast-0.5/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_shap_explanations.py` & `bluecast-0.5/bluecast/tests/test_shap_explanations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     df_train = create_synthetic_dataframe(200, random_state=20)
     df_val = create_synthetic_dataframe(100, random_state=21)
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.num_leaves_max = 16
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
-    train_config.enable_feature_selection = True
+    train_config.enable_feature_selection = False
     train_config.hypertuning_cv_folds = 2
 
     automl = BlueCast(
         class_problem="binary",
         target_column="target",
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
```

### Comparing `bluecast-0.4.2/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.5/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.5/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/bluecast/tests/test_train_test_split.py` & `bluecast-0.5/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.4.2/pyproject.toml` & `bluecast-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.4.2"
+version = "0.5"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `bluecast-0.4.2/PKG-INFO` & `bluecast-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.4.2
+Version: 0.5
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -47,15 +47,16 @@
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
 BlueCast focuses on a few model architectures (on default Xgboost
 only) and a few preprocessing options (only what is
 needed for Xgboost). This allows for a much faster development
 cycle and a much more stable codebase while also having as few dependencies
 as possible for the library. Despite being lightweight in its core BlueCast
-offers high customization options for advanced users.
+offers high customization options for advanced users. Find
+the full documentation [here](https://bluecast.readthedocs.io/en/latest/).
 
 <!-- toc -->
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
@@ -293,49 +294,67 @@
         conf_training=train_config,
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
-Also this step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
-Otherwise the pipeline will fail. To surpass the `RFECV` limitation a custom feature
-selection algorithm can also be passed as part of a custom last mile computation.
-Here is an example adjusting the in-built solution via `RFECV`:
+Also this step can be customized. The following example shows how to:
 
 ```sh
 from bluecast.config.training_config import FeatureSelectionConfig
 from bluecast.config.training_config import TrainingConfig
+from bluecast.preprocessing.custom import CustomPreprocessing
 from sklearn.feature_selection import RFECV
 from sklearn.metrics import make_scorer, matthews_corrcoef
 from sklearn.model_selection import StratifiedKFold
+from typing import Optional, Tuple
 
 
 # Create a custom training config and adjust general training parameters
 train_config = TrainingConfig()
 train_config.enable_feature_selection = True
 
 # add custom feature selection
-custom_feat_sel = FeatureSelectionConfig()
-# custom_feat_sel.execute_selection = False
-custom_feat_sel.selection_strategy = RFECV(
-    estimator=xgb.XGBClassifier(),
-    step=1,
-    cv=StratifiedKFold(10, random_state=0, shuffle=True),
-    min_features_to_select=1,
-    scoring=make_scorer(matthews_corrcoef),
-    n_jobs=1,
-)
+class RFECVSelector(CustomPreprocessing):
+    def __init__(self, random_state: int = 0):
+        super().__init__()
+        self.selected_features = None
+        self.random_state = random_state
+        self.selection_strategy: RFECV = RFECV(
+            estimator=xgb.XGBClassifier(),
+            step=1,
+            cv=StratifiedKFold(5, random_state=random_state, shuffle=True),
+            min_features_to_select=1,
+            scoring=make_scorer(matthews_corrcoef),
+            n_jobs=2,
+        )
+
+    def fit_transform(self, df: pd.DataFrame, target: pd.Series) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        self.selection_strategy.fit(df, target)
+        self.selected_features = self.selection_strategy.support_
+        df = df.loc[:, self.selected_features]
+        return df, target
+
+    def transform(self,
+                  df: pd.DataFrame,
+                  target: Optional[pd.Series] = None,
+                  predicton_mode: bool = False) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        df = df.loc[:, self.selected_features]
+        return df, target
+
+custom_feature_selector = RFECVSelector()
 
 # Create an instance of the BlueCast class with the custom model
 bluecast = BlueCast(
     class_problem="binary",
     target_column="target",
     conf_feature_selection=custom_feat_sel,
     conf_training=train_config,
+    custom_feature_selector=custom_feature_selector,
 
 # Create some sample data for testing
 x_train = pd.DataFrame(
     {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
 )
 y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
 x_test = pd.DataFrame(
```

