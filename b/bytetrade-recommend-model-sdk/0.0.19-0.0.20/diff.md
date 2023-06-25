# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.19.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.19.tar", last modified: Tue Jun 20 08:41:32 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.20.tar", last modified: Sun Jun 25 06:06:05 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.19.tar` & `bytetrade-recommend-model-sdk-0.0.20.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-20 08:41:32.000000 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-06-20 08:41:32.000000 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-20 08:41:32.000000 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-06-20 08:41:32.000000 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-20 08:41:32.000000 bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-06-20 08:36:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 06:43:29.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:12:28.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-06-16 07:42:45.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2023-06-10 21:00:03.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 21:32:28.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2023-06-10 21:40:00.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-06-12 05:18:24.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-06-09 01:37:52.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:36:32.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-07 22:40:09.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11614 2023-06-13 09:09:31.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-06-07 07:14:04.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:01:07.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9414 2023-06-16 07:32:06.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/model/content_similar_model.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.485070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-06-16 05:57:06.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-06-16 07:52:03.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-06-16 07:54:02.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-06-06 23:52:17.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-06-12 05:13:22.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-20 08:41:32.489070 bytetrade-recommend-model-sdk-0.0.19/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-06-20 08:38:18.000000 bytetrade-recommend-model-sdk-0.0.19/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2116 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-06-20 08:36:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 06:43:29.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:12:28.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-06-16 07:42:45.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-06-24 23:59:37.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 21:32:28.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-06-25 00:55:03.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-06-25 03:47:07.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1694 2023-06-25 03:52:55.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-06-12 05:18:24.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-06-09 01:37:52.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:36:32.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-07 22:40:09.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11614 2023-06-13 09:09:31.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-06-07 07:14:04.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:01:07.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9414 2023-06-16 07:32:06.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2066 2023-06-24 06:04:38.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 09:34:20.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-06-24 11:18:18.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/mind_dnn_click_predictor_train_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-06-16 05:57:06.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-06-16 07:52:03.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-06-25 05:52:52.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-06-06 23:52:17.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-06-12 05:13:22.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-06-25 06:05:33.000000 bytetrade-recommend-model-sdk-0.0.20/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.19/README.md` & `bytetrade-recommend-model-sdk-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 recommend_model_sdk/embeddings/word2vec_embedding.py
 recommend_model_sdk/mind_sdk/__init__.py
 recommend_model_sdk/mind_sdk/experiment_enum.py
 recommend_model_sdk/mind_sdk/config/__init__.py
 recommend_model_sdk/mind_sdk/config/content_similar_config.py
 recommend_model_sdk/mind_sdk/config/mind_base_config.py
 recommend_model_sdk/mind_sdk/dataset/__init__.py
+recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
 recommend_model_sdk/mind_sdk/eval/__init_.py
 recommend_model_sdk/mind_sdk/eval/eval_operation.py
 recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
 recommend_model_sdk/mind_sdk/model/__init__.py
 recommend_model_sdk/mind_sdk/model/content_similar_model.py
+recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+recommend_model_sdk/mind_sdk/train/__init__.py
+recommend_model_sdk/mind_sdk/train/mind_dnn_click_predictor_train_tool.py
 recommend_model_sdk/proto_class/__init__.py
 recommend_model_sdk/proto_class/embedding_pb2.py
 recommend_model_sdk/recommend/__init__.py
 recommend_model_sdk/recommend/recommend_common_util.py
 recommend_model_sdk/recommend/recommend_tool.py
 recommend_model_sdk/recommend/time_weight_decay_tool.py
 recommend_model_sdk/resources/__init__.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 from recommend_model_sdk.mind_sdk.config.mind_base_config import MINDBaseConfig
 
 class MINDBehaviorsDataset(Dataset):
     """
     Load behaviors for evaluation, (user, time) pair as session
     """
     def __init__(self, behaviors_path,config):
+        """_summary_
+
+        Args:
+            behaviors_path (_type_): _description_ is behaviors.tsv. not behaviors_parsed.tsv
+            config (_type_): _description_
+
+        Raises:
+            ValueError: _description_
+        """
         super(MINDBehaviorsDataset, self).__init__()
         if isinstance(config,MINDBaseConfig) is False:
             raise ValueError("config is not MINDBaseConfig")
         self.__config = config
         self.behaviors = pd.read_table(behaviors_path,
                                        header=None,
                                        usecols=range(5),
```

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/model_management.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'bert'": "{'v1': {'embedding_dim': 384}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "bert": {
         "v1": {
             "active": true,
-            "embedding_dim": 768,
+            "embedding_dim": 384,
             "model_related_files": [],
             "model_related_files_public": {},
             "model_related_files_suffix": {},
             "mongodb_embedding_field": "bert_v1",
             "pg_embedding_mark_field": "bert_v1",
             "s3_bucket": "gpu-model-data"
         }
```

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/model_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.19/setup.py` & `bytetrade-recommend-model-sdk-0.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.19",
+    version="0.0.20",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

