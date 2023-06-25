# Comparing `tmp/prodsys-0.1.1.tar.gz` & `tmp/prodsys-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.1.1.tar", max compression
+gzip compressed data, was "prodsys-0.2.0.tar", max compression
```

## Comparing `prodsys-0.1.1.tar` & `prodsys-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1096 2023-06-24 14:26:43.531947 prodsys-0.1.1/LICENSE
--rw-r--r--   0        0        0      354 2023-06-24 14:44:43.036304 prodsys-0.1.1/prodsys/__init__.py
--rw-r--r--   0        0        0     1248 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    39617 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     6381 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0      148 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9028 2023-06-24 21:54:59.751088 prodsys-0.1.1/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-06-24 16:53:52.840810 prodsys-0.1.1/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2138 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/core.py
--rw-r--r--   0        0        0     6525 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/process.py
--rw-r--r--   0        0        0     2435 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/product.py
--rw-r--r--   0        0        0     6508 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8240 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/resources.py
--rw-r--r--   0        0        0     2558 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/sink.py
--rw-r--r--   0        0        0     3684 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/state.py
--rw-r--r--   0        0        0     4895 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    10091 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5141 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1436 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     3303 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0     5896 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     4917 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1937 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/queue_data.py
--rw-r--r--   0        0        0     8849 2023-06-24 14:26:43.594400 prodsys-0.1.1/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10959 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     1481 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     2697 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/source_data.py
--rw-r--r--   0        0        0     9272 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/state_data.py
--rw-r--r--   0        0        0     5486 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    11007 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    26252 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4640 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    37201 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     7919 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    10551 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    21394 2023-06-24 21:21:16.011649 prodsys-0.1.1/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2023-06-24 21:05:31.351971 prodsys-0.1.1/prodsys/simulation/logger.py
--rw-r--r--   0        0        0     3779 2023-06-24 19:21:30.926240 prodsys-0.1.1/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9601 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0     2750 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/process.py
--rw-r--r--   0        0        0    12772 2023-06-24 21:55:13.927288 prodsys-0.1.1/prodsys/simulation/product.py
--rw-r--r--   0        0        0     3512 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/request.py
--rw-r--r--   0        0        0    15739 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/resources.py
--rw-r--r--   0        0        0    11773 2023-06-24 22:00:47.085210 prodsys-0.1.1/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     1785 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     2949 2023-06-24 19:10:14.857664 prodsys-0.1.1/prodsys/simulation/source.py
--rw-r--r--   0        0        0    25952 2023-06-24 21:18:25.179417 prodsys-0.1.1/prodsys/simulation/state.py
--rw-r--r--   0        0        0     1987 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7193 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/__init__.py
--rw-r--r--   0        0        0     6585 2023-06-24 21:35:21.997690 prodsys-0.1.1/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    28347 2023-06-24 21:28:17.758211 prodsys-0.1.1/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    11756 2023-06-24 21:36:38.638350 prodsys-0.1.1/prodsys/util/runner.py
--rw-r--r--   0        0        0     2426 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4260 2023-06-24 14:26:43.610024 prodsys-0.1.1/prodsys/util/util.py
--rw-r--r--   0        0        0     1384 2023-06-24 14:44:39.015456 prodsys-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5936 2023-06-24 14:44:14.913154 prodsys-0.1.1/README.md
--rw-r--r--   0        0        0     7827 1970-01-01 00:00:00.000000 prodsys-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-24 14:26:43.531947 prodsys-0.2.0/LICENSE
+-rw-r--r--   0        0        0      354 2023-06-25 14:17:03.886594 prodsys-0.2.0/prodsys/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    39617 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     6381 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0      148 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9028 2023-06-24 21:54:59.751088 prodsys-0.2.0/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-06-25 13:59:04.678477 prodsys-0.2.0/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2138 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/core.py
+-rw-r--r--   0        0        0     6525 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/process.py
+-rw-r--r--   0        0        0     2435 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/product.py
+-rw-r--r--   0        0        0     6508 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8240 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2558 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3684 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/state.py
+-rw-r--r--   0        0        0     4895 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    10091 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5141 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1436 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     3303 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0     5896 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     4917 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1937 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0     8849 2023-06-24 14:26:43.594400 prodsys-0.2.0/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10959 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     1481 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     2697 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/models/source_data.py
+-rw-r--r--   0        0        0     9272 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     5486 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    11007 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    26252 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4640 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    37201 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     7919 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    10551 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    21394 2023-06-24 21:21:16.011649 prodsys-0.2.0/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2023-06-24 21:05:31.351971 prodsys-0.2.0/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0     3779 2023-06-24 19:21:30.926240 prodsys-0.2.0/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9601 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0     2750 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    12772 2023-06-24 21:55:13.927288 prodsys-0.2.0/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     3512 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    15739 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0    11773 2023-06-24 22:00:47.085210 prodsys-0.2.0/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3199 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     1785 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     2949 2023-06-24 19:10:14.857664 prodsys-0.2.0/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    25952 2023-06-24 21:18:25.179417 prodsys-0.2.0/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     1987 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7193 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     6585 2023-06-24 21:35:21.997690 prodsys-0.2.0/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    28347 2023-06-24 21:28:17.758211 prodsys-0.2.0/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    11756 2023-06-24 21:36:38.638350 prodsys-0.2.0/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2426 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4260 2023-06-24 14:26:43.610024 prodsys-0.2.0/prodsys/util/util.py
+-rw-r--r--   0        0        0     1384 2023-06-25 14:16:59.285987 prodsys-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6238 2023-06-25 14:39:29.480577 prodsys-0.2.0/README.md
+-rw-r--r--   0        0        0     8124 1970-01-01 00:00:00.000000 prodsys-0.2.0/PKG-INFO
```

### Comparing `prodsys-0.1.1/LICENSE` & `prodsys-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/adapters/__init__.py` & `prodsys-0.2.0/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/adapters/adapter.py` & `prodsys-0.2.0/prodsys/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/adapters/json_adapter.py` & `prodsys-0.2.0/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/control/routing_control_env.py` & `prodsys-0.2.0/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/control/sequencing_control_env.py` & `prodsys-0.2.0/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/__init__.py` & `prodsys-0.2.0/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/core.py` & `prodsys-0.2.0/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/process.py` & `prodsys-0.2.0/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/product.py` & `prodsys-0.2.0/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/production_system.py` & `prodsys-0.2.0/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/resources.py` & `prodsys-0.2.0/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/sink.py` & `prodsys-0.2.0/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/source.py` & `prodsys-0.2.0/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/state.py` & `prodsys-0.2.0/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/express/time_model.py` & `prodsys-0.2.0/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/__init__.py` & `prodsys-0.2.0/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/process_factory.py` & `prodsys-0.2.0/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/product_factory.py` & `prodsys-0.2.0/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/queue_factory.py` & `prodsys-0.2.0/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/resource_factory.py` & `prodsys-0.2.0/prodsys/factories/resource_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/sink_factory.py` & `prodsys-0.2.0/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/source_factory.py` & `prodsys-0.2.0/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/state_factory.py` & `prodsys-0.2.0/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/factories/time_model_factory.py` & `prodsys-0.2.0/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/__init__.py` & `prodsys-0.2.0/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/core_asset.py` & `prodsys-0.2.0/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/performance_data.py` & `prodsys-0.2.0/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/performance_indicators.py` & `prodsys-0.2.0/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/processes_data.py` & `prodsys-0.2.0/prodsys/models/processes_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/product_data.py` & `prodsys-0.2.0/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/queue_data.py` & `prodsys-0.2.0/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/resource_data.py` & `prodsys-0.2.0/prodsys/models/resource_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/scenario_data.py` & `prodsys-0.2.0/prodsys/models/scenario_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/sink_data.py` & `prodsys-0.2.0/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/source_data.py` & `prodsys-0.2.0/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/state_data.py` & `prodsys-0.2.0/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/models/time_model_data.py` & `prodsys-0.2.0/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/__init__.py` & `prodsys-0.2.0/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.2.0/prodsys/optimization/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/math_opt.py` & `prodsys-0.2.0/prodsys/optimization/math_opt.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/optimization_analysis.py` & `prodsys-0.2.0/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/optimization_util.py` & `prodsys-0.2.0/prodsys/optimization/optimization_util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/simulated_annealing.py` & `prodsys-0.2.0/prodsys/optimization/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/optimization/tabu_search.py` & `prodsys-0.2.0/prodsys/optimization/tabu_search.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/__init__.py` & `prodsys-0.2.0/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/control.py` & `prodsys-0.2.0/prodsys/simulation/control.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/logger.py` & `prodsys-0.2.0/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/observer.py` & `prodsys-0.2.0/prodsys/simulation/observer.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/proces_models.py` & `prodsys-0.2.0/prodsys/simulation/proces_models.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/process.py` & `prodsys-0.2.0/prodsys/simulation/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/product.py` & `prodsys-0.2.0/prodsys/simulation/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/request.py` & `prodsys-0.2.0/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/resources.py` & `prodsys-0.2.0/prodsys/simulation/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/router.py` & `prodsys-0.2.0/prodsys/simulation/router.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/sim.py` & `prodsys-0.2.0/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/sink.py` & `prodsys-0.2.0/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/source.py` & `prodsys-0.2.0/prodsys/simulation/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/state.py` & `prodsys-0.2.0/prodsys/simulation/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/store.py` & `prodsys-0.2.0/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/simulation/time_model.py` & `prodsys-0.2.0/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/util/kpi_visualization.py` & `prodsys-0.2.0/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/util/post_processing.py` & `prodsys-0.2.0/prodsys/util/post_processing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/util/runner.py` & `prodsys-0.2.0/prodsys/util/runner.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/util/statistical_functions.py` & `prodsys-0.2.0/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/prodsys/util/util.py` & `prodsys-0.2.0/prodsys/util/util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.1.1/pyproject.toml` & `prodsys-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.1.1"
+version = "0.2.0"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
```

### Comparing `prodsys-0.1.1/README.md` & `prodsys-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-# prodsys
+# prodsys - modeling, simulating and optimizing production systems
 
-prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
+![Build-sucess](https://img.shields.io/badge/build-success-green)
+![PyPI](https://img.shields.io/pypi/v/prodsys)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
+![Docu](https://img.shields.io/badge/docu-100%-green)
+
+prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
```

### Comparing `prodsys-0.1.1/PKG-INFO` & `prodsys-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.1.1
+Version: 0.2.0
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,17 +19,22 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: simanneal (>=0.5.0,<0.6.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
-# prodsys
+# prodsys - modeling, simulating and optimizing production systems
 
-prodsys is a python package for modeling, simulating, and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
+![Build-sucess](https://img.shields.io/badge/build-success-green)
+![PyPI](https://img.shields.io/pypi/v/prodsys)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
+![Docu](https://img.shields.io/badge/docu-100%-green)
+
+prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
```

