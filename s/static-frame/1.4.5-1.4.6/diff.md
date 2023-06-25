# Comparing `tmp/static-frame-1.4.5.tar.gz` & `tmp/static-frame-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.5.tar", last modified: Fri Jun  2 14:29:23 2023, max compression
+gzip compressed data, was "static-frame-1.4.6.tar", last modified: Sun Jun 25 04:40:42 2023, max compression
```

## Comparing `static-frame-1.4.5.tar` & `static-frame-1.4.6.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.803140 static-frame-1.4.5/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.4.5/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.4.5/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23224 2023-06-02 14:29:23.803140 static-frame-1.4.5/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23901 2023-05-28 22:47:27.000000 static-frame-1.4.5/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.4.5/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-27 18:00:43.000000 static-frame-1.4.5/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-27 18:00:43.000000 static-frame-1.4.5/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-06-02 14:29:23.807140 static-frame-1.4.5/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-01-27 15:25:04.000000 static-frame-1.4.5/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.755144 static-frame-1.4.5/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-06-02 13:56:30.000000 static-frame-1.4.5/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.779142 static-frame-1.4.5/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    59324 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-02-27 23:01:10.000000 static-frame-1.4.5/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2022-10-01 15:52:09.000000 static-frame-1.4.5/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 21:18:03.000000 static-frame-1.4.5/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-02-01 00:09:42.000000 static-frame-1.4.5/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-01-28 23:33:40.000000 static-frame-1.4.5/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-01-28 23:33:40.000000 static-frame-1.4.5/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    32016 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 21:18:03.000000 static-frame-1.4.5/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-02-28 22:54:13.000000 static-frame-1.4.5/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2022-11-10 00:09:54.000000 static-frame-1.4.5/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2022-10-13 03:47:27.000000 static-frame-1.4.5/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 18:53:08.000000 static-frame-1.4.5/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15150 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-08 23:21:40.000000 static-frame-1.4.5/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-02-03 19:24:20.000000 static-frame-1.4.5/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21484 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   177922 2023-05-28 21:54:57.000000 static-frame-1.4.5/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   129931 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2022-12-20 03:10:29.000000 static-frame-1.4.5/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-02-28 22:54:13.000000 static-frame-1.4.5/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.783142 static-frame-1.4.5/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.4.5/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.803140 static-frame-1.4.5/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-02-23 22:39:48.000000 static-frame-1.4.5/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-05-02 20:46:35.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-09 00:42:47.000000 static-frame-1.4.5/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-08 23:21:40.000000 static-frame-1.4.5/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-09 00:42:47.000000 static-frame-1.4.5/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.759143 static-frame-1.4.5/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23224 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.430760 static-frame-1.4.6/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.6/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.6/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23469 2023-06-25 04:40:42.430760 static-frame-1.4.6/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24106 2023-06-25 02:02:42.000000 static-frame-1.4.6/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.6/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-06-25 02:02:42.000000 static-frame-1.4.6/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-06-25 02:02:42.000000 static-frame-1.4.6/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-06-25 04:40:42.430760 static-frame-1.4.6/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.6/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.410759 static-frame-1.4.6/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-06-25 02:02:56.000000 static-frame-1.4.6/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.422759 static-frame-1.4.6/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    59324 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    32016 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15150 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21484 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   177922 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   129931 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.422759 static-frame-1.4.6/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.430760 static-frame-1.4.6/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.414759 static-frame-1.4.6/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23469 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.5/LICENSE.txt` & `static-frame-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/PKG-INFO` & `static-frame-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.5
+Version: 1.4.6
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -43,24 +43,29 @@
         -------------------------------
         
         StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
         
             conda install -c conda-forge static-frame
         
         
+        Installation via Pyodide
+        -------------------------------
+        
+        StaticFrame can be run in the browser via Pyodide with the ``static_frame_pyodide`` package: https://github.com/static-frame/static-frame-pyodide
+        
         
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - arraymap==0.1.9
-        - arraykit==0.4.8
+        - arraykit==0.4.9
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.4.5/README.rst` & `static-frame-1.4.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -85,24 +85,29 @@
 -------------------------------
 
 StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
 
     conda install -c conda-forge static-frame
 
 
+Installation via Pyodide
+-------------------------------
+
+StaticFrame can be run in the browser via Pyodide with the ``static_frame_pyodide`` package: https://github.com/static-frame/static-frame-pyodide
+
 
 Dependencies
 --------------
 
 Core StaticFrame requires the following:
 
 - Python>=3.7
 - NumPy>=1.18.5
 - arraymap==0.1.9
-- arraykit==0.4.8
+- arraykit==0.4.9
 
 For extended input and output, the following packages are required:
 
 - pandas>=0.24.2
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
 - xarray>=0.13.0
```

### Comparing `static-frame-1.4.5/setup.py` & `static-frame-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/__init__.py` & `static-frame-1.4.6/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.5'
+__version__ = '1.4.6'
```

### Comparing `static-frame-1.4.5/static_frame/__main__.py` & `static-frame-1.4.6/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/archive_npy.py` & `static-frame-1.4.6/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/axis_map.py` & `static-frame-1.4.6/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/batch.py` & `static-frame-1.4.6/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/bus.py` & `static-frame-1.4.6/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/container.py` & `static-frame-1.4.6/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/container_util.py` & `static-frame-1.4.6/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/display.py` & `static-frame-1.4.6/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/display_color.py` & `static-frame-1.4.6/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/display_config.py` & `static-frame-1.4.6/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/display_html_datatables.py` & `static-frame-1.4.6/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/display_visidata.py` & `static-frame-1.4.6/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/doc_str.py` & `static-frame-1.4.6/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/exception.py` & `static-frame-1.4.6/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/fill_value_auto.py` & `static-frame-1.4.6/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/frame.py` & `static-frame-1.4.6/static_frame/core/frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/hloc.py` & `static-frame-1.4.6/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index.py` & `static-frame-1.4.6/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_auto.py` & `static-frame-1.4.6/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_base.py` & `static-frame-1.4.6/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_correspondence.py` & `static-frame-1.4.6/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_datetime.py` & `static-frame-1.4.6/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_hierarchy.py` & `static-frame-1.4.6/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.6/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/interface.py` & `static-frame-1.4.6/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/interface_meta.py` & `static-frame-1.4.6/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/join.py` & `static-frame-1.4.6/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/loc_map.py` & `static-frame-1.4.6/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/memory_measure.py` & `static-frame-1.4.6/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_dt.py` & `static-frame-1.4.6/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_fill_value.py` & `static-frame-1.4.6/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_hashlib.py` & `static-frame-1.4.6/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_iter.py` & `static-frame-1.4.6/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_re.py` & `static-frame-1.4.6/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_selector.py` & `static-frame-1.4.6/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_str.py` & `static-frame-1.4.6/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_transpose.py` & `static-frame-1.4.6/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/node_values.py` & `static-frame-1.4.6/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/pivot.py` & `static-frame-1.4.6/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/platform.py` & `static-frame-1.4.6/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/protocol_dfi.py` & `static-frame-1.4.6/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.6/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/quilt.py` & `static-frame-1.4.6/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/rank.py` & `static-frame-1.4.6/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/series.py` & `static-frame-1.4.6/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store.py` & `static-frame-1.4.6/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_client_mixin.py` & `static-frame-1.4.6/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_config.py` & `static-frame-1.4.6/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_filter.py` & `static-frame-1.4.6/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_hdf5.py` & `static-frame-1.4.6/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_sqlite.py` & `static-frame-1.4.6/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_xlsx.py` & `static-frame-1.4.6/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/store_zip.py` & `static-frame-1.4.6/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/style_config.py` & `static-frame-1.4.6/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/type_blocks.py` & `static-frame-1.4.6/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/util.py` & `static-frame-1.4.6/static_frame/core/util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/www.py` & `static-frame-1.4.6/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/core/yarn.py` & `static-frame-1.4.6/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/test_case.py` & `static-frame-1.4.6/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.6/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.6/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_batch.py` & `static-frame-1.4.6/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_bus.py` & `static-frame-1.4.6/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_container.py` & `static-frame-1.4.6/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.6/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_display.py` & `static-frame-1.4.6/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.6/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_doc.py` & `static-frame-1.4.6/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.6/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.6/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.6/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index.py` & `static-frame-1.4.6/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_interface.py` & `static-frame-1.4.6/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.6/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.6/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.6/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.6/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.6/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.6/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_rank.py` & `static-frame-1.4.6/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_series.py` & `static-frame-1.4.6/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.6/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store.py` & `static-frame-1.4.6/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.6/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.6/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.6/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.6/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.6/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.6/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.6/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_util.py` & `static-frame-1.4.6/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_www.py` & `static-frame-1.4.6/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.6/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.5/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.6/static_frame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.5
+Version: 1.4.6
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -43,24 +43,29 @@
         -------------------------------
         
         StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
         
             conda install -c conda-forge static-frame
         
         
+        Installation via Pyodide
+        -------------------------------
+        
+        StaticFrame can be run in the browser via Pyodide with the ``static_frame_pyodide`` package: https://github.com/static-frame/static-frame-pyodide
+        
         
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - arraymap==0.1.9
-        - arraykit==0.4.8
+        - arraykit==0.4.9
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.4.5/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.6/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

