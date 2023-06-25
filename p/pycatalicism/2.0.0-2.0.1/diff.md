# Comparing `tmp/pycatalicism-2.0.0.tar.gz` & `tmp/pycatalicism-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatalicism-2.0.0.tar", last modified: Sat Feb 11 16:00:36 2023, max compression
+gzip compressed data, was "pycatalicism-2.0.1.tar", last modified: Sun Jun 25 17:08:41 2023, max compression
```

## Comparing `pycatalicism-2.0.0.tar` & `pycatalicism-2.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/
--rw-r--r--   0 d         (1000) d         (1000)    33507 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)    33035 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/README.md
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.225572 pycatalicism-2.0.0/pycatalicism/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     3167 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/activation_config.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.235572 pycatalicism-2.0.0/pycatalicism/calc/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      255 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/activity.py
--rw-r--r--   0 d         (1000) d         (1000)     3994 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/calc.py
--rw-r--r--   0 d         (1000) d         (1000)     2423 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/calculator.py
--rw-r--r--   0 d         (1000) d         (1000)     1458 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/calculator_factory.py
--rw-r--r--   0 d         (1000) d         (1000)       97 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/calculatorexception.py
--rw-r--r--   0 d         (1000) d         (1000)     8320 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py
--rw-r--r--   0 d         (1000) d         (1000)     3348 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co2_hydrogenation_exporter.py
--rw-r--r--   0 d         (1000) d         (1000)     6353 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co2_hydrogenation_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)     5972 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co2hydrogenationcalculator.py
--rw-r--r--   0 d         (1000) d         (1000)     4311 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py
--rw-r--r--   0 d         (1000) d         (1000)     2468 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co_oxidation_exporter.py
--rw-r--r--   0 d         (1000) d         (1000)     2662 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/co_oxidation_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)     2541 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/conversion.py
--rw-r--r--   0 d         (1000) d         (1000)     3412 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/cooxidationcalculator.py
--rw-r--r--   0 d         (1000) d         (1000)     1027 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/exporter.py
--rw-r--r--   0 d         (1000) d         (1000)     1013 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/exporter_factory.py
--rw-r--r--   0 d         (1000) d         (1000)      103 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/exporterexception.py
--rw-r--r--   0 d         (1000) d         (1000)      903 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/parser.py
--rw-r--r--   0 d         (1000) d         (1000)      837 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/parser_factory.py
--rw-r--r--   0 d         (1000) d         (1000)       98 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/parserexception.py
--rw-r--r--   0 d         (1000) d         (1000)     1117 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/plotter.py
--rw-r--r--   0 d         (1000) d         (1000)      970 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/plotter_factory.py
--rw-r--r--   0 d         (1000) d         (1000)       84 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/plotterexception.py
--rw-r--r--   0 d         (1000) d         (1000)     8075 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/rawdata.py
--rw-r--r--   0 d         (1000) d         (1000)     4674 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/calc/selectivity.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.235572 pycatalicism-2.0.0/pycatalicism/chromatograph/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     6738 2023-02-11 15:57:57.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_analytic_modbus.py
--rw-r--r--   0 d         (1000) d         (1000)     8950 2023-02-11 15:57:57.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_control_panel_modbus.py
--rw-r--r--   0 d         (1000) d         (1000)    10008 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_crystal_5000.py
--rw-r--r--   0 d         (1000) d         (1000)      214 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/chromatograph_exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)      817 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/chromatograph_logging.py
--rw-r--r--   0 d         (1000) d         (1000)      392 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/logging_config.py
--rw-r--r--   0 d         (1000) d         (1000)     3679 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/chromatograph/modbus_converter.py
--rw-r--r--   0 d         (1000) d         (1000)     6211 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/config.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.235572 pycatalicism-2.0.0/pycatalicism/furnace/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)      317 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/furnace_exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)      814 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/furnace_logging.py
--rw-r--r--   0 d         (1000) d         (1000)      201 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/logging_config.py
--rw-r--r--   0 d         (1000) d         (1000)    27452 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/owen_protocol.py
--rw-r--r--   0 d         (1000) d         (1000)     3566 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/furnace/owen_tmp101.py
--rw-r--r--   0 d         (1000) d         (1000)     1884 2023-02-11 15:49:54.000000 pycatalicism-2.0.0/pycatalicism/init_conc_config.py
--rw-r--r--   0 d         (1000) d         (1000)     3453 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/logging_decorator.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     6373 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py
--rw-r--r--   0 d         (1000) d         (1000)     1385 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py
--rw-r--r--   0 d         (1000) d         (1000)      160 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/logging_config.py
--rw-r--r--   0 d         (1000) d         (1000)      874 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py
--rw-r--r--   0 d         (1000) d         (1000)      240 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/mass_flow_controller/mfc_exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)     2124 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/measurement_config.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/pycatalicism/plotters/
--rw-r--r--   0 d         (1000) d         (1000)        0 2022-09-10 14:55:06.000000 pycatalicism-2.0.0/pycatalicism/plotters/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     1764 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/plotters/data.py
--rw-r--r--   0 d         (1000) d         (1000)     4662 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/plotters/non_blocking_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)     1124 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/plotters/point.py
--rw-r--r--   0 d         (1000) d         (1000)     4261 2022-09-23 14:28:14.000000 pycatalicism-2.0.0/pycatalicism/plotters/process_plotter.py
--rw-r--r--   0 d         (1000) d         (1000)    36180 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/pycat.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/pycatalicism/valves/
--rw-r--r--   0 d         (1000) d         (1000)        0 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/valves/__init__.py
--rw-r--r--   0 d         (1000) d         (1000)     7381 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/valves/arduino_valve_controller.py
--rw-r--r--   0 d         (1000) d         (1000)      155 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/valves/logging_config.py
--rw-r--r--   0 d         (1000) d         (1000)     1163 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/valves/valves_exceptions.py
--rw-r--r--   0 d         (1000) d         (1000)      860 2023-02-11 15:48:24.000000 pycatalicism-2.0.0/pycatalicism/valves/valves_logging.py
-drwxr-xr-x   0 d         (1000) d         (1000)        0 2023-02-11 16:00:36.225572 pycatalicism-2.0.0/pycatalicism.egg-info/
--rw-r--r--   0 d         (1000) d         (1000)    33507 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/PKG-INFO
--rw-r--r--   0 d         (1000) d         (1000)     2799 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/SOURCES.txt
--rw-r--r--   0 d         (1000) d         (1000)        1 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/dependency_links.txt
--rw-r--r--   0 d         (1000) d         (1000)       50 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/entry_points.txt
--rw-r--r--   0 d         (1000) d         (1000)       90 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/requires.txt
--rw-r--r--   0 d         (1000) d         (1000)       13 2023-02-11 16:00:36.000000 pycatalicism-2.0.0/pycatalicism.egg-info/top_level.txt
--rw-r--r--   0 d         (1000) d         (1000)       38 2023-02-11 16:00:36.238906 pycatalicism-2.0.0/setup.cfg
--rw-r--r--   0 d         (1000) d         (1000)     1098 2023-02-11 15:50:14.000000 pycatalicism-2.0.0/setup.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/
+-rw-rw-r--   0 d         (1000) d         (1000)    33826 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)    33353 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/README.md
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.769925 pycatalicism-2.0.1/pycatalicism/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3167 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/activation_config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/calc/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      255 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/activity.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3994 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calc.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2423 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1458 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculator_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       97 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculatorexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8320 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3348 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6353 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     5972 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationcalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4311 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2468 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2662 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2541 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/conversion.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3412 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/cooxidationcalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1027 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1013 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporter_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)      103 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporterexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)      903 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parser.py
+-rw-rw-r--   0 d         (1000) d         (1000)      837 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parser_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       98 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parserexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1117 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)      970 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotter_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       84 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotterexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8075 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/rawdata.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4674 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/selectivity.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/chromatograph/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6738 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_analytic_modbus.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8950 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_control_panel_modbus.py
+-rw-rw-r--   0 d         (1000) d         (1000)    10008 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_crystal_5000.py
+-rw-rw-r--   0 d         (1000) d         (1000)      214 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      817 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      392 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3679 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/modbus_converter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6211 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/furnace/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      317 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/furnace_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      814 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/furnace_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      201 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)    27681 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/pycatalicism/furnace/owen_protocol.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3566 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/owen_tmp101.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1884 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/init_conc_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3453 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/logging_decorator.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6373 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1385 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py
+-rw-rw-r--   0 d         (1000) d         (1000)      160 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)      874 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      240 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mfc_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2124 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/measurement_config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/pycatalicism/plotters/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1764 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/data.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4662 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/non_blocking_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1124 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/point.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4261 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/process_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)    36180 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/pycat.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/pycatalicism/valves/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     7381 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/arduino_valve_controller.py
+-rw-rw-r--   0 d         (1000) d         (1000)      155 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1163 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/valves_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      860 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/valves_logging.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.769925 pycatalicism-2.0.1/pycatalicism.egg-info/
+-rw-rw-r--   0 d         (1000) d         (1000)    33826 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)     2799 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/SOURCES.txt
+-rw-rw-r--   0 d         (1000) d         (1000)        1 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/dependency_links.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       50 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/entry_points.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       90 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/requires.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       13 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/top_level.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       38 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/setup.cfg
+-rw-rw-r--   0 d         (1000) d         (1000)     1099 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/setup.py
```

### Comparing `pycatalicism-2.0.0/PKG-INFO` & `pycatalicism-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycatalicism
-Version: 2.0.0
-Summary: Program controls catalytic activity of materials measurement equipment as well calculations
+Version: 2.0.1
+Summary: Program controls catalytic activity of materials measurement equipment as well as calculations
 Home-page: https://github.com/leybodv/pycatalicism
 Author: Denis Leybo
-Author-email: leybodv@gmail.com
+Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 
 <h1>pycatalicism</h1>
@@ -20,14 +20,15 @@
     <li><a href="#furnace-control">Управление печи</a></li>
     <li><a href="#chromatograph-control">Управление хроматографом</a></li>
     <li><a href="#mfc">Управление регуляторами расхода газов</a></li>
     <li><a href="#valves">Управление соленоидными клапанами</a></li>
     <li><a href="#activation">Проведение активации</a></li>
     <li><a href="#measurement">Проведение измерения</a></li>
     <li><a href="#init-conc-measurement">Проведение измерения исходной концентрации реагентов</a></li>
+    <li><a href="#changes">Изменения в новых версиях</a></li>
   </ol>
   <h2 id="installation">Установка программы</h2>
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
@@ -334,7 +335,12 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
+    <h2 id="changes">Изменения в новых версиях</h2>
+    <ul>
+      <li>2.0.1</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+    </ul>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.0 Summary: Program
-controls catalytic activity of materials measurement equipment as well
+Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.1 Summary: Program
+controls catalytic activity of materials measurement equipment as well as
 calculations Home-page: https://github.com/leybodv/pycatalicism Author: Denis
-Leybo Author-email: leybodv@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >3.10.0 Description-
-Content-Type: text/markdown
+Leybo Author-email: denis@leybo.xyz Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >3.10.0 Description-Content-Type:
+text/markdown
 ****** pycatalicism ******
 ÐÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ ÐºÐ¾Ð½ÑÑÐ¾Ð»Ñ Ð¾Ð±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ñ Ð´Ð»Ñ
 Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ ÐºÐ°ÑÐ°Ð»Ð¸ÑÐ¸ÑÐµÑÐºÐ¸Ñ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº
 Ð¼Ð°ÑÐµÑÐ¸Ð°Ð»Ð¾Ð² Ð² Ð¿ÑÐ¾ÑÐ¾ÑÐ½Ð¾Ð¼ ÑÐµÐ¶Ð¸Ð¼Ðµ Ð² ÑÐµÐ°ÐºÑÐ¸ÑÑ
 Ð¾ÐºÐ¸ÑÐ»ÐµÐ½Ð¸Ñ CO Ð¸ Ð³Ð¸Ð´ÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð¸Ñ CO2 Ñ
 Ð¾Ð±ÑÐ°Ð·Ð¾Ð²Ð°Ð½Ð¸ÐµÐ¼ CO Ð¸ Ð°Ð»ÐºÐ°Ð½Ð¾Ð² Ð´Ð¾ Ð¿ÐµÐ½ÑÐ°Ð½Ð°.
 ÐÐ±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ðµ ÑÐ¾ÑÑÐ¾Ð¸Ñ Ð¸Ð· 3Ñ ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ¾Ð²
@@ -26,14 +26,15 @@
    4. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÑÐ¾Ð¼Ð°ÑÐ¾Ð³ÑÐ°ÑÐ¾Ð¼
    5. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ°Ð¼Ð¸_ÑÐ°ÑÑÐ¾Ð´Ð°_Ð³Ð°Ð·Ð¾Ð²
    6. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐ¾Ð»ÐµÐ½Ð¾Ð¸Ð´Ð½ÑÐ¼Ð¸_ÐºÐ»Ð°Ð¿Ð°Ð½Ð°Ð¼Ð¸
    7. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð°ÐºÑÐ¸Ð²Ð°ÑÐ¸Ð¸
    8. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ
    9. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ_Ð¸ÑÑÐ¾Ð´Ð½Ð¾Ð¹
       ÐºÐ¾Ð½ÑÐµÐ½ÑÑÐ°ÑÐ¸Ð¸_ÑÐµÐ°Ð³ÐµÐ½ÑÐ¾Ð²
+  10. ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ_Ð²_Ð½Ð¾Ð²ÑÑ_Ð²ÐµÑÑÐ¸ÑÑ
 ***** Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ *****
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
@@ -391,7 +392,10 @@
 ***** Ð¢ÑÐÑ *****
     * Ð¿ÐµÑÐµÐ¿Ð¸ÑÐ°ÑÑ Ð¼Ð¾Ð´ÑÐ»Ñ calc: ÑÐµÐ»ÐµÐºÑÐ¸Ð²Ð½Ð¾ÑÑÑ
       Ð´Ð¾Ð»Ð¶Ð½Ð° ÑÐ°ÑÑÑÐ¸ÑÑÐ²Ð°ÑÑÑÑ Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸,
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
+***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
+    * 2.0.1
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
```

### Comparing `pycatalicism-2.0.0/README.md` & `pycatalicism-2.0.1/pycatalicism.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,34 @@
+Metadata-Version: 2.1
+Name: pycatalicism
+Version: 2.0.1
+Summary: Program controls catalytic activity of materials measurement equipment as well as calculations
+Home-page: https://github.com/leybodv/pycatalicism
+Author: Denis Leybo
+Author-email: denis@leybo.xyz
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.10.0
+Description-Content-Type: text/markdown
+
 <h1>pycatalicism</h1>
 <p>Программа для контроля оборудования для измерения каталитических характеристик материалов в проточном режиме в реакциях окисления CO и гидрирования CO<sub>2</sub> с образованием CO и алканов до пентана. Оборудование состоит из 3х регуляторов расхода газа, печи и хроматографа. Контроль температуры печи осуществляется с помощью ПИД регулятора. Также с помощью программы можно проводить расчёт основных параметров: конверсии (степени превращения) каталитической реакции, активности и селективности.</p>
   <h2>Содержание</h2>
   <ol>
     <li><a href="#installation">Установка программы</a></li>
     <li><a href="#calc">Рассчёт параметров</a></li>
     <li><a href="#furnace-control">Управление печи</a></li>
     <li><a href="#chromatograph-control">Управление хроматографом</a></li>
     <li><a href="#mfc">Управление регуляторами расхода газов</a></li>
     <li><a href="#valves">Управление соленоидными клапанами</a></li>
     <li><a href="#activation">Проведение активации</a></li>
     <li><a href="#measurement">Проведение измерения</a></li>
     <li><a href="#init-conc-measurement">Проведение измерения исходной концентрации реагентов</a></li>
+    <li><a href="#changes">Изменения в новых версиях</a></li>
   </ol>
   <h2 id="installation">Установка программы</h2>
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
@@ -321,7 +335,12 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
+    <h2 id="changes">Изменения в новых версиях</h2>
+    <ul>
+      <li>2.0.1</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+    </ul>
```

#### html2text {}

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.1 Summary: Program
+controls catalytic activity of materials measurement equipment as well as
+calculations Home-page: https://github.com/leybodv/pycatalicism Author: Denis
+Leybo Author-email: denis@leybo.xyz Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >3.10.0 Description-Content-Type:
+text/markdown
 ****** pycatalicism ******
 ÐÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ ÐºÐ¾Ð½ÑÑÐ¾Ð»Ñ Ð¾Ð±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ñ Ð´Ð»Ñ
 Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ ÐºÐ°ÑÐ°Ð»Ð¸ÑÐ¸ÑÐµÑÐºÐ¸Ñ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº
 Ð¼Ð°ÑÐµÑÐ¸Ð°Ð»Ð¾Ð² Ð² Ð¿ÑÐ¾ÑÐ¾ÑÐ½Ð¾Ð¼ ÑÐµÐ¶Ð¸Ð¼Ðµ Ð² ÑÐµÐ°ÐºÑÐ¸ÑÑ
 Ð¾ÐºÐ¸ÑÐ»ÐµÐ½Ð¸Ñ CO Ð¸ Ð³Ð¸Ð´ÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð¸Ñ CO2 Ñ
 Ð¾Ð±ÑÐ°Ð·Ð¾Ð²Ð°Ð½Ð¸ÐµÐ¼ CO Ð¸ Ð°Ð»ÐºÐ°Ð½Ð¾Ð² Ð´Ð¾ Ð¿ÐµÐ½ÑÐ°Ð½Ð°.
 ÐÐ±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ðµ ÑÐ¾ÑÑÐ¾Ð¸Ñ Ð¸Ð· 3Ñ ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ¾Ð²
@@ -19,14 +26,15 @@
    4. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÑÐ¾Ð¼Ð°ÑÐ¾Ð³ÑÐ°ÑÐ¾Ð¼
    5. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ°Ð¼Ð¸_ÑÐ°ÑÑÐ¾Ð´Ð°_Ð³Ð°Ð·Ð¾Ð²
    6. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐ¾Ð»ÐµÐ½Ð¾Ð¸Ð´Ð½ÑÐ¼Ð¸_ÐºÐ»Ð°Ð¿Ð°Ð½Ð°Ð¼Ð¸
    7. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð°ÐºÑÐ¸Ð²Ð°ÑÐ¸Ð¸
    8. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ
    9. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ_Ð¸ÑÑÐ¾Ð´Ð½Ð¾Ð¹
       ÐºÐ¾Ð½ÑÐµÐ½ÑÑÐ°ÑÐ¸Ð¸_ÑÐµÐ°Ð³ÐµÐ½ÑÐ¾Ð²
+  10. ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ_Ð²_Ð½Ð¾Ð²ÑÑ_Ð²ÐµÑÑÐ¸ÑÑ
 ***** Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ *****
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
@@ -384,7 +392,10 @@
 ***** Ð¢ÑÐÑ *****
     * Ð¿ÐµÑÐµÐ¿Ð¸ÑÐ°ÑÑ Ð¼Ð¾Ð´ÑÐ»Ñ calc: ÑÐµÐ»ÐµÐºÑÐ¸Ð²Ð½Ð¾ÑÑÑ
       Ð´Ð¾Ð»Ð¶Ð½Ð° ÑÐ°ÑÑÑÐ¸ÑÑÐ²Ð°ÑÑÑÑ Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸,
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
+***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
+    * 2.0.1
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
```

### Comparing `pycatalicism-2.0.0/pycatalicism/activation_config.py` & `pycatalicism-2.0.1/pycatalicism/activation_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/calc.py` & `pycatalicism-2.0.1/pycatalicism/calc/calc.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/calculator.py` & `pycatalicism-2.0.1/pycatalicism/calc/calculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/calculator_factory.py` & `pycatalicism-2.0.1/pycatalicism/calc/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py` & `pycatalicism-2.0.1/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co2_hydrogenation_exporter.py` & `pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co2_hydrogenation_plotter.py` & `pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co2hydrogenationcalculator.py` & `pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationcalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py` & `pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co_oxidation_exporter.py` & `pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/co_oxidation_plotter.py` & `pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/conversion.py` & `pycatalicism-2.0.1/pycatalicism/calc/conversion.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/cooxidationcalculator.py` & `pycatalicism-2.0.1/pycatalicism/calc/cooxidationcalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/exporter.py` & `pycatalicism-2.0.1/pycatalicism/calc/exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/exporter_factory.py` & `pycatalicism-2.0.1/pycatalicism/calc/exporter_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/parser.py` & `pycatalicism-2.0.1/pycatalicism/calc/parser.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/parser_factory.py` & `pycatalicism-2.0.1/pycatalicism/calc/parser_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/plotter.py` & `pycatalicism-2.0.1/pycatalicism/calc/plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/plotter_factory.py` & `pycatalicism-2.0.1/pycatalicism/calc/plotter_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/rawdata.py` & `pycatalicism-2.0.1/pycatalicism/calc/rawdata.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/calc/selectivity.py` & `pycatalicism-2.0.1/pycatalicism/calc/selectivity.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_analytic_modbus.py` & `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_analytic_modbus.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_control_panel_modbus.py` & `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_control_panel_modbus.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/chromatograph/chromatec_crystal_5000.py` & `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_crystal_5000.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/chromatograph/chromatograph_logging.py` & `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/chromatograph/modbus_converter.py` & `pycatalicism-2.0.1/pycatalicism/chromatograph/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/config.py` & `pycatalicism-2.0.1/pycatalicism/config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/furnace/furnace_logging.py` & `pycatalicism-2.0.1/pycatalicism/furnace/furnace_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/furnace/owen_protocol.py` & `pycatalicism-2.0.1/pycatalicism/furnace/owen_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,29 +128,31 @@
                     count += 1
                     time.sleep(1)
                 self._logger.warning(f'Connection problems were encountered: {ex}, trying to repeat. Trial #{count}')
         return pic
 
     def send_PIC(self, parameter:str, value:float):
         """
-        Set parameter value of type PIC to specified value.
+        Set parameter value of type PIC to specified value. If the value is not multiple of 0.5, the value will be rounded to the nearest integer (see issue #19).
 
         parameters
         ----------
         parameters:str
             parameter id
         value:float
             new value to set the parameter to
 
         raises
         ------
         FurnaceConnectionException
             if several trials were unsuccessful to set the new value
         """
-        data = self._float_to_PIC(value=value)
+        if (10 * value % 5) != 0:
+            self._logger.warning(f'Value {value} will be rounded to {round(value)}')
+        data = self._float_to_PIC(value=round(value))
         message = self._pack_message(command=parameter, is_request=False, data=data)
         count = 0
         while True:
             self._logger.debug(f'Sending PIC parameter "{parameter}". Trial #{count}.')
             try:
                 self._change_parameter_value(message=message)
                 break
```

### Comparing `pycatalicism-2.0.0/pycatalicism/furnace/owen_tmp101.py` & `pycatalicism-2.0.1/pycatalicism/furnace/owen_tmp101.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/init_conc_config.py` & `pycatalicism-2.0.1/pycatalicism/init_conc_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/logging_decorator.py` & `pycatalicism-2.0.1/pycatalicism/logging_decorator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py` & `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py` & `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py` & `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/measurement_config.py` & `pycatalicism-2.0.1/pycatalicism/measurement_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/plotters/data.py` & `pycatalicism-2.0.1/pycatalicism/plotters/data.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/plotters/non_blocking_plotter.py` & `pycatalicism-2.0.1/pycatalicism/plotters/non_blocking_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/plotters/point.py` & `pycatalicism-2.0.1/pycatalicism/plotters/point.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/plotters/process_plotter.py` & `pycatalicism-2.0.1/pycatalicism/plotters/process_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/pycat.py` & `pycatalicism-2.0.1/pycatalicism/pycat.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/valves/arduino_valve_controller.py` & `pycatalicism-2.0.1/pycatalicism/valves/arduino_valve_controller.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/valves/valves_exceptions.py` & `pycatalicism-2.0.1/pycatalicism/valves/valves_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism/valves/valves_logging.py` & `pycatalicism-2.0.1/pycatalicism/valves/valves_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/pycatalicism.egg-info/PKG-INFO` & `pycatalicism-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-Metadata-Version: 2.1
-Name: pycatalicism
-Version: 2.0.0
-Summary: Program controls catalytic activity of materials measurement equipment as well calculations
-Home-page: https://github.com/leybodv/pycatalicism
-Author: Denis Leybo
-Author-email: leybodv@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.10.0
-Description-Content-Type: text/markdown
-
 <h1>pycatalicism</h1>
 <p>Программа для контроля оборудования для измерения каталитических характеристик материалов в проточном режиме в реакциях окисления CO и гидрирования CO<sub>2</sub> с образованием CO и алканов до пентана. Оборудование состоит из 3х регуляторов расхода газа, печи и хроматографа. Контроль температуры печи осуществляется с помощью ПИД регулятора. Также с помощью программы можно проводить расчёт основных параметров: конверсии (степени превращения) каталитической реакции, активности и селективности.</p>
   <h2>Содержание</h2>
   <ol>
     <li><a href="#installation">Установка программы</a></li>
     <li><a href="#calc">Рассчёт параметров</a></li>
     <li><a href="#furnace-control">Управление печи</a></li>
     <li><a href="#chromatograph-control">Управление хроматографом</a></li>
     <li><a href="#mfc">Управление регуляторами расхода газов</a></li>
     <li><a href="#valves">Управление соленоидными клапанами</a></li>
     <li><a href="#activation">Проведение активации</a></li>
     <li><a href="#measurement">Проведение измерения</a></li>
     <li><a href="#init-conc-measurement">Проведение измерения исходной концентрации реагентов</a></li>
+    <li><a href="#changes">Изменения в новых версиях</a></li>
   </ol>
   <h2 id="installation">Установка программы</h2>
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
@@ -334,7 +322,12 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
+    <h2 id="changes">Изменения в новых версиях</h2>
+    <ul>
+      <li>2.0.1</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+    </ul>
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.0 Summary: Program
-controls catalytic activity of materials measurement equipment as well
-calculations Home-page: https://github.com/leybodv/pycatalicism Author: Denis
-Leybo Author-email: leybodv@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >3.10.0 Description-
-Content-Type: text/markdown
 ****** pycatalicism ******
 ÐÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ ÐºÐ¾Ð½ÑÑÐ¾Ð»Ñ Ð¾Ð±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ñ Ð´Ð»Ñ
 Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ ÐºÐ°ÑÐ°Ð»Ð¸ÑÐ¸ÑÐµÑÐºÐ¸Ñ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº
 Ð¼Ð°ÑÐµÑÐ¸Ð°Ð»Ð¾Ð² Ð² Ð¿ÑÐ¾ÑÐ¾ÑÐ½Ð¾Ð¼ ÑÐµÐ¶Ð¸Ð¼Ðµ Ð² ÑÐµÐ°ÐºÑÐ¸ÑÑ
 Ð¾ÐºÐ¸ÑÐ»ÐµÐ½Ð¸Ñ CO Ð¸ Ð³Ð¸Ð´ÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð¸Ñ CO2 Ñ
 Ð¾Ð±ÑÐ°Ð·Ð¾Ð²Ð°Ð½Ð¸ÐµÐ¼ CO Ð¸ Ð°Ð»ÐºÐ°Ð½Ð¾Ð² Ð´Ð¾ Ð¿ÐµÐ½ÑÐ°Ð½Ð°.
 ÐÐ±Ð¾ÑÑÐ´Ð¾Ð²Ð°Ð½Ð¸Ðµ ÑÐ¾ÑÑÐ¾Ð¸Ñ Ð¸Ð· 3Ñ ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ¾Ð²
@@ -26,14 +19,15 @@
    4. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÑÐ¾Ð¼Ð°ÑÐ¾Ð³ÑÐ°ÑÐ¾Ð¼
    5. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐµÐ³ÑÐ»ÑÑÐ¾ÑÐ°Ð¼Ð¸_ÑÐ°ÑÑÐ¾Ð´Ð°_Ð³Ð°Ð·Ð¾Ð²
    6. Ð£Ð¿ÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ_ÑÐ¾Ð»ÐµÐ½Ð¾Ð¸Ð´Ð½ÑÐ¼Ð¸_ÐºÐ»Ð°Ð¿Ð°Ð½Ð°Ð¼Ð¸
    7. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð°ÐºÑÐ¸Ð²Ð°ÑÐ¸Ð¸
    8. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ
    9. ÐÑÐ¾Ð²ÐµÐ´ÐµÐ½Ð¸Ðµ_Ð¸Ð·Ð¼ÐµÑÐµÐ½Ð¸Ñ_Ð¸ÑÑÐ¾Ð´Ð½Ð¾Ð¹
       ÐºÐ¾Ð½ÑÐµÐ½ÑÑÐ°ÑÐ¸Ð¸_ÑÐµÐ°Ð³ÐµÐ½ÑÐ¾Ð²
+  10. ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ_Ð²_Ð½Ð¾Ð²ÑÑ_Ð²ÐµÑÑÐ¸ÑÑ
 ***** Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ *****
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
@@ -391,7 +385,10 @@
 ***** Ð¢ÑÐÑ *****
     * Ð¿ÐµÑÐµÐ¿Ð¸ÑÐ°ÑÑ Ð¼Ð¾Ð´ÑÐ»Ñ calc: ÑÐµÐ»ÐµÐºÑÐ¸Ð²Ð½Ð¾ÑÑÑ
       Ð´Ð¾Ð»Ð¶Ð½Ð° ÑÐ°ÑÑÑÐ¸ÑÑÐ²Ð°ÑÑÑÑ Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸,
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
+***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
+    * 2.0.1
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
```

### Comparing `pycatalicism-2.0.0/pycatalicism.egg-info/SOURCES.txt` & `pycatalicism-2.0.1/pycatalicism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.0/setup.py` & `pycatalicism-2.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     "pyserial>=3.5",
     "pymodbus>=2.5.3,<2.6",
     "bronkhorst-propar>=1.0",
     ]
 
 setuptools.setup(
      name='pycatalicism',
-     version='2.0.0',
+     version='2.0.1',
      author="Denis Leybo",
-     author_email="leybodv@gmail.com",
-     description="Program controls catalytic activity of materials measurement equipment as well calculations",
+     author_email="denis@leybo.xyz",
+     description="Program controls catalytic activity of materials measurement equipment as well as calculations",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/leybodv/pycatalicism",
      packages=setuptools.find_packages(),
      install_requires = install_requires,
      python_requires='>3.10.0',
      entry_points={
```

