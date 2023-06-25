# Comparing `tmp/LibRecommender-1.2.0.tar.gz` & `tmp/LibRecommender-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibRecommender-1.2.0.tar", last modified: Tue Jun  6 16:26:24 2023, max compression
+gzip compressed data, was "LibRecommender-1.2.1.tar", last modified: Sun Jun 25 08:46:35 2023, max compression
```

## Comparing `LibRecommender-1.2.0.tar` & `LibRecommender-1.2.1.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.690417 LibRecommender-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.622418 LibRecommender-1.2.0/LibRecommender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28977 2023-06-06 16:26:24.000000 LibRecommender-1.2.0/LibRecommender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-06-06 16:26:24.000000 LibRecommender-1.2.0/LibRecommender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 16:26:24.000000 LibRecommender-1.2.0/LibRecommender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-06 16:26:24.000000 LibRecommender-1.2.0/LibRecommender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-06 16:26:24.000000 LibRecommender-1.2.0/LibRecommender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    28977 2023-06-06 16:26:24.690417 LibRecommender-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    27809 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.622418 LibRecommender-1.2.0/libreco/
--rwxr-xr-x   0 runner    (1001) docker     (122)       22 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.638418 LibRecommender-1.2.0/libreco/algorithms/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1156 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   949314 2023-06-06 16:26:21.000000 LibRecommender-1.2.0/libreco/algorithms/_als.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)     9206 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/_als.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   909347 2023-06-06 16:26:22.000000 LibRecommender-1.2.0/libreco/algorithms/_bpr.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    13747 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/_bpr.pyx
--rwxr-xr-x   0 runner    (1001) docker     (122)    11407 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/als.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11454 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/autoint.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14587 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/bpr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8628 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/caser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12216 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/deepfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/deepwalk.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16665 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/din.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11547 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/fm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/graphsage.py
--rw-r--r--   0 runner    (1001) docker     (122)     7535 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/graphsage_dgl.py
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/item2vec.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6082 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/item_cf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/lightgcn.py
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/ncf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/ngcf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6749 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/pinsage.py
--rw-r--r--   0 runner    (1001) docker     (122)     7210 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/pinsage_dgl.py
--rw-r--r--   0 runner    (1001) docker     (122)     9299 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/rnn4rec.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5877 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/svd.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7629 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/svdpp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.642418 LibRecommender-1.2.0/libreco/algorithms/torch_modules/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/torch_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6726 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/torch_modules/graphsage_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/torch_modules/lightgcn_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/torch_modules/ngcf_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/torch_modules/pinsage_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    19898 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/two_tower.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6799 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/user_cf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8341 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/wave_net.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12002 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/wide_deep.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10863 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/youtube_ranking.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13542 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/algorithms/youtube_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.646418 LibRecommender-1.2.0/libreco/bases/
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4267 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    13085 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/cf_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    12160 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/dyn_embed_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    19199 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/embed_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/gensim_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/sage_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    14925 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/bases/tf_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.650418 LibRecommender-1.2.0/libreco/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/batch_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5495 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/batch_unit.py
--rw-r--r--   0 runner    (1001) docker     (122)    18061 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/collators.py
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3616 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/sequence.py
--rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/batch/tf_feed_dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.654418 LibRecommender-1.2.0/libreco/data/
--rwxr-xr-x   0 runner    (1001) docker     (122)      599 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/consumed.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    20843 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/data_info.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    26422 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5947 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/processing.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13860 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/split.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4785 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/data/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.654418 LibRecommender-1.2.0/libreco/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/embedding/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.658418 LibRecommender-1.2.0/libreco/evaluation/
--rwxr-xr-x   0 runner    (1001) docker     (122)       87 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/evaluation/computation.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6426 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/evaluation/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3394 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.658418 LibRecommender-1.2.0/libreco/feature/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1979 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5187 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/multi_sparse.py
--rw-r--r--   0 runner    (1001) docker     (122)     7384 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/sparse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/ssl.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2167 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/unique.py
--rw-r--r--   0 runner    (1001) docker     (122)     8111 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/feature/update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.662418 LibRecommender-1.2.0/libreco/graph/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/graph/from_dgl.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/graph/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/graph/neighbor_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.662418 LibRecommender-1.2.0/libreco/prediction/
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4012 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/prediction/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/prediction/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.666418 LibRecommender-1.2.0/libreco/recommendation/
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/recommendation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/recommendation/cold_start.py
--rw-r--r--   0 runner    (1001) docker     (122)     8064 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/recommendation/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/recommendation/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)     3026 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/recommendation/recommend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.666418 LibRecommender-1.2.0/libreco/sampling/
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/sampling/negatives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5773 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/sampling/random_walks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.670418 LibRecommender-1.2.0/libreco/tfops/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/configs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/features.py
--rw-r--r--   0 runner    (1001) docker     (122)     5757 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     5110 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/tfops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.674418 LibRecommender-1.2.0/libreco/torchops/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/torchops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/torchops/configs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/torchops/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/torchops/rebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.674418 LibRecommender-1.2.0/libreco/training/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/training/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10497 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/training/tf_trainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9466 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/training/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1334 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/training/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.682417 LibRecommender-1.2.0/libreco/utils/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)  1114135 2023-06-06 16:26:23.000000 LibRecommender-1.2.0/libreco/utils/_similarities.cpp
--rwxr-xr-x   0 runner    (1001) docker     (122)    16758 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/_similarities.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1634 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/initializers.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2588 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14284 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/save_load.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7383 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/similarities.py
--rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libreco/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.682417 LibRecommender-1.2.0/libserving/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.686417 LibRecommender-1.2.0/libserving/sanic_serving/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/embed_deploy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/knn_deploy.py
--rw-r--r--   0 runner    (1001) docker     (122)    15205 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/online_deploy.py
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/sanic_serving/tf_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 16:26:24.690417 LibRecommender-1.2.0/libserving/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/knn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5954 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/online.py
--rw-r--r--   0 runner    (1001) docker     (122)     7042 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/redis.py
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/libserving/serialization/tfmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2949 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/requirements-serving.txt
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-06 16:26:24.690417 LibRecommender-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-06-06 16:25:08.000000 LibRecommender-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.810808 LibRecommender-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.790807 LibRecommender-1.2.1/LibRecommender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28977 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/LibRecommender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/LibRecommender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/LibRecommender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/LibRecommender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/LibRecommender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    28977 2023-06-25 08:46:35.810808 LibRecommender-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    27809 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.790807 LibRecommender-1.2.1/libreco/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       22 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.794808 LibRecommender-1.2.1/libreco/algorithms/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1156 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   949314 2023-06-25 08:46:32.000000 LibRecommender-1.2.1/libreco/algorithms/_als.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9206 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/_als.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   909347 2023-06-25 08:46:33.000000 LibRecommender-1.2.1/libreco/algorithms/_bpr.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13747 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/_bpr.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11407 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/als.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11454 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/autoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14587 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8628 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/caser.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12216 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/deepfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/deepwalk.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16665 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/din.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11547 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/fm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/graphsage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7718 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/graphsage_dgl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/item2vec.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6082 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/item_cf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/lightgcn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/ncf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/ngcf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6749 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/pinsage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7393 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/pinsage_dgl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9299 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/rnn4rec.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5877 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/svd.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7629 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/svdpp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.794808 LibRecommender-1.2.1/libreco/algorithms/torch_modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/torch_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6953 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/torch_modules/graphsage_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/torch_modules/lightgcn_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/torch_modules/ngcf_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6143 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/torch_modules/pinsage_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19898 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/two_tower.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6799 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/user_cf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8341 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/wave_net.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12002 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/wide_deep.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10863 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/youtube_ranking.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13542 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/algorithms/youtube_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/bases/
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4267 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13085 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/cf_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12160 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/dyn_embed_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19199 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/embed_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/gensim_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6241 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/sage_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14925 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/bases/tf_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/batch_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5495 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/batch_unit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18061 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/collators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3616 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/batch/tf_feed_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      599 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2307 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/consumed.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21492 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/data_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    26964 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5947 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13860 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/split.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4785 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/data/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/embedding/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/evaluation/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       87 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/evaluation/computation.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6426 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/evaluation/evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3394 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.798807 LibRecommender-1.2.1/libreco/feature/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1979 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5187 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/multi_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7384 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/ssl.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2167 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/unique.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8111 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/feature/update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/graph/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/graph/from_dgl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/graph/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/graph/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/graph/neighbor_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4012 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/prediction/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/prediction/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/recommendation/
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/recommendation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/recommendation/cold_start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8064 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/recommendation/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/recommendation/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3026 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/recommendation/recommend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/sampling/negatives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5773 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/sampling/random_walks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/tfops/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/configs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5757 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5110 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/tfops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.802807 LibRecommender-1.2.1/libreco/torchops/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/torchops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/torchops/configs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/torchops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/torchops/rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.806808 LibRecommender-1.2.1/libreco/training/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/training/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10497 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/training/tf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9466 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/training/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1334 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/training/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.806808 LibRecommender-1.2.1/libreco/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1114135 2023-06-25 08:46:35.000000 LibRecommender-1.2.1/libreco/utils/_similarities.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16758 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/_similarities.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1634 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/initializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2588 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14284 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/save_load.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7383 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/similarities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libreco/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.806808 LibRecommender-1.2.1/libserving/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.806808 LibRecommender-1.2.1/libserving/sanic_serving/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/embed_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/knn_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15205 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/online_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/sanic_serving/tf_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-25 08:46:35.810808 LibRecommender-1.2.1/libserving/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/knn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5954 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/online.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7042 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/redis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/libserving/serialization/tfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/requirements-serving.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-25 08:46:35.810808 LibRecommender-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-06-25 08:46:09.000000 LibRecommender-1.2.1/setup.py
```

### Comparing `LibRecommender-1.2.0/LICENSE` & `LibRecommender-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/LibRecommender.egg-info/PKG-INFO` & `LibRecommender-1.2.1/LibRecommender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibRecommender
-Version: 1.2.0
+Version: 1.2.1
 Summary: Versatile end-to-end recommender system.
 Home-page: https://github.com/massquantity/LibRecommender
 Author: massquantity
 Author-email: massquantity <jinxin_madie@163.com>
 License: MIT
 Project-URL: documentation, https://librecommender.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/massquantity/LibRecommender
```

### Comparing `LibRecommender-1.2.0/LibRecommender.egg-info/SOURCES.txt` & `LibRecommender-1.2.1/LibRecommender.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 libreco/feature/multi_sparse.py
 libreco/feature/sparse.py
 libreco/feature/ssl.py
 libreco/feature/unique.py
 libreco/feature/update.py
 libreco/graph/__init__.py
 libreco/graph/from_dgl.py
+libreco/graph/inference.py
 libreco/graph/message.py
 libreco/graph/neighbor_walk.py
 libreco/prediction/__init__.py
 libreco/prediction/predict.py
 libreco/prediction/preprocess.py
 libreco/recommendation/__init__.py
 libreco/recommendation/cold_start.py
```

### Comparing `LibRecommender-1.2.0/PKG-INFO` & `LibRecommender-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibRecommender
-Version: 1.2.0
+Version: 1.2.1
 Summary: Versatile end-to-end recommender system.
 Home-page: https://github.com/massquantity/LibRecommender
 Author: massquantity
 Author-email: massquantity <jinxin_madie@163.com>
 License: MIT
 Project-URL: documentation, https://librecommender.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/massquantity/LibRecommender
```

### Comparing `LibRecommender-1.2.0/README.md` & `LibRecommender-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/__init__.py` & `LibRecommender-1.2.1/libreco/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/_als.cpp` & `LibRecommender-1.2.1/libreco/algorithms/_als.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             "-std=c++11"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "libreco.algorithms._als",
         "sources": [
             "libreco/algorithms/_als.pyx"
         ]
     },
```

### Comparing `LibRecommender-1.2.0/libreco/algorithms/_als.pyx` & `LibRecommender-1.2.1/libreco/algorithms/_als.pyx`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/_bpr.cpp` & `LibRecommender-1.2.1/libreco/algorithms/_bpr.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             "-std=c++11"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "libreco.algorithms._bpr",
         "sources": [
             "libreco/algorithms/_bpr.pyx"
         ]
     },
```

### Comparing `LibRecommender-1.2.0/libreco/algorithms/_bpr.pyx` & `LibRecommender-1.2.1/libreco/algorithms/_bpr.pyx`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/als.py` & `LibRecommender-1.2.1/libreco/algorithms/als.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/autoint.py` & `LibRecommender-1.2.1/libreco/algorithms/autoint.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/bpr.py` & `LibRecommender-1.2.1/libreco/algorithms/bpr.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/caser.py` & `LibRecommender-1.2.1/libreco/algorithms/caser.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/deepfm.py` & `LibRecommender-1.2.1/libreco/algorithms/deepfm.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/deepwalk.py` & `LibRecommender-1.2.1/libreco/algorithms/deepwalk.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/din.py` & `LibRecommender-1.2.1/libreco/algorithms/din.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/fm.py` & `LibRecommender-1.2.1/libreco/algorithms/fm.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/graphsage.py` & `LibRecommender-1.2.1/libreco/algorithms/graphsage.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/graphsage_dgl.py` & `LibRecommender-1.2.1/libreco/algorithms/graphsage_dgl.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         probability on unpopular items, which may increase diversity but hurt metrics.
         This only applies in ``'i2i'`` paradigm.
     focus_start : bool, default: False
         Whether to keep the start nodes in random walk sampling. The purpose of the
         parameter ``start_node`` and ``focus_start`` is oversampling unpopular items.
         If you set ``start_node='popular'`` and ``focus_start=True``, unpopular items will
         be kept in positive samples, which may increase diversity.
+    full_inference : bool, default: False
+        Whether to get item embedding by aggregating over all neighbor embeddings.
     seed : int, default: 42
         Random seed.
     device : {'cpu', 'cuda'}, default: 'cuda'
         Refer to `torch.device <https://pytorch.org/docs/stable/tensor_attributes.html#torch.device>`_.
 
         .. versionchanged:: 1.0.0
            Accept str type ``'cpu'`` or ``'cuda'``, instead of ``torch.device(...)``.
@@ -146,14 +148,15 @@
         num_neighbors=3,
         num_walks=10,
         sample_walk_len=5,
         margin=1.0,
         sampler="random",
         start_node="random",
         focus_start=False,
+        full_inference=False,
         seed=42,
         device="cuda",
         lower_upper_bound=None,
     ):
         super().__init__(
             task,
             data_info,
@@ -177,14 +180,15 @@
             margin,
             sampler,
             start_node,
             focus_start,
             seed,
             device,
             lower_upper_bound,
+            full_inference,
         )
         self.all_args = locals()
         self.aggregator_type = aggregator_type
         if aggregator_type not in ("mean", "gcn", "pool", "lstm"):
             raise ValueError(
                 f"Unsupported `aggregator_type`: {aggregator_type} for GraphSageDGL"
             )
```

### Comparing `LibRecommender-1.2.0/libreco/algorithms/item2vec.py` & `LibRecommender-1.2.1/libreco/algorithms/item2vec.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/item_cf.py` & `LibRecommender-1.2.1/libreco/algorithms/item_cf.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/lightgcn.py` & `LibRecommender-1.2.1/libreco/algorithms/lightgcn.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/ncf.py` & `LibRecommender-1.2.1/libreco/algorithms/ncf.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/ngcf.py` & `LibRecommender-1.2.1/libreco/algorithms/ngcf.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/pinsage.py` & `LibRecommender-1.2.1/libreco/algorithms/pinsage.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/pinsage_dgl.py` & `LibRecommender-1.2.1/libreco/algorithms/pinsage_dgl.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         probability on unpopular items, which may increase diversity but hurt metrics.
         This only applies in ``'i2i'`` paradigm.
     focus_start : bool, default: False
         Whether to keep the start nodes in random walk sampling. The purpose of the
         parameter ``start_node`` and ``focus_start`` is oversampling unpopular items.
         If you set ``start_node='popular'`` and ``focus_start=True``, unpopular items will
         be kept in positive samples, which may increase diversity.
+    full_inference : bool, default: False
+        Whether to get item embedding by aggregating over all neighbor embeddings.
     seed : int, default: 42
         Random seed.
     device : {'cpu', 'cuda'}, default: 'cuda'
         Refer to `torch.device <https://pytorch.org/docs/stable/tensor_attributes.html#torch.device>`_.
 
         .. versionchanged:: 1.0.0
            Accept str type ``'cpu'`` or ``'cuda'``, instead of ``torch.device(...)``.
@@ -143,14 +145,15 @@
         neighbor_walk_len=2,
         sample_walk_len=5,
         termination_prob=0.5,
         margin=1.0,
         sampler="random",
         start_node="random",
         focus_start=False,
+        full_inference=False,
         seed=42,
         device="cuda",
         lower_upper_bound=None,
     ):
         super().__init__(
             task,
             data_info,
@@ -174,14 +177,15 @@
             margin,
             sampler,
             start_node,
             focus_start,
             seed,
             device,
             lower_upper_bound,
+            full_inference,
         )
         self.all_args = locals()
         self.neighbor_walk_len = neighbor_walk_len
         self.termination_prob = termination_prob
 
     def build_model(self):
         self._dgl.seed(self.seed)
```

### Comparing `LibRecommender-1.2.0/libreco/algorithms/rnn4rec.py` & `LibRecommender-1.2.1/libreco/algorithms/rnn4rec.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/svd.py` & `LibRecommender-1.2.1/libreco/algorithms/svd.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/svdpp.py` & `LibRecommender-1.2.1/libreco/algorithms/svdpp.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/torch_modules/graphsage_module.py` & `LibRecommender-1.2.1/libreco/algorithms/torch_modules/graphsage_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,84 +6,116 @@
     check_dense_values,
     check_sparse_indices,
     dense_field_size,
     sparse_feat_size,
 )
 
 
-class GraphSageModel(nn.Module):
-    def __init__(
-        self,
-        paradigm,
-        data_info,
-        embed_size,
-        batch_size,
-        num_layers,
-        dropout_rate,
-    ):
-        super(GraphSageModel, self).__init__()
+class GraphSageModelBase(nn.Module):
+    def __init__(self, paradigm, data_info, embed_size, batch_size, num_layers):
+        super(GraphSageModelBase, self).__init__()
         self.paradigm = paradigm
         self.embed_size = embed_size
         self.batch_size = batch_size
         self.num_layers = num_layers
-        self.dropout = nn.Dropout(dropout_rate)
         self.item_embeds = nn.Embedding(data_info.n_items, embed_size)
         item_input_dim = (len(data_info.item_col) + 1) * embed_size
         self.item_proj = nn.Linear(item_input_dim, embed_size)
         self.item_dense_col_indices = data_info.item_dense_col.index
-        self.w_linears = nn.ModuleList(
-            [nn.Linear(embed_size * 2, embed_size) for _ in range(num_layers)]
-        )
         if paradigm == "u2i":
             self.user_embeds = nn.Embedding(data_info.n_users, embed_size)
             user_input_dim = (len(data_info.user_col) + 1) * embed_size
             self.user_proj = nn.Linear(user_input_dim, embed_size)
             self.user_dense_col_indices = data_info.user_dense_col.index
         self.sparse = check_sparse_indices(data_info)
         self.dense = check_dense_values(data_info)
         if self.sparse:
             self.sparse_embeds = nn.Embedding(sparse_feat_size(data_info), embed_size)
         if self.dense:
             self.dense_embeds = nn.Parameter(
                 torch.empty(dense_field_size(data_info), embed_size)
             )
-        self.init_parameters()
 
     def init_parameters(self):
-        gain = nn.init.calculate_gain("relu")
         if self.paradigm == "u2i":
             nn.init.xavier_uniform_(self.user_embeds.weight)
             nn.init.xavier_uniform_(self.user_proj.weight)
             nn.init.zeros_(self.user_proj.bias)
         nn.init.xavier_uniform_(self.item_embeds.weight)
         nn.init.xavier_uniform_(self.item_proj.weight)
         nn.init.zeros_(self.item_proj.bias)
+        if self.sparse:
+            nn.init.xavier_uniform_(self.sparse_embeds.weight)
+        if self.dense:
+            nn.init.xavier_uniform_(self.dense_embeds)
+
+    def user_repr(self, users, sparse_indices, dense_values):
+        return self.get_raw_features(users, sparse_indices, dense_values, is_user=True)
+
+    def get_raw_features(self, ids, sparse_indices, dense_values, is_user):
+        concat_features = []
+        if sparse_indices is not None:
+            sparse_feature = self.sparse_embeds(sparse_indices)
+            concat_features.append(sparse_feature.flatten(start_dim=1))
+        if dense_values is not None:
+            batch_size = dense_values.shape[0]
+            # B * F_dense * K
+            index = (
+                self.user_dense_col_indices if is_user else self.item_dense_col_indices
+            )
+            dense_embeds = self.dense_embeds[index].repeat(batch_size, 1, 1)
+            # B * F_dense * 1
+            dense_vals = dense_values.unsqueeze(2)
+            dense_feature = torch.mul(dense_embeds, dense_vals)
+            concat_features.append(dense_feature.flatten(start_dim=1))
+
+        if is_user:
+            concat_features.append(self.user_embeds(ids))
+            concat_features = torch.cat(concat_features, dim=1)
+            proj_features = self.user_proj(concat_features)
+        else:
+            concat_features.append(self.item_embeds(ids))
+            concat_features = torch.cat(concat_features, dim=1)
+            proj_features = self.item_proj(concat_features)
+        return proj_features
+
+
+class GraphSageModel(GraphSageModelBase):
+    def __init__(
+        self, paradigm, data_info, embed_size, batch_size, num_layers, dropout_rate
+    ):
+        super().__init__(paradigm, data_info, embed_size, batch_size, num_layers)
+        self.dropout = nn.Dropout(dropout_rate)
+        self.w_linears = nn.ModuleList(
+            [nn.Linear(embed_size * 2, embed_size) for _ in range(num_layers)]
+        )
+        self.init_parameters()
+
+    def init_parameters(self):
+        super().init_parameters()
+        gain = nn.init.calculate_gain("relu")
         for i, w in enumerate(self.w_linears):
             if i == self.num_layers - 1:
                 nn.init.xavier_uniform_(w.weight)
             else:
                 nn.init.xavier_uniform_(w.weight, gain=gain)
             nn.init.zeros_(w.bias)
-        if self.sparse:
-            nn.init.xavier_uniform_(self.sparse_embeds.weight)
-        if self.dense:
-            nn.init.xavier_uniform_(self.dense_embeds)
 
+    # paper author's implementation: https://github.com/williamleif/GraphSAGE/blob/master/graphsage/models.py#L299
     def forward(
         self,
         items,
         sparse_indices,
         dense_values,
         neighbors,
         neighbor_sparse_indices,
         neighbor_dense_values,
         offsets,
         weights=None,
     ):
-        # paper author's implementation: https://github.com/williamleif/GraphSAGE/blob/master/graphsage/models.py#L299
         hidden = [
             self.get_raw_features(items, sparse_indices, dense_values, is_user=False)
         ]
         for n, s, d in zip(neighbors, neighbor_sparse_indices, neighbor_dense_values):
             hidden.append(self.get_raw_features(n, s, d, is_user=False))
         for layer in range(self.num_layers):
             w_linear = self.w_linears[layer]
@@ -103,76 +135,45 @@
                     h = w_linear(h)
                 else:
                     h = F.relu(w_linear(h))
                 next_hidden.append(h)
             hidden = next_hidden
         return hidden[0]
 
-    def user_repr(self, users, sparse_indices, dense_values):
-        return self.get_raw_features(users, sparse_indices, dense_values, is_user=True)
-
-    def get_raw_features(self, ids, sparse_indices, dense_values, is_user):
-        concat_features = []
-        if sparse_indices is not None:
-            sparse_feature = self.sparse_embeds(sparse_indices)
-            concat_features.append(sparse_feature.flatten(start_dim=1))
-        if dense_values is not None:
-            batch_size = dense_values.shape[0]
-            # B * F_dense * K
-            index = (
-                self.user_dense_col_indices if is_user else self.item_dense_col_indices
-            )
-            dense_embeds = self.dense_embeds[index].repeat(batch_size, 1, 1)
-            # B * F_dense * 1
-            dense_vals = dense_values.unsqueeze(2)
-            dense_feature = torch.mul(dense_embeds, dense_vals)
-            concat_features.append(dense_feature.flatten(start_dim=1))
-
-        if is_user:
-            concat_features.append(self.user_embeds(ids))
-            concat_features = torch.cat(concat_features, dim=1)
-            proj_features = self.user_proj(concat_features)
-        else:
-            concat_features.append(self.item_embeds(ids))
-            concat_features = torch.cat(concat_features, dim=1)
-            proj_features = self.item_proj(concat_features)
-        return proj_features
 
-
-class GraphSageDGLModel(GraphSageModel):
+class GraphSageDGLModel(GraphSageModelBase):
     def __init__(
         self,
         paradigm,
         data_info,
         embed_size,
         batch_size,
         num_layers,
         dropout_rate,
         aggregator_type,
     ):
         # noinspection PyUnresolvedReferences
         from dgl.nn import SAGEConv
 
-        super().__init__(
-            paradigm, data_info, embed_size, batch_size, num_layers, dropout_rate
-        )
+        super().__init__(paradigm, data_info, embed_size, batch_size, num_layers)
         self.layers = nn.ModuleList(
             [
                 SAGEConv(
                     in_feats=embed_size,
                     out_feats=embed_size,
                     aggregator_type=aggregator_type,
                     feat_drop=dropout_rate,
                     bias=True,
                     norm=None,
                     activation=None,
                 )
                 for _ in range(num_layers)
             ]
         )
+        self.init_parameters()
 
     def forward(self, blocks, nodes, sparse_indices, dense_values, *_):
         h = self.get_raw_features(nodes, sparse_indices, dense_values, is_user=False)
         for i, (layer, block) in enumerate(zip(self.layers, blocks)):
             h = layer(block, h)
             if i != self.num_layers - 1:
                 h = F.relu(h)
```

### Comparing `LibRecommender-1.2.0/libreco/algorithms/torch_modules/lightgcn_module.py` & `LibRecommender-1.2.1/libreco/algorithms/torch_modules/lightgcn_module.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/torch_modules/ngcf_module.py` & `LibRecommender-1.2.1/libreco/algorithms/torch_modules/ngcf_module.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/two_tower.py` & `LibRecommender-1.2.1/libreco/algorithms/two_tower.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/user_cf.py` & `LibRecommender-1.2.1/libreco/algorithms/user_cf.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/wave_net.py` & `LibRecommender-1.2.1/libreco/algorithms/wave_net.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/wide_deep.py` & `LibRecommender-1.2.1/libreco/algorithms/wide_deep.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/youtube_ranking.py` & `LibRecommender-1.2.1/libreco/algorithms/youtube_ranking.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/algorithms/youtube_retrieval.py` & `LibRecommender-1.2.1/libreco/algorithms/youtube_retrieval.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/base.py` & `LibRecommender-1.2.1/libreco/bases/base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/cf_base.py` & `LibRecommender-1.2.1/libreco/bases/cf_base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/dyn_embed_base.py` & `LibRecommender-1.2.1/libreco/bases/dyn_embed_base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/embed_base.py` & `LibRecommender-1.2.1/libreco/bases/embed_base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/gensim_base.py` & `LibRecommender-1.2.1/libreco/bases/gensim_base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/meta.py` & `LibRecommender-1.2.1/libreco/bases/meta.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/bases/sage_base.py` & `LibRecommender-1.2.1/libreco/bases/sage_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from ..bases import EmbedBase
 from ..graph import NeighborWalker
+from ..graph.inference import full_neighbor_embeddings
 from ..graph.message import ItemMessage, ItemMessageDGL, UserMessage
 from ..torchops import device_config
 
 
 class SageBase(EmbedBase):
     """Base class for GraphSage and PinSage.
 
@@ -48,14 +49,15 @@
         margin=1.0,
         sampler="random",
         start_node="random",
         focus_start=False,
         seed=42,
         device="cuda",
         lower_upper_bound=None,
+        full_inference=False,
     ):
         super().__init__(task, data_info, embed_size, lower_upper_bound)
 
         self.all_args = locals()
         self.loss_type = loss_type
         self.paradigm = paradigm
         self.n_epochs = n_epochs
@@ -73,14 +75,15 @@
         self.num_walks = num_walks
         self.sample_walk_len = sample_walk_len
         self.margin = margin
         self.sampler = sampler
         self.start_node = start_node
         self.focus_start = focus_start
         self.neighbor_walker = None
+        self.full_inference = full_inference
         self.seed = seed
         self.device = device_config(device)
         self.use_dgl = "DGL" in self.model_name
         self.torch_model = None
         self._check_params()
 
     def _check_params(self):
@@ -131,25 +134,28 @@
             blocks, start_nodes, sparse_indices, dense_values = astuple(item_data)
             return self.torch_model(blocks, start_nodes, sparse_indices, dense_values)
 
     @torch.no_grad()
     def set_embeddings(self):
         assert isinstance(self.neighbor_walker, NeighborWalker)
         self.torch_model.eval()
-        item_embed = []
-        all_items = list(range(self.n_items))
-        for i in tqdm(range(0, self.n_items, self.batch_size), desc="item embedding"):
-            batch_items = all_items[i : i + self.batch_size]
-            if self.use_dgl:
-                batch_items = torch.tensor(batch_items, dtype=torch.long)
-            item_data = self.neighbor_walker(batch_items)
-            item_data = item_data.to_device(self.device)
-            item_reprs = self.get_item_repr(item_data)
-            item_embed.append(item_reprs.detach().cpu().numpy())
-        self.item_embeds_np = np.concatenate(item_embed, axis=0)
+        if self.full_inference and self.use_dgl:
+            self.item_embeds_np = full_neighbor_embeddings(self)
+        else:
+            item_embed = []
+            all_items = list(range(self.n_items))
+            for i in tqdm(range(0, self.n_items, self.batch_size), desc="item embeds"):
+                batch_items = all_items[i : i + self.batch_size]
+                if self.use_dgl:
+                    batch_items = torch.tensor(batch_items, dtype=torch.long)
+                item_data = self.neighbor_walker(batch_items)
+                item_data = item_data.to_device(self.device)
+                item_reprs = self.get_item_repr(item_data)
+                item_embed.append(item_reprs.detach().cpu().numpy())
+            self.item_embeds_np = np.concatenate(item_embed, axis=0)
         self.user_embeds_np = self._compute_user_embeddings()
 
     @torch.no_grad()
     def _compute_user_embeddings(self):
         self.torch_model.eval()
         user_embed = []
         if self.paradigm == "u2i":
```

### Comparing `LibRecommender-1.2.0/libreco/bases/tf_base.py` & `LibRecommender-1.2.1/libreco/bases/tf_base.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/batch/batch_data.py` & `LibRecommender-1.2.1/libreco/batch/batch_data.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/batch/batch_unit.py` & `LibRecommender-1.2.1/libreco/batch/batch_unit.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/batch/collators.py` & `LibRecommender-1.2.1/libreco/batch/collators.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/batch/sequence.py` & `LibRecommender-1.2.1/libreco/batch/sequence.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/batch/tf_feed_dicts.py` & `LibRecommender-1.2.1/libreco/batch/tf_feed_dicts.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/data/__init__.py` & `LibRecommender-1.2.1/libreco/data/__init__.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/data/consumed.py` & `LibRecommender-1.2.1/libreco/data/consumed.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,30 +25,25 @@
     else:  # pragma: no cover
         dict_func = OrderedDict.fromkeys
     user_dedup = {u: list(dict_func(items)) for u, items in user_consumed.items()}
     item_dedup = {i: list(dict_func(users)) for i, users in item_consumed.items()}
     return user_dedup, item_dedup
 
 
-def update_consumed(new_data_info, data_info, merge_behavior):
+def update_consumed(
+    user_indices, item_indices, n_users, n_items, old_info, merge_behavior
+):
+    user_consumed, item_consumed = interaction_consumed(user_indices, item_indices)
     if merge_behavior:
-        new_data_info.user_consumed = _merge_dedup(
-            new_data_info.user_consumed, new_data_info.n_users, data_info.user_consumed
-        )
-        new_data_info.item_consumed = _merge_dedup(
-            new_data_info.item_consumed, new_data_info.n_items, data_info.item_consumed
-        )
+        user_consumed = _merge_dedup(user_consumed, n_users, old_info.user_consumed)
+        item_consumed = _merge_dedup(item_consumed, n_items, old_info.item_consumed)
     else:
-        new_data_info.user_consumed = _fill_empty(
-            new_data_info.user_consumed, new_data_info.n_users, data_info.user_consumed
-        )
-        new_data_info.item_consumed = _fill_empty(
-            new_data_info.item_consumed, new_data_info.n_items, data_info.item_consumed
-        )
-    return new_data_info
+        user_consumed = _fill_empty(user_consumed, n_users, old_info.user_consumed)
+        item_consumed = _fill_empty(item_consumed, n_items, old_info.item_consumed)
+    return user_consumed, item_consumed
 
 
 def _merge_dedup(new_consumed, num, old_consumed):
     result = dict()
     for i in range(num):
         assert i in new_consumed or i in old_consumed
         if i in new_consumed and i in old_consumed:
```

### Comparing `LibRecommender-1.2.0/libreco/data/data_info.py` & `LibRecommender-1.2.1/libreco/data/data_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Classes for Storing Various Data Information."""
 import inspect
 import json
-import os
+import pickle
 from collections import namedtuple
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Any, Dict, Iterable, List
 
 import numpy as np
 import pandas as pd
 
-from .consumed import interaction_consumed
 from ..feature.update import (
     get_row_id_masks,
     update_new_dense_feats,
     update_new_sparse_feats,
 )
 
 Feature = namedtuple("Feature", ["name", "index"])
@@ -65,18 +65,18 @@
         Unique sparse features for all users in train data.
     user_dense_unique : numpy.ndarray or None, default: None
         Unique dense features for all users in train data.
     item_sparse_unique : numpy.ndarray or None, default: None
         Unique sparse features for all items in train data.
     item_dense_unique : numpy.ndarray or None, default: None
         Unique dense features for all items in train data.
-    user_indices : numpy.ndarray or None, default: None
-        Mapped inner user indices from train data.
-    item_indices : numpy.ndarray or None, default: None
-        Mapped inner item indices from train data.
+    user_consumed : dict of {int : list} or None, default: None
+        All consumed items by each user.
+    item_consumed : dict of {int : list} or None, default: None
+        All consumed users by each item.
     user_unique_vals : numpy.ndarray or None, default: None
         All the unique users in train data.
     item_unique_vals : numpy.ndarray or None, default: None
         All the unique items in train data.
     sparse_unique_vals : dict of {str : numpy.ndarray} or None, default: None
         All sparse features' unique values.
     sparse_offset : numpy.ndarray or None, default: None
@@ -106,33 +106,32 @@
         self,
         col_name_mapping=None,
         interaction_data=None,
         user_sparse_unique=None,
         user_dense_unique=None,
         item_sparse_unique=None,
         item_dense_unique=None,
-        user_indices=None,
-        item_indices=None,
+        user_consumed=None,
+        item_consumed=None,
         user_unique_vals=None,
         item_unique_vals=None,
         sparse_unique_vals=None,
         sparse_offset=None,
         sparse_oov=None,
         multi_sparse_unique_vals=None,
         multi_sparse_combine_info=None,
     ):
         self.col_name_mapping = col_name_mapping
         self.interaction_data = interaction_data
         self.user_sparse_unique = user_sparse_unique
         self.user_dense_unique = user_dense_unique
         self.item_sparse_unique = item_sparse_unique
         self.item_dense_unique = item_dense_unique
-        self.user_consumed, self.item_consumed = interaction_consumed(
-            user_indices, item_indices
-        )
+        self.user_consumed = user_consumed
+        self.item_consumed = item_consumed
         self.user_unique_vals = user_unique_vals
         self.item_unique_vals = item_unique_vals
         self.sparse_unique_vals = sparse_unique_vals
         self.sparse_offset = sparse_offset
         self.sparse_oov = sparse_oov
         self.multi_sparse_unique_vals = multi_sparse_unique_vals
         self.multi_sparse_combine_info = multi_sparse_combine_info
@@ -436,35 +435,38 @@
         Parameters
         ----------
         path : str
             File folder path to save :class:`DataInfo`.
         model_name : str
             Name of the saved file.
         """
-        if not os.path.isdir(path):
+        path = Path(path)
+        if not path.is_dir():
             print(f"file folder {path} doesn't exists, creating a new one...")
-            os.makedirs(path)
+            path.mkdir()
         if self.col_name_mapping is not None:
-            name_mapping_path = os.path.join(
-                path, f"{model_name}_data_info_name_mapping.json"
-            )
-            with open(name_mapping_path, "w") as f:
+            with open(path / f"{model_name}_data_info_name_mapping.json", "w") as f:
                 json.dump(
                     self.all_args["col_name_mapping"],
                     f,
                     separators=(",", ":"),
                     indent=4,
                 )
+        if self.user_consumed is not None:
+            with open(path / f"{model_name}_user_consumed.pkl", "wb") as f:
+                pickle.dump(self.user_consumed, f, protocol=pickle.HIGHEST_PROTOCOL)
+        if self.item_consumed is not None:
+            with open(path / f"{model_name}_item_consumed.pkl", "wb") as f:
+                pickle.dump(self.item_consumed, f, protocol=pickle.HIGHEST_PROTOCOL)
 
-        other_path = os.path.join(path, f"{model_name}_data_info")
         hparams = dict()
         arg_names = inspect.signature(self.__init__).parameters.keys()
         for arg in arg_names:
             if (
-                arg == "col_name_mapping"
+                arg in ("col_name_mapping", "user_consumed", "item_consumed")
                 or arg not in self.all_args
                 or self.all_args[arg] is None
             ):
                 continue
             if arg == "interaction_data":
                 hparams[arg] = self.all_args[arg].to_numpy()
             elif arg == "sparse_unique_vals":
@@ -474,40 +476,47 @@
             elif arg == "multi_sparse_unique_vals":
                 multi_sparse_unique_vals = self.all_args[arg]
                 for col, val in multi_sparse_unique_vals.items():
                     hparams["munique_" + str(col)] = np.asarray(val)
             else:
                 hparams[arg] = self.all_args[arg]
 
-        np.savez_compressed(other_path, **hparams)
+        np.savez_compressed(path / f"{model_name}_data_info", **hparams)
 
     @classmethod
     def load(cls, path, model_name):
         """Load saved :class:`DataInfo`.
 
         Parameters
         ----------
         path : str
             File folder path to save :class:`DataInfo`.
         model_name : str
             Name of the saved file.
         """
-        if not os.path.exists(path):
+        path = Path(path)
+        if not path.exists():
             raise OSError(f"file folder {path} doesn't exists...")
 
         hparams = dict()
-        name_mapping_path = os.path.join(
-            path, f"{model_name}_data_info_name_mapping.json"
-        )
-        if os.path.exists(name_mapping_path):
+        name_mapping_path = path / f"{model_name}_data_info_name_mapping.json"
+        if name_mapping_path.exists():
             with open(name_mapping_path, "r") as f:
                 hparams["col_name_mapping"] = json.load(f)
 
-        other_path = os.path.join(path, f"{model_name}_data_info.npz")
-        info = np.load(other_path, allow_pickle=True)
+        user_consumed_path = path / f"{model_name}_user_consumed.pkl"
+        if user_consumed_path.exists():
+            with open(user_consumed_path, "rb") as f:
+                hparams["user_consumed"] = pickle.load(f)
+        item_consumed_path = path / f"{model_name}_item_consumed.pkl"
+        if item_consumed_path.exists():
+            with open(item_consumed_path, "rb") as f:
+                hparams["item_consumed"] = pickle.load(f)
+
+        info = np.load(path / f"{model_name}_data_info.npz", allow_pickle=True)
         info = dict(info.items())
         for arg in info:
             if arg == "interaction_data":
                 hparams[arg] = pd.DataFrame(
                     info[arg], columns=["user", "item", "label"]
                 )
             elif arg == "multi_sparse_combine_info":
@@ -552,14 +561,15 @@
             multi_sparse_unique is not None
             and "multi_sparse" in data_info.col_name_mapping
             and col in data_info.col_name_mapping["multi_sparse"]
         ):
             # multi_sparse case, second to last cols are redundant.
             # Used in `rebuild_tf_model`, `rebuild_torch_model`
             sparse_len.append(-1)
+
     return OldInfo(
         data_info.n_users,
         data_info.n_items,
         sparse_len,
         sparse_oov,
         data_info.popular_items,
     )
```

### Comparing `LibRecommender-1.2.0/libreco/data/dataset.py` & `LibRecommender-1.2.1/libreco/data/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Classes for Transforming and Building Data."""
 import functools
 import itertools
 
 import numpy as np
 
-from .consumed import update_consumed
+from .consumed import interaction_consumed, update_consumed
 from .data_info import DataInfo, store_old_info
 from .transformed import TransformedSet
 from ..feature.column_mapping import col_name2index
 from ..feature.multi_sparse import (
     get_multi_sparse_info,
     multi_sparse_col_map,
     recover_sparse_cols,
@@ -242,18 +242,19 @@
         train_transformed, user_indices, item_indices = _build_transformed_set(
             train_data,
             cls.user_unique_vals,
             cls.item_unique_vals,
             is_train=True,
             is_ordered=True,
         )
+        user_consumed, item_consumed = interaction_consumed(user_indices, item_indices)
         data_info = DataInfo(
             interaction_data=train_data[["user", "item", "label"]],
-            user_indices=user_indices,
-            item_indices=item_indices,
+            user_consumed=user_consumed,
+            item_consumed=item_consumed,
             user_unique_vals=cls.user_unique_vals,
             item_unique_vals=cls.item_unique_vals,
         )
         cls.train_called = True
         return train_transformed, data_info
 
     @classmethod
@@ -299,22 +300,30 @@
         merge_transformed, user_indices, item_indices = _build_transformed_set(
             train_data,
             cls.user_unique_vals,
             cls.item_unique_vals,
             is_train=True,
             is_ordered=False,
         )
+        user_consumed, item_consumed = update_consumed(
+            user_indices,
+            item_indices,
+            len(cls.user_unique_vals),
+            len(cls.item_unique_vals),
+            data_info,
+            merge_behavior,
+        )
+
         new_data_info = DataInfo(
             interaction_data=train_data[["user", "item", "label"]],
-            user_indices=user_indices,
-            item_indices=item_indices,
+            user_consumed=user_consumed,
+            item_consumed=item_consumed,
             user_unique_vals=cls.user_unique_vals,
             item_unique_vals=cls.item_unique_vals,
         )
-        new_data_info = update_consumed(new_data_info, data_info, merge_behavior)
         new_data_info.old_info = store_old_info(data_info)
         cls.train_called = True
         return merge_transformed, new_data_info
 
 
 class DatasetFeat(_Dataset):
     """Dataset class used for building data contains features.
@@ -507,23 +516,24 @@
             cls.multi_sparse_unique_vals,
             pad_val_dict,
         )
         if cls.multi_sparse_col:
             col_name_mapping["multi_sparse"] = multi_sparse_col_map(multi_sparse_col)
 
         interaction_data = train_data[["user", "item", "label"]]
+        user_consumed, item_consumed = interaction_consumed(user_indices, item_indices)
         data_info = DataInfo(
             col_name_mapping,
             interaction_data,
             user_sparse_unique,
             user_dense_unique,
             item_sparse_unique,
             item_dense_unique,
-            user_indices,
-            item_indices,
+            user_consumed,
+            item_consumed,
             cls.user_unique_vals,
             cls.item_unique_vals,
             cls.sparse_unique_vals,
             sparse_offset,
             sparse_oov,
             cls.multi_sparse_unique_vals,
             multi_sparse_info,
@@ -628,32 +638,40 @@
             unique_ids=cls.user_unique_vals, is_user=True
         )
         item_sparse_unique, item_dense_unique = _update_func(
             unique_ids=cls.item_unique_vals, is_user=False
         )
 
         interaction_data = train_data[["user", "item", "label"]]
+        user_consumed, item_consumed = update_consumed(
+            user_indices,
+            item_indices,
+            len(cls.user_unique_vals),
+            len(cls.item_unique_vals),
+            data_info,
+            merge_behavior,
+        )
+
         new_data_info = DataInfo(
             data_info.col_name_mapping,
             interaction_data,
             user_sparse_unique,
             user_dense_unique,
             item_sparse_unique,
             item_dense_unique,
-            user_indices,
-            item_indices,
+            user_consumed,
+            item_consumed,
             cls.user_unique_vals,
             cls.item_unique_vals,
             cls.sparse_unique_vals,
             sparse_offset,
             sparse_oov,
             cls.multi_sparse_unique_vals,
             multi_sparse_info,
         )
-        new_data_info = update_consumed(new_data_info, data_info, merge_behavior)
         new_data_info.old_info = store_old_info(data_info)
         cls.train_called = True
         return merge_transformed, new_data_info
 
 
 def _get_sparse_unique_vals(sparse_col, train_data):
     if not sparse_col:
```

### Comparing `LibRecommender-1.2.0/libreco/data/processing.py` & `LibRecommender-1.2.1/libreco/data/processing.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/data/split.py` & `LibRecommender-1.2.1/libreco/data/split.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/data/transformed.py` & `LibRecommender-1.2.1/libreco/data/transformed.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/embedding/normalize.py` & `LibRecommender-1.2.1/libreco/embedding/normalize.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/evaluation/computation.py` & `LibRecommender-1.2.1/libreco/evaluation/computation.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/evaluation/evaluate.py` & `LibRecommender-1.2.1/libreco/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/evaluation/metrics.py` & `LibRecommender-1.2.1/libreco/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/column_mapping.py` & `LibRecommender-1.2.1/libreco/feature/column_mapping.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/multi_sparse.py` & `LibRecommender-1.2.1/libreco/feature/multi_sparse.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/sparse.py` & `LibRecommender-1.2.1/libreco/feature/sparse.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/ssl.py` & `LibRecommender-1.2.1/libreco/feature/ssl.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/unique.py` & `LibRecommender-1.2.1/libreco/feature/unique.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/feature/update.py` & `LibRecommender-1.2.1/libreco/feature/update.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/graph/from_dgl.py` & `LibRecommender-1.2.1/libreco/graph/from_dgl.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/graph/message.py` & `LibRecommender-1.2.1/libreco/graph/message.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/graph/neighbor_walk.py` & `LibRecommender-1.2.1/libreco/graph/neighbor_walk.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/prediction/predict.py` & `LibRecommender-1.2.1/libreco/prediction/predict.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/prediction/preprocess.py` & `LibRecommender-1.2.1/libreco/prediction/preprocess.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/recommendation/cold_start.py` & `LibRecommender-1.2.1/libreco/recommendation/cold_start.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/recommendation/preprocess.py` & `LibRecommender-1.2.1/libreco/recommendation/preprocess.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/recommendation/ranking.py` & `LibRecommender-1.2.1/libreco/recommendation/ranking.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/recommendation/recommend.py` & `LibRecommender-1.2.1/libreco/recommendation/recommend.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/sampling/__init__.py` & `LibRecommender-1.2.1/libreco/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/sampling/negatives.py` & `LibRecommender-1.2.1/libreco/sampling/negatives.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/sampling/random_walks.py` & `LibRecommender-1.2.1/libreco/sampling/random_walks.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/__init__.py` & `LibRecommender-1.2.1/libreco/tfops/__init__.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/configs.py` & `LibRecommender-1.2.1/libreco/tfops/configs.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/features.py` & `LibRecommender-1.2.1/libreco/tfops/features.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/layers.py` & `LibRecommender-1.2.1/libreco/tfops/layers.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/loss.py` & `LibRecommender-1.2.1/libreco/tfops/loss.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/rebuild.py` & `LibRecommender-1.2.1/libreco/tfops/rebuild.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/tfops/variables.py` & `LibRecommender-1.2.1/libreco/tfops/variables.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/torchops/__init__.py` & `LibRecommender-1.2.1/libreco/torchops/__init__.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/torchops/configs.py` & `LibRecommender-1.2.1/libreco/torchops/configs.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/torchops/loss.py` & `LibRecommender-1.2.1/libreco/torchops/loss.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/torchops/rebuild.py` & `LibRecommender-1.2.1/libreco/torchops/rebuild.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/training/dispatch.py` & `LibRecommender-1.2.1/libreco/training/dispatch.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/training/tf_trainer.py` & `LibRecommender-1.2.1/libreco/training/tf_trainer.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/training/torch_trainer.py` & `LibRecommender-1.2.1/libreco/training/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/training/trainer.py` & `LibRecommender-1.2.1/libreco/training/trainer.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/_similarities.cpp` & `LibRecommender-1.2.1/libreco/utils/_similarities.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-maybe-uninitialized",
             "-O3",
             "-ffast-math",
             "-fopenmp",
             "-std=c++11"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "libreco.utils._similarities",
         "sources": [
             "libreco/utils/_similarities.pyx"
         ]
     },
@@ -1149,195 +1149,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1377,42 +1377,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -8099,15 +8099,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_x_count, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8116,29 +8116,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8149,15 +8149,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8166,29 +8166,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8199,15 +8199,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8216,29 +8216,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8249,15 +8249,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8266,29 +8266,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8299,15 +8299,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8316,29 +8316,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8349,212 +8349,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8570,15 +8570,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8586,53 +8586,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -8640,30 +8640,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8678,15 +8678,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8702,15 +8702,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8718,53 +8718,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -8772,30 +8772,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8810,15 +8810,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8834,15 +8834,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8850,53 +8850,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -8904,30 +8904,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8942,176 +8942,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23188,26 +23188,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-znxlnr76/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-ve1qys_x/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `LibRecommender-1.2.0/libreco/utils/_similarities.pyx` & `LibRecommender-1.2.1/libreco/utils/_similarities.pyx`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/constants.py` & `LibRecommender-1.2.1/libreco/utils/constants.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/initializers.py` & `LibRecommender-1.2.1/libreco/utils/initializers.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/misc.py` & `LibRecommender-1.2.1/libreco/utils/misc.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/sampling.py` & `LibRecommender-1.2.1/libreco/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/save_load.py` & `LibRecommender-1.2.1/libreco/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/similarities.py` & `LibRecommender-1.2.1/libreco/utils/similarities.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libreco/utils/validate.py` & `LibRecommender-1.2.1/libreco/utils/validate.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/request.py` & `LibRecommender-1.2.1/libserving/request.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/benchmark.py` & `LibRecommender-1.2.1/libserving/sanic_serving/benchmark.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/common.py` & `LibRecommender-1.2.1/libserving/sanic_serving/common.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/embed_deploy.py` & `LibRecommender-1.2.1/libserving/sanic_serving/embed_deploy.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/knn_deploy.py` & `LibRecommender-1.2.1/libserving/sanic_serving/knn_deploy.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/online_deploy.py` & `LibRecommender-1.2.1/libserving/sanic_serving/online_deploy.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/sanic_serving/tf_deploy.py` & `LibRecommender-1.2.1/libserving/sanic_serving/tf_deploy.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/common.py` & `LibRecommender-1.2.1/libserving/serialization/common.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/embed.py` & `LibRecommender-1.2.1/libserving/serialization/embed.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/knn.py` & `LibRecommender-1.2.1/libserving/serialization/knn.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/online.py` & `LibRecommender-1.2.1/libserving/serialization/online.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/redis.py` & `LibRecommender-1.2.1/libserving/serialization/redis.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/libserving/serialization/tfmodel.py` & `LibRecommender-1.2.1/libserving/serialization/tfmodel.py`

 * *Files identical despite different names*

### Comparing `LibRecommender-1.2.0/pyproject.toml` & `LibRecommender-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "scipy>=1.2.1",
     "tomli",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LibRecommender"
-version = "1.2.0"
+version = "1.2.1"
 description = "Versatile end-to-end recommender system."
 authors = [
     { name = "massquantity", email = "jinxin_madie@163.com" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.6"
@@ -86,15 +86,15 @@
     "ignore:`build_negative_samples` is deprecated",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py38"
 show-source = true
-ignore = ["E501"]
+ignore = ["E501", "RUF012"]
 select = [
     # pyflakes
     "F",
     # pycodestyle(Error, Warning)
     "E",
     "W",
     # flake8-2020
```

### Comparing `LibRecommender-1.2.0/setup.py` & `LibRecommender-1.2.1/setup.py`

 * *Files identical despite different names*

