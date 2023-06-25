# Comparing `tmp/tumourkit-0.7.3.tar.gz` & `tmp/tumourkit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.7.3.tar", last modified: Sat Jun  3 14:18:58 2023, max compression
+gzip compressed data, was "tumourkit-0.8.0.tar", last modified: Sun Jun 25 09:04:29 2023, max compression
```

## Comparing `tumourkit-0.7.3.tar` & `tumourkit-0.8.0.tar`

### file list

```diff
@@ -1,157 +1,161 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.989195 tumourkit-0.7.3/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.3/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-03 14:18:58.988704 tumourkit-0.7.3/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1580 2023-05-30 20:14:30.000000 tumourkit-0.7.3/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.856442 tumourkit-0.7.3/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.856222 tumourkit-0.7.3/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.869508 tumourkit-0.7.3/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.3/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.870110 tumourkit-0.7.3/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.3/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.3/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.3/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-03 14:18:58.989306 tumourkit-0.7.3/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.888004 tumourkit-0.7.3/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.3/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.3/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.3/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.3/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.3/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.3/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.3/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.3/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.3/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.3/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.3/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.3/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.3/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.3/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.3/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.3/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.3/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.3/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.3/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.3/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.892680 tumourkit-0.7.3/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-06-03 14:17:01.000000 tumourkit-0.7.3/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.902812 tumourkit-0.7.3/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.3/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.3/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.3/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.3/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.907183 tumourkit-0.7.3/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.3/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.3/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.3/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.3/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.3/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.3/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.3/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.3/tumourkit/classification/train_xgboost.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.909784 tumourkit-0.7.3/tumourkit/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.3/tumourkit/demo/app.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14850 2023-06-03 14:07:59.000000 tumourkit-0.7.3/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-31 20:15:09.000000 tumourkit-0.7.3/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.3/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.915939 tumourkit-0.7.3/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.3/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.3/tumourkit/postprocessing/draw_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.3/tumourkit/postprocessing/draw_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-06-03 11:50:00.000000 tumourkit-0.7.3/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-06-03 11:32:58.000000 tumourkit-0.7.3/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.3/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.3/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.925371 tumourkit-0.7.3/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.3/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.3/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.3/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.3/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.3/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.3/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.3/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.3/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.3/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.927018 tumourkit-0.7.3/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.3/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.3/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.3/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.928457 tumourkit-0.7.3/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.3/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-06-03 11:40:22.000000 tumourkit-0.7.3/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.932433 tumourkit-0.7.3/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.936252 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.940284 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.942255 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.946473 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.947607 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.959518 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.964703 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.974884 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.3/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.3/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.986264 tumourkit-0.7.3/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.3/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.3/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.3/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.3/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.3/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.3/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.3/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.3/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.3/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-03 14:18:58.896312 tumourkit-0.7.3/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       42 2023-06-03 14:18:58.000000 tumourkit-0.7.3/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.799968 tumourkit-0.8.0/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.8.0/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-25 09:04:29.799512 tumourkit-0.8.0/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1580 2023-05-30 20:14:30.000000 tumourkit-0.8.0/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.710879 tumourkit-0.8.0/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.710701 tumourkit-0.8.0/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.725884 tumourkit-0.8.0/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.8.0/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.726632 tumourkit-0.8.0/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.8.0/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2410 2023-06-24 13:06:46.000000 tumourkit-0.8.0/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      888 2023-06-24 14:09:20.000000 tumourkit-0.8.0/requirements.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.727118 tumourkit-0.8.0/results/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      657 2023-06-03 16:01:15.000000 tumourkit-0.8.0/results/comp_perc.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-06-25 09:04:29.800097 tumourkit-0.8.0/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.743585 tumourkit-0.8.0/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.8.0/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.8.0/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.8.0/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.8.0/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.8.0/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.8.0/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.8.0/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.8.0/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.8.0/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2218 2023-06-25 09:02:26.000000 tumourkit-0.8.0/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.8.0/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.8.0/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.8.0/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.8.0/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.8.0/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.8.0/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.8.0/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.8.0/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.8.0/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.8.0/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.747072 tumourkit-0.8.0/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-06-25 08:34:25.000000 tumourkit-0.8.0/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.754501 tumourkit-0.8.0/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.8.0/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.8.0/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.8.0/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7792 2023-06-25 07:52:45.000000 tumourkit-0.8.0/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.757677 tumourkit-0.8.0/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.8.0/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3011 2023-06-24 17:52:20.000000 tumourkit-0.8.0/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2463 2023-06-24 17:51:11.000000 tumourkit-0.8.0/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8284 2023-06-24 16:45:53.000000 tumourkit-0.8.0/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.8.0/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7994 2023-06-24 17:42:37.000000 tumourkit-0.8.0/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    23897 2023-06-24 17:54:49.000000 tumourkit-0.8.0/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.8.0/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.758148 tumourkit-0.8.0/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.8.0/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    15133 2023-06-25 07:52:59.000000 tumourkit-0.8.0/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9778 2023-06-24 15:41:13.000000 tumourkit-0.8.0/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.8.0/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.763679 tumourkit-0.8.0/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.8.0/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.8.0/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.8.0/tumourkit/postprocessing/draw_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4851 2023-06-24 14:22:10.000000 tumourkit-0.8.0/tumourkit/postprocessing/extract_tensorboard.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-06-03 11:50:00.000000 tumourkit-0.8.0/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8042 2023-06-24 17:06:04.000000 tumourkit-0.8.0/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.8.0/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3362 2023-06-24 14:56:13.000000 tumourkit-0.8.0/tumourkit/postprocessing/plot_logs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.8.0/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.769416 tumourkit-0.8.0/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.8.0/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.8.0/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.8.0/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.8.0/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3788 2023-06-25 09:01:32.000000 tumourkit-0.8.0/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.8.0/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.8.0/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.8.0/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.8.0/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.770608 tumourkit-0.8.0/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.8.0/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.8.0/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.8.0/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.771940 tumourkit-0.8.0/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.8.0/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    15663 2023-06-25 08:17:30.000000 tumourkit-0.8.0/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.774292 tumourkit-0.8.0/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.775977 tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.777783 tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.778633 tumourkit-0.8.0/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.780942 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.781397 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.786661 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.788278 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.792169 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.8.0/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12570 2023-06-25 07:45:28.000000 tumourkit-0.8.0/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.797361 tumourkit-0.8.0/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.8.0/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.8.0/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5746 2023-06-24 17:43:01.000000 tumourkit-0.8.0/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.8.0/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.8.0/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.8.0/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.8.0/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.8.0/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6472 2023-06-24 17:48:06.000000 tumourkit-0.8.0/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-06-25 09:04:29.750675 tumourkit-0.8.0/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42352 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5055 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1178 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      888 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       42 2023-06-25 09:04:29.000000 tumourkit-0.8.0/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.7.3/LICENSE` & `tumourkit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/PKG-INFO` & `tumourkit-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.3
+Version: 0.8.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.3/README.md` & `tumourkit-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2html.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2man.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.8.0/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.8.0/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/docs/source/conf.py` & `tumourkit-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/pyproject.toml` & `tumourkit-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -52,8 +52,10 @@
 run_inference = "tumourkit.infer_pipe:main"
 run_research = "tumourkit.research_pipe:main"
 run_evaluation = "tumourkit.eval_pipe:main"
 merge_cells = "tumourkit.postprocessing.merge_cells:main"
 remove_uncertain = "tumourkit.preprocessing.remove_uncertain:main"
 draw_cells = "tumourkit.postprocessing.draw_cells:main"
 start_app = "tumourkit.demo.app:main"
-draw_graph = "tumourkit.postprocessing.draw_graph:main"
+draw_graph = "tumourkit.postprocessing.draw_graph:main"
+extract_tensorboard = "tumourkit.postprocessing.extract_tensorboard:main"
+plot_logs = "tumourkit.postprocessing.plot_logs:main"
```

### Comparing `tumourkit-0.7.3/requirements.txt` & `tumourkit-0.8.0/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 attrs==22.2.0
+altair==5.0.1
+vl-convert-python
 beautifulsoup4==4.12.2
 certifi==2022.12.7
 charset-normalizer==3.0.1
 contourpy==1.0.7
 cycler==0.11.0
 docopt==0.6.2
 exceptiongroup==1.1.0
```

### Comparing `tumourkit-0.7.3/tests/centroidspng2csv_test.py` & `tumourkit-0.8.0/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/conf_matrix_sum_test.py` & `tumourkit-0.8.0/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/cpairs_test.py` & `tumourkit-0.8.0/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/example_test.py` & `tumourkit-0.8.0/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/generate_centroids.py` & `tumourkit-0.8.0/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/generate_rswoosh.py` & `tumourkit-0.8.0/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/get_conn_comp_test.py` & `tumourkit-0.8.0/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/graph2centroids_test.py` & `tumourkit-0.8.0/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/graph_idx_test.py` & `tumourkit-0.8.0/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/hov_prob_pipe_test.py` & `tumourkit-0.8.0/tests/hov_prob_pipe_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     args.by_img = False
     args.draw = False
     eval_class(args)
     args.json_dir = JSON_DIR
     args.graph_dir = TMP_DIR
     args.output_dir = TMP_DIR
     args.num_classes = 2
+    args.enable_background = False
     join_hovprob_graph_main(args)
     args.node_dir = TMP_DIR
     args.save_file = TEST_DIR + 'tmp2'
     eval_class(args)
     res1 = pd.read_csv(TEST_DIR + 'tmp.csv')
     res2 = pd.read_csv(TEST_DIR + 'tmp2.csv')
     assert (abs(res1['Accuracy'] - res2['Accuracy']) < 0.01)[0]
```

### Comparing `tumourkit-0.7.3/tests/hov_prob_test.py` & `tumourkit-0.8.0/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/hovernet_patches_test.py` & `tumourkit-0.8.0/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/metrics_pairs_test.py` & `tumourkit-0.8.0/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/metrics_test.py` & `tumourkit-0.8.0/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/png2graph_test.py` & `tumourkit-0.8.0/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/pngcsv2geojson_test.py` & `tumourkit-0.8.0/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/pngcsv2graph_test.py` & `tumourkit-0.8.0/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/read_nodes_test.py` & `tumourkit-0.8.0/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/remove_idx_test.py` & `tumourkit-0.8.0/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tests/rswoosh_test.py` & `tumourkit-0.8.0/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.8.0/tumourkit/classification/compute_imbalance.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/classification/evaluate.py` & `tumourkit-0.8.0/tumourkit/classification/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/classification/infer.py` & `tumourkit-0.8.0/tumourkit/classification/infer.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,33 +31,35 @@
 import pickle
 import numpy as np
 import pandas as pd
 import argparse
 import os
 
 
-def load_saved_model(weights_path: str, conf_path: str, num_classes: int, num_feats: int) -> nn.Module:
+def load_saved_model(weights_path: str, conf_path: str, num_classes: int, num_feats: int, enable_background: bool) -> nn.Module:
     """
     Loads a saved model from the given weights_path and conf_path.
 
     :param weights_path: The path to the saved weights file.
     :type weights_path: str
     :param conf_path: The path to the configuration file.
     :type conf_path: str
     :param num_classes: The number of classes for the model.
     :type num_classes: int
     :param num_feats: The number of features for the model.
     :type num_feats: int
+    :param enable_background: Enable when model has extra head to correct extra cells.
+    :type enable_background: bool
     :return: The loaded model.
     :rtype: nn.Module
     """
     state_dict = torch.load(weights_path, map_location='cpu')
     with open(conf_path, 'r') as f:
         conf = json.load(f)
-    model = load_model(conf, num_classes, num_feats)
+    model = load_model(conf, num_classes, num_feats, enable_background)
     model.load_state_dict(state_dict)
     return model
 
 
 def load_normalizer(norm_path: str) -> Tuple[Any]:
     """
     Loads the normalizers used in training from the given norm_path.
@@ -68,61 +70,85 @@
     :rtype: Tuple[Any]
     """
     with open(norm_path, 'rb') as f:
         normalizers = pickle.load(f)
     return normalizers
 
 
-def run_inference(model: nn.Module, loader: GraphDataLoader, device: str, num_classes: int) -> Dict[str, np.ndarray]:
+def run_inference(
+        model: nn.Module,
+        loader: GraphDataLoader,
+        device: str,
+        num_classes: int,
+        enable_background: bool,
+        ) -> Dict[str, np.ndarray]:
     """
     Runs inference using the specified model on the provided data loader.
 
     :param model: The model used for inference.
     :type model: nn.Module
     :param loader: The graph data loader.
     :type loader: GraphDataLoader
     :param device: The device used for inference (e.g., 'cpu' or 'cuda').
     :type device: str
     :param num_classes: The number of classes.
     :type num_classes: int
+    :param enable_background: Enable when model has extra head to correct extra cells.
+    :type enable_background: bool
     :return: The probabilities for all the nodes.
     :rtype: Dict[str, np.ndarray]
     """
     probs = {}
     for g, name in loader:
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
         features = g.ndata['X'].to(device)
         # Forward
         logits = model(g, features)
+        if enable_background:
+            logits, logits_bkgr = logits
         if num_classes == 2:
             prob = F.softmax(logits, dim=1).detach().numpy()[:, 1].reshape(-1, 1)
         else:
             prob = F.softmax(logits, dim=1).detach().numpy()
+        if enable_background:
+            prob_bkgr = F.softmax(logits_bkgr, dim=1).detach().numpy()[:, 1].reshape(-1, 1)
+            prob = np.hstack((prob_bkgr, prob))
         probs[name[0]] = prob
     return probs
 
 
-def save_probs(probs: Dict[str, np.ndarray], node_dir: str, output_dir: str, num_classes: int) -> None:
+def save_probs(
+        probs: Dict[str, np.ndarray],
+        node_dir: str,
+        output_dir: str,
+        num_classes: int,
+        enable_background: bool,
+        ) -> None:
     """
     Saves the probabilities in .nodes.csv files by appending a column to the original .nodes.csv file.
 
     :param probs: The probabilities for each graph.
     :type probs: Dict[str, np.ndarray]
     :param node_dir: The directory containing the original .nodes.csv files.
     :type node_dir: str
     :param output_dir: The directory where the updated .nodes.csv files will be saved.
     :type output_dir: str
+    :param enable_background: Enable when model has extra head to correct extra cells.
+    :type enable_background: bool
     :param num_classes: The number of classes.
     :type num_classes: int
     """
     for name, prob in probs.items():
         orig = pd.read_csv(os.path.join(node_dir, name))
+        if enable_background:
+            orig['prob0'] = prob[:, 0]
+            prob = prob[:, 1:]
         if num_classes == 2:
             orig['prob1'] = prob
         else:
             for k in range(1, num_classes + 1):
                 orig['prob' + str(k)] = prob[:, (k - 1)]
         orig.to_csv(output_dir + name, index=False)
 
@@ -138,14 +164,15 @@
     parser.add_argument('--conf', type=str, required=True,
                         help='Configuration file for the model.')
     parser.add_argument('--normalizers', type=str, required=True,
                         help='Path to normalizer objects for the model.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
     parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main_with_args(args):
     node_dir = parse_path(args.node_dir)
     output_dir = parse_path(args.output_dir)
     create_dir(output_dir)
@@ -158,17 +185,17 @@
     num_feats = 18 + (1 if args.num_classes == 2 else args.num_classes)
     if args.disable_morph_feats:
         num_feats -= 18
     if args.disable_prior:
         num_feats -= (1 if args.num_classes == 2 else args.num_classes)
     if num_feats == 0:
         num_feats = 1
-    model = load_saved_model(args.weights, args.conf, args.num_classes, num_feats)
+    model = load_saved_model(args.weights, args.conf, args.num_classes, num_feats, args.enable_background)
     model.eval()
-    probs = run_inference(model, eval_dataloader, 'cpu', args.num_classes)
-    save_probs(probs, node_dir, output_dir, args.num_classes)
+    probs = run_inference(model, eval_dataloader, 'cpu', args.num_classes, args.enable_background)
+    save_probs(probs, node_dir, output_dir, args.num_classes, args.enable_background)
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
     main(args)
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/models/gat.py` & `tumourkit-0.8.0/tumourkit/classification/models/gat.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 
 import torch.nn as nn
 import torch.nn.functional as F
 from dgl.nn import GATConv
 from .norm import Norm
 
 class GAT(nn.Module):
-    def __init__(self, in_size, hid_size, out_size, heads, num_layers, dropout, norm_type):
+    def __init__(self, in_size, hid_size, out_size, heads, num_layers, dropout, norm_type, enable_background=False):
         super().__init__()
         self.gat_layers = nn.ModuleList()
-        # two-layer GAT
         self.gat_layers.append(
             GATConv(
                 in_size,
                 hid_size,
                 heads[0],
                 feat_drop=dropout,
                 attn_drop=dropout,
@@ -63,16 +62,31 @@
                 heads[-1],
                 feat_drop=dropout,
                 attn_drop=dropout,
                 activation=None,
             )
         )
 
+        self.enable_background = enable_background
+        if enable_background:
+            self.bkgr_head = GATConv(
+                hid_size * heads[-2],
+                2,
+                heads[-1],
+                feat_drop=dropout,
+                attn_drop=dropout,
+                activation=None,
+            )
+
+
     def forward(self, g, inputs):
         h = inputs
         for i, layer in enumerate(self.gat_layers):
-            h = layer(g, h)
             if i == len(self.gat_layers)-1:  # last layer
-                h = h.mean(1)
+                if self.enable_background:
+                    h_bkgr = self.bkgr_head(g, h).mean(1)
+                    h = layer(g, h).mean(1)
+                    return h, h_bkgr
             else:  # other layer(s)
+                h = layer(g, h)
                 h = h.flatten(1)
         return h
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/models/gcn.py` & `tumourkit-0.8.0/tumourkit/classification/models/gcn.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,27 +26,39 @@
 
 import torch.nn as nn
 import torch.nn.functional as F
 from dgl.nn import GraphConv
 from .norm import Norm
 
 class GCN(nn.Module):
-    def __init__(self, in_feats, h_feats, num_classes, num_layers, drop_rate, norm_type):
+    def __init__(self, in_feats, h_feats, num_classes, num_layers, drop_rate, norm_type, enable_background=False):
         super(GCN, self).__init__()
         self.conv_layers = nn.ModuleList()
         self.conv_layers.append(GraphConv(in_feats, h_feats, activation=F.elu))
         self.conv_layers.append(nn.Dropout(drop_rate)) # Feature map dropout
         self.conv_layers.append(Norm(norm_type=norm_type, hidden_dim=h_feats))
         for l in range(1,num_layers):
             self.conv_layers.append(GraphConv(h_feats, h_feats, activation=F.elu))
             self.conv_layers.append(nn.Dropout(drop_rate))
             self.conv_layers.append(Norm(norm_type=norm_type, hidden_dim=h_feats))
         self.conv_layers.append(GraphConv(h_feats, num_classes))
 
+        self.enable_background = enable_background
+        if enable_background:
+            self.bkgr_head = GraphConv(h_feats, 2)
+
+
     def forward(self, g, in_feat):
         h = in_feat
         for i, layer in enumerate(self.conv_layers):
-            if i % 3 == 1:
-                h = layer(h) # Dropout
+            if i == len(self.conv_layers) - 1:
+                if self.enable_background:  # Last layer
+                    h_bkgr = self.bkgr_head(g, h)
+                    h = layer(g, h)
+                    return h, h_bkgr 
+                h = layer(g, h)
             else:
-                h = layer(g, h) # Other layers
+                if i % 3 == 1:
+                    h = layer(h)  # Dropout
+                else:
+                    h = layer(g, h)  # Other layers
         return h
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/models/hgao.py` & `tumourkit-0.8.0/tumourkit/classification/models/hgao.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         num_layers,
         dropout,
         norm_type,
         activation=F.elu,
         negative_slope=0.2,
         residual=False,
         k=8,
+        enable_background=False,
     ):
         super(HardGAT, self).__init__()
         feat_drop=dropout
         attn_drop=dropout
         self.num_layers = num_layers
         self.gat_layers = nn.ModuleList()
         self.activation = activation
@@ -211,13 +212,29 @@
                 attn_drop,
                 negative_slope,
                 False,
                 None,
             )
         )
 
+        self.enable_background = enable_background
+        if enable_background:
+            self.bkgr_head = gat_layer(
+                num_hidden * heads[-2],
+                2,
+                heads[-1],
+                feat_drop,
+                attn_drop,
+                negative_slope,
+                False,
+                None,
+            )
+
     def forward(self, g, inputs):
         h = inputs
         for l in range(self.num_layers):
             h = self.gat_layers[l](g, h).flatten(1)
         logits = self.gat_layers[-1](g, h).mean(1)
+        if self.enable_background:
+            logits_bkgr = self.bkgr_head(g, h).mean(1)
+            return logits, logits_bkgr
         return logits
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/models/norm.py` & `tumourkit-0.8.0/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/classification/read_graph.py` & `tumourkit-0.8.0/tumourkit/classification/read_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             column_normalize: Optional[bool] = False,
             row_normalize: Optional[bool] = False,
             normalizers: Optional[Tuple[Any]] = None,
             return_names: Optional[bool] = False,
             is_inference: Optional[bool] = False,
             remove_prior: Optional[bool] = False,
             remove_morph: Optional[bool] = False,
+            enable_background: Optional[bool] = False,
             ):
         """
         node_dir: Path to .nodes.csv files.
         max_dist: Maximum distance to consider two nodes as neighbours.
         max_degree: Maximum degree for each node.
         files: List of names to include in the dataset. If None all names are included.
         column_normalize: Whether to subtract mean and divide by standard deviation each feature.
@@ -73,46 +74,56 @@
         self.max_degree = max_degree
         self.transform = transform
         self.column_normalize = column_normalize
         self.row_normalize = row_normalize
         self.normalizers = normalizers
         self.remove_prior = remove_prior
         self.remove_morph = remove_morph
-        self.initialize_normalizers()
         self.return_names = return_names
         self.is_inference = is_inference
+        self.enable_background = enable_background
+        self.initialize_normalizers()
+
 
     def __getitem__(self, idx):
         file_name = self.node_names[idx] + '.nodes.csv'
-        X, y, xx, yy = read_node_matrix(
+        tmp = read_node_matrix(
             os.path.join(self.node_dir, file_name), return_coordinates=True, return_class=not self.is_inference,
-            remove_prior=self.remove_prior, remove_morph=self.remove_morph
+            remove_prior=self.remove_prior, remove_morph=self.remove_morph, enable_background=self.enable_background
             )
+        if self.enable_background:
+            X, y, xx, yy, y_bkgr = tmp
+        else:
+            X, y, xx, yy = tmp
         if self.column_normalize:
             X = self.col_sc.transform(X)
         if self.row_normalize:
             X = self.row_sc.transform(X)
         if self.normalizers is not None:
             for normalizer in self.normalizers:
                 X = normalizer.transform(X)
         if self.transform is not None:
             X = self.transform(X)
         source, dest, dists = GraphDataset.create_edges(xx, yy, self.max_degree, self.max_dist)
         g = dgl.graph((source, dest), num_nodes=len(X))
         g.ndata['X'] = torch.tensor(X, dtype=torch.float32)
         if not self.is_inference:
             g.ndata['y'] = torch.tensor(y, dtype=torch.long)
+            if self.enable_background:
+                g.ndata['y_bkgr'] = torch.tensor(y_bkgr, dtype=torch.long)
         g.edata['dist'] = torch.tensor(dists, dtype=torch.float32).reshape((-1, 1))
         if self.return_names:
             return g, file_name
         return g
 
+
     def __len__(self):
         return len(self.node_names)
 
+
     @staticmethod
     def create_edges(
             xx: List[float], yy: List[float],
             max_degree: int, threshold: float
             ) -> Tuple[List[int], List[int]]:
         """
         Creates edges between nearby nodes.
@@ -135,31 +146,33 @@
             tmp1, tmp2 = tee(tmp)
             dists, idx = list(x[0] for x in tmp1), list(x[1] for x in tmp2)
             source.extend([i for _ in range(len(idx))])
             dest.extend(idx)
             distances.extend(dists)
         return source, dest, distances
 
+
     def initialize_normalizers(self):
         """
         Fits normalizers for later use and also checks they contain transform method.
         """
         if self.normalizers is not None:
             for normalizer in self.normalizers:
                 assert callable(getattr(normalizer, "transform", None)), \
                     'Normalizers provided must have transform method.'
         if self.column_normalize:
-            self.col_sc = fit_column_normalizer(self.node_dir, self.node_names, remove_morph=self.remove_morph, remove_prior=self.remove_prior)
+            self.col_sc = fit_column_normalizer(self.node_dir, self.node_names, remove_morph=self.remove_morph, remove_prior=self.remove_prior, enable_background=self.enable_background)
             assert callable(getattr(self.col_sc, "transform", None)), \
                 'Error loading column normalizer.'
         if self.row_normalize:
             self.row_sc = Normalizer(norm='l1')
             assert callable(getattr(self.row_sc, "transform", None)), \
                 'Error loading row normalizer.'
 
+
     def get_normalizers(self) -> Tuple[Any]:
         """
         Returns a tuple with all the normalizers in the order they are used.
         """
         if self.column_normalize and self.row_normalize and self.normalizers is not None:
             return [self.col_sc, self.row_sc, *self.normalizers]
         if self.column_normalize and self.row_normalize:
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/train_graphs.py` & `tumourkit-0.8.0/tumourkit/classification/train_graphs.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,41 +49,60 @@
         loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         writer: Optional[SummaryWriter] = None,
         epoch: Optional[int] = None,
         log_suffix: Optional[str] = None,
         num_classes: Optional[str] = 2,
+        enable_background: Optional[bool] = False,
         ) -> List[float]:
     """
     Evaluates model in loader.
     Logs to tensorboard with suffix log_suffix.
     Returns the model in evaluation mode.
     """
     model.eval()
     preds, labels, probs = np.array([]).reshape(0, 1), np.array([]).reshape(0, 1), np.array([]).reshape(0, 1 if num_classes == 2 else num_classes)
+    preds_bkgr, labels_bkgr, probs_bkgr = np.array([]).reshape(0, 1), np.array([]).reshape(0, 1), np.array([]).reshape(0, 1)
     for g in loader:
         g = g.to(device)
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
         features = g.ndata['X']
         # Forward
         logits = model(g, features)
+        if enable_background:
+            logits, logits_bkgr = logits
+            pred_bkgr = logits_bkgr.argmax(1).detach().cpu().numpy().reshape(-1, 1)
+            preds_bkgr = np.vstack((preds_bkgr, pred_bkgr))
+            prob_bkgr = F.softmax(logits_bkgr, dim=1).detach().cpu().numpy()[:, 1].reshape(-1, 1)
+            probs_bkgr = np.vstack((probs_bkgr, prob_bkgr))
+            label_bkgr = g.ndata['y_bkgr'].detach().cpu().numpy().reshape(-1, 1)
+            labels_bkgr = np.vstack((labels_bkgr, label_bkgr))
         pred = logits.argmax(1).detach().cpu().numpy().reshape(-1, 1)
         preds = np.vstack((preds, pred))
         if num_classes == 2:
             prob = F.softmax(logits, dim=1).detach().cpu().numpy()[:, 1].reshape(-1, 1)
         else:
             prob = F.softmax(logits, dim=1).detach().cpu().numpy()
         probs = np.vstack((probs, prob))
         label = g.ndata['y'].detach().cpu().numpy().reshape(-1, 1)
         labels = np.vstack((labels, label))
     # Compute metrics on validation
+    if enable_background:
+        acc_bkgr, f1_bkgr, auc_bkgr, perc_err_bkgr, ece_bkgr = metrics_from_predictions(labels_bkgr, preds_bkgr, probs_bkgr, 2)
+        # Tensorboard
+        if writer is not None:
+            writer.add_scalar('Accuracy-bkgr/' + log_suffix, acc_bkgr, epoch)
+            writer.add_scalar('F1-bkgr/' + log_suffix, f1_bkgr, epoch)
+            writer.add_scalar('ROC_AUC-bkgr/' + log_suffix, auc_bkgr, epoch)
+            writer.add_scalar('ECE-bkgr/' + log_suffix, ece_bkgr, epoch)
+            writer.add_scalar('Percentage Error-bkgr/' + log_suffix, perc_err_bkgr, epoch)
     if num_classes == 2:
         acc, f1, auc, perc_err, ece = metrics_from_predictions(labels, preds, probs, 2)
         # Tensorboard
         if writer is not None:
             assert (log_suffix is not None and epoch is not None)
             writer.add_scalar('Accuracy/' + log_suffix, acc, epoch)
             writer.add_scalar('F1/' + log_suffix, f1, epoch)
@@ -106,30 +125,37 @@
         tr_loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         optimizer: Optimizer,
         epoch: int,
         writer: SummaryWriter,
         num_classes: int,
+        enable_background: Optional[bool] = False,
         ) -> None:
     """
     Trains for one iteration, as the name says.
     """
     model.train()
     for step, tr_g in enumerate(tr_loader):
         tr_g = tr_g.to(device)
         # self-loops
         tr_g = dgl.remove_self_loop(tr_g)
         tr_g = dgl.add_self_loop(tr_g)
         # data
         features = tr_g.ndata['X']
         labels = tr_g.ndata['y']
+        if enable_background:
+            labels_bkgr = tr_g.ndata['y_bkgr']
         # Forward
         logits = model(tr_g, features)
+        if enable_background:
+            logits, logits_bkgr = logits
         loss = F.cross_entropy(logits, labels)
+        if enable_background:
+            loss += F.cross_entropy(logits_bkgr, labels_bkgr)
         # Backward
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
         # Compute metrics on training
         preds = logits.argmax(1).detach().cpu().numpy()
         labels = labels.detach().cpu().numpy()
@@ -147,14 +173,26 @@
             train_micro, train_macro, train_weighted, train_ece = metrics_from_predictions(labels, preds, probs, num_classes)
             # Tensorboard
             writer.add_scalar('Accuracy/train', train_micro, step + len(tr_loader) * epoch)
             writer.add_scalar('Macro F1/train', train_macro, step + len(tr_loader) * epoch)
             writer.add_scalar('Weighted F1/train', train_weighted, step + len(tr_loader) * epoch)
             writer.add_scalar('ECE/train', train_ece, step + len(tr_loader) * epoch)
 
+        if enable_background:
+            preds_bkgr = logits_bkgr.argmax(1).detach().cpu().numpy()
+            labels_bkgr = labels_bkgr.detach().cpu().numpy()
+            probs_bkgr = F.softmax(logits_bkgr, dim=1).detach().cpu().numpy()[:, 1]
+            train_acc_bkgr, train_f1_bkgr, train_auc_bkgr, train_perc_err_bkgr, train_ece_bkgr = metrics_from_predictions(labels_bkgr, preds_bkgr, probs_bkgr, 2)
+            # Tensorboard
+            writer.add_scalar('Accuracy-bkgr/train', train_acc_bkgr, step + len(tr_loader) * epoch)
+            writer.add_scalar('F1-bkgr/train', train_f1_bkgr, step + len(tr_loader) * epoch)
+            writer.add_scalar('ROC_AUC-bkgr/train', train_auc_bkgr, step + len(tr_loader) * epoch)
+            writer.add_scalar('ECE-bkgr/train', train_ece_bkgr, step + len(tr_loader) * epoch)
+            writer.add_scalar('Percentage Error-bkgr/train', train_perc_err_bkgr, step + len(tr_loader) * epoch)
+
 
 def train(
         save_dir: str,
         save_weights: bool,
         tr_loader: GraphDataLoader,
         val_loader: GraphDataLoader,
         model: nn.Module,
@@ -162,25 +200,26 @@
         writer: SummaryWriter,
         n_early: int,
         device: Optional[str] = 'cpu',
         check_iters: Optional[int] = -1,
         conf: Optional[Dict[str, Any]] = None,
         normalizers: Optional[Tuple[Normalizer]] = None,
         num_classes: Optional[int] = 2,
+        enable_background: Optional[bool] = False,
         ) -> None:
     """
     Train the model with early stopping on F1 score (weighted) or until 1000 iterations.
     """
     model = model.to(device)
     n_epochs = 1000
     best_val_f1 = 0
     early_stop_rounds = 0
     for epoch in range(n_epochs):
-        train_one_iter(tr_loader, model, device, optimizer, epoch, writer, num_classes)
-        val_metrics = evaluate(val_loader, model, device, writer, epoch, 'validation', num_classes=num_classes)
+        train_one_iter(tr_loader, model, device, optimizer, epoch, writer, num_classes, enable_background=enable_background)
+        val_metrics = evaluate(val_loader, model, device, writer, epoch, 'validation', num_classes=num_classes, enable_background=enable_background)
         if num_classes == 2:
             val_f1, val_acc, val_auc, val_perc_error, val_ece = val_metrics
         else:
             val_micro, val_macro, val_f1, val_ece = val_metrics
         # Save checkpoint
         if save_weights and check_iters != -1 and epoch % check_iters == 0:
             save_model(save_dir, model, conf, normalizers, prefix='last_')
@@ -199,14 +238,15 @@
 def load_dataset(
         train_node_dir: str,
         val_node_dir: str,
         test_node_dir: str,
         bsize: int,
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
+        enable_background: Optional[bool] = False,
         ) -> Tuple[GraphDataLoader, GraphDataLoader, GraphDataLoader]:
     """
     Creates Torch dataloaders for training.
     Folder structure:
     node_dir:
      - train
       - graphs
@@ -219,23 +259,25 @@
      - test
       - graphs
        - file1.nodes.csv
        ...
     """
     train_dataset = GraphDataset(
         node_dir=train_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
-        max_dist=200, max_degree=10, column_normalize=True)
+        max_dist=200, max_degree=10, column_normalize=True, enable_background=enable_background)
     train_dataloader = GraphDataLoader(train_dataset, batch_size=bsize, shuffle=True)
     val_dataset = GraphDataset(
         node_dir=val_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
-        max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers())
+        max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers(),
+        enable_background=enable_background)
     val_dataloader = GraphDataLoader(val_dataset, batch_size=1, shuffle=False)
     test_dataset = GraphDataset(
         node_dir=test_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
-        max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers())
+        max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers(),
+        enable_background=enable_background)
     test_dataloader = GraphDataLoader(test_dataset, batch_size=1, shuffle=False)
     return train_dataloader, val_dataloader, test_dataloader
 
 
 def generate_configurations(max_confs: int, model_name: str) -> List[Dict[str, int]]:
     """
     Generates a grid in the search space with no more than max_confs configurations.
@@ -261,29 +303,29 @@
             conf['NUM_LAYERS'] = num_layers
             conf['DROPOUT'] = dropout
             conf['NORM_TYPE'] = None
             confs.append(conf)
     return confs
 
 
-def load_model(conf: Dict[str, Any], num_classes: int, num_feats: int) -> nn.Module:
+def load_model(conf: Dict[str, Any], num_classes: int, num_feats: int, enable_background: bool) -> nn.Module:
     """
     Available models: GCN, ATT, HATT, SAGE, BOOST
     Configuration space: NUM_LAYERS, DROPOUT, NORM_TYPE
     """
     hidden_feats = 100
     if conf['MODEL_NAME'] == 'GCN':
-        return GCN(num_feats, hidden_feats, num_classes, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+        return GCN(num_feats, hidden_feats, num_classes, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], enable_background)
     if conf['MODEL_NAME'] == 'ATT' or conf['MODEL_NAME'] == 'HATT':
         num_heads = 8
         num_out_heads = 1
         heads = ([num_heads] * conf['NUM_LAYERS']) + [num_out_heads]
         if conf['MODEL_NAME'] == 'ATT':
-            return GAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
-        return HardGAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+            return GAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], enable_background)
+        return HardGAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], enable_background)
     assert False, 'Model not implemented.'
 
 
 def create_results_file(filename: str, num_classes: int) -> None:
     """
     Creates header of .csv result file to append results.
     filename must not contain extension.
@@ -351,24 +393,26 @@
         save_dir: str,
         num_classes: int,
         num_feats: int
         ) -> Tuple[List[float], nn.Module, Dict[str, Any]]:
     # Tensorboard logs
     writer = SummaryWriter(log_dir=os.path.join(log_dir, name_from_conf(conf)))
     # Model
-    model = load_model(conf, num_classes, num_feats)
+    model = load_model(conf, num_classes, num_feats, args.enable_background)
     optimizer = torch.optim.Adam(model.parameters(), lr=0.001)
     # Train
     train(
         save_dir, save_weights, train_dataloader, val_dataloader,
         model, optimizer, writer, args.early_stopping_rounds,
         args.device, args.checkpoint_iters, conf, train_dataloader.dataset.get_normalizers(),
-        num_classes=num_classes
+        num_classes=num_classes, enable_background=args.enable_background
+    )
+    test_metrics = evaluate(
+        test_dataloader, model, args.device, num_classes=num_classes, enable_background=args.enable_background
     )
-    test_metrics = evaluate(test_dataloader, model, args.device, num_classes=num_classes)
     model = model.cpu()
     if num_classes == 2:
         test_f1, test_acc, test_auc, test_perc_err, test_ece = test_metrics
         return test_f1, test_acc, test_auc, test_perc_err, test_ece, model, conf
     else:
         test_micro, test_macro, test_weighted, test_ece = test_metrics
         return test_micro, test_macro, test_weighted, test_ece, model, conf
@@ -401,14 +445,15 @@
     parser.add_argument('--num-workers', type=int, default=1,
                         help='Number of processors to use. Default: 1.')
     parser.add_argument('--checkpoint-iters', type=int, default=-1,
                         help='Number of iterations at which to save model periodically while training. Set to -1 for no checkpointing. Default: -1.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
     parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main_with_args(args: Namespace):
     log_dir = parse_path(args.log_dir)
     create_dir(log_dir)
     save_weights = False
@@ -422,15 +467,16 @@
     # Datasets
     train_dataloader, val_dataloader, test_dataloader = load_dataset(
         train_node_dir=args.train_node_dir,
         val_node_dir=args.validation_node_dir,
         test_node_dir=args.test_node_dir,
         bsize=args.batch_size,
         remove_prior=args.disable_prior,
-        remove_morph=args.disable_morph_feats
+        remove_morph=args.disable_morph_feats,
+        enable_background=args.enable_background,
     )
     # Configurations
     confs = generate_configurations(args.num_confs, args.model_name)
     create_results_file(args.save_file, args.num_classes)
     num_feats = 18 + (1 if args.num_classes == 2 else args.num_classes)
     if args.disable_morph_feats:
         num_feats -= 18
```

### Comparing `tumourkit-0.7.3/tumourkit/classification/train_xgboost.py` & `tumourkit-0.8.0/tumourkit/classification/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/demo/app.py` & `tumourkit-0.8.0/tumourkit/demo/app.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/eval_pipe.py` & `tumourkit-0.8.0/tumourkit/eval_pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 )
         # Add hov probabilities
         newargs = Namespace(
             json_dir=os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
             graph_dir=os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'raw'),
             output_dir=os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'),
             num_classes=args.num_classes,
+            enable_background=args.enable_background,
         )
         join_hovprob_graph_main(newargs, logger)
         for file in os.listdir(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds')):
             df = pd.read_csv(os.path.join(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'), file))
             assert (df['class'].to_numpy() == ((df['prob1'].to_numpy() > 0.5) * 1 + 1)).all(), f"Probs and prediction of Hovernet don't coincide. {file}"
             df.drop('class', axis=1).to_csv(os.path.join(os.path.join(args.root_dir, 'tmp_graphs', 'graphs', 'hovpreds'), file), index=False)
         model_name = 'best_' + args.best_arch + '_' + args.best_num_layers + '_' \
@@ -118,24 +119,26 @@
             output_dir=os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds'),
             weights=os.path.join(args.gnn_dir, 'weights', model_name + '.pth'),
             conf=os.path.join(args.gnn_dir, 'confs', model_name + '.json'),
             normalizers=os.path.join(args.gnn_dir, 'normalizers', model_name + '.pkl'),
             num_classes=args.num_classes,
             disable_prior=args.disable_prior,
             disable_morph_feats=args.disable_morph,
+            enable_background=args.enable_background,
         )
         infer_gnn(newargs)
     # Postproc to obtain centroids
     if check_void(os.path.join(args.root_dir, 'tmp_graphs', 'centroids')):
         logger.info('Parsing gnn output.')
         logger.info('   Converting .nodes.csv to .centroids.csv.')
         newargs = Namespace(
             graph_dir=os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds'),
             centroids_dir=os.path.join(args.root_dir, 'tmp_graphs', 'centroids'),
             num_classes=args.num_classes,
+            enable_background=args.enable_background,
         )
         graph2centroids_main(newargs)
 
     logger.info('Creating folders.')
     os.makedirs(os.path.join(args.save_dir, 'conf-matrices', 'gnn_individual'), exist_ok=True)
     os.makedirs(os.path.join(args.save_dir, 'conf-matrices', 'hov_individual'), exist_ok=True)
     for split in ['train', 'validation', 'test']:
@@ -211,24 +214,24 @@
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
             pred_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
             save_name=os.path.join(args.save_dir, split, 'hov'),
             debug_path=os.path.join(args.save_dir, 'conf-matrices', 'hov_individual', 'debug_hov') if args.debug else None,
-            num_classes=args.num_classes
+            num_classes=args.num_classes,
         )
         eval_segment(newargs, logger)
         compute_ece(args, split, is_hov=True)
         if args.debug:
             shutil.move(
                 os.path.join(args.save_dir, 'conf-matrices', 'hov_individual', 'debug_hov_global.csv'),
                 os.path.join(args.save_dir, 'conf-matrices', 'debug_hov_global_' + split + '.csv'))
     # Evaluate graph output same as hov output
-    logger.info('Starting evaluation of Hovernet output.')
+    logger.info('Starting evaluation of GNN output.')
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split (with background)')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
             pred_path=os.path.join(args.root_dir, 'tmp_graphs', 'centroids'),
             save_name=os.path.join(args.save_dir, split, 'gnn'),
@@ -241,15 +244,14 @@
                 os.path.join(args.save_dir, 'conf-matrices', 'gnn_individual', 'debug_gnn_global.csv'),
                 os.path.join(args.save_dir, 'conf-matrices', 'debug_gnn_global_' + split + '.csv'))
     for split in ['train', 'validation', 'test']:
         os.makedirs(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds_gt', split), exist_ok=True)
         for file in get_names(os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'), '.nodes.csv'):
             df_gt = pd.read_csv(os.path.join(args.root_dir, 'data', split, 'graphs', 'preds', file + '.nodes.csv'))
             df = pd.read_csv(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds', file + '.nodes.csv'))
-            # import pdb;pdb.set_trace()
             df = df[df.id.isin(df_gt.id)]
             df = df.set_index(df.id)
             df_gt = df_gt.set_index(df_gt.id)
             df['class'] = df_gt['class']
             assert not df['class'].isna().any()
             df.to_csv(os.path.join(args.root_dir, 'tmp_graphs', 'gnn_preds_gt', split, file + '.nodes.csv'), index=False)
         compute_ece(args, split, is_hov=False)
@@ -266,14 +268,15 @@
     parser.add_argument('--best-dropout', type=str, help='Optimal dropout rate when training GNNs')
     parser.add_argument('--best-norm-type', type=str, help='Optimal type of normalization layers when training GNNs')
     parser.add_argument('--best-arch', type=str, help='Best architecture (convolutional, attention, ...) when training GNNs', choices=['GCN', 'ATT'])
     parser.add_argument('--debug', action='store_true', help='Whether to save confusion matrices.')
     parser.add_argument('--gnn-dir', type=str, help='Path where the gnn is saved, otherwise the default in root-dir will be used. It must have three folder inside: confs, weights and normalizers.')
     parser.add_argument('--disable-prior', action='store_true', help='Whether to disable the use of Hovernet probabilities.')
     parser.add_argument('--disable-morph', action='store_true', help='Whether to disable the use of morphological properties.')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.7.3/tumourkit/infer_pipe.py` & `tumourkit-0.8.0/tumourkit/infer_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         output_dir=os.path.join(args.output_dir, 'gnn_preds'),
         weights=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
         conf=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'confs', model_name + '.json'),
         normalizers=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'normalizers', model_name + '.pkl'),
         num_classes=args.num_classes,
         disable_prior=False,
         disable_morph_feats=False,
+        enable_background=args.enable_background,
     )
     infer_gnn(newargs)
     return
 
 
 def run_postgraphs(args: Namespace, logger: Logger) -> None:
     """
@@ -179,14 +180,15 @@
     """
     logger.info('Parsing gnn output.')
     logger.info('   Converting .nodes.csv to .centroids.csv.')
     newargs = Namespace(
         graph_dir=os.path.join(args.output_dir, 'gnn_preds'),
         centroids_dir=os.path.join(args.output_dir, 'centroids'),
         num_classes=args.num_classes,
+        enable_background=args.enable_background,
     )
     graph2centroids_main(newargs)
     logger.info('   Converting .centroids.csv and .GT_cells.png to .class.csv.')
     newargs = Namespace(
         centroids_dir=os.path.join(args.output_dir, 'centroids'),
         png_dir=os.path.join(args.output_dir, 'png_hov'),
         csv_dir=os.path.join(args.output_dir, 'csv_gnn'),
@@ -211,14 +213,15 @@
     parser.add_argument('--gpu', type=str, default='0')
     parser.add_argument('--num-workers', type=int, default=0)
     parser.add_argument('--best-num-layers', type=str, help='Optimal number of layers when training GNNs.')
     parser.add_argument('--best-dropout', type=str, help='Optimal dropout rate when training GNNs')
     parser.add_argument('--best-norm-type', type=str, help='Optimal type of normalization layers when training GNNs')
     parser.add_argument('--best-arch', type=str, help='Best architecture (convolutional, attention, ...) when training GNNs', required=True, choices=['GCN', 'ATT', 'HATT', 'SAGE', 'BOOST'])
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
     create_dir(args.output_dir)
```

### Comparing `tumourkit-0.7.3/tumourkit/make_dirs.py` & `tumourkit-0.8.0/tumourkit/make_dirs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/draw_cells.py` & `tumourkit-0.8.0/tumourkit/postprocessing/draw_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/draw_graph.py` & `tumourkit-0.8.0/tumourkit/postprocessing/draw_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.8.0/tumourkit/postprocessing/join_graph_gt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.8.0/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,59 +68,79 @@
             if num_classes == 2:
                 centroids_.append((inst_centroid[1], inst_centroid[0], inst_prob1))
             else:
                 centroids_.append((inst_centroid[1], inst_centroid[0], *inst_probs))
     return centroids_
 
 
-def add_probability(graph: pd.DataFrame, hov_json: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> pd.DataFrame:
+def add_probability(
+        graph: pd.DataFrame,
+        hov_json: Dict[str, Any],
+        logger: Optional[Logger] = None,
+        num_classes: Optional[int] = 2,
+        enable_background: Optional[bool] = False,
+        ) -> pd.DataFrame:
     """
     Adds probability information from the Hovernet JSON nuclei dictionary to the graph DataFrame.
 
     This function extracts the type probabilities from the Hovernet JSON nuclei dictionary (`hov_json`) and adds them as columns to the `graph` DataFrame.
     The join between the `graph` DataFrame and the `hov_json` dictionary is based on the 'id' field.
 
     :param graph: The graph DataFrame containing the nodes.
     :type graph: pd.DataFrame
     :param hov_json: The Hovernet JSON nuclei dictionary.
     :type hov_json: Dict[str, Any]
     :param logger: Optional logger object to log warnings.
     :type logger: Optional[Logger]
     :param num_classes: Optional number of classes. Defaults to 2 for binary classification.
     :type num_classes: Optional[int]
+    :param enable_background: If True, extra cells are included. They are represented with a value of 1 in the column background.
+    :type enable_background: Optional[bool]
     :return: The updated graph DataFrame with probability information.
     :rtype: pd.DataFrame
     """
-    centroids = parse_centroids_probs(hov_json, logger, num_classes)
-    centroids = np.array(centroids)
-    assert len(centroids) > 0, 'Hov json must contain at least one cell.'
     graph = graph.copy()
     if 'prob1' not in graph.columns:
         n_cols = len(graph.columns)
         graph.insert(n_cols, 'prob1', [-1] * len(graph))
     else:
         graph['prob1'] = -1
+    if enable_background:
+        if 'background' not in graph.columns:
+            n_cols = len(graph.columns)
+            graph.insert(n_cols, 'background', [0] * len(graph))
+        else:
+            graph['background'] = 0
     if num_classes > 2:
         for k in range(2, num_classes + 1):
             if not 'prob' + str(k) in graph.columns:
                 n_cols = len(graph.columns)
                 graph.insert(n_cols, 'prob' + str(k), [-1] * len(graph))
             else:
                 graph['prob' + str(k)] = -1
-    gt_tree = generate_tree(centroids[:, :2])
-    pred_centroids = graph[['X', 'Y']].to_numpy(dtype=int)
-    pred_tree = generate_tree(pred_centroids)
-    for point_id, point in enumerate(centroids):
-        closest_id = find_nearest(point[:2], pred_tree)
+    pred_centroids = parse_centroids_probs(hov_json, logger, num_classes)
+    pred_centroids = np.array(pred_centroids)
+    assert len(pred_centroids) > 0, 'Hov json must contain at least one cell.'
+    pred_tree = generate_tree(pred_centroids[:, :2])
+    gt_centroids = graph[['X', 'Y']].to_numpy(dtype=int)
+    gt_tree = generate_tree(gt_centroids)
+    for point_id, point in enumerate(pred_centroids):
+        closest_id = find_nearest(point[:2], gt_tree)
         closest = graph.loc[closest_id, ['X', 'Y', 'prob1']]
-        if point_id == find_nearest(closest[:2], gt_tree):
+        if point_id == find_nearest(closest[:2], pred_tree):
             graph.loc[closest_id, 'prob1'] = point[2]  # 1-1 matchings
             if num_classes > 2:
                 for k in range(2, num_classes + 1):
                     graph.loc[closest_id, 'prob' + str(k)] = point[k + 1]  # 1-1 matchings
+        elif enable_background:
+            graph.loc[closest_id, 'background'] = 1  # Pred not in GT
+            graph.loc[closest_id, 'prob1'] = point[2]  # closest matching
+            if num_classes > 2:
+                for k in range(2, num_classes + 1):
+                    graph.loc[closest_id, 'prob' + str(k)] = point[k + 1]  # closest matching
     graph.drop(graph[graph['prob1'] == -1].index, inplace=True)
     return graph
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -132,28 +152,29 @@
         help='Path to directory to .nodes.csv containing graph information.'
     )
     parser.add_argument(
         '--output-dir', type=str, required=True,
         help='Path where to save new .nodes.csv. If same as --graph-dir, overwrites its content.'
     )
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main_with_args(args: Namespace, logger: Optional[Logger] = None) -> None:
     json_dir = parse_path(args.json_dir)
     graph_dir = parse_path(args.graph_dir)
     output_dir = parse_path(args.output_dir)
     create_dir(output_dir)
     names = get_names(graph_dir, '.nodes.csv')
     for name in tqdm(names):
         try:
             graph = pd.read_csv(os.path.join(graph_dir, name + '.nodes.csv'))
             hov_json = read_json(os.path.join(json_dir, name + '.json'))
-            graph = add_probability(graph, hov_json, logger, args.num_classes)
+            graph = add_probability(graph, hov_json, logger, args.num_classes, args.enable_background)
             save_graph(graph, os.path.join(output_dir, name + '.nodes.csv'))
         except FileNotFoundError:
             continue
     return
 
 
 def main():
```

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.8.0/tumourkit/postprocessing/merge_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.8.0/tumourkit/postprocessing/rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/__init__.py` & `tumourkit-0.8.0/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.8.0/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.8.0/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.8.0/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.8.0/tumourkit/preprocessing/graph2centroids.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import argparse
 from argparse import Namespace
+from typing import Optional
 from ..utils.preprocessing import get_names, create_dir, parse_path, save_centroids, read_graph
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 
 
-def graph2centroids(graph_file: pd.DataFrame, num_classes: int) -> np.ndarray:
+def graph2centroids(
+        graph_file: pd.DataFrame,
+        num_classes: int,
+        enable_background: Optional[bool] = False) -> np.ndarray:
     """
     Extracts X, Y and class attributes from graphs nodes.
 
     :param graph_file: The Pandas DataFrame containing the graph nodes.
     :type graph_file: pd.DataFrame
+    :param enable_background: Enable when model has extra head to correct extra cells.
+    :type enable_background: Optional[bool]
     :return: A NumPy array containing the X, Y and class attributes from the graph nodes.
     :rtype: np.ndarray
 
     If the graph file has a 'class' column, the function returns the 'X', 'Y' and 'class' columns as a NumPy array with integer data type.
     Otherwise, the function assumes that the graph file has a 'prob1' column, which contains the probability of a node belonging to a particular class.
     In this case, the function sets the class attribute to 1 if the probability is greater than 0.5, and to 2 otherwise.
     """
     if 'class' in graph_file.columns:
         return graph_file[['X', 'Y', 'class']].to_numpy(dtype=int)
+    if enable_background:
+        graph_file = graph_file[graph_file.prob0 < 0.5]
     if num_classes == 2:
         res = graph_file[['X', 'Y', 'prob1']].to_numpy()
         res[:, 2] = (res[:, 2] > 0.5) * 1 + 1
     else:
         res = graph_file[['X', 'Y', 'prob1']].to_numpy()
         prob_cols = graph_file[['prob' + str(k) for k in range(1, num_classes + 1)]].to_numpy()
         class_col = np.argmax(prob_cols, axis=1) + 1
@@ -53,25 +61,26 @@
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--graph-dir', type=str, required=True, help='Path to folder containing .nodes.csv.')
     parser.add_argument('--centroids-dir', type=str, required=True, help='Path to folder where to save .centroids.csv.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main_with_args(args: Namespace) -> None:
     graph_dir = parse_path(args.graph_dir)
     centroids_dir = parse_path(args.centroids_dir)
     create_dir(centroids_dir)
     names = get_names(graph_dir, '.nodes.csv')
     for name in tqdm(names):
         graph_file = read_graph(name, graph_dir)
-        centroids_file = graph2centroids(graph_file, args.num_classes)
+        centroids_file = graph2centroids(graph_file, args.num_classes, args.enable_background)
         save_centroids(centroids_file, centroids_dir, name)
     return
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.8.0/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.8.0/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.8.0/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.8.0/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/preprocessing/remove_uncertain.py` & `tumourkit-0.8.0/tumourkit/preprocessing/remove_uncertain.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.8.0/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.8.0/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/research_pipe.py` & `tumourkit-0.8.0/tumourkit/research_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/evaluate.py` & `tumourkit-0.8.0/tumourkit/segmentation/evaluate.py`

 * *Files 11% similar despite different names*

```diff
@@ -216,14 +216,35 @@
     else:
         res = np.zeros((n, n))
         res[:m, :m] += B
         res += A
     return res
 
 
+def compute_perc_error_bkgr(
+        gt_centroids: List[Tuple[int, int, int]],
+        pred_centroids: List[Tuple[int, int, int]]
+        ) -> float:
+    """
+    Computes absolute difference in percentages of the classes.
+
+    :param gt_centroids: Ground truth.
+    :type gt_centroids: List[Tuple[int, int, int]]
+    :param pred_centroids: Predictions.
+    :type pred_centroids: List[Tuple[int, int, int]]
+    :return: The percentage error.
+    :rtype: float
+    """
+    gt_cls = gt_centroids[:, 2]
+    pred_cls = pred_centroids[:, 2]
+    gt_perc = (gt_cls == 2).sum() / len(gt_cls)
+    pred_perc = (pred_cls == 2).sum() / len(pred_cls)
+    return abs(gt_perc - pred_perc)
+
+
 def save_csv(
         metrics: Dict[str, List[float]],
         save_path: str
         ) -> None:
     """
     Saves metrics in CSV format for later use.
 
@@ -269,29 +290,32 @@
 
 
 def main_with_args(args: Namespace, logger: Logger):
     names = read_names(args.names)
     if args.num_classes == 2:
         metrics = {
             'Name': [], 'F1': [], 'Accuracy': [], 'ROC_AUC': [], 'Perc_err': [], 'ECE': [],
-            'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': []
+            'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': [], 'Perc_err (bkgr)': []
         }
     else:
         metrics = {
             'Name': [], 'Macro F1': [], 'Weighted F1': [], 'Micro F1': [], 'ECE': [],
             'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': []
         }
     global_conf_mat = None
     global_pred, global_true = [], []
+    global_gt_centroids, global_pred_centroids = np.array([]).reshape(0,3), np.array([]).reshape(0,3)
     for k, name in enumerate(names):
         logger.info('Progress: {:2d}/{}'.format(k + 1, len(names)))
         metrics['Name'].append(name)
         # Read
         gt_centroids = read_centroids(name, args.gt_path)
         pred_centroids = read_centroids(name, args.pred_path)
+        global_gt_centroids = np.vstack((global_gt_centroids, gt_centroids))
+        global_pred_centroids = np.vstack((global_pred_centroids, pred_centroids))
         # Compute pairs and confusion matrix
         conf_mat = get_confusion_matrix(gt_centroids, pred_centroids)
         if args.debug_path is not None:
             save_debug_matrix(conf_mat, args.debug_path + '_' + name)
         try:
             true_labels, pred_labels = get_pairs(gt_centroids, pred_centroids)
         except Exception as e:
@@ -308,14 +332,16 @@
             global_conf_mat = conf_mat
         else:
             global_conf_mat = add_matrices(global_conf_mat, conf_mat)
         # Compute per image scores and percentages
         try:
             _metrics = metrics_from_predictions(true_labels, pred_labels, None, args.num_classes)
             macro_bkgr, weighted_bkgr, micro_bkgr = compute_metrics_from_matrix(conf_mat)
+            if args.num_classes == 2:
+                perc_error_bkgr = compute_perc_error_bkgr(gt_centroids, pred_centroids)
         except Exception as e:
             logger.error(e)
             logger.error(name)
             _metrics = [-1] * 5 if args.num_classes == 2 else [-1] * 4
             macro_bkgr, weighted_bkgr, micro_bkgr = -1, -1, -1
         if args.num_classes == 2:
             acc, f1, auc, perc_error, ece = _metrics
@@ -323,14 +349,15 @@
             metrics['Accuracy'].append(acc)
             metrics['ROC_AUC'].append(auc)
             metrics['Perc_err'].append(perc_error)
             metrics['ECE'].append(ece)
             metrics['Macro F1 (bkgr)'].append(macro_bkgr)
             metrics['Weighted F1 (bkgr)'].append(weighted_bkgr)
             metrics['Micro F1 (bkgr)'].append(micro_bkgr)
+            metrics['Perc_err (bkgr)'].append(perc_error_bkgr)
         else:
             micro, macro, weighted, ece = _metrics
             metrics['Macro F1'].append(macro)
             metrics['Weighted F1'].append(weighted)
             metrics['Micro F1'].append(micro)
             metrics['ECE'].append(ece)
             metrics['Macro F1 (bkgr)'].append(macro_bkgr)
@@ -340,17 +367,19 @@
         save_debug_matrix(global_conf_mat, args.debug_path + '_global')
     save_csv(metrics, args.save_name)
     # Global scores and percentages
     _global_metrics = metrics_from_predictions(np.array(global_true), np.array(global_pred), None, args.num_classes)
     macro_bkgr, weighted_bkgr, micro_bkgr = compute_metrics_from_matrix(global_conf_mat)
     if args.num_classes == 2:
         acc, f1, auc, perc_error, ece = _global_metrics
+        perc_error_bkgr = compute_perc_error_bkgr(global_gt_centroids, global_pred_centroids)
         global_metrics = {
             'Name': ['All'], 'F1': [f1], 'Accuracy': [acc], 'ROC_AUC': [auc], 'Perc_err': [perc_error], 'ECE': [ece],
-            'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr]
+            'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr],
+            'Perc_err (bkgr)': [perc_error_bkgr]
         }
     else:
         micro, macro, weighted, ece = _global_metrics
         global_metrics = {
             'Name': ['All'], 'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro], 'ECE': [ece],
             'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr]
         }
```

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.8.0/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/train_pipe.py` & `tumourkit-0.8.0/tumourkit/train_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         join_graph_gt_main(newargs)
         logger.info('   Adding hovernet predictions to .nodes.csv.')
         newargs = Namespace(
             json_dir=os.path.join(args.root_dir, 'data', split, 'json'),
             graph_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'GT'),
             output_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'),
             num_classes=args.num_classes,
+            enable_background=args.enable_background,
         )
         join_hovprob_graph_main(newargs, logger)
     return
 
 
 def run_graph_pipe(args: Namespace, logger: Logger) -> None:
     """
@@ -226,14 +227,15 @@
         save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
         device='cpu' if args.gpu == '' else 'cuda',
         num_workers=args.num_workers,
         checkpoint_iters=-1,
         num_classes=args.num_classes,
         disable_prior=False,
         disable_morph_feats=False,
+        enable_background=args.enable_background,
     )
     train_gnn(newargs)
     newargs = Namespace(
         train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
         validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
         test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
         log_dir=os.path.join(args.root_dir, 'gnn_logs'),
@@ -245,26 +247,28 @@
         save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
         device='cpu' if args.gpu == '' else 'cuda',
         num_workers=args.num_workers,
         checkpoint_iters=-1,
         num_classes=args.num_classes,
         disable_prior=False,
         disable_morph_feats=False,
+        enable_background=args.enable_background,
     )
     train_gnn(newargs)
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--root-dir', type=str, default='./.internals/', help='Root folder to save data and models.')
     parser.add_argument('--pretrained-path', type=str, help='Path to initial Hovernet weights.')
     parser.add_argument('--gpu', type=str, default='0')
     parser.add_argument('--num-workers', type=int, default=0)
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--enable-background', action='store_true', help='If enabled, GNNs are allowed to predict the class 0 (background) and correct extra cells.')
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.7.3/tumourkit/utils/calibration_error.py` & `tumourkit-0.8.0/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/classification.py` & `tumourkit-0.8.0/tumourkit/utils/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 
 def fit_column_normalizer(
         node_dir: str,
         names: List[str],
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
+        enable_background: Optional[bool] = False,
         ) -> StandardScaler:
     """
     Fits a StandardScaler object to the input data and returns it.
 
     :param node_dir: The directory containing node data files.
     :type node_dir: str
     :param names: A list of node names to read from the node directory.
@@ -63,15 +64,15 @@
     :param remove_prior: If True, hovernet probabilites are ignored.
     :type remove_prior: Optional[bool]
     :param remove_morph: If True, morphological features are removed.
     :type remove_morph: Optional[bool]
     :return: A StandardScaler object fitted to the input data.
     :rtype: StandardScaler
     """
-    X, y = _read_all_nodes(node_dir, [x + '.nodes.csv' for x in names], remove_morph=remove_morph, remove_prior=remove_prior)
+    X, y = _read_all_nodes(node_dir, [x + '.nodes.csv' for x in names], remove_morph=remove_morph, remove_prior=remove_prior, enable_background=enable_background)
     sc = StandardScaler()
     sc.fit(X)
     return sc
 
 
 def check_imbalance(y_true: np.ndarray) -> bool:
     """
```

### Comparing `tumourkit-0.7.3/tumourkit/utils/folder2txt.py` & `tumourkit-0.8.0/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/nearest.py` & `tumourkit-0.8.0/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/pipes.py` & `tumourkit-0.8.0/tumourkit/utils/pipes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/postprocessing.py` & `tumourkit-0.8.0/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/preprocessing.py` & `tumourkit-0.8.0/tumourkit/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.3/tumourkit/utils/read_nodes.py` & `tumourkit-0.8.0/tumourkit/utils/read_nodes.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 def read_node_matrix(
         file: str,
         return_coordinates: Optional[bool] = False,
         return_class: Optional[bool] = True,
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
-        ) -> Tuple[np.ndarray, np.ndarray]:
+        enable_background: Optional[bool] = False,
+        ) -> List[np.ndarray]:
     """
     Read csv and creates X and y matrices.
     Centroids coordinates are removed.
     Labels are subtracted 1 to be in 0-1 range.
     """
     df = pd.read_csv(file)
     remove_vars = ['id', 'class', 'X', 'Y']
@@ -47,55 +48,72 @@
             'area', 'perimeter', 'std',
             'red0', 'red1', 'red2', 'red3', 'red4',
             'green0', 'green1', 'green2', 'green3', 'green4',
             'blue0', 'blue1', 'blue2', 'blue3', 'blue4'
         ])
     if remove_prior:
         remove_vars.extend(list(filter(lambda x: 'prob' in x, df.columns)))
+    if enable_background:
+        y_bkgr = df['background'].to_numpy()
+    if 'background' in df.columns:
+        df = df.drop(['background'], axis=1)
     if return_class:
         y = df['class'].to_numpy() - 1
         X = df.drop(remove_vars, axis=1).to_numpy()
         if remove_morph and remove_prior:
             X = np.zeros((len(y), 1))
         if not return_coordinates:
+            if enable_background:
+                return X, y, y_bkgr
             return X, y
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
+            if enable_background:
+                return X, y, xx, yy, y_bkgr
             return X, y, xx, yy
     else:
         remove_vars.remove('class')
         X = df.drop(remove_vars, axis=1).to_numpy()
         if remove_morph and remove_prior:
             X = np.zeros((len(X), 1))
         if not return_coordinates:
+            if enable_background:
+                return X, None, None
             return X, None
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
+            if enable_background:
+                return X, None, xx, yy, None
             return X, None, xx, yy
 
 
 def _read_all_nodes(
         node_dir: str,
         names: List[str],
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
+        enable_background: Optional[bool] = False,
         ) -> List[np.ndarray]:
     """
     Input
       node_dir: Path to folder with csv files containing node features.
       names: List of files to read. Must have file extension.
     Output
       X: Input data in array format.
       y: Labels in array format.
     """
     X, y = None, None
     for name in names:
-        X_, y_ = read_node_matrix(os.path.join(node_dir, name), remove_morph=remove_morph, remove_prior=remove_prior)
+        tmp = read_node_matrix(os.path.join(node_dir, name), remove_morph=remove_morph, remove_prior=remove_prior, enable_background=enable_background)
+        if enable_background:
+            X_, y_, y_bkgr = tmp
+        else:
+            X_, y_ = tmp
         if X is None:
             X = X_  # Shape (n_samples, n_features)
             y = y_  # Shape (n_samples,)
         else:
             X = np.vstack([X, X_])
             y = np.hstack([y, y_])
     return X, y
```

### Comparing `tumourkit-0.7.3/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.8.0/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.3
+Version: 0.8.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.3/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.8.0/tumourkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 docs/buildenv/bin/rst2odt_prepstyles.py
 docs/buildenv/bin/rst2pseudoxml.py
 docs/buildenv/bin/rst2s5.py
 docs/buildenv/bin/rst2xetex.py
 docs/buildenv/bin/rst2xml.py
 docs/buildenv/bin/rstpep2html.py
 docs/source/conf.py
+results/comp_perc.py
 tests/centroidspng2csv_test.py
 tests/conf_matrix_sum_test.py
 tests/cpairs_test.py
 tests/example_test.py
 tests/generate_centroids.py
 tests/generate_rswoosh.py
 tests/get_conn_comp_test.py
@@ -59,17 +60,19 @@
 tumourkit/classification/models/gcn.py
 tumourkit/classification/models/hgao.py
 tumourkit/classification/models/norm.py
 tumourkit/demo/app.py
 tumourkit/postprocessing/__init__.py
 tumourkit/postprocessing/draw_cells.py
 tumourkit/postprocessing/draw_graph.py
+tumourkit/postprocessing/extract_tensorboard.py
 tumourkit/postprocessing/join_graph_gt.py
 tumourkit/postprocessing/join_hovprob_graph.py
 tumourkit/postprocessing/merge_cells.py
+tumourkit/postprocessing/plot_logs.py
 tumourkit/postprocessing/rswoosh.py
 tumourkit/preprocessing/__init__.py
 tumourkit/preprocessing/centroids2png.py
 tumourkit/preprocessing/centroidspng2csv.py
 tumourkit/preprocessing/geojson2pngcsv.py
 tumourkit/preprocessing/graph2centroids.py
 tumourkit/preprocessing/hovernet2centroids.py
```

### Comparing `tumourkit-0.7.3/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.8.0/tumourkit.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [console_scripts]
 centroids2png = tumourkit.preprocessing.centroids2png:main
 centroidspng2csv = tumourkit.preprocessing.centroidspng2csv:main
 draw_cells = tumourkit.postprocessing.draw_cells:main
 draw_graph = tumourkit.postprocessing.draw_graph:main
+extract_tensorboard = tumourkit.postprocessing.extract_tensorboard:main
 geojson2pngcsv = tumourkit.preprocessing.geojson2pngcsv:main
 graph2centroids = tumourkit.preprocessing.graph2centroids:main
 hovernet2centroids = tumourkit.preprocessing.hovernet2centroids:main
 hovernet2geojson = tumourkit.preprocessing.hovernet2geojson:main
 make_dirs = tumourkit.make_dirs:main
 merge_cells = tumourkit.postprocessing.merge_cells:main
+plot_logs = tumourkit.postprocessing.plot_logs:main
 pngcsv2centroids = tumourkit.preprocessing.pngcsv2centroids:main
 pngcsv2geojson = tumourkit.preprocessing.pngcsv2geojson:main
 pngcsv2graph = tumourkit.preprocessing.pngcsv2graph:main
 remove_uncertain = tumourkit.preprocessing.remove_uncertain:main
 run_evaluation = tumourkit.eval_pipe:main
 run_inference = tumourkit.infer_pipe:main
 run_research = tumourkit.research_pipe:main
```

### Comparing `tumourkit-0.7.3/tumourkit.egg-info/requires.txt` & `tumourkit-0.8.0/tumourkit.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 attrs==22.2.0
+altair==5.0.1
+vl-convert-python
 beautifulsoup4==4.12.2
 certifi==2022.12.7
 charset-normalizer==3.0.1
 contourpy==1.0.7
 cycler==0.11.0
 docopt==0.6.2
 exceptiongroup==1.1.0
```

