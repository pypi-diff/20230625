# Comparing `tmp/apache-sedona-1.4.0.tar.gz` & `tmp/apache-sedona-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-sedona-1.4.0.tar", last modified: Sun Mar 19 21:16:10 2023, max compression
+gzip compressed data, was "apache-sedona-1.4.1.tar", last modified: Sun Jun 25 01:25:08 2023, max compression
```

## Comparing `apache-sedona-1.4.0.tar` & `apache-sedona-1.4.1.tar`

### file list

```diff
@@ -1,101 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.200771 apache-sedona-1.4.0/apache_sedona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-19 21:16:10.000000 apache-sedona-1.4.0/apache_sedona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-19 21:16:10.000000 apache-sedona-1.4.0/apache_sedona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 21:16:10.000000 apache-sedona-1.4.0/apache_sedona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-19 21:16:10.000000 apache-sedona-1.4.0/apache_sedona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-19 21:16:10.000000 apache-sedona-1.4.0/apache_sedona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.200771 apache-sedona-1.4.0/sedona/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.200771 apache-sedona-1.4.0/sedona/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.200771 apache-sedona-1.4.0/sedona/core/SpatialRDD/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/circle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/linestring_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/point_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/polygon_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/rectangle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/SpatialRDD/spatial_rdd_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/file_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/grid_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/index_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/join_build_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/enums/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/formatMapper/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/disc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/geo_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/geo_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/formatMapper/shapefileParser/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/shapefileParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/wkb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/formatMapper/wkt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/geom/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/geom/envelope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/jvm/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/jvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/jvm/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/jvm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/jvm/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/core/spatialOperator/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/join_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/join_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/join_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/knn_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/range_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/range_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/spatialOperator/rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.204771 apache-sedona-1.4.0/sedona/register/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/register/geo_registrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/register/java_libs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/sedona/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/dataframe_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/st_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/st_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    43391 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/st_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/st_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/sedona/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/abstract_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/binary_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/geometry_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/geometry_serde.py
--rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/geometry_serde_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/serde.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/spatial_rdd_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/sedona/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/src/geom_buf.c
--rw-r--r--   0 runner    (1001) docker     (123)    24131 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/src/geomserde.c
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/src/geomserde_speedup_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-19 21:16:01.000000 apache-sedona-1.4.0/src/geos_c_dyn.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:16:10.208771 apache-sedona-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-19 21:16:02.000000 apache-sedona-1.4.0/tests/test_assign_raw_spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-19 21:16:02.000000 apache-sedona-1.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-19 21:16:02.000000 apache-sedona-1.4.0/tests/test_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-19 21:16:02.000000 apache-sedona-1.4.0/tests/test_multiple_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-03-19 21:16:02.000000 apache-sedona-1.4.0/tests/test_scala_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.672859 apache-sedona-1.4.1/apache_sedona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-25 01:25:08.000000 apache-sedona-1.4.1/apache_sedona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-25 01:25:08.000000 apache-sedona-1.4.1/apache_sedona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:25:08.000000 apache-sedona-1.4.1/apache_sedona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-25 01:25:08.000000 apache-sedona-1.4.1/apache_sedona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 01:25:08.000000 apache-sedona-1.4.1/apache_sedona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.676859 apache-sedona-1.4.1/sedona/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.676859 apache-sedona-1.4.1/sedona/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.676859 apache-sedona-1.4.1/sedona/core/SpatialRDD/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/circle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/linestring_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/point_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/polygon_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/rectangle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/SpatialRDD/spatial_rdd_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.676859 apache-sedona-1.4.1/sedona/core/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/file_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/grid_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/index_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/join_build_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/enums/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/core/formatMapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/disc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/geo_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/geo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/core/formatMapper/shapefileParser/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/shapefileParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/wkb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/formatMapper/wkt_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/core/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/geom/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/geom/envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/core/jvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/jvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/jvm/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/jvm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/jvm/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/core/spatialOperator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/join_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/join_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/join_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/knn_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/range_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/range_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/spatialOperator/rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.680859 apache-sedona-1.4.1/sedona/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/register/geo_registrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/register/java_libs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.684860 apache-sedona-1.4.1/sedona/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/spark/SedonaContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.684860 apache-sedona-1.4.1/sedona/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/dataframe_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/st_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/st_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49568 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/st_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/st_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.684860 apache-sedona-1.4.1/sedona/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/abstract_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/binary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/geometry_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/geometry_serde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/geometry_serde_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/serde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/spatial_rdd_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/sedona/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geom_buf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geom_buf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24131 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geomserde.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geomserde.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geomserde_speedup_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geos_c_dyn.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geos_c_dyn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/geos_c_dyn_funcs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/src/pygeos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/src/pygeos/c_api.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:25:08.688860 apache-sedona-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/tests/test_assign_raw_spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/tests/test_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/tests/test_multiple_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-25 01:24:57.000000 apache-sedona-1.4.1/tests/test_scala_example.py
```

### Comparing `apache-sedona-1.4.0/PKG-INFO` & `apache-sedona-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-sedona
-Version: 1.4.0
+Version: 1.4.1
 Summary: Apache Sedona is a cluster computing system for processing large-scale spatial data
 Home-page: https://sedona.apache.org
 Author: Apache Sedona
 Author-email: dev@sedona.apache.org
 License: Apache License v2.0
 Project-URL: Documentation, https://sedona.apache.org
 Project-URL: Source code, https://github.com/apache/sedona
@@ -20,7 +20,9 @@
 This library is the Python wrapper for Apache Sedona.
 
 Apache Sedona is a cluster computing system for processing large-scale spatial data. 
 Apache Sedona extends Apache Spark / SparkSQL with a set of out-of-the-box Spatial Resilient Distributed Datasets (SRDDs)/ SpatialSQL that efficiently load, process, and analyze large-scale spatial data across machines.
 
 Please visit the official Apache Sedona website:
 https://sedona.apache.org/
+
+Development environment setup docs: https://sedona.apache.org/latest-snapshot/setup/compile/#run-python-test
```

### Comparing `apache-sedona-1.4.0/apache_sedona.egg-info/PKG-INFO` & `apache-sedona-1.4.1/apache_sedona.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-sedona
-Version: 1.4.0
+Version: 1.4.1
 Summary: Apache Sedona is a cluster computing system for processing large-scale spatial data
 Home-page: https://sedona.apache.org
 Author: Apache Sedona
 Author-email: dev@sedona.apache.org
 License: Apache License v2.0
 Project-URL: Documentation, https://sedona.apache.org
 Project-URL: Source code, https://github.com/apache/sedona
@@ -20,7 +20,9 @@
 This library is the Python wrapper for Apache Sedona.
 
 Apache Sedona is a cluster computing system for processing large-scale spatial data. 
 Apache Sedona extends Apache Spark / SparkSQL with a set of out-of-the-box Spatial Resilient Distributed Datasets (SRDDs)/ SpatialSQL that efficiently load, process, and analyze large-scale spatial data across machines.
 
 Please visit the official Apache Sedona website:
 https://sedona.apache.org/
+
+Development environment setup docs: https://sedona.apache.org/latest-snapshot/setup/compile/#run-python-test
```

### Comparing `apache-sedona-1.4.0/apache_sedona.egg-info/SOURCES.txt` & `apache-sedona-1.4.1/apache_sedona.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.py
 apache_sedona.egg-info/PKG-INFO
 apache_sedona.egg-info/SOURCES.txt
 apache_sedona.egg-info/dependency_links.txt
 apache_sedona.egg-info/requires.txt
 apache_sedona.egg-info/top_level.txt
@@ -46,14 +47,16 @@
 sedona/core/spatialOperator/knn_query.py
 sedona/core/spatialOperator/range_query.py
 sedona/core/spatialOperator/range_query_raw.py
 sedona/core/spatialOperator/rdd.py
 sedona/register/__init__.py
 sedona/register/geo_registrator.py
 sedona/register/java_libs.py
+sedona/spark/SedonaContext.py
+sedona/spark/__init__.py
 sedona/sql/__init__.py
 sedona/sql/dataframe_api.py
 sedona/sql/exceptions.py
 sedona/sql/st_aggregates.py
 sedona/sql/st_constructors.py
 sedona/sql/st_functions.py
 sedona/sql/st_predicates.py
@@ -69,15 +72,20 @@
 sedona/utils/jvm.py
 sedona/utils/meta.py
 sedona/utils/prep.py
 sedona/utils/serde.py
 sedona/utils/spatial_rdd_parser.py
 sedona/utils/types.py
 src/geom_buf.c
+src/geom_buf.h
 src/geomserde.c
+src/geomserde.h
 src/geomserde_speedup_module.c
 src/geos_c_dyn.c
+src/geos_c_dyn.h
+src/geos_c_dyn_funcs.h
+src/pygeos/c_api.h
 tests/test_assign_raw_spatial_rdd.py
 tests/test_base.py
 tests/test_circle.py
 tests/test_multiple_meta.py
 tests/test_scala_example.py
```

### Comparing `apache-sedona-1.4.0/sedona/__init__.py` & `apache-sedona-1.4.1/sedona/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/__init__.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/circle_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/circle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/linestring_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/linestring_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/point_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/point_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/polygon_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/polygon_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/rectangle_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/rectangle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/spatial_rdd.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/spatial_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/SpatialRDD/spatial_rdd_factory.py` & `apache-sedona-1.4.1/sedona/core/SpatialRDD/spatial_rdd_factory.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/__init__.py` & `apache-sedona-1.4.1/sedona/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/__init__.py` & `apache-sedona-1.4.1/sedona/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/file_data_splitter.py` & `apache-sedona-1.4.1/sedona/core/enums/file_data_splitter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/grid_type.py` & `apache-sedona-1.4.1/sedona/core/enums/grid_type.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/index_type.py` & `apache-sedona-1.4.1/sedona/core/enums/index_type.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/join_build_side.py` & `apache-sedona-1.4.1/sedona/core/enums/join_build_side.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/enums/spatial.py` & `apache-sedona-1.4.1/sedona/core/enums/spatial.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/__init__.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/disc_utils.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/disc_utils.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/geo_json_reader.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/geo_json_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/geo_reader.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/geo_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/shapefileParser/__init__.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/shapefileParser/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/shapefileParser/shape_file_reader.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/shapefileParser/shape_file_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/wkb_reader.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/wkb_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/formatMapper/wkt_reader.py` & `apache-sedona-1.4.1/sedona/core/formatMapper/wkt_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/geom/__init__.py` & `apache-sedona-1.4.1/sedona/core/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/geom/circle.py` & `apache-sedona-1.4.1/sedona/core/geom/circle.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/geom/envelope.py` & `apache-sedona-1.4.1/sedona/core/geom/envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  specific language governing permissions and limitations
 #  under the License.
 
 from shapely.geometry import Polygon, Point
 from shapely.geometry.base import BaseGeometry
 
 from sedona.utils.decorators import require
-
+import math
 
 class Envelope(Polygon):
 
     def __init__(self, minx=0, maxx=1, miny=0, maxy=1):
         self.minx = minx
         self.maxx = maxx
         self.miny = miny
@@ -31,14 +31,23 @@
         super().__init__([
             [self.minx, self.miny],
             [self.minx, self.maxy],
             [self.maxx, self.maxy],
             [self.maxx, self.miny]
         ])
 
+    def isClose(self, a, b) -> bool:
+        return math.isclose(a, b, rel_tol=1e-9)
+
+    def __eq__(self, other) -> bool:
+        return self.isClose(self.minx, other.minx) and\
+                self.isClose(self.miny, other.miny) and\
+                self.isClose(self.maxx, other.maxx) and\
+                self.isClose(self.maxy, other.maxy)
+
     @require(["Envelope"])
     def create_jvm_instance(self, jvm):
         return jvm.Envelope(
             self.minx, self.maxx, self.miny, self.maxy
         )
 
     @classmethod
```

### Comparing `apache-sedona-1.4.0/sedona/core/jvm/__init__.py` & `apache-sedona-1.4.1/sedona/core/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/jvm/abstract.py` & `apache-sedona-1.4.1/sedona/core/jvm/abstract.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/jvm/config.py` & `apache-sedona-1.4.1/sedona/core/jvm/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 import os
 from re import findall
 from typing import Any, Optional, Tuple
 
 from py4j.protocol import Py4JJavaError
 from pyspark.sql import SparkSession
 from sedona.utils.decorators import classproperty
+import functools
+import inspect
+import warnings
 
+string_types = (type(b''), type(u''))
 
 def is_greater_or_equal_version(version_a: str, version_b: str) -> bool:
     if all([version_b, version_a]):
         version_numbers = version_a.split("."), version_b.split(".")
         if any([version[0] == "" for version in version_numbers]):
             return False
 
@@ -55,28 +59,85 @@
             return result
 
         return applier
 
     return wrapper
 
 
-def depreciated(version: str, substitute: str):
-    def wrapper(function):
-        def applier(*args, **kwargs):
-            result = function(*args, **kwargs)
-            sedona_version = SedonaMeta.version
-            if sedona_version >= version:
-                logging.warning("Function is depreciated")
-                if substitute:
-                    logging.warning(f"Please use {substitute} instead")
-            return result
+def deprecated(reason):
+    """
+    This is a decorator which can be used to mark functions
+    as deprecated. It will result in a warning being emitted
+    when the function is used.
+    """
+
+    if isinstance(reason, string_types):
+
+        # The @deprecated is used with a 'reason'.
+        #
+        # .. code-block:: python
+        #
+        #    @deprecated("please, use another function")
+        #    def old_function(x, y):
+        #      pass
+
+        def decorator(func1):
+
+            if inspect.isclass(func1):
+                fmt1 = "Call to deprecated class {name} ({reason})."
+            else:
+                fmt1 = "Call to deprecated function {name} ({reason})."
+
+            @functools.wraps(func1)
+            def new_func1(*args, **kwargs):
+                warnings.simplefilter('always', DeprecationWarning)
+                warnings.warn(
+                    fmt1.format(name=func1.__name__, reason=reason),
+                    category=DeprecationWarning,
+                    stacklevel=2
+                )
+                warnings.simplefilter('default', DeprecationWarning)
+                return func1(*args, **kwargs)
 
-        return applier
+            return new_func1
 
-    return wrapper
+        return decorator
+
+    elif inspect.isclass(reason) or inspect.isfunction(reason):
+
+        # The @deprecated is used without any 'reason'.
+        #
+        # .. code-block:: python
+        #
+        #    @deprecated
+        #    def old_function(x, y):
+        #      pass
+
+        func2 = reason
+
+        if inspect.isclass(func2):
+            fmt2 = "Call to deprecated class {name}."
+        else:
+            fmt2 = "Call to deprecated function {name}."
+
+        @functools.wraps(func2)
+        def new_func2(*args, **kwargs):
+            warnings.simplefilter('always', DeprecationWarning)
+            warnings.warn(
+                fmt2.format(name=func2.__name__),
+                category=DeprecationWarning,
+                stacklevel=2
+            )
+            warnings.simplefilter('default', DeprecationWarning)
+            return func2(*args, **kwargs)
+
+        return new_func2
+
+    else:
+        raise TypeError(repr(type(reason)))
 
 
 class SparkJars:
     @staticmethod
     def get_used_jars():
         spark = SparkSession._instantiatedSession
```

### Comparing `apache-sedona-1.4.0/sedona/core/jvm/translate.py` & `apache-sedona-1.4.1/sedona/core/jvm/translate.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/__init__.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/join_params.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/join_params.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/join_query.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/join_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/join_query_raw.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/join_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/knn_query.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/knn_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/range_query.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/range_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/range_query_raw.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/range_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/spatialOperator/rdd.py` & `apache-sedona-1.4.1/sedona/core/spatialOperator/rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/core/utils.py` & `apache-sedona-1.4.1/sedona/core/utils.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/exceptions.py` & `apache-sedona-1.4.1/sedona/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/register/__init__.py` & `apache-sedona-1.4.1/sedona/register/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/register/geo_registrator.py` & `apache-sedona-1.4.1/sedona/register/geo_registrator.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,54 +12,56 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import attr
-from pyspark.sql import SparkSession
 from py4j.java_gateway import java_import
+from pyspark.sql import SparkSession
 
+from sedona.core.jvm.config import deprecated
 from sedona.register.java_libs import SedonaJvmLib
 from sedona.utils.prep import assign_all
 
 assign_all()
 jvm_import = str
 
 
 @attr.s
 class SedonaRegistrator:
 
     @classmethod
+    @deprecated("Deprecated since 1.4.1, use SedonaContext.create() instead.")
     def registerAll(cls, spark: SparkSession) -> bool:
         """
         This is the core of whole package, It uses py4j to run wrapper which takes existing SparkSession
         and register all User Defined Functions by Apache Sedona developers, for this SparkSession.
 
         :param spark: pyspark.sql.SparkSession, spark session instance
         :return: bool, True if registration was correct.
         """
         spark.sql("SELECT 1 as geom").count()
         PackageImporter.import_jvm_lib(spark._jvm)
         cls.register(spark)
         return True
 
     @classmethod
+    @deprecated("Deprecated since 1.4.1, use SedonaContext.create() instead.")
     def register(cls, spark: SparkSession):
         return spark._jvm.SedonaSQLRegistrator.registerAll(spark._jsparkSession)
 
-
 class PackageImporter:
 
     @staticmethod
     def import_jvm_lib(jvm) -> bool:
         from sedona.core.utils import ImportedJvmLib
         """
         Imports all the specified methods and functions in jvm
         :param jvm: Jvm gateway from py4j
         :return:
         """
         for lib in SedonaJvmLib:
             java_import(jvm, lib.value)
             ImportedJvmLib.import_lib(lib.name)
 
-        return True
+        return True
```

### Comparing `apache-sedona-1.4.0/sedona/register/java_libs.py` & `apache-sedona-1.4.1/sedona/register/java_libs.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     GeometryAdapter = "org.apache.sedona.python.wrapper.adapters.GeometryAdapter"
     PointRDD = "org.apache.sedona.core.spatialRDD.PointRDD"
     PolygonRDD = "org.apache.sedona.core.spatialRDD.PolygonRDD"
     CircleRDD = "org.apache.sedona.core.spatialRDD.CircleRDD"
     LineStringRDD = "org.apache.sedona.core.spatialRDD.LineStringRDD"
     RectangleRDD = "org.apache.sedona.core.spatialRDD.RectangleRDD"
     SpatialRDD = "org.apache.sedona.core.spatialRDD.SpatialRDD"
-    FileDataSplitter = "org.apache.sedona.core.enums.FileDataSplitter"
+    FileDataSplitter = "org.apache.sedona.common.enums.FileDataSplitter"
     GeoJsonReader = "org.apache.sedona.core.formatMapper.GeoJsonReader"
     ShapeFileReader = "org.apache.sedona.core.formatMapper.shapefileParser.ShapefileReader"
     SedonaSQLRegistrator = "org.apache.sedona.sql.utils.SedonaSQLRegistrator"
     StorageLevel = "org.apache.spark.storage.StorageLevel"
     GridType = "org.apache.sedona.core.enums.GridType"
     IndexType = "org.apache.sedona.core.enums.IndexType"
     AdapterWrapper = "org.apache.sedona.python.wrapper.utils.PythonAdapterWrapper"
@@ -48,14 +48,15 @@
     EnvelopeAdapter = "org.apache.sedona.python.wrapper.adapters.EnvelopeAdapter"
     PythonConverter = "org.apache.sedona.python.wrapper.adapters.PythonConverter"
     PythonRddToJavaRDDAdapter = "org.apache.sedona.python.wrapper.adapters.PythonRddToJavaRDDAdapter"
     st_constructors = "org.apache.spark.sql.sedona_sql.expressions.st_constructors"
     st_functions = "org.apache.spark.sql.sedona_sql.expressions.st_functions"
     st_predicates = "org.apache.spark.sql.sedona_sql.expressions.st_predicates"
     st_aggregates = "org.apache.spark.sql.sedona_sql.expressions.st_aggregates"
+    SedonaContext = "org.apache.sedona.spark.SedonaContext"
 
     @classmethod
     def from_str(cls, geo_lib: str) -> 'SedonaJvmLib':
         try:
             lib = getattr(cls, geo_lib.upper())
         except AttributeError:
             raise AttributeError(f"{cls.__class__.__name__} has no {geo_lib} attribute")
```

### Comparing `apache-sedona-1.4.0/sedona/sql/__init__.py` & `apache-sedona-1.4.1/sedona/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/dataframe_api.py` & `apache-sedona-1.4.1/sedona/sql/dataframe_api.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/exceptions.py` & `apache-sedona-1.4.1/sedona/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/st_aggregates.py` & `apache-sedona-1.4.1/sedona/sql/st_aggregates.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/st_constructors.py` & `apache-sedona-1.4.1/sedona/sql/st_constructors.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/st_functions.py` & `apache-sedona-1.4.1/sedona/sql/st_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from sedona.sql.dataframe_api import call_sedona_function, ColumnOrName, ColumnOrNameOrNumber, validate_argument_types
 
 
 __all__ = [
     "ST_3DDistance",
     "ST_AddPoint",
     "ST_Area",
+    "ST_AreaSpheroid",
     "ST_AsBinary",
     "ST_AsEWKB",
     "ST_AsEWKT",
     "ST_AsGeoJSON",
     "ST_AsGML",
     "ST_AsKML",
     "ST_AsText",
@@ -41,32 +42,36 @@
     "ST_Centroid",
     "ST_Collect",
     "ST_CollectionExtract",
     "ST_ConcaveHull",
     "ST_ConvexHull",
     "ST_Difference",
     "ST_Distance",
+    "ST_DistanceSphere",
+    "ST_DistanceSpheroid",
     "ST_Dump",
     "ST_DumpPoints",
     "ST_EndPoint",
     "ST_Envelope",
     "ST_ExteriorRing",
     "ST_FlipCoordinates",
     "ST_Force_2D",
     "ST_GeoHash",
+    "ST_GeometricMedian",
     "ST_GeometryN",
     "ST_GeometryType",
     "ST_InteriorRingN",
     "ST_Intersection",
     "ST_IsClosed",
     "ST_IsEmpty",
     "ST_IsRing",
     "ST_IsSimple",
     "ST_IsValid",
     "ST_Length",
+    "ST_LengthSpheroid",
     "ST_LineFromMultiPoint",
     "ST_LineInterpolatePoint",
     "ST_LineMerge",
     "ST_LineSubstring",
     "ST_MakePolygon",
     "ST_MakeValid",
     "ST_MinimumBoundingCircle",
@@ -99,14 +104,18 @@
     "ST_XMin",
     "ST_Y",
     "ST_YMax",
     "ST_YMin",
     "ST_Z",
     "ST_ZMax",
     "ST_ZMin",
+    "ST_NumPoints",
+    "ST_Force3D",
+    "ST_NRings",
+    "ST_Translate"
 ]
 
 
 _call_st_function = partial(call_sedona_function, "st_functions")
 
 
 @validate_argument_types
@@ -148,14 +157,25 @@
     :param geometry: Geometry column to calculate the area of.
     :type geometry: ColumnOrName
     :return: Area of geometry as a double column.
     :rtype: Column
     """
     return _call_st_function("ST_Area", geometry)
 
+@validate_argument_types
+def ST_AreaSpheroid(geometry: ColumnOrName) -> Column:
+    """Calculate the area of a geometry using WGS84 spheroid.
+
+    :param geometry: Geometry column to calculate the area of.
+    :type geometry: ColumnOrName
+    :return: Area of geometry as a double column. Unit is meter.
+    :rtype: Column
+    """
+    return _call_st_function("ST_AreaSpheroid", geometry)
+
 
 @validate_argument_types
 def ST_AsBinary(geometry: ColumnOrName) -> Column:
     """Generate the Well-Known Binary (WKB) representation of a geometry.
 
     :param geometry: Geometry column to generate WKB for.
     :type geometry: ColumnOrName
@@ -390,14 +410,41 @@
     :param b: Other geometry column to use in the calculation.
     :type b: ColumnOrName
     :return: Two-dimensional cartesian distance between a and b as a double column.
     :rtype: Column
     """
     return _call_st_function("ST_Distance", (a, b))
 
+@validate_argument_types
+def ST_DistanceSpheroid(a: ColumnOrName, b: ColumnOrName) -> Column:
+    """Calculate the geodesic distance between two geometry columns using WGS84 spheroid.
+
+    :param a: Geometry column to use in the calculation.
+    :type a: ColumnOrName
+    :param b: Other geometry column to use in the calculation.
+    :type b: ColumnOrName
+    :return: Two-dimensional geodesic distance between a and b as a double column. Unit is meter.
+    :rtype: Column
+    """
+    return _call_st_function("ST_DistanceSpheroid", (a, b))
+
+@validate_argument_types
+def ST_DistanceSphere(a: ColumnOrName, b: ColumnOrName, radius: Optional[Union[ColumnOrName, float]] = 6371008.0) -> Column:
+    """Calculate the haversine/great-circle distance between two geometry columns using a given radius.
+
+    :param a: Geometry column to use in the calculation.
+    :type a: ColumnOrName
+    :param b: Other geometry column to use in the calculation.
+    :type b: ColumnOrName
+    :param radius: Radius of the sphere, defaults to 6371008.0
+    :type radius: Optional[Union[ColumnOrName, float]], optional
+    :return: Two-dimensional haversine/great-circle distance between a and b as a double column. Unit is meter.
+    :rtype: Column
+    """
+    return _call_st_function("ST_DistanceSphere", (a, b, radius))
 
 @validate_argument_types
 def ST_Dump(geometry: ColumnOrName) -> Column:
     """Returns an array of geometries that are members of a multi-geometry
     or geometry collection column. If the input geometry is a regular geometry
     then the geometry is returned inside of a single element array.
 
@@ -492,14 +539,39 @@
     :param precision: Precision level to hash geometry at, given as an integer or an integer column.
     :type precision: Union[ColumnOrName, int]
     :return: Geohash of geometry as a string column.
     :rtype: Column
     """
     return _call_st_function("ST_GeoHash", (geometry, precision))
 
+@validate_argument_types
+def ST_GeometricMedian(geometry: ColumnOrName, tolerance: Optional[Union[ColumnOrName, float]] = 1e-6,
+                       max_iter: Optional[Union[ColumnOrName, int]] = 1000,
+                       fail_if_not_converged: Optional[Union[ColumnOrName, bool]] = False) -> Column:
+    """Computes the approximate geometric median of a MultiPoint geometry using the Weiszfeld algorithm.
+    The geometric median provides a centrality measure that is less sensitive to outlier points than the centroid.
+    The algorithm will iterate until the distance change between successive iterations is less than the
+    supplied `tolerance` parameter. If this condition has not been met after `maxIter` iterations, the function will
+    produce an error and exit, unless `failIfNotConverged` is set to `false`. If a `tolerance` value is not provided,
+    a default `tolerance` value is `1e-6`.
+
+    :param geometry: MultiPoint or Point geometry.
+    :type geometry: ColumnOrName
+    :param tolerance: Distance limit change between successive iterations, defaults to 1e-6.
+    :type tolerance: Optional[Union[ColumnOrName, float]], optional
+    :param max_iter: Max number of iterations, defaults to 1000.
+    :type max_iter: Optional[Union[ColumnOrName, int]], optional
+    :param fail_if_not_converged: Generate error if not converged within given tolerance and number of iterations, defaults to False
+    :type fail_if_not_converged: Optional[Union[ColumnOrName, boolean]], optional
+    :return: Point geometry column.
+    :rtype: Column
+    """
+    args = (geometry, tolerance, max_iter, fail_if_not_converged)
+    return _call_st_function("ST_GeometricMedian", args)
+
 
 @validate_argument_types
 def ST_GeometryN(multi_geometry: ColumnOrName, n: Union[ColumnOrName, int]) -> Column:
     """Return the geometry at index n (0-th based) of a multi-geometry column.
 
     :param multi_geometry: Multi-geometry column to get from.
     :type multi_geometry: ColumnOrName
@@ -624,14 +696,24 @@
     :param geometry: Linestring geometry column to calculate length for.
     :type geometry: ColumnOrName
     :return: Length of geometry as a double column.
     :rtype: Column
     """
     return _call_st_function("ST_Length", geometry)
 
+@validate_argument_types
+def ST_LengthSpheroid(geometry: ColumnOrName) -> Column:
+    """Calculate the perimeter of a geometry using WGS84 spheroid.
+
+    :param geometry: Geometry column to calculate length for.
+    :type geometry: ColumnOrName
+    :return: perimeter of geometry as a double column. Unit is meter.
+    :rtype: Column
+    """
+    return _call_st_function("ST_LengthSpheroid", geometry)
 
 @validate_argument_types
 def ST_LineFromMultiPoint(geometry: ColumnOrName) -> Column:
     """Creates a LineString from a MultiPoint geometry.
 
     :param geometry: MultiPoint geometry column to create LineString from.
     :type geometry: ColumnOrName
@@ -1149,7 +1231,49 @@
 
     :param geometry: Geometry column to get the minimum Z coordinate from.
     :type geometry: ColumnOrName
     :return: Minimum Z coordinate for the geometry as a double column.
     :rtype: Column
     """
     return _call_st_function("ST_ZMin", geometry)
+@validate_argument_types
+def ST_NumPoints(geometry: ColumnOrName) -> Column:
+    """Return the number of points in a LineString
+    :param geometry: Geometry column to get number of points from.
+    :type geometry: ColumnOrName
+    :return: Number of points in a LineString as an integer column
+    :rtype: Column
+    """
+    return _call_st_function("ST_NumPoints", geometry)
+
+@validate_argument_types
+def ST_Force3D(geometry: ColumnOrName, zValue: Optional[Union[ColumnOrName, float]] = 0.0) -> Column:
+    """
+    Return a geometry with a 3D coordinate of value 'zValue' forced upon it. No change happens if the geometry is already 3D
+    :param zValue: Optional value of z coordinate to be potentially added, default value is 0.0
+    :param geometry: Geometry column to make 3D
+    :return: 3D geometry with either already present z coordinate if any, or zcoordinate with given zValue
+    """
+    args = (geometry, zValue)
+    return _call_st_function("ST_Force3D", args)
+
+@validate_argument_types
+def ST_NRings(geometry: ColumnOrName) -> Column:
+    """
+    Returns the total number of rings in a Polygon or MultiPolygon. Compared to ST_NumInteriorRings, ST_NRings takes exterior rings into account as well.
+    :param geometry: Geometry column to calculate rings for
+    :return: Number of exterior rings + interior rings (if any) for the given Polygon or MultiPolygon
+    """
+    return _call_st_function("ST_NRings", geometry)
+@validate_argument_types
+def ST_Translate(geometry: ColumnOrName, deltaX: Union[ColumnOrName, float], deltaY: Union[ColumnOrName, float], deltaZ: Optional[Union[ColumnOrName, float]] = 0.0) -> Column:
+    """
+    Returns the geometry with x, y and z (if present) coordinates offset by given deltaX, deltaY, and deltaZ values.
+    :param geometry: Geometry column whose coordinates are to be translated.
+    :param deltaX: value by which to offset X coordinate.
+    :param deltaY: value by which to offset Y coordinate.
+    :param deltaZ: value by which to offset Z coordinate (if present).
+    :return: The input geometry with its coordinates translated.
+    """
+    args = (geometry, deltaX, deltaY, deltaZ)
+    return _call_st_function("ST_Translate", args)
+
```

### Comparing `apache-sedona-1.4.0/sedona/sql/st_predicates.py` & `apache-sedona-1.4.1/sedona/sql/st_predicates.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/sql/types.py` & `apache-sedona-1.4.1/sedona/sql/types.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/__init__.py` & `apache-sedona-1.4.1/sedona/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/abstract_parser.py` & `apache-sedona-1.4.1/sedona/utils/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/adapter.py` & `apache-sedona-1.4.1/sedona/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/binary_parser.py` & `apache-sedona-1.4.1/sedona/utils/binary_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/decorators.py` & `apache-sedona-1.4.1/sedona/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/geometry_adapter.py` & `apache-sedona-1.4.1/sedona/utils/geometry_adapter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/geometry_serde.py` & `apache-sedona-1.4.1/sedona/utils/geometry_serde.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/geometry_serde_general.py` & `apache-sedona-1.4.1/sedona/utils/geometry_serde_general.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/jvm.py` & `apache-sedona-1.4.1/sedona/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/meta.py` & `apache-sedona-1.4.1/sedona/utils/meta.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/prep.py` & `apache-sedona-1.4.1/sedona/utils/prep.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/serde.py` & `apache-sedona-1.4.1/sedona/utils/serde.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/spatial_rdd_parser.py` & `apache-sedona-1.4.1/sedona/utils/spatial_rdd_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/utils/types.py` & `apache-sedona-1.4.1/sedona/utils/types.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/sedona/version.py` & `apache-sedona-1.4.1/sedona/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-version = "1.4.0"
+version = "1.4.1"
```

### Comparing `apache-sedona-1.4.0/setup.py` & `apache-sedona-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/src/geom_buf.c` & `apache-sedona-1.4.1/src/geom_buf.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/src/geomserde.c` & `apache-sedona-1.4.1/src/geomserde.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/src/geomserde_speedup_module.c` & `apache-sedona-1.4.1/src/geomserde_speedup_module.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/src/geos_c_dyn.c` & `apache-sedona-1.4.1/src/geos_c_dyn.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/tests/test_assign_raw_spatial_rdd.py` & `apache-sedona-1.4.1/tests/test_assign_raw_spatial_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/tests/test_base.py` & `apache-sedona-1.4.1/tests/test_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,35 +11,24 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-from pyspark.sql import SparkSession
-
-from sedona.register import SedonaRegistrator
-from sedona.utils import KryoSerializer, SedonaKryoRegistrator
+from sedona.spark import *
 from sedona.utils.decorators import classproperty
 
 
 class TestBase:
 
     @classproperty
     def spark(self):
         if not hasattr(self, "__spark"):
-            spark = SparkSession. \
-                builder. \
-                config("spark.serializer", KryoSerializer.getName).\
-                config("spark.kryo.registrator", SedonaKryoRegistrator.getName) .\
-                master("local[*]").\
-                getOrCreate()
-
-            SedonaRegistrator.registerAll(spark)
-
+            spark = SedonaContext.create(SedonaContext.builder().master("local[*]").getOrCreate())
             setattr(self, "__spark", spark)
         return getattr(self, "__spark")
 
     @classproperty
     def sc(self):
         if not hasattr(self, "__spark"):
             setattr(self, "__sc", self.spark._sc)
```

### Comparing `apache-sedona-1.4.0/tests/test_circle.py` & `apache-sedona-1.4.1/tests/test_circle.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/tests/test_multiple_meta.py` & `apache-sedona-1.4.1/tests/test_multiple_meta.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.4.0/tests/test_scala_example.py` & `apache-sedona-1.4.1/tests/test_scala_example.py`

 * *Files identical despite different names*

