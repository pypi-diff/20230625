# Comparing `tmp/fb-python-sdk-1.1.4.tar.gz` & `tmp/fb-python-sdk-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.1.4.tar", last modified: Fri Jun 23 00:07:43 2023, max compression
+gzip compressed data, was "fb-python-sdk-1.1.5.tar", last modified: Sun Jun 25 15:58:25 2023, max compression
```

## Comparing `fb-python-sdk-1.1.4.tar` & `fb-python-sdk-1.1.5.tar`

### file list

```diff
@@ -1,54 +1,51 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.762469 fb-python-sdk-1.1.4/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.4/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)    12546 2023-06-23 00:07:43.762018 fb-python-sdk-1.1.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)    11474 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/README.md
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/dev-requirements.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.745746 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    12546 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1249 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      218 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       34 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.754281 fb-python-sdk-1.1.4/fbclient/
--rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/category.py
--rw-r--r--   0 mac        (501) staff       (20)    18476 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/client.py
--rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.4/fbclient/common_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.4/fbclient/config.py
--rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)    12387 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.4/fbclient/event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/event_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8579 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/flag_change_notification.py
--rw-r--r--   0 mac        (501) staff       (20)     9861 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     2126 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/notice_broadcaster.py
--rw-r--r--   0 mac        (501) staff       (20)     3794 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/status.py
--rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/status_types.py
--rw-r--r--   0 mac        (501) staff       (20)    12866 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/streaming.py
--rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.4/fbclient/update_processor.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.757039 fb-python-sdk-1.1.4/fbclient/utils/
--rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/fbclient/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/http_client.py
--rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/repeatable_task.py
--rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/rwlock.py
--rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/version.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.758493 fb-python-sdk-1.1.4/intergration_tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.4/intergration_tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.4/intergration_tests/readme.py
--rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.4/intergration_tests/run_in_start_no_wait.py
--rw-------   0 mac        (501) staff       (20)     1898 2023-06-22 22:09:31.000000 fb-python-sdk-1.1.4/intergration_tests/run_in_start_wait.py
--rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 00:07:43.762573 fb-python-sdk-1.1.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.4/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.761510 fb-python-sdk-1.1.4/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.4/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/tests/test_data_update_status_provider.py
--rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)    10800 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/tests/test_fbclient.py
--rw-r--r--   0 mac        (501) staff       (20)     3423 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/tests/test_flag_change_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fbclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/flag_change_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/notice_broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/status_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/update_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fbclient/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/release/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/release/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_data_update_status_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_fbclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_flag_change_notification.py
```

### Comparing `fb-python-sdk-1.1.4/LICENSE` & `fb-python-sdk-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/PKG-INFO` & `fb-python-sdk-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -166,18 +166,25 @@
 
 If you would like to get variations of all feature flags in a special environment, you can use `fbclient.client.FBClient.get_all_latest_flag_variations`, SDK will return `fbclient.common_types.AllFlagStates`, that explain the details of all feature flags. `fbclient.common_types.AllFlagStates.get()` returns the detail of a given feature flag key.
 
 ```python
 if client.initialize:
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
-    detail = all_flag_values.get(flag_key, default=None)
+    # get all feature flag keys
+    keys = all_flag_values.keys()
+    for flag_key in keys:
+        # get viariation detail
+        detail = all_flag_values.get(flag_key, default=None)
+        # get viariation
+        value = all_flag_values.get_variation(flag_key, default=None)
 ```
 
-> Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
+> **Note**
+> If evaluation happened before the client is initialized, or you provide the wrong flag key/user for evaluation, the `variation` calls will return the default value. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error reason.
 
 ### Flag Tracking
 
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
```

### Comparing `fb-python-sdk-1.1.4/README.md` & `fb-python-sdk-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,18 +140,25 @@
 
 If you would like to get variations of all feature flags in a special environment, you can use `fbclient.client.FBClient.get_all_latest_flag_variations`, SDK will return `fbclient.common_types.AllFlagStates`, that explain the details of all feature flags. `fbclient.common_types.AllFlagStates.get()` returns the detail of a given feature flag key.
 
 ```python
 if client.initialize:
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
-    detail = all_flag_values.get(flag_key, default=None)
+    # get all feature flag keys
+    keys = all_flag_values.keys()
+    for flag_key in keys:
+        # get viariation detail
+        detail = all_flag_values.get(flag_key, default=None)
+        # get viariation
+        value = all_flag_values.get_variation(flag_key, default=None)
 ```
 
-> Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
+> **Note**
+> If evaluation happened before the client is initialized, or you provide the wrong flag key/user for evaluation, the `variation` calls will return the default value. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error reason.
 
 ### Flag Tracking
 
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
```

### Comparing `fb-python-sdk-1.1.4/fb_python_sdk.egg-info/PKG-INFO` & `fb-python-sdk-1.1.5/fb_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -166,18 +166,25 @@
 
 If you would like to get variations of all feature flags in a special environment, you can use `fbclient.client.FBClient.get_all_latest_flag_variations`, SDK will return `fbclient.common_types.AllFlagStates`, that explain the details of all feature flags. `fbclient.common_types.AllFlagStates.get()` returns the detail of a given feature flag key.
 
 ```python
 if client.initialize:
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
-    detail = all_flag_values.get(flag_key, default=None)
+    # get all feature flag keys
+    keys = all_flag_values.keys()
+    for flag_key in keys:
+        # get viariation detail
+        detail = all_flag_values.get(flag_key, default=None)
+        # get viariation
+        value = all_flag_values.get_variation(flag_key, default=None)
 ```
 
-> Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
+> **Note**
+> If evaluation happened before the client is initialized, or you provide the wrong flag key/user for evaluation, the `variation` calls will return the default value. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error reason.
 
 ### Flag Tracking
 
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
```

### Comparing `fb-python-sdk-1.1.4/fb_python_sdk.egg-info/SOURCES.txt` & `fb-python-sdk-1.1.5/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 fbclient/version.py
 fbclient/utils/__init__.py
 fbclient/utils/exponential_backoff_jitter_strategy.py
 fbclient/utils/http_client.py
 fbclient/utils/repeatable_task.py
 fbclient/utils/rwlock.py
 fbclient/utils/variation_splitting_algorithm.py
-intergration_tests/__init__.py
-intergration_tests/readme.py
-intergration_tests/run_in_start_no_wait.py
-intergration_tests/run_in_start_wait.py
+release/package.json
 tests/__init__.py
 tests/test_data_storage.py
 tests/test_data_update_status_provider.py
 tests/test_evaluator.py
 tests/test_event_processor.py
 tests/test_fbclient.py
 tests/test_flag_change_notification.py
```

### Comparing `fb-python-sdk-1.1.4/fbclient/__init__.py` & `fb-python-sdk-1.1.5/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/category.py` & `fb-python-sdk-1.1.5/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/client.py` & `fb-python-sdk-1.1.5/fbclient/client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/common_types.py` & `fb-python-sdk-1.1.5/fbclient/common_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,32 @@
         :param data: a dictionary containing latest evaluation of all feature flags and their events
         :event_handler: callback function used to send events to feature flag center
         """
         super().__init__(success, reason)
         self._data = dict((ed.key_name, (ed, fb_event)) for ed, fb_event in data.items()) if data else {}
         self._event_handler = event_handler
 
+    def keys(self):
+        """
+        return all feature flag keys
+        """
+        return self._data.keys()
+
+    def get_variation(self, key_name: str, default: Any = None) -> Any:
+        """Return the variation of a given feature flag key
+
+        This method will send event to back to feature flag center immediately
+
+        The default value should be a string, boolean, numeric, or json type.
+
+        :param key_name: key name of the flag
+        :return: the variation of the flag in any type of string, boolean, numeric, or json type
+        """
+        return self.get(key_name, default).variation
+
     def get(self, key_name: str, default: Any = None) -> EvalDetail:
         """Return the flag evaluation details of a given feature flag key
 
         This method will send event to back to feature flag center immediately
 
         The default value should be a string, boolean, numeric, or json type.
```

### Comparing `fb-python-sdk-1.1.4/fbclient/config.py` & `fb-python-sdk-1.1.5/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/data_storage.py` & `fb-python-sdk-1.1.5/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/evaluator.py` & `fb-python-sdk-1.1.5/fbclient/evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/event_processor.py` & `fb-python-sdk-1.1.5/fbclient/event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/event_types.py` & `fb-python-sdk-1.1.5/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/flag_change_notification.py` & `fb-python-sdk-1.1.5/fbclient/flag_change_notification.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/interfaces.py` & `fb-python-sdk-1.1.5/fbclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/notice_broadcaster.py` & `fb-python-sdk-1.1.5/fbclient/notice_broadcaster.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/status.py` & `fb-python-sdk-1.1.5/fbclient/status.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/status_types.py` & `fb-python-sdk-1.1.5/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/streaming.py` & `fb-python-sdk-1.1.5/fbclient/streaming.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/update_processor.py` & `fb-python-sdk-1.1.5/fbclient/update_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/__init__.py` & `fb-python-sdk-1.1.5/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb-python-sdk-1.1.5/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/http_client.py` & `fb-python-sdk-1.1.5/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/repeatable_task.py` & `fb-python-sdk-1.1.5/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/rwlock.py` & `fb-python-sdk-1.1.5/fbclient/utils/rwlock.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/fbclient/utils/variation_splitting_algorithm.py` & `fb-python-sdk-1.1.5/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/setup.py` & `fb-python-sdk-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+import json
 from setuptools import setup, find_packages
 
-version = {}
-
 
 def last_version():
-    with open("./fbclient/version.py") as fp:
-        exec(fp.read(), version)
-    return version['VERSION']
+    with open("./release/package.json") as fp:
+        version = json.load(fp)
+    return version['version']
 
 
 fb_version = last_version()
 
 
 def parse_requirements(filename):
     lineiter = (line.strip() for line in open(filename))
```

### Comparing `fb-python-sdk-1.1.4/tests/test_data_storage.py` & `fb-python-sdk-1.1.5/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/tests/test_data_update_status_provider.py` & `fb-python-sdk-1.1.5/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/tests/test_evaluator.py` & `fb-python-sdk-1.1.5/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/tests/test_event_processor.py` & `fb-python-sdk-1.1.5/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.4/tests/test_fbclient.py` & `fb-python-sdk-1.1.5/tests/test_fbclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -202,23 +202,38 @@
 
 
 def test_get_all_latest_flag_variations():
     with make_fb_client_offline() as client:
         assert client.initialize
         all_states = client.get_all_latest_flag_variations(USER_1)
         ed = all_states.get("ff-test-bool", False)
+        value = all_states.get_variation("ff-test-bool", False)
         assert ed is not None and ed.variation is True
+        assert value is True
+        assert "ff-test-bool" in all_states.keys()
         ed = all_states.get("ff-test-number", -1)
+        value = all_states.get_variation("ff-test-number", -1)
         assert ed is not None and ed.variation == 1
+        assert value == 1
+        assert "ff-test-number" in all_states.keys()
         ed = all_states.get("ff-test-string", 'error')
+        value = all_states.get_variation("ff-test-string", 'error')
         assert ed is not None and ed.variation == "others"
+        assert value == "others"
+        assert "ff-test-string" in all_states.keys()
         ed = all_states.get("ff-test-seg", 'error')
+        value = all_states.get_variation("ff-test-seg", 'error')
         assert ed is not None and ed.variation == "teamA"
+        assert value == "teamA"
+        assert "ff-test-seg" in all_states.keys()
         ed = all_states.get("ff-test-json", {})
+        value = all_states.get_variation("ff-test-json", {})
         assert ed is not None and ed.variation["code"] == 200
+        assert value["code"] == 200
+        assert "ff-test-json" in all_states.keys()
 
 
 def test_variation_argument_error():
     with make_fb_client_offline() as client:
         assert client.initialize
         detail = client.variation_detail("ff-not-existed", USER_1, False)
         assert detail.variation is False
```

### Comparing `fb-python-sdk-1.1.4/tests/test_flag_change_notification.py` & `fb-python-sdk-1.1.5/tests/test_flag_change_notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 from fbclient.interfaces import Notice
 from fbclient.notice_broadcaster import NoticeBroadcater
 
 TEST_NOTICE_TYPE = 'test_notice_type'
 
 
 class TestNotice(Notice):
+    # https://stackoverflow.com/questions/62460557/cannot-collect-test-class-testmain-because-it-has-a-init-constructor-from
+    __test__ = False
+
     def __init__(self, notice_type: str, content: str):
         self.__notice_type = notice_type
         self.__content = content
 
     @property
     def notice_type(self) -> str:
         return self.__notice_type
 
     @property
     def content(self) -> str:
         return self.__content
 
 
 class FakeFlagChangedListener(FlagChangedListener):
+    __test__ = False
+
     def __init__(self, queue: Queue):
         self.__queue = queue
 
     def on_flag_change(self, notice: FlagChangedNotice):
         self.__queue.put(notice)
```

