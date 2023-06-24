# Comparing `tmp/prodsys-0.1.0.tar.gz` & `tmp/prodsys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.1.0.tar", max compression
+gzip compressed data, was "prodsys-0.1.1.tar", max compression
```

## Comparing `prodsys-0.1.0.tar` & `prodsys-0.1.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0     1096 2023-04-08 10:54:01.763443 prodsys-0.1.0/LICENSE
--rw-r--r--   0        0        0      354 2023-06-01 01:11:43.140962 prodsys-0.1.0/prodsys/__init__.py
--rw-r--r--   0        0        0     1248 2023-06-01 01:11:43.141968 prodsys-0.1.0/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    39617 2023-06-01 01:11:43.142961 prodsys-0.1.0/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     6381 2023-06-01 01:11:43.143962 prodsys-0.1.0/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0      148 2023-06-01 01:11:43.144969 prodsys-0.1.0/prodsys/control/__init__.py
--rw-r--r--   0        0        0    14413 2023-06-01 01:11:43.145967 prodsys-0.1.0/prodsys/control/gym_env.py
--rw-r--r--   0        0        0     2138 2023-06-01 01:11:43.146970 prodsys-0.1.0/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-06-01 01:11:43.147982 prodsys-0.1.0/prodsys/express/core.py
--rw-r--r--   0        0        0     6525 2023-06-01 01:11:43.147982 prodsys-0.1.0/prodsys/express/process.py
--rw-r--r--   0        0        0     2435 2023-06-01 01:11:43.148970 prodsys-0.1.0/prodsys/express/product.py
--rw-r--r--   0        0        0     6508 2023-06-01 01:11:43.149967 prodsys-0.1.0/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8240 2023-06-01 01:11:43.150977 prodsys-0.1.0/prodsys/express/resources.py
--rw-r--r--   0        0        0     2558 2023-06-01 01:11:43.152971 prodsys-0.1.0/prodsys/express/sink.py
--rw-r--r--   0        0        0     3684 2023-06-01 01:11:43.152971 prodsys-0.1.0/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2023-06-01 01:11:43.153975 prodsys-0.1.0/prodsys/express/state.py
--rw-r--r--   0        0        0     4895 2023-06-01 01:11:43.154974 prodsys-0.1.0/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-06-01 01:11:43.155961 prodsys-0.1.0/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-01 01:11:43.156962 prodsys-0.1.0/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2023-06-01 01:11:43.157961 prodsys-0.1.0/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2023-06-01 01:11:43.158969 prodsys-0.1.0/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    10091 2023-06-01 01:11:43.159962 prodsys-0.1.0/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-06-01 01:11:43.160970 prodsys-0.1.0/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5141 2023-06-01 01:11:43.161965 prodsys-0.1.0/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-06-01 01:11:43.162972 prodsys-0.1.0/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-06-01 01:11:43.163973 prodsys-0.1.0/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1436 2023-06-01 01:11:43.164964 prodsys-0.1.0/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-06-01 01:11:43.164964 prodsys-0.1.0/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     3303 2023-06-01 01:11:43.165962 prodsys-0.1.0/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2023-06-01 01:11:43.166969 prodsys-0.1.0/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0     5896 2023-06-01 01:11:43.167961 prodsys-0.1.0/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     4917 2023-06-01 01:11:43.168974 prodsys-0.1.0/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1937 2023-06-01 01:11:43.168974 prodsys-0.1.0/prodsys/models/queue_data.py
--rw-r--r--   0        0        0     8849 2023-06-01 01:11:43.169970 prodsys-0.1.0/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10959 2023-06-01 01:11:43.170964 prodsys-0.1.0/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     1481 2023-06-01 01:11:43.170964 prodsys-0.1.0/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     2697 2023-06-01 01:11:43.173292 prodsys-0.1.0/prodsys/models/source_data.py
--rw-r--r--   0        0        0     9272 2023-06-01 01:11:43.174295 prodsys-0.1.0/prodsys/models/state_data.py
--rw-r--r--   0        0        0     5486 2023-06-01 01:11:43.175301 prodsys-0.1.0/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-06-01 01:11:43.176297 prodsys-0.1.0/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    11007 2023-06-01 01:11:43.177291 prodsys-0.1.0/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    26252 2023-06-01 01:11:43.178292 prodsys-0.1.0/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4640 2023-06-01 01:11:43.179324 prodsys-0.1.0/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    37201 2023-06-01 01:11:43.180292 prodsys-0.1.0/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     7919 2023-06-01 01:11:43.181297 prodsys-0.1.0/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    10551 2023-06-01 01:11:43.182307 prodsys-0.1.0/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-06-01 01:11:43.182307 prodsys-0.1.0/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    20956 2023-06-01 01:11:43.183292 prodsys-0.1.0/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6747 2023-06-01 01:11:43.184296 prodsys-0.1.0/prodsys/simulation/logger.py
--rw-r--r--   0        0        0     3737 2023-06-01 01:11:43.185294 prodsys-0.1.0/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9601 2023-06-01 01:11:43.187294 prodsys-0.1.0/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0     2750 2023-06-01 01:11:43.189293 prodsys-0.1.0/prodsys/simulation/process.py
--rw-r--r--   0        0        0    11981 2023-06-01 01:11:43.191305 prodsys-0.1.0/prodsys/simulation/product.py
--rw-r--r--   0        0        0     3512 2023-06-01 01:11:43.192295 prodsys-0.1.0/prodsys/simulation/request.py
--rw-r--r--   0        0        0    15739 2023-06-01 01:11:43.194296 prodsys-0.1.0/prodsys/simulation/resources.py
--rw-r--r--   0        0        0    10891 2023-06-01 01:11:43.195293 prodsys-0.1.0/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2023-06-01 01:11:43.196293 prodsys-0.1.0/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     1785 2023-06-01 01:11:43.197295 prodsys-0.1.0/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     2938 2023-06-01 01:11:43.198292 prodsys-0.1.0/prodsys/simulation/source.py
--rw-r--r--   0        0        0    25658 2023-06-01 01:11:43.201302 prodsys-0.1.0/prodsys/simulation/state.py
--rw-r--r--   0        0        0     1987 2023-06-01 01:11:43.203293 prodsys-0.1.0/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7193 2023-06-01 01:11:43.204292 prodsys-0.1.0/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-06-01 01:11:43.205292 prodsys-0.1.0/prodsys/util/__init__.py
--rw-r--r--   0        0        0     5698 2023-06-01 01:11:43.206302 prodsys-0.1.0/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    26763 2023-06-01 01:11:43.208293 prodsys-0.1.0/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    11704 2023-06-01 01:11:43.209299 prodsys-0.1.0/prodsys/util/runner.py
--rw-r--r--   0        0        0     2426 2023-06-01 01:11:43.210292 prodsys-0.1.0/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4260 2023-06-01 01:11:43.211292 prodsys-0.1.0/prodsys/util/util.py
--rw-r--r--   0        0        0     1384 2023-06-01 01:11:43.214294 prodsys-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5784 2023-06-01 01:11:43.029970 prodsys-0.1.0/README.md
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 prodsys-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-24 14:26:43.531947 prodsys-0.1.1/LICENSE
+-rw-r--r--   0        0        0      354 2023-06-24 14:44:43.036304 prodsys-0.1.1/prodsys/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    39617 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     6381 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0      148 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9028 2023-06-24 21:54:59.751088 prodsys-0.1.1/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-06-24 16:53:52.840810 prodsys-0.1.1/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2138 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/core.py
+-rw-r--r--   0        0        0     6525 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/process.py
+-rw-r--r--   0        0        0     2435 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/product.py
+-rw-r--r--   0        0        0     6508 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8240 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2558 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3684 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/state.py
+-rw-r--r--   0        0        0     4895 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    10091 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5141 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1436 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     3303 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0     5896 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     4917 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1937 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0     8849 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10959 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     1481 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     2697 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/source_data.py
+-rw-r--r--   0        0        0     9272 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     5486 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    11007 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    26252 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4640 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    37201 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     7919 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    10551 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    21394 2023-06-24 21:21:16.011649 prodsys-0.1.1/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2023-06-24 21:05:31.351971 prodsys-0.1.1/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0     3779 2023-06-24 19:21:30.926240 prodsys-0.1.1/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9601 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0     2750 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    12772 2023-06-24 21:55:13.927288 prodsys-0.1.1/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     3512 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    15739 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0    11773 2023-06-24 22:00:47.085210 prodsys-0.1.1/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3199 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     1785 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     2949 2023-06-24 19:10:14.857664 prodsys-0.1.1/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    25952 2023-06-24 21:18:25.179417 prodsys-0.1.1/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     1987 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7193 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     6585 2023-06-24 21:35:21.997690 prodsys-0.1.1/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    28347 2023-06-24 21:28:17.758211 prodsys-0.1.1/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    11756 2023-06-24 21:36:38.638350 prodsys-0.1.1/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2426 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4260 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/util.py
+-rw-r--r--   0        0        0     1384 2023-06-24 14:44:39.015456 prodsys-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5936 2023-06-24 14:44:14.913154 prodsys-0.1.1/README.md
+-rw-r--r--   0        0        0     7827 1970-01-01 00:00:00.000000 prodsys-0.1.1/PKG-INFO
```

### Comparing `prodsys-0.1.0/LICENSE` & `prodsys-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/adapters/__init__.py` & `prodsys-0.1.1/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/adapters/adapter.py` & `prodsys-0.1.1/prodsys/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/adapters/json_adapter.py` & `prodsys-0.1.1/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/__init__.py` & `prodsys-0.1.1/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/core.py` & `prodsys-0.1.1/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/process.py` & `prodsys-0.1.1/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/product.py` & `prodsys-0.1.1/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/production_system.py` & `prodsys-0.1.1/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/resources.py` & `prodsys-0.1.1/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/sink.py` & `prodsys-0.1.1/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/source.py` & `prodsys-0.1.1/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/state.py` & `prodsys-0.1.1/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/express/time_model.py` & `prodsys-0.1.1/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/__init__.py` & `prodsys-0.1.1/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/process_factory.py` & `prodsys-0.1.1/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/product_factory.py` & `prodsys-0.1.1/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/queue_factory.py` & `prodsys-0.1.1/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/resource_factory.py` & `prodsys-0.1.1/prodsys/factories/resource_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/sink_factory.py` & `prodsys-0.1.1/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/source_factory.py` & `prodsys-0.1.1/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/state_factory.py` & `prodsys-0.1.1/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/factories/time_model_factory.py` & `prodsys-0.1.1/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/__init__.py` & `prodsys-0.1.1/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/core_asset.py` & `prodsys-0.1.1/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/performance_data.py` & `prodsys-0.1.1/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/performance_indicators.py` & `prodsys-0.1.1/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/processes_data.py` & `prodsys-0.1.1/prodsys/models/processes_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/product_data.py` & `prodsys-0.1.1/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/queue_data.py` & `prodsys-0.1.1/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/resource_data.py` & `prodsys-0.1.1/prodsys/models/resource_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/scenario_data.py` & `prodsys-0.1.1/prodsys/models/scenario_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/sink_data.py` & `prodsys-0.1.1/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/source_data.py` & `prodsys-0.1.1/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/state_data.py` & `prodsys-0.1.1/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/models/time_model_data.py` & `prodsys-0.1.1/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/__init__.py` & `prodsys-0.1.1/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.1.1/prodsys/optimization/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/math_opt.py` & `prodsys-0.1.1/prodsys/optimization/math_opt.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/optimization_analysis.py` & `prodsys-0.1.1/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/optimization_util.py` & `prodsys-0.1.1/prodsys/optimization/optimization_util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/simulated_annealing.py` & `prodsys-0.1.1/prodsys/optimization/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/optimization/tabu_search.py` & `prodsys-0.1.1/prodsys/optimization/tabu_search.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/__init__.py` & `prodsys-0.1.1/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/control.py` & `prodsys-0.1.1/prodsys/simulation/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from pydantic import BaseModel, Field, validator, Extra
-from typing import List, Generator, TYPE_CHECKING, Union
+from typing import List, Generator, TYPE_CHECKING, Union, Optional
 
 # from process import Process
 from simpy import events
 
 from prodsys.simulation import request, sim, state
 
 if TYPE_CHECKING:
     from prodsys.simulation import product, process, state, resources, request, sink
-    from prodsys.control import gym_env
+    from prodsys.control import sequencing_control_env
 
 
 class Controller(ABC, BaseModel):
     """
     A controller is responsible for controlling the processes of a resource. The controller is requested by materials requiring processes. The controller decides has a control policy that determines with which sequence requests are processed.
 
     Args:
@@ -233,15 +233,15 @@
             target_product (product.Product): The product that is processed.
         """
         input_state.prepare_for_run()
         input_state.state_info.log_product(
             target_product, state.StateTypeEnum.production
         )
         target_product.product_info.log_start_process(
-            target_product.next_resource,
+            target_product.next_production_resource,
             target_product,
             self.env.now,
             state.StateTypeEnum.production,
         )
         input_state.process = self.env.process(input_state.process_state())
         yield input_state.process
 
@@ -254,14 +254,15 @@
     requests: List[request.TransportResquest] = Field(default_factory=list)
     control_policy: Callable[
         [
             List[request.TransportResquest],
         ],
         None,
     ]
+    _current_position: Optional[product.Location] = Field(init=False, default=None)
 
     def get_next_product_for_process(
         self, resource: product.Location, product: product.Product
     ) -> List[events.Event]:
         """
         Get the next product for a process from the input queue of a resource.
 
@@ -329,14 +330,15 @@
         4. If the resource is full or there are no requests, go to 1.
         5. Sort the queue according to the control policy.
         6. Start the next process. Go to 1.
 
         Yields:
             Generator: The generator yields when a request is made or a process is finished.
         """
+        self._current_position = self.resource
         while True:
             yield events.AnyOf(
                 env=self.env, events=self.running_processes + [self.requested]
             )
             if self.requested.triggered:
                 self.requested = events.Event(self.env)
             for process in self.running_processes:
@@ -395,16 +397,17 @@
                             state.process
                             for state in possible_states
                             if state.process is not None and state.process.is_alive
                         ],
                     )
 
                 yield self.env.process(
-                    self.run_process(transport_state, product, target=origin)
+                    self.run_process(transport_state, product, target=origin, empty_transport=True)
                 )
+                self._current_position = origin
                 transport_state.process = None
 
             eventss = self.get_next_product_for_process(origin, product)
             yield events.AllOf(resource.env, eventss)
             possible_states = resource.get_processes(process)
             while True:
                 transport_state = resource.get_free_process(process)
@@ -417,43 +420,48 @@
                         for state in possible_states
                         if state.process is not None and state.process.is_alive
                     ],
                 )
             yield self.env.process(
                 self.run_process(transport_state, product, target=target)
             )
+            self._current_position = target
             transport_state.process = None
             eventss = self.put_product_to_input_queue(target, product)
             yield events.AllOf(resource.env, eventss)
             if isinstance(target, resources.ProductionResource):
                 target.unreserve_input_queues()
             product.finished_process.succeed()
 
     def run_process(
         self,
         input_state: state.State,
         product: product.Product,
         target: product.Location,
+        empty_transport: bool = False,
     ):
         """
         Run the process of a product. The process is started and the product is logged.
 
         Args:
             input_state (state.State): The transport state of the process.
             product (product.Product): The product that is transported.
             target (product.Location): The target of the transport.
         """
         target_location = target.get_location()
         input_state.prepare_for_run()
         input_state.state_info.log_product(product, state.StateTypeEnum.transport)
-        input_state.state_info.log_target_location(
-            target, state.StateTypeEnum.transport
+
+        input_state.state_info.log_transport(
+            self._current_position,
+            target, state.StateTypeEnum.transport,
+            empty_transport=empty_transport
         )
         product.product_info.log_start_process(
-            product.next_resource,
+            product.next_production_resource,
             product,
             self.env.now,
             state.StateTypeEnum.transport,
         )
         input_state.process = self.env.process(
             input_state.process_state(target=target_location)  # type: ignore False
         )
@@ -501,15 +509,15 @@
         key=lambda x: x.process.get_expected_process_time(
             x.origin.get_location(), x.target.get_location()
         )
     )
 
 
 def agent_control_policy(
-    gym_env: gym_env.ProductionControlEnv, requests: List[request.Request]
+    gym_env: sequencing_control_env.AbstractSequencingControlEnv, requests: List[request.Request]
 ) -> None:
     """
     Sort the requests according to the agent's policy.
 
     Args:
         gym_env (gym_env.ProductionControlEnv): A gym environment, where the agent can interact with the simulation.
         requests (List[request.Request]): The list of requests.
```

### Comparing `prodsys-0.1.0/prodsys/simulation/logger.py` & `prodsys-0.1.1/prodsys/simulation/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,17 @@
         "Time": state_info._event_time,
         "Resource": state_info.resource_ID,
         "State": state_info.ID,
         "State Type": state_info._state_type,
         "Activity": state_info._activity,
         "Expected End Time": state_info._expected_end_time,
         "Product": state_info._product_ID,
+        "Origin location": state_info._origin_ID,
         "Target location": state_info._target_ID,
+        "Empty Transport": state_info._empty_transport,
     }
     data.append(item)
 
 
 def post_monitor_product_info(data: List[dict], product_info: product.ProductInfo):
     """
     Post function for monitoring product info. With this post monitor, every product creation and finish is logged.
```

### Comparing `prodsys-0.1.0/prodsys/simulation/observer.py` & `prodsys-0.1.1/prodsys/simulation/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     for queue in resource.input_queues:
         for product_data in queue.items:
             product = product_factory.get_product(product_data.ID)
 
             production_process_info = QueueObservation(
                 product=product_data.ID,
                 activity="waiting",
-                process=product.next_process.process_data.ID,
-                next_resource=product.next_resource.data.ID,
+                process=product.next_prodution_process.process_data.ID,
+                next_resource=product.next_production_resource.data.ID,
                 waiting_since=product.product_info.event_time
             )
             queue_observation.append(production_process_info)
 
     return queue_observation
 
 def observe_output_queue(resource: resources.Resource, product_factory: product_factory.ProductFactory) -> List[QueueObservation]:
@@ -59,16 +59,16 @@
     for queue in resource.output_queues:
         for product_data in queue.items:
             product = product_factory.get_product(product_data.ID)
 
             production_process_info = QueueObservation(
                 product=product_data.ID,
                 activity="waiting",
-                process=product.next_process,
-                next_resource=product.next_resource,
+                process=product.next_prodution_process,
+                next_resource=product.next_production_resource,
                 waiting_since=product.product_info.event_time
             )
             queue_observation.append(production_process_info)
 
     return queue_observation
 
 class ResourceAvailableObservation(BaseModel):
```

### Comparing `prodsys-0.1.0/prodsys/simulation/proces_models.py` & `prodsys-0.1.1/prodsys/simulation/proces_models.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/process.py` & `prodsys-0.1.1/prodsys/simulation/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/product.py` & `prodsys-0.1.1/prodsys/simulation/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,58 +151,61 @@
 
     env: sim.Environment
     product_data: product_data.ProductData
     process_model: proces_models.ProcessModel
     transport_process: process.TransportProcess
     product_router: router.Router
 
-    next_process: Optional[process.PROCESS_UNION] = Field(default=None, init=False)
+    next_prodution_process: Optional[process.PROCESS_UNION] = Field(default=None, init=False)
     process: events.Process = Field(default=None, init=False)
-    next_resource: Location = Field(default=None, init=False)
+    next_production_resource: Location = Field(default=None, init=False)
+    next_production_resources: List[resources.ProductionResource] = Field(default=None, init=False)
+    next_transport_resource: Optional[resources.TransportResource] = Field(default=None, init=False)
+    next_transport_resources: List[resources.TransportResource] = Field(default=None, init=False)
     finished_process: events.Event = Field(default=None, init=False)
     product_info: ProductInfo = ProductInfo()
 
     class Config:
         arbitrary_types_allowed = True
 
     def process_product(self):
         self.finished_process = events.Event(self.env)
         self.product_info.log_create_product(
-            resource=self.next_resource, _product=self, event_time=self.env.now
+            resource=self.next_production_resource, _product=self, event_time=self.env.now
         )
         """
         Processes the product object in a simpy process. The product object is processed after creation until all required production processes are performed and it reaches a sink.
         """
         yield self.env.process(self.transport_to_queue_of_resource())
-        while self.next_process:
+        while self.next_prodution_process:
             self.request_process()
             yield self.finished_process
             self.product_info.log_end_process(
-                resource=self.next_resource,
+                resource=self.next_production_resource,
                 _product=self,
                 event_time=self.env.now,
                 state_type=state.StateTypeEnum.production,
             )
             self.finished_process = events.Event(self.env)
             yield self.env.process(self.transport_to_queue_of_resource())
         self.product_info.log_finish_product(
-            resource=self.next_resource, _product=self, event_time=self.env.now
+            resource=self.next_production_resource, _product=self, event_time=self.env.now
         )
-        self.next_resource.register_finished_product(self)
+        self.next_production_resource.register_finished_product(self)
 
     def request_process(self) -> None:
         """
         Requests the next production process of the product object from the next production resource by creating a request event and registering it at the environment.
         """
-        if self.next_process:
+        if self.next_prodution_process:
             self.env.request_process_of_resource(
                 request.Request(
-                    process=self.next_process,
+                    process=self.next_prodution_process,
                     product=self,
-                    resource=self.next_resource,
+                    resource=self.next_production_resource,
                 )
             )
 
     def request_transport(
         self,
         transport_resource: resources.TransportResource,
         origin_resource: Location,
@@ -222,76 +225,79 @@
                 product=self,
                 resource=transport_resource,
                 origin=origin_resource,
                 target=target_resource,
             )
         )
 
-    def set_next_process(self):
+    def set_next_production_process(self):
         """
         Sets the next process of the product object based on the current state of the product and its process model.
         """
         next_possible_processes = self.process_model.get_next_possible_processes()
         if not next_possible_processes:
-            self.next_process = None
+            self.next_prodution_process = None
         else:
-            self.next_process = np.random.choice(next_possible_processes)  # type: ignore
-            self.process_model.update_marking_from_transition(self.next_process)  # type: ignore
+            self.next_prodution_process = np.random.choice(next_possible_processes)  # type: ignore
+            self.process_model.update_marking_from_transition(self.next_prodution_process)  # type: ignore
 
     def transport_to_queue_of_resource(self):
         """
         Simpy process that transports the product object to the queue of the next resource.
         """
-        origin_resource = self.next_resource
-        transport_resource = self.product_router.get_next_resource(
-            self.transport_process
+        origin_resource = self.next_production_resource
+        self.product_router.set_next_transport_resources(
+            self
         )
         yield self.env.timeout(0)
-        self.set_next_process()
-        yield self.env.process(self.set_next_resource())
-        self.request_transport(transport_resource, origin_resource, self.next_resource)  # type: ignore False
+        transport_resource = self.next_transport_resources.pop(0)
+        if not transport_resource:
+            raise ValueError("No transport resource found.")
+        self.set_next_production_process()
+        yield self.env.process(self.set_next_production_resource())
+        self.request_transport(transport_resource, origin_resource, self.next_production_resource)  # type: ignore False
         yield self.finished_process
         self.product_info.log_end_process(
             resource=transport_resource,
             _product=self,
             event_time=self.env.now,
             state_type=state.StateTypeEnum.transport,
         )
         self.finished_process = events.Event(self.env)
 
-    def set_next_resource(self):
+    def set_next_production_resource(self):
         """
         Sets the next resource of the product object based on the current state of the product and its process model.
         If no production process is required, the next resource is set to the sink of the product type.
         If no resource can be found with a free input queue, the product object waits until a resource is free.
         """
-        if not self.next_process:
-            self.next_resource = self.product_router.get_sink(
+        if not self.next_prodution_process:
+            self.next_production_resource = self.product_router.get_sink(
                 self.product_data.product_type
             )
         else:
-            self.next_resource = self.product_router.get_next_resource(
-                self.next_process
-            )
+
             while True:
-                if self.next_resource is not None and isinstance(
-                    self.next_resource, resources.ProductionResource
-                ):
-                    self.next_resource.reserve_input_queues()
-                    yield self.env.timeout(0)
-                    break
+                self.product_router.set_next_production_resources(
+                    self
+                )
+                yield self.env.timeout(0)
+                if self.next_production_resources and all(isinstance(
+                    next_resource, resources.ProductionResource
+                ) for next_resource in self.next_production_resources): 
+                    self.next_production_resource = self.next_production_resources.pop(0)
+                    if not any(q.full for q in self.next_production_resource.input_queues):
+                        self.next_production_resource.reserve_input_queues()
+                        break
                 resource_got_free_events = [
                     resource.got_free
                     for resource in self.product_router.get_possible_resources(
-                        self.next_process
+                        self.next_prodution_process
                     )
                 ]
                 yield events.AnyOf(self.env, resource_got_free_events)
                 for resource in self.product_router.get_possible_resources(
-                    self.next_process
+                    self.next_prodution_process
                 ):
                     if resource.got_free.triggered:
                         resource.got_free = events.Event(self.env)
 
-                self.next_resource = self.product_router.get_next_resource(
-                    self.next_process
-                )
```

### Comparing `prodsys-0.1.0/prodsys/simulation/request.py` & `prodsys-0.1.1/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/resources.py` & `prodsys-0.1.1/prodsys/simulation/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/router.py` & `prodsys-0.1.1/prodsys/simulation/router.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,115 +2,159 @@
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import List, TYPE_CHECKING, Optional
 import numpy as np
 
+from simpy import events
+
 from prodsys.simulation import process
 from prodsys.simulation import resources
 
 
 if TYPE_CHECKING:
     from prodsys.simulation import resources, process, product, sink
     from prodsys.factories import resource_factory, sink_factory
-    from prodsys.control import gym_env
+    from prodsys.control import routing_control_env
 
 
 class Router:
     """
     Base class for all routers.
 
     Args:
         resource_factory (resource_factory.ResourceFactory): The resource factory of the production system.
         sink_factory (sink_factory.SinkFactory): The sink factory of the production system.
         routing_heuristic (Callable[[List[resources.Resource]], resources.Resource]): The routing heuristic to be used, needs to be a callable that takes a list of resources and returns a resource.
     """
+
     def __init__(
         self,
         resource_factory: resource_factory.ResourceFactory,
         sink_factory: sink_factory.SinkFactory,
         routing_heuristic: Callable[[List[resources.Resource]], resources.Resource],
     ):
         self.resource_factory: resource_factory.ResourceFactory = resource_factory
         self.sink_factory: sink_factory.SinkFactory = sink_factory
-        self.routing_heuristic: Callable[[List[resources.Resource]], resources.Resource] = routing_heuristic
+        self.routing_heuristic: Callable[[List[resources.Resource]]] = routing_heuristic
 
     @abstractmethod
-    def get_next_resource(self, __process: process.Process) -> Optional[resources.Resource]:
+    def get_free_resources(
+        self, requested_process: process.Process
+    ) -> List[resources.Resource]:
         """
-        Abstract method that returns the next resource for a process.
+        Abstract mehtod that returns a list of resources that have space in their input queues for the requested process.
 
         Args:
-            __process (process.Process): The process required by the product that needs to be routed.
+            requested_process (process.Process): The requested process.
 
         Returns:
-            Optional[resources.Resource]: The next resource for the process. If no resource is available, None is returned.
+            List[resources.Resource]: A list of resources that have space in their input queues for the requested process.
         """
         pass
 
+    
+    def set_next_production_resources(self, product_to_route: product.Product):
+        """
+        Sets the next resources for a product requring a production process. Resources that have full input queues are not considered.
+
+        Args:
+            product_to_route (product.Product): The product to route.
+        """
+        free_resources = self.get_free_resources(
+            product_to_route.next_prodution_process
+        )
+        product_to_route.next_production_resources = free_resources
+        if free_resources:
+            self.routing_heuristic(free_resources)
+
+    def set_next_transport_resources(self, product_to_route: product.Product):
+        """
+        Sets the next resources for a product requring a transport process.
+
+        Args:
+            product_to_route (product.Product): _description_
+        """
+        free_resources = self.get_free_resources(product_to_route.transport_process)
+        product_to_route.next_transport_resources = free_resources
+        if free_resources:
+            self.routing_heuristic(free_resources)
+
     def get_sink(self, _product_type: str) -> sink.Sink:
         """
         Returns the sink for a product type.
 
         Args:
             _product_type (str): The product type.
 
         Returns:
             sink.Sink: The sink for the product type.
         """
         possible_sinks = self.sink_factory.get_sinks_with_product_type(_product_type)
-        chosen_sink = self.routing_heuristic(possible_sinks)
+        chosen_sink = np.random.choice(possible_sinks)
         return chosen_sink  # type: ignore False
-    
-    def get_possible_resources(self, target_process: process.Process) -> List[resources.Resource]:
+
+    def get_possible_resources(
+        self, target_process: process.Process
+    ) -> List[resources.Resource]:
         """
         Returns a list of possible resources for a process.
 
         Args:
             target_process (process.Process): The process required by the product that needs to be routed.
 
         Returns:
             List[resources.Resource]: A list of possible resources for the process.
         """
-        possible_resources = self.resource_factory.get_resources_with_process(target_process)
+        possible_resources = self.resource_factory.get_resources_with_process(
+            target_process
+        )
         return possible_resources
 
 
 class SimpleRouter(Router):
     """
-    Simple router that routes products based on the IDs of the processes. 
+    Simple router that routes products based on the IDs of the processes.
 
-    Args:       
+    Args:
         resource_factory (resource_factory.ResourceFactory): The resource factory of the production system.
         sink_factory (sink_factory.SinkFactory): The sink factory of the production system.
         routing_heuristic (Callable[[List[resources.Resource]], resources.Resource]): The routing heuristic to be used, needs to be a callable that takes a list of resources and returns a resource.
     """
-    def get_next_resource(self, target_process: process.Process) -> Optional[resources.Resource]:
+
+    def get_free_resources(
+        self, requested_process: process.Process
+    ) -> List[resources.Resource]:
         """
-        Returns the next resource for a process. Resources that have full input queues are not considered. Returns None if no resource is available.
+        Returns a list of resources that have space in their input queues for the requested process.
 
         Args:
-            target_process (process.Process): The process required by the product that needs to be routed.
+            requested_process (process.Process): The requested process.
 
         Returns:
-            Optional[resources.Resource]: The next resource for the process. If no resource has space in the input queues, None is returned.
+            List[resources.Resource]: A list of resources that have space in their input queues for the requested process.
         """
-        possible_resources = self.resource_factory.get_resources_with_process(target_process)
+        possible_resources = self.resource_factory.get_resources_with_process(
+            requested_process
+        )
         left_resources = [resource for resource in possible_resources]
 
         for resource in possible_resources:
             if isinstance(resource, resources.ProductionResource):
                 for input_queue in resource.input_queues:
-                    if input_queue.full:  
-                        left_resources = [r for r in left_resources if not r.data.ID==resource.data.ID]
+                    if input_queue.full:
+                        left_resources = [
+                            r
+                            for r in left_resources
+                            if not r.data.ID == resource.data.ID
+                        ]
                         break
-        if not left_resources:
-            return None
-        return self.routing_heuristic(left_resources)
+        return left_resources
+
 
 
 def get_resource_capabilities(resource: resources.Resource) -> List[str]:
     """
     Returns a list of capabilities of a resource.
 
     Args:
@@ -119,144 +163,142 @@
     Returns:
         List[str]: A list of capabilities of the resource.
     """
     capabilities = []
     for resource_process in resource.processes:
         if isinstance(resource_process, process.CapabilityProcess):
             capabilities.append(resource_process.process_data.capability)
-        
+
     return capabilities
 
 
 class CapabilityRouter(Router):
     """
     Router that routes products based on the capabilities of the processes.
 
     Args:
         resource_factory (resource_factory.ResourceFactory): The resource factory of the production system.
         sink_factory (sink_factory.SinkFactory): The sink factory of the production system.
         routing_heuristic (Callable[[List[resources.Resource]], resources.Resource]): The routing heuristic to be used, needs to be a callable that takes a list of resources and returns a resource.
     """
-    def get_next_resource_per_ID(self, target_process: process.Process) -> resources.Resource:
+
+    def get_free_resources_per_ID(
+        self, requested_process: process.Process
+    ) -> List[resources.Resource]:
         """
-        Returns the next resource for a transport process based on the ID of the process.
+        Returns a list of resources that have space in their input queues for the requested process.
 
         Args:
-            target_process (process.Process): The process required by the product that needs to be routed.
+            requested_process (process.Process): The requested process.
 
         Returns:
-            resources.Resource: The next resource for the process.
+            List[resources.Resource]: A list of resources that have space in their input queues for the requested process.
         """
         possible_resources = self.resource_factory.get_resources_with_process(
-            target_process
+            requested_process
         )
-        return self.routing_heuristic(possible_resources)
+        left_resources = [resource for resource in possible_resources]
 
-    def get_next_resource(self, target_process: process.Process) -> Optional[resources.Resource]:
+        for resource in possible_resources:
+            if isinstance(resource, resources.ProductionResource):
+                for input_queue in resource.input_queues:
+                    if input_queue.full:
+                        left_resources = [
+                            r
+                            for r in left_resources
+                            if not r.data.ID == resource.data.ID
+                        ]
+                        break
+        return left_resources
+
+    def get_free_resources(
+        self, requested_process: process.Process
+    ) -> List[resources.Resource]:
         """
-        Returns the next resource for a process. Resources that have full input queues are not considered. Returns None if no resource is available.
+        Returns a list of resources that have space in their input queues for the requested process.
 
         Args:
-            target_process (process.Process): The process required by the product that needs to be routed.
+            requested_process (process.Process): The requested process.
 
         Raises:
-            ValueError: If the process is not a CapabilityProcess or TransportProcess.
+            ValueError: If the requested process is not a CapabilityProcess.
 
         Returns:
-            Optional[resources.Resource]: The next resource for the process. If no resource is available, None is returned.
+            List[resources.Resource]: _description_
         """
-        if isinstance(target_process, process.TransportProcess):
-            return self.get_next_resource_per_ID(target_process)
-        elif not isinstance(target_process, process.CapabilityProcess):
+        if isinstance(requested_process, process.TransportProcess):
+            return self.get_free_resources_per_ID(requested_process)
+        elif not isinstance(requested_process, process.CapabilityProcess):
             raise ValueError(
                 "CapabilityRouter can only be used with CapabilityProcess or TransportProcess"
             )
         possible_resources = []
         for resource in self.resource_factory.resources:
             resource_capabilities = get_resource_capabilities(resource)
-
-            if (target_process.process_data.capability in resource_capabilities) and not any(q.full for q in resource.input_queues):
+            if (
+                requested_process.process_data.capability in resource_capabilities
+            ) and not any(q.full for q in resource.input_queues):
                 possible_resources.append(resource)
-        if not possible_resources:
-            return None
-        return self.routing_heuristic(possible_resources)
+        return possible_resources
+
 
-def FIFO_routing_heuristic(possible_resources: List[resources.Resource]) -> resources.Resource:
+def FIFO_routing_heuristic(possible_resources: List[resources.Resource]):
     """
-    Returns the first resource in the list.
+    Sorts the list by the FIFO principle.
 
     Args:
         possible_resources (List[resources.Resource]): A list of possible resources.
-
-    Returns:
-        resources.Resource: The first resource in the list.
     """
-    return possible_resources.pop(0)
+    pass
 
 
-def random_routing_heuristic(possible_resources: List[resources.Resource]) -> resources.Resource:
+def random_routing_heuristic(possible_resources: List[resources.Resource]):
     """
-    Returns a random resource from the list.
+    Shuffles the list of possible resources.
 
     Args:
         possible_resources (List[resources.Resource]): A list of possible resources.
-
-    Returns:
-        resources.Resource: A random resource from the list.
     """
     possible_resources.sort(key=lambda x: x.data.ID)
-    return np.random.choice(possible_resources)  # type: ignore
+    np.random.shuffle(possible_resources)
 
 
 def shortest_queue_routing_heuristic(
     possible_resources: List[resources.Resource],
-) -> resources.Resource:
+):
     """
-    Returns the resource with the shortest input queue.
+    Sorts the list of possible resources by the length of their input queues and returns the first resource.
 
     Args:
         possible_resources (List[resources.Resource]): A list of possible resources.
-
-    Returns:
-        resources.Resource: The resource with the shortest input queue.
     """
-    queue_list = []
-    for resource in possible_resources:
-        if not isinstance(resource, resources.ProductionResource):
-            continue
-        if resource.input_queues:
-            for q in resource.input_queues:
-                queue_list.append((q, resource))
-    if queue_list:
-        queue_list.sort(key=lambda x: len(x[0].items))
-        min_length = len(queue_list[0][0].items)
-        resource_list = [
-            queue[1] for queue in queue_list if len(queue[0].items) <= min_length
-        ]
-        return np.random.choice(resource_list)
-    return random_routing_heuristic(possible_resources=possible_resources)
+    if any(not isinstance(resource, resources.ProductionResource) for resource in possible_resources):
+        random_routing_heuristic(possible_resources)
+        return
+    possible_resources.sort(key=lambda x: sum([len(q.items) for q in x.input_queues]))
+
 
-def agent_routing_heuristic(gym_env: gym_env.ProductionRoutingEnv, possible_resources: List[resources.Resource]
-                            ) -> resources.Resource:
+def agent_routing_heuristic(
+    gym_env: routing_control_env.AbstractRoutingControlEnv,
+    possible_resources: List[resources.Resource],
+):
     """
-    Returns the resource chosen by the agent. Has to be preloaded with the gym_env by using the partial function.
+    Sorts the list of possible resources by an reinforcement learning agent
 
     Args:
         gym_env (gym_env.ProductionRoutingEnv): Environment for the reinforcement learning agent.
         possible_resources (List[resources.Resource]): A list of possible resources.
-
-    Returns:
-        resources.Resource: The resource chosen by the agent.
     """
-    gym_env.load_possible_resources(possible_resources)
+    if gym_env.interrupt_simulation_event.triggered:
+        # Avoid that multiple requests trigger event multiple times -> delay them
+        while possible_resources:
+            possible_resources.pop()
+        return
+    gym_env.set_possible_resources(possible_resources)
     gym_env.interrupt_simulation_event.succeed()
-    return gym_env.get_chosen_resource()
-
-    
-
 
 ROUTING_HEURISTIC = {
     "shortest_queue": shortest_queue_routing_heuristic,
     "random": random_routing_heuristic,
     "FIFO": FIFO_routing_heuristic,
 }
 """
```

### Comparing `prodsys-0.1.0/prodsys/simulation/sim.py` & `prodsys-0.1.1/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/sink.py` & `prodsys-0.1.1/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/source.py` & `prodsys-0.1.1/prodsys/simulation/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             )
             available_events_events = []
             for queue in self.output_queues:
                 available_events_events.append(queue.put(product.product_data))
             yield events.AllOf(self.env, available_events_events)
 
             product.process = self.env.process(product.process_product())
-            product.next_resource = self
+            product.next_production_resource = self
 
     def get_location(self) -> List[float]:
         """
         Returns the location of the source.
 
         Returns:
             List[float]: The location. Has to be a list of length 2.
```

### Comparing `prodsys-0.1.0/prodsys/simulation/state.py` & `prodsys-0.1.1/prodsys/simulation/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,25 +65,32 @@
     resource_ID: str
     _event_time: Optional[float] = 0.0
     _expected_end_time: Optional[float] = 0.0
     _activity: Optional[StateEnum] = None
     _state_type: Optional[StateTypeEnum] = None
     _product_ID: str = ""
     _target_ID: str = ""
+    _origin_ID: str = ""
+    _empty_transport: Optional[bool] = None
 
-    def log_target_location(self, target: product.Location, state_type: StateTypeEnum):
+    def log_transport(self, origin: Optional[product.Location], target: product.Location, state_type: StateTypeEnum, empty_transport: bool):
         """
         Logs the target location of a transport state.
 
         Args:
             target (product.Location): The target location, either a resource, source or a sink.
             state_type (StateTypeEnum): The type of the state.
         """
+        if not origin:
+            self._origin_ID = None
+        else:
+            self._origin_ID = origin.data.ID
         self._target_ID = target.data.ID
         self._state_type = state_type
+        self._empty_transport = empty_transport
 
     def log_product(self, _product: product.Product, state_type: StateTypeEnum):
         """
         Logs the product of a transport or production state.
 
         Args:
             _product (product.Product): The product.
```

### Comparing `prodsys-0.1.0/prodsys/simulation/store.py` & `prodsys-0.1.1/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/simulation/time_model.py` & `prodsys-0.1.1/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/util/kpi_visualization.py` & `prodsys-0.1.1/prodsys/util/kpi_visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,14 +154,42 @@
         opacity=0.01,
     )
     fig.data = [t for t in fig.data if t.mode == "lines"]
     fig.update_traces(showlegend=True)
 
     fig.show()
 
+def plot_WIP_per_resource(post_processor: post_processing.PostProcessor):
+    """
+    Plots the WIP of the production system and the resources in the production system over time of the simulation.
+
+    Args:
+        post_processor (post_processing.PostProcessor): Post processor of the simulation.
+    """
+    df = post_processor.df_WIP.copy()
+    fig = px.scatter(df, x="Time", y="WIP")
+    df["Resource"] = "Total"
+
+    df_per_resource = post_processor.df_WIP_per_resource.copy()
+    df_per_resource["Resource"] = df_per_resource["WIP_resource"]
+
+    df = pd.concat([df, df_per_resource])
+    fig = px.scatter(
+        df,
+        x="Time",
+        y="WIP",
+        color="Resource",
+        trendline="expanding",
+        opacity=0.01,
+    )
+    fig.data = [t for t in fig.data if t.mode == "lines"]
+    fig.update_traces(showlegend=True)
+
+    fig.show()
+
 def print_aggregated_data(post_processor: post_processing.PostProcessor):
     """
     Prints the aggregated data of the simulation, comprising the throughput, WIP, throughput time and resource states.
 
     Args:
         post_processor (post_processing.PostProcessor): Post processor of the simulation.
     """
```

### Comparing `prodsys-0.1.0/prodsys/util/post_processing.py` & `prodsys-0.1.1/prodsys/util/post_processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -481,15 +481,15 @@
                     value=values["percentage"],
                     context=context,
                     resource=values["Resource"],
                 )
             )
         return KPIs
 
-    def get_WIP_KPI(self, df) -> pd.DataFrame:
+    def get_WIP_KPI(self, df: pd.DataFrame) -> pd.DataFrame:
         CREATED_CONDITION = df["Activity"] == "created product"
         FINISHED_CONDITION = df["Activity"] == "finished product"
 
         df["WIP_Increment"] = 0
         df.loc[CREATED_CONDITION, "WIP_Increment"] = 1
         df.loc[FINISHED_CONDITION, "WIP_Increment"] = -1
 
@@ -525,14 +525,49 @@
             df_temp = df.loc[df["Product_type"] == product_type].copy()
             df_temp = self.get_WIP_KPI(df_temp)
 
             df = df.combine_first(df_temp)
 
         return df
     
+    def get_WIP_per_resource_KPI(self, df: pd.DataFrame) -> pd.DataFrame:
+        CREATED_CONDITION = df["Activity"] == "created product"
+        FINISHED_CONDITION = df["Activity"] == "finished product"
+
+        df["WIP_Increment"] = 0
+        df.loc[CREATED_CONDITION, "WIP_Increment"] = 1
+        df.loc[FINISHED_CONDITION, "WIP_Increment"] = -1
+        df.loc[CREATED_CONDITION | FINISHED_CONDITION, "WIP_resource"] = df.loc[CREATED_CONDITION | FINISHED_CONDITION, "Resource"]
+        
+        MOVE_AWAY_CONDITION = (df["Empty Transport"] == False) & (df["Activity"] == "start state")
+        MOVE_IN_CONDITION = (df["Empty Transport"] == False) & (df["Activity"] == "end state")
+
+        df.loc[MOVE_AWAY_CONDITION, "WIP_Increment"] = -1
+        df.loc[MOVE_AWAY_CONDITION, "WIP_resource"] = df.loc[MOVE_AWAY_CONDITION, "Origin location"]
+        df.loc[MOVE_IN_CONDITION, "WIP_Increment"] = 1
+        df.loc[MOVE_IN_CONDITION, "WIP_resource"] = df.loc[MOVE_IN_CONDITION, "Target location"]
+
+        df["WIP"] = df.groupby(by="WIP_resource")["WIP_Increment"].cumsum()
+
+        return df
+    
+    @cached_property
+    def df_WIP_per_resource(self) -> pd.DataFrame:
+        """
+        Returns a data frame with the WIP over time for each resource.
+
+        Returns:
+            pd.DataFrame: Data frame with the WIP over time for each resource.
+        """
+        df = self.df_resource_states.copy()
+        # df = self.get_df_with_product_entries(df).copy()
+        df = self.get_WIP_per_resource_KPI(df)
+
+        return df
+    
     @cached_property
     def dynamic_WIP_KPIs(self) -> List[performance_indicators.KPI]:
         """
         Returns a list of Dynamic WIP KPI values for the WIP over time for each product type and the whole system.
 
         Returns:
             List[performance_indicators.KPI]: List of Dynamic WIP KPI values.
```

### Comparing `prodsys-0.1.0/prodsys/util/runner.py` & `prodsys-0.1.1/prodsys/util/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     def plot_results(self):
         """
         Plots the aggregated simulation results, comprising the throughput time over time, WIP over time, throughput time distribution and the time per state of the resources.
         """
         p = self.get_post_processor()
         kpi_visualization.plot_throughput_time_over_time(p)
         kpi_visualization.plot_WIP(p)
+        kpi_visualization.plot_WIP_per_resource(p)
         kpi_visualization.plot_throughput_time_distribution(p)
         kpi_visualization.plot_time_per_state_of_resources(p)
 
     def get_event_data_of_simulation(self) -> List[performance_data.Event]:
         """
         Returns the event data of the simulation.
```

### Comparing `prodsys-0.1.0/prodsys/util/statistical_functions.py` & `prodsys-0.1.1/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/prodsys/util/util.py` & `prodsys-0.1.1/prodsys/util/util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.0/pyproject.toml` & `prodsys-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.1.0"
+version = "0.1.1"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
```

### Comparing `prodsys-0.1.0/README.md` & `prodsys-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # prodsys
 
-prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle.
+prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
@@ -89,22 +89,22 @@
 
 ```python
 import numpy as np
 wip = np.array(wip_values).mean(axis=0)
 print(wip)
 ```
 
-These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](Tutorials/tutorial_0_overview.md). For a complete overview of the package's functionality, please see the [API reference](API_reference/API_reference_0_overview.md).
+These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](https://sdm4fzi.github.io/prodsys/Tutorials/tutorial_0_overview). For a complete overview of the package's functionality, please see the [API reference](https://sdm4fzi.github.io/prodsys/API_reference/API_reference_0_overview/).
 
 ## Contributing
 
 `prodsys` is a new project and has therefore much room for improvement. Therefore, it would be a pleasure to get feedback or support! If you want to contribute to the package, either create issues on [prodsys' github page](https://github.com/sdm4fzi/prodsys) for discussing new features or contact me directly via [github](https://github.com/SebBehrendt) or [email](mailto:sebastian.behrendt@kit.edu).
 
 ## License
 
 The package is licensed under the [MIT license](LICENSE).
 
 ## Acknowledgements
 
 We extend our sincere thanks to the German Federal Ministry for Economic Affairs and Climate Action
 (BMWK) for supporting this research project 13IK001ZF “Software-Defined Manufacturing for the
-automotive and supplying industry  [https://www.sdm4fzi.de/](https://www.sdm4fzi.de/)”.
+automotive and supplying industry [https://www.sdm4fzi.de/](https://www.sdm4fzi.de/).
```

### Comparing `prodsys-0.1.0/PKG-INFO` & `prodsys-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.1.0
+Version: 0.1.1
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 Requires-Dist: simanneal (>=0.5.0,<0.6.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # prodsys
 
-prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle.
+prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
@@ -114,29 +114,29 @@
 
 ```python
 import numpy as np
 wip = np.array(wip_values).mean(axis=0)
 print(wip)
 ```
 
-These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](Tutorials/tutorial_0_overview.md). For a complete overview of the package's functionality, please see the [API reference](API_reference/API_reference_0_overview.md).
+These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](https://sdm4fzi.github.io/prodsys/Tutorials/tutorial_0_overview). For a complete overview of the package's functionality, please see the [API reference](https://sdm4fzi.github.io/prodsys/API_reference/API_reference_0_overview/).
 
 ## Contributing
 
 `prodsys` is a new project and has therefore much room for improvement. Therefore, it would be a pleasure to get feedback or support! If you want to contribute to the package, either create issues on [prodsys' github page](https://github.com/sdm4fzi/prodsys) for discussing new features or contact me directly via [github](https://github.com/SebBehrendt) or [email](mailto:sebastian.behrendt@kit.edu).
 
 ## License
 
 The package is licensed under the [MIT license](LICENSE).
 
 ## Acknowledgements
 
 We extend our sincere thanks to the German Federal Ministry for Economic Affairs and Climate Action
 (BMWK) for supporting this research project 13IK001ZF “Software-Defined Manufacturing for the
-automotive and supplying industry  [https://www.sdm4fzi.de/](https://www.sdm4fzi.de/)”.
+automotive and supplying industry [https://www.sdm4fzi.de/](https://www.sdm4fzi.de/).
 
 MIT License
 
 Copyright (c) 2023 sebastian.behrendt
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

