# Comparing `tmp/apache-airflow-client-2.6.2rc1.tar.gz` & `tmp/apache-airflow-client-2.6.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-client-2.6.2rc1.tar", last modified: Sun Jun 18 19:56:46 2023, max compression
+gzip compressed data, was "apache-airflow-client-2.6.2rc2.tar", last modified: Wed Jun 21 20:07:11 2023, max compression
```

## Comparing `apache-airflow-client-2.6.2rc1.tar` & `apache-airflow-client-2.6.2rc2.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.317438 apache-airflow-client-2.6.2rc1/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10850 2023-01-14 23:05:13.000000 apache-airflow-client-2.6.2rc1/LICENSE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      240 2023-01-14 23:05:13.000000 apache-airflow-client-2.6.2rc1/NOTICE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6453 2023-06-18 19:56:46.317438 apache-airflow-client-2.6.2rc1/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5615 2023-06-18 17:58:01.000000 apache-airflow-client-2.6.2rc1/README.md
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.293439 apache-airflow-client-2.6.2rc1/airflow_client/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      786 2023-06-18 17:54:32.000000 apache-airflow-client-2.6.2rc1/airflow_client/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.293439 apache-airflow-client-2.6.2rc1/airflow_client/client/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9536 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.297438 apache-airflow-client-2.6.2rc1/airflow_client/client/api/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1010 2023-06-18 17:54:33.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13979 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/config_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    39520 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/connection_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    69062 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    61203 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_run_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    15645 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_warning_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    32132 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/dataset_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19853 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/event_log_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19906 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/import_error_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    18391 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/monitoring_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14793 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/permission_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14780 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/plugin_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    34138 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/pool_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14230 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/provider_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    34452 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/role_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    86137 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/task_instance_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    34755 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/user_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    34736 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/variable_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22538 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api/x_com_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    46382 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/api_client.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.297438 apache-airflow-client-2.6.2rc1/airflow_client/client/apis/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2311 2023-06-18 17:54:33.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/apis/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    25588 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/configuration.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13802 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/exceptions.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.305438 apache-airflow-client-2.6.2rc1/airflow_client/client/model/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1134 2023-06-18 17:54:33.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19821 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/action.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22705 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19973 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20253 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_resource.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22847 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/basic_dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20083 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/class_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20186 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/clear_dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    25136 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/clear_task_instances.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20030 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/collection_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20250 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/color.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19983 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/config.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19999 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/config_option.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20200 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/config_section.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24468 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20200 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22885 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20133 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21512 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20125 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_test.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20011 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/cron_expression.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    31229 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22645 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19928 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    38045 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_detail.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24667 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_detail_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    27046 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22712 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19979 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20491 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_schedule_dataset_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20763 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20769 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22797 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20044 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21977 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22725 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19988 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22631 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22832 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20069 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21637 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/error.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22259 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22752 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20009 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20414 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/extra_link.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20009 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/extra_link_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20778 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/health_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20388 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/health_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20772 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22812 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20054 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20039 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/inline_response200.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19794 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/inline_response2001.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21858 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/job.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24999 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/list_dag_runs_form.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    25560 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/list_task_instance_form.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19996 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/metadatabase_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22805 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20073 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    23836 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22378 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22665 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19943 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20393 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/provider.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19988 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/provider_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    23021 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/relative_delta.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19801 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/resource.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20456 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/role.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22665 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/role_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19943 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/role_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    25425 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/schedule_interval.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20452 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/scheduler_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19856 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/set_dag_run_note.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19918 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/set_task_instance_note.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21169 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/sla_miss.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19734 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/tag.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    26402 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19928 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20013 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_extra_links.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    26384 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22832 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20069 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20656 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20145 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_reference_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20746 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_outlet_dataset_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22492 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20487 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/time_delta.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20596 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/trigger.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21690 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/trigger_rule.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20452 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/triggerer_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19972 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_dag_run_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20555 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_task_instance.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22984 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_task_instances_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    26484 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19772 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22765 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20043 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24062 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19793 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_item_roles.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22661 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19769 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22845 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20103 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20150 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20157 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/version_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20449 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/weight_rule.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    23081 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19779 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22802 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20079 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20586 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    90823 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/model_utils.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.305438 apache-airflow-client-2.6.2rc1/airflow_client/client/models/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9210 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/models/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22933 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/client/rest.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.317438 apache-airflow-client-2.6.2rc1/airflow_client/test/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      786 2023-06-18 17:54:33.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9526 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_action.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9942 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9717 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9757 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_resource.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9655 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_basic_dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_class_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9563 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_clear_dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9612 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_clear_task_instances.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_collection_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9519 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_color.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9638 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_config.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9527 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9569 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_option.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9684 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_section.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9832 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9591 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10277 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10060 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9819 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9654 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_test.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_cron_expression.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9700 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10971 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9897 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9684 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10028 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_detail.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9681 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_detail_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9619 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10715 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9945 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9719 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9676 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_schedule_dataset_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9541 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9555 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9552 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10005 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9763 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9869 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9990 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9957 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9728 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9674 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10035 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9785 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9519 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_error.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9541 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9675 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9975 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9741 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9664 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_extra_link.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9715 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_extra_link_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9927 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_health_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9569 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_health_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9708 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10020 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9774 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9604 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_inline_response200.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9611 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_inline_response2001.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9505 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_job.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9592 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_list_dag_runs_form.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9723 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_list_task_instance_form.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9719 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_metadatabase_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9683 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_monitoring_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_permission_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9532 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10000 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9775 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9626 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9512 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9912 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9695 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9540 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9532 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9702 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9576 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_relative_delta.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9540 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_resource.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9628 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_role.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9912 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9695 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9921 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_schedule_interval.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9698 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_scheduler_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9578 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_set_dag_run_note.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9620 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_set_task_instance_note.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9534 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_sla_miss.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9505 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_tag.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10195 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9658 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9700 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_extra_links.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9911 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11213 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10035 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9785 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9633 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9849 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_reference_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9669 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_outlet_dataset_reference.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_time_delta.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9533 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_trigger.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_trigger_rule.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9698 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_triggerer_status.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9606 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_dag_run_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9612 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_task_instance.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9655 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_task_instances_state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9896 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9549 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9970 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9753 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9766 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9648 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_item_roles.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9802 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9577 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10095 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10030 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9797 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9640 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection_item.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_version_info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9555 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_weight_rule.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9745 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9550 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9664 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_api.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9973 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9755 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection_all_of.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9613 2023-06-18 19:43:48.000000 apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection_item.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-18 19:56:46.317438 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6453 2023-06-18 19:56:46.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12530 2023-06-18 19:56:46.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-06-18 19:56:46.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-06-18 19:52:19.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       32 2023-06-18 19:56:46.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       15 2023-06-18 19:56:46.000000 apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/top_level.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      798 2023-06-18 19:56:46.317438 apache-airflow-client-2.6.2rc1/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1519 2023-06-18 19:51:34.000000 apache-airflow-client-2.6.2rc1/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.380117 apache-airflow-client-2.6.2rc2/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10850 2023-01-14 23:05:13.000000 apache-airflow-client-2.6.2rc2/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      240 2023-01-14 23:05:13.000000 apache-airflow-client-2.6.2rc2/NOTICE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6453 2023-06-21 20:07:11.380117 apache-airflow-client-2.6.2rc2/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5615 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/README.md
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.356118 apache-airflow-client-2.6.2rc2/airflow_client/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      786 2023-06-19 23:57:32.000000 apache-airflow-client-2.6.2rc2/airflow_client/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.356118 apache-airflow-client-2.6.2rc2/airflow_client/client/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9536 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.356118 apache-airflow-client-2.6.2rc2/airflow_client/client/api/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1010 2023-06-19 23:57:33.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13979 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/config_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    39520 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/connection_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    69062 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    61203 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_run_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15645 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_warning_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    32132 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/dataset_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19853 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/event_log_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19906 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/import_error_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    18391 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/monitoring_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14793 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/permission_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14780 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/plugin_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    34138 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/pool_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14230 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/provider_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    34452 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/role_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    86137 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/task_instance_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    34755 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/user_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    34736 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/variable_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22538 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api/x_com_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    46382 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/api_client.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.356118 apache-airflow-client-2.6.2rc2/airflow_client/client/apis/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2311 2023-06-19 23:57:33.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/apis/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    25588 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/configuration.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13802 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/exceptions.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.368117 apache-airflow-client-2.6.2rc2/airflow_client/client/model/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1134 2023-06-19 23:57:33.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19821 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/action.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22705 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19973 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20253 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_resource.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22847 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/basic_dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20083 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/class_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20186 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/clear_dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    25136 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/clear_task_instances.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20030 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/collection_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20250 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/color.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19983 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/config.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19999 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/config_option.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20200 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/config_section.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24468 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20200 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22885 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20133 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21512 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20125 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_test.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20011 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/cron_expression.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    31229 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22645 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19928 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    38045 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_detail.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24700 2023-06-21 20:02:53.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_detail_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    27046 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22712 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19979 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20491 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_schedule_dataset_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20763 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20769 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22797 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20044 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21977 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22725 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19988 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22631 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22832 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20069 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21637 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/error.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22259 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22752 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20009 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20414 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/extra_link.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20009 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/extra_link_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20778 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/health_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20388 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/health_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20772 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22812 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20054 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20039 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/inline_response200.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19794 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/inline_response2001.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21858 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/job.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24999 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/list_dag_runs_form.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    25560 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/list_task_instance_form.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19996 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/metadatabase_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22805 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20073 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    23836 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22378 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22665 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19943 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20393 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/provider.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19988 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/provider_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    23021 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/relative_delta.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19801 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/resource.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20456 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/role.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22665 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/role_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19943 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/role_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    25425 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/schedule_interval.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20452 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/scheduler_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19856 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/set_dag_run_note.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19918 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/set_task_instance_note.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21169 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/sla_miss.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19734 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/tag.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    26435 2023-06-21 20:02:53.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19928 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20013 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_extra_links.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    26384 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22832 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20069 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20656 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20145 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_reference_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20746 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_outlet_dataset_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22492 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20487 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/time_delta.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20596 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/trigger.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21690 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/trigger_rule.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20452 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/triggerer_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19972 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_dag_run_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20555 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_task_instance.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22984 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_task_instances_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    26484 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19772 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22765 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20043 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24062 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19793 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_item_roles.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22661 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19769 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22845 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20103 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20150 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20157 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/version_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20449 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/weight_rule.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    23081 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    19779 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22802 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20079 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    20586 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    90823 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/model_utils.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.368117 apache-airflow-client-2.6.2rc2/airflow_client/client/models/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9210 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/models/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22933 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/client/rest.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.380117 apache-airflow-client-2.6.2rc2/airflow_client/test/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      786 2023-06-19 23:57:33.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9526 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_action.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9942 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9717 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9757 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_resource.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9655 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_basic_dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_class_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9563 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_clear_dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9612 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_clear_task_instances.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_collection_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9519 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_color.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9638 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_config.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9527 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9569 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_option.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9684 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_section.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9832 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9591 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10277 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10060 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9819 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9654 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_test.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9583 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_cron_expression.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9700 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10971 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9897 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9684 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10028 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_detail.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9681 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_detail_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9619 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10715 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9945 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9719 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9676 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_schedule_dataset_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9541 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9555 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9552 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10005 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9763 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9869 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9990 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9957 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9728 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9674 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10035 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9785 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9519 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_error.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9541 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9675 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9975 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9741 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9664 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_extra_link.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9715 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_extra_link_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9927 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_health_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9569 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_health_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9708 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10020 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9774 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9604 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_inline_response200.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9611 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_inline_response2001.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9505 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_job.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9592 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_list_dag_runs_form.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9723 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_list_task_instance_form.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9719 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_metadatabase_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9683 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_monitoring_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_permission_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9532 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10000 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9775 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9626 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9512 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9912 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9695 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9540 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9532 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9702 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9576 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_relative_delta.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9540 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_resource.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9628 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_role.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9912 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9695 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9921 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_schedule_interval.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9698 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_scheduler_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9578 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_set_dag_run_note.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9620 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_set_task_instance_note.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9534 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_sla_miss.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9505 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_tag.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10195 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9658 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9700 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_extra_links.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9911 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    11213 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10035 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9785 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9633 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9849 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_reference_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9669 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_outlet_dataset_reference.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9548 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_time_delta.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9533 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_trigger.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_trigger_rule.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9698 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_triggerer_status.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9606 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_dag_run_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9612 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_task_instance.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9655 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_task_instances_state.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9896 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9549 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10013 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9970 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9753 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9766 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9648 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_item_roles.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9802 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9577 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10095 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10030 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9797 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9640 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection_item.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9562 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_version_info.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9555 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_weight_rule.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9745 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9550 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9664 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_api.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9973 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9755 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection_all_of.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9613 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection_item.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-21 20:07:11.380117 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6453 2023-06-21 20:07:11.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12530 2023-06-21 20:07:11.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-06-21 20:07:11.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-06-21 20:04:33.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       32 2023-06-21 20:07:11.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       15 2023-06-21 20:07:11.000000 apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/top_level.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      798 2023-06-21 20:07:11.380117 apache-airflow-client-2.6.2rc2/setup.cfg
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1519 2023-06-21 17:39:26.000000 apache-airflow-client-2.6.2rc2/setup.py
```

### Comparing `apache-airflow-client-2.6.2rc1/LICENSE` & `apache-airflow-client-2.6.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/PKG-INFO` & `apache-airflow-client-2.6.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.2rc1
+Version: 2.6.2rc2
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.2
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.2rc1/README.md` & `apache-airflow-client-2.6.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/config_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/connection_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_run_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/dag_warning_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/dataset_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/event_log_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/import_error_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/monitoring_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/permission_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/plugin_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/pool_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/provider_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/role_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/task_instance_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/user_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/variable_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api/x_com_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api/x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/api_client.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/api_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/apis/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/configuration.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/configuration.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/exceptions.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/action.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/action_resource.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/basic_dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/class_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/clear_dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/clear_task_instances.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/collection_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/color.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/config.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/config_option.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/config_section.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/connection_test.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/cron_expression.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_detail.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_detail_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_detail_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         lazy_import()
         return {
             'timezone': (str,),  # noqa: E501
             'catchup': (bool,),  # noqa: E501
             'orientation': (str,),  # noqa: E501
             'concurrency': (float,),  # noqa: E501
             'start_date': (datetime, none_type,),  # noqa: E501
-            'dag_run_timeout': (TimeDelta,),  # noqa: E501
+            'dag_run_timeout': (TimeDelta, none_type,),  # noqa: E501
             'doc_md': (str, none_type,),  # noqa: E501
             'default_view': (str,),  # noqa: E501
             'params': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'end_date': (datetime, none_type,),  # noqa: E501
             'is_paused_upon_creation': (bool, none_type,),  # noqa: E501
             'last_parsed': (datetime, none_type,),  # noqa: E501
             'template_search_path': ([str], none_type,),  # noqa: E501
@@ -196,15 +196,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             timezone (str): [optional]  # noqa: E501
             catchup (bool): [optional]  # noqa: E501
             orientation (str): [optional]  # noqa: E501
             concurrency (float): [optional]  # noqa: E501
             start_date (datetime, none_type): The DAG's start date.  *Changed in version 2.0.1*&#58; Field becomes nullable. . [optional]  # noqa: E501
-            dag_run_timeout (TimeDelta): [optional]  # noqa: E501
+            dag_run_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             doc_md (str, none_type): [optional]  # noqa: E501
             default_view (str): [optional]  # noqa: E501
             params ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): User-specified DAG params.  *New in version 2.0.1* . [optional]  # noqa: E501
             end_date (datetime, none_type): The DAG's end date.  *New in version 2.3.0*. . [optional]  # noqa: E501
             is_paused_upon_creation (bool, none_type): Whether the DAG is paused upon creation.  *New in version 2.3.0* . [optional]  # noqa: E501
             last_parsed (datetime, none_type): The last time the DAG was parsed.  *New in version 2.3.0* . [optional]  # noqa: E501
             template_search_path ([str], none_type): The template search path.  *New in version 2.3.0* . [optional]  # noqa: E501
@@ -291,15 +291,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             timezone (str): [optional]  # noqa: E501
             catchup (bool): [optional]  # noqa: E501
             orientation (str): [optional]  # noqa: E501
             concurrency (float): [optional]  # noqa: E501
             start_date (datetime, none_type): The DAG's start date.  *Changed in version 2.0.1*&#58; Field becomes nullable. . [optional]  # noqa: E501
-            dag_run_timeout (TimeDelta): [optional]  # noqa: E501
+            dag_run_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             doc_md (str, none_type): [optional]  # noqa: E501
             default_view (str): [optional]  # noqa: E501
             params ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): User-specified DAG params.  *New in version 2.0.1* . [optional]  # noqa: E501
             end_date (datetime, none_type): The DAG's end date.  *New in version 2.3.0*. . [optional]  # noqa: E501
             is_paused_upon_creation (bool, none_type): Whether the DAG is paused upon creation.  *New in version 2.3.0* . [optional]  # noqa: E501
             last_parsed (datetime, none_type): The last time the DAG was parsed.  *New in version 2.3.0* . [optional]  # noqa: E501
             template_search_path ([str], none_type): The template search path.  *New in version 2.3.0* . [optional]  # noqa: E501
```

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_run_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/error.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/event_log_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/extra_link.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/extra_link_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/health_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/health_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/import_error_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/inline_response200.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/inline_response2001.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/job.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/list_dag_runs_form.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/list_task_instance_form.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/metadatabase_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/plugin_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/pool_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/provider.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/provider_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/relative_delta.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/resource.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/role.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/role_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/role_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/schedule_interval.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/scheduler_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/set_dag_run_note.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/set_task_instance_note.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/sla_miss.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/tag.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             'depends_on_past': (bool,),  # noqa: E501
             'is_mapped': (bool,),  # noqa: E501
             'wait_for_downstream': (bool,),  # noqa: E501
             'retries': (float,),  # noqa: E501
             'queue': (str, none_type,),  # noqa: E501
             'pool': (str,),  # noqa: E501
             'pool_slots': (float,),  # noqa: E501
-            'execution_timeout': (TimeDelta,),  # noqa: E501
+            'execution_timeout': (TimeDelta, none_type,),  # noqa: E501
             'retry_delay': (TimeDelta,),  # noqa: E501
             'retry_exponential_backoff': (bool,),  # noqa: E501
             'priority_weight': (float,),  # noqa: E501
             'weight_rule': (WeightRule,),  # noqa: E501
             'ui_color': (Color,),  # noqa: E501
             'ui_fgcolor': (Color,),  # noqa: E501
             'template_fields': ([str],),  # noqa: E501
@@ -242,15 +242,15 @@
             depends_on_past (bool): [optional]  # noqa: E501
             is_mapped (bool): [optional]  # noqa: E501
             wait_for_downstream (bool): [optional]  # noqa: E501
             retries (float): [optional]  # noqa: E501
             queue (str, none_type): [optional]  # noqa: E501
             pool (str): [optional]  # noqa: E501
             pool_slots (float): [optional]  # noqa: E501
-            execution_timeout (TimeDelta): [optional]  # noqa: E501
+            execution_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             retry_delay (TimeDelta): [optional]  # noqa: E501
             retry_exponential_backoff (bool): [optional]  # noqa: E501
             priority_weight (float): [optional]  # noqa: E501
             weight_rule (WeightRule): [optional]  # noqa: E501
             ui_color (Color): [optional]  # noqa: E501
             ui_fgcolor (Color): [optional]  # noqa: E501
             template_fields ([str]): [optional]  # noqa: E501
@@ -347,15 +347,15 @@
             depends_on_past (bool): [optional]  # noqa: E501
             is_mapped (bool): [optional]  # noqa: E501
             wait_for_downstream (bool): [optional]  # noqa: E501
             retries (float): [optional]  # noqa: E501
             queue (str, none_type): [optional]  # noqa: E501
             pool (str): [optional]  # noqa: E501
             pool_slots (float): [optional]  # noqa: E501
-            execution_timeout (TimeDelta): [optional]  # noqa: E501
+            execution_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             retry_delay (TimeDelta): [optional]  # noqa: E501
             retry_exponential_backoff (bool): [optional]  # noqa: E501
             priority_weight (float): [optional]  # noqa: E501
             weight_rule (WeightRule): [optional]  # noqa: E501
             ui_color (Color): [optional]  # noqa: E501
             ui_fgcolor (Color): [optional]  # noqa: E501
             template_fields ([str]): [optional]  # noqa: E501
```

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_extra_links.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_instance_reference_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/task_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/time_delta.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/trigger.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/trigger_rule.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/triggerer_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/triggerer_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_dag_run_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_task_instance.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/update_task_instances_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/user_collection_item_roles.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/variable_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/version_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/weight_rule.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model/x_com_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model/x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/model_utils.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/models/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/client/rest.py` & `apache-airflow-client-2.6.2rc2/airflow_client/client/rest.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/__init__.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_action.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_action_resource.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_basic_dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_class_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_clear_dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_clear_task_instances.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_collection_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_color.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_config.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_option.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_config_section.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_connection_test.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_cron_expression.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_detail.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_detail_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_run_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_error.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_event_log_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_extra_link.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_extra_link_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_health_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_health_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_import_error_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_inline_response200.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_inline_response2001.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_job.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_list_dag_runs_form.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_list_task_instance_form.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_metadatabase_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_monitoring_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_permission_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_plugin_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_pool_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_provider_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_relative_delta.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_resource.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_role.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_role_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_schedule_interval.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_scheduler_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_set_dag_run_note.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_set_task_instance_note.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_sla_miss.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_tag.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_extra_links.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_instance_reference_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_task_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_time_delta.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_trigger.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_trigger_rule.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_triggerer_status.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_triggerer_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_dag_run_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_task_instance.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_update_task_instances_state.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_user_collection_item_roles.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_variable_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_version_info.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_weight_rule.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_api.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection_all_of.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/airflow_client/test/test_x_com_collection_item.py` & `apache-airflow-client-2.6.2rc2/airflow_client/test/test_x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/PKG-INFO` & `apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.2rc1
+Version: 2.6.2rc2
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.2
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.2rc1/apache_airflow_client.egg-info/SOURCES.txt` & `apache-airflow-client-2.6.2rc2/apache_airflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.2rc1/setup.cfg` & `apache-airflow-client-2.6.2rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = ~=3.7
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-client-2.6.2rc1/setup.py` & `apache-airflow-client-2.6.2rc2/setup.py`

 * *Files identical despite different names*

