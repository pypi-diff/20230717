# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.25.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.25.tar", last modified: Mon Jul 10 21:46:10 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.26.tar", last modified: Mon Jul 17 01:45:56 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.25.tar` & `bytetrade-recommend-model-sdk-0.0.26.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10528 2023-07-06 00:59:59.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17830 2023-07-03 09:21:19.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33393 2023-07-10 21:20:14.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-10 21:25:29.000000 bytetrade-recommend-model-sdk-0.0.25/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19923 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33591 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/README.md` & `bytetrade-recommend-model-sdk-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from recommend_model_sdk.mind_sdk.config.content_similar_config import ContentSimilarConfig
 from recommend_model_sdk.tools.aws_s3_tool import AWSS3Tool
 from recommend_model_sdk.recommend.recommend_common_util import RecommendCommonUtil
 
 
 from datetime import datetime
 import faiss
+
 import numpy as np
 import torch
 import torch.nn.functional as F
 
 
 
+
 class ContentSimilarModel:
     def __init__(self,config) -> None:
         if isinstance(config, ContentSimilarConfig) is False:
             raise ValueError("ContentSimilarModel is not model")
         self.__config = config
         self.__aws_tool = AWSS3Tool()
         self.__bucket_name = "gpu-model-data"
@@ -125,14 +127,94 @@
         if candidate_news_vector.shape[1] != self.__config.embedding_dim:
             raise ValueError("candidate_news_vector embedding dim is not right")
         if user_vec.shape[0] != self.__config.embedding_dim:
             raise ValueError("user_vec embedding dim is not right")       
         cos_sim = F.cosine_similarity(candidate_news_vector, user_vec, dim=1)
         return cos_sim
     
+class ContentSimilarMultipleEmbeddingModelRecall:
+    def __init__(self,base_document_id_to_list_embedding,config) -> None:
+        self.__recommend_common_util = RecommendCommonUtil()
+        self.__recommend_common_util.validate_base_document_id_to_item(base_document_id_to_list_embedding,True)
+        if isinstance(config, ContentSimilarConfig) is False:
+            raise ValueError("ContentSimilarModel is not model")
+        self.__config = config
+        set_shape = set()
+        list_current_embedding = list()
+        self.__base_length = len(base_document_id_to_list_embedding)
+        self.__base_index_to_document_id = dict()
+        self.__base_document_id_to_index_set = dict()
+        self.__common_tool = CommonTool()
+        self.__logger = self.__common_tool.get_logger()
+        current_index = 0
+        self.__base_document_id_to_created_at_tuple_list = list()
+        for current_document_id, current_embedding_info in base_document_id_to_list_embedding.items():
+            current_embedding_list = current_embedding_info["embedding"]
+            created_at = current_embedding_info["created_at"]
+            self.__base_document_id_to_created_at_tuple_list.append((current_document_id, created_at))
+            for current_embedding in current_embedding_list:
+                set_shape.add(current_embedding.shape)
+                list_current_embedding.append(current_embedding)
+                self.__base_index_to_document_id[current_index] = current_document_id
+                if current_document_id not in self.__base_document_id_to_index_set:
+                    self.__base_document_id_to_index_set[current_document_id] = set()
+                self.__base_document_id_to_index_set[current_document_id].add(current_index)
+                current_index = current_index + 1
+                
+        self.__base_document_id_to_created_at_tuple_list.sort(key=lambda tup: tup[1], reverse=True)
+        #self.__logger.debug(self.__base_document_id_to_created_at_tuple_list)
+        if len(set_shape) > 1:
+            raise ValueError(f'have different shape embeddings')
+        self.__embedding_shape = set_shape.pop()
+        self.__original_base_embedding = np.stack(list_current_embedding)
+        self.__normalized_base_embedding = np.copy(self.__original_base_embedding)
+        faiss.normalize_L2(self.__normalized_base_embedding)
+        # self.__original_base_embedding_index =  faiss.IndexFlatL2(self.__original_base_embedding)
+        self.__cosin_index = faiss.index_factory(self.__embedding_shape[0], "Flat", faiss.METRIC_INNER_PRODUCT)
+        self.__cosin_index.add(self.__normalized_base_embedding)
+    
+    
+
+            
+    def recall_empty(self,limit):
+        result_tuple_list = list()
+        for current_tuple in self.__base_document_id_to_created_at_tuple_list:
+            result_tuple_list.append((current_tuple[0],0.5))
+            if len(result_tuple_list) >= limit:
+                break
+        return result_tuple_list
+    
+    def recall(self,candidate_news_id_to_embedding_list,limit):
+        """
+        """
+        if len(candidate_news_id_to_embedding_list) < 1:
+            self.__logger.debug(f'candidate_news_id_to_embedding_list length samll than 1')
+            return self.recall_empty(limit)
+        self.__recommend_common_util.validate_candidate_document_id_to_item(candidate_news_id_to_embedding_list,self.__embedding_shape,True)
+        # todo 
+        # 
+        result_tuple_list = []
+        '''
+        faiss.normalize_L2(user_embedding)
+        consin_similar, nearest_indexes = self.__cosin_index.search(user_embedding, limit) # cosin similar,
+        result_tuple_list = list()
+        for current_similar,current_index in zip(consin_similar[0],nearest_indexes[0]):
+              current_weight = (2 - (1 - current_similar)) * 1.0 / 2
+              if current_index not in self.__base_index_to_document_id:
+                  self.__logger.debug(f'current_index {current_index} is not exist')
+                  continue
+              result_tuple_list.append((self.__base_index_to_document_id[current_index],current_weight))
+        
+        if len(result_tuple_list)  < 1:
+            self.__logger.debug('after complete result_tuple_list is small than 1')
+            return self.recall_empty(limit)
+        '''
+        return result_tuple_list
+              
+              
 
 
 class ContentSimilarModelRecall:
     def __init__(self,base_document_id_to_embedding,config) -> None:
         self.__recommend_common_util = RecommendCommonUtil()
         self.__recommend_common_util.validate_base_document_id_to_item(base_document_id_to_embedding)
         if isinstance(config, ContentSimilarConfig) is False:
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='embedding.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xb5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\"W\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feedb\x06proto3')
+  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xb5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feedb\x06proto3')
 )
 
 
 
 
 _ARTICLE = _descriptor.Descriptor(
   name='Article',
@@ -150,28 +150,73 @@
     _descriptor.FieldDescriptor(
       name='embeddings', full_name='Embedding.embeddings', index=3,
       number=4, type=2, cpp_type=6, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='subdocembeddings', full_name='Embedding.subdocembeddings', index=4,
+      number=5, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=203,
-  serialized_end=290,
+  serialized_start=204,
+  serialized_end=335,
+)
+
+
+_SUBDOCEMBEDDING = _descriptor.Descriptor(
+  name='SubdocEmbedding',
+  full_name='SubdocEmbedding',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='subdoc_index', full_name='SubdocEmbedding.subdoc_index', index=0,
+      number=1, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='embeddings', full_name='SubdocEmbedding.embeddings', index=1,
+      number=2, type=2, cpp_type=6, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=337,
+  serialized_end=396,
 )
 
 
 _LATESTPACKAGE = _descriptor.Descriptor(
   name='LatestPackage',
   full_name='LatestPackage',
   filename=None,
@@ -200,16 +245,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=292,
-  serialized_end=367,
+  serialized_start=398,
+  serialized_end=473,
 )
 
 
 _ARTICLEPACKAGE = _descriptor.Descriptor(
   name='ArticlePackage',
   full_name='ArticlePackage',
   filename=None,
@@ -231,16 +276,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=369,
-  serialized_end=413,
+  serialized_start=475,
+  serialized_end=519,
 )
 
 
 _EMBEDDINGPAKCAGE = _descriptor.Descriptor(
   name='EmbeddingPakcage',
   full_name='EmbeddingPakcage',
   filename=None,
@@ -262,16 +307,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=415,
-  serialized_end=465,
+  serialized_start=521,
+  serialized_end=571,
 )
 
 
 _FEED = _descriptor.Descriptor(
   name='Feed',
   full_name='Feed',
   filename=None,
@@ -356,16 +401,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=468,
-  serialized_end=661,
+  serialized_start=574,
+  serialized_end=767,
 )
 
 
 _FEEDPACKAGE = _descriptor.Descriptor(
   name='FeedPackage',
   full_name='FeedPackage',
   filename=None,
@@ -387,25 +432,27 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=663,
-  serialized_end=698,
+  serialized_start=769,
+  serialized_end=804,
 )
 
+_EMBEDDING.fields_by_name['subdocembeddings'].message_type = _SUBDOCEMBEDDING
 _LATESTPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _LATESTPACKAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _ARTICLEPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _EMBEDDINGPAKCAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _FEEDPACKAGE.fields_by_name['feeds'].message_type = _FEED
 DESCRIPTOR.message_types_by_name['Article'] = _ARTICLE
 DESCRIPTOR.message_types_by_name['Embedding'] = _EMBEDDING
+DESCRIPTOR.message_types_by_name['SubdocEmbedding'] = _SUBDOCEMBEDDING
 DESCRIPTOR.message_types_by_name['LatestPackage'] = _LATESTPACKAGE
 DESCRIPTOR.message_types_by_name['ArticlePackage'] = _ARTICLEPACKAGE
 DESCRIPTOR.message_types_by_name['EmbeddingPakcage'] = _EMBEDDINGPAKCAGE
 DESCRIPTOR.message_types_by_name['Feed'] = _FEED
 DESCRIPTOR.message_types_by_name['FeedPackage'] = _FEEDPACKAGE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
@@ -419,14 +466,21 @@
 Embedding = _reflection.GeneratedProtocolMessageType('Embedding', (_message.Message,), dict(
   DESCRIPTOR = _EMBEDDING,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:Embedding)
   ))
 _sym_db.RegisterMessage(Embedding)
 
+SubdocEmbedding = _reflection.GeneratedProtocolMessageType('SubdocEmbedding', (_message.Message,), dict(
+  DESCRIPTOR = _SUBDOCEMBEDDING,
+  __module__ = 'embedding_pb2'
+  # @@protoc_insertion_point(class_scope:SubdocEmbedding)
+  ))
+_sym_db.RegisterMessage(SubdocEmbedding)
+
 LatestPackage = _reflection.GeneratedProtocolMessageType('LatestPackage', (_message.Message,), dict(
   DESCRIPTOR = _LATESTPACKAGE,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:LatestPackage)
   ))
 _sym_db.RegisterMessage(LatestPackage)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from datetime import datetime
 import numpy as np
 
 class RecommendCommonUtil:
     def __init__(self) -> None:
         pass
     
-    def validate_base_document_id_to_item(self,base_document_id_to_embedding):
+    def validate_base_document_id_to_item(self,base_document_id_to_embedding,subdocument_embedding=False):
         if isinstance(base_document_id_to_embedding, dict) is False:
             raise ValueError("base_document_id_to_embedding is not dict")
         if len(base_document_id_to_embedding) < 1:
             raise ValueError('base_document_id_to_embedding length small than 1')
         for current_document_id, current_embedding_info in base_document_id_to_embedding.items():
             if isinstance(current_document_id, str) is False:
                 raise ValueError(f"current_document_id {current_document_id} is not str")
             if isinstance(current_embedding_info, dict) is False:
                 raise ValueError("current_embedding_info is not dict")
             if "embedding" not in current_embedding_info:
                 raise ValueError("embedding not in current_embedding_info")
-            current_embedding = current_embedding_info["embedding"]
-            # if isinstance(current_embedding,np.array)
-            if isinstance(current_embedding, np.ndarray) is False:
-                raise ValueError('there is embedding is not np.ndarray')
-            if current_embedding.dtype != np.float32:
-                raise ValueError("embedding_value is not float32")
+            
+            if subdocument_embedding is False:   
+                current_embedding = current_embedding_info["embedding"]
+                # if isinstance(current_embedding,np.array)
+                if isinstance(current_embedding, np.ndarray) is False:
+                    raise ValueError('there is embedding is not np.ndarray')
+                if current_embedding.dtype != np.float32:
+                    raise ValueError("embedding_value is not float32")
+            else:
+                current_embedding_list = current_embedding_info["embedding"]
+                if isinstance(current_embedding_list,list) is False:
+                    raise ValueError("current_embedding_list is not list")
+                for current_embedding in current_embedding_list:
+                    if isinstance(current_embedding, np.ndarray) is False:
+                        raise ValueError('there is embedding is not np.ndarray')
+                    if current_embedding.dtype != np.float32:
+                        raise ValueError("embedding_value is not float32")
+                        
             if "created_at" not in current_embedding_info:
                 raise ValueError("created_at not in current_embedding_info")
             created_at = current_embedding_info["created_at"]
             if isinstance(created_at, datetime) is False:
                 raise ValueError("created_at is not datetime")
     
-    def validate_candidate_document_id_to_item(self,document_id_to_document_info,base_embedding_shape):
+    def validate_candidate_document_id_to_item(self,document_id_to_document_info,base_embedding_shape,subdocument_embedding=False):
         if isinstance(document_id_to_document_info,dict) is False:
             raise ValueError('document_id_to_document_info is not dict')
         if isinstance(base_embedding_shape,tuple) is False:
             raise ValueError('base_embedding_shape is not tuple')
         for current_element in base_embedding_shape:
             if isinstance(current_element,int) is False:
                 raise ValueError("current_element in tuple is not int")
@@ -42,15 +54,28 @@
         for current_document_id, current_embedding_info in document_id_to_document_info.items():
             if isinstance(current_document_id, str) is False:
                 raise ValueError("current_document_id is not str")
             if isinstance(current_embedding_info, dict) is False:
                 raise ValueError('current_embedding_info is not dict')
             if "embedding" not in current_embedding_info:
                 raise ValueError("embedding not in current_embedding_info")
-            current_embedding = current_embedding_info["embedding"]
-            if isinstance(current_embedding, np.ndarray) is False:
-                raise ValueError('there is embedding is not np.ndarray')
-            if current_embedding.dtype != np.float32:
-                raise ValueError("embedding_value is not float32")
-            if current_embedding.shape != base_embedding_shape:
-                raise ValueError("embedding shape is not equal to shape in base embedding")
+            
+            if subdocument_embedding is False:
+                current_embedding = current_embedding_info["embedding"]
+                if isinstance(current_embedding, np.ndarray) is False:
+                    raise ValueError('there is embedding is not np.ndarray')
+                if current_embedding.dtype != np.float32:
+                    raise ValueError("embedding_value is not float32")
+                if current_embedding.shape != base_embedding_shape:
+                    raise ValueError("embedding shape is not equal to shape in base embedding")
+            else:
+                current_embedding_list = current_embedding_info["embedding"]
+                if isinstance(current_embedding_list,list) is False:
+                    raise ValueError("current_embedding_list is not list")
+                for current_embedding in current_embedding_list:
+                    if isinstance(current_embedding, np.ndarray) is False:
+                        raise ValueError('there is embedding is not np.ndarray')
+                    if current_embedding.dtype != np.float32:
+                        raise ValueError("embedding_value is not float32")
+                    if current_embedding.shape != base_embedding_shape:
+                        raise ValueError("embedding shape is not equal to shape in base embedding")
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/model_management.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'bert'": "{'v2': OrderedDict([('mongodb_embedding_field', 'bert_v2'), "*

 * *           "('pg_embedding_mark_field', 'bert_v2'), ('s3_bucket', 'gpu-model-data'), "*

 * *           "('model_related_files', []), ('model_related_files_suffix', OrderedDict()), "*

 * *           "('model_related_files_public', OrderedDict()), ('active', True), "*

 * *           '(\'sentence_transformer\', OrderedDict([(\'model_name\', "\'all-MiniLM-L6-v2")])), '*

 * *           "('character_text_splitter', OrderedDict([('chunk_size', 100), ('chunk_ove […]*

```diff
@@ -5,14 +5,31 @@
             "embedding_dim": 384,
             "model_related_files": [],
             "model_related_files_public": {},
             "model_related_files_suffix": {},
             "mongodb_embedding_field": "bert_v1",
             "pg_embedding_mark_field": "bert_v1",
             "s3_bucket": "gpu-model-data"
+        },
+        "v2": {
+            "active": true,
+            "character_text_splitter": {
+                "chunk_overlap": 10,
+                "chunk_size": 100
+            },
+            "embedding_dim": 384,
+            "model_related_files": [],
+            "model_related_files_public": {},
+            "model_related_files_suffix": {},
+            "mongodb_embedding_field": "bert_v2",
+            "pg_embedding_mark_field": "bert_v2",
+            "s3_bucket": "gpu-model-data",
+            "sentence_transformer": {
+                "model_name": "'all-MiniLM-L6-v2"
+            }
         }
     },
     "word2vec_google": {
         "v1": {
             "active": false,
             "embedding_dim": 300,
             "model_related_files": [
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/model_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,21 @@
             if isinstance(current_file_name_public,bool) is False:
                 raise ValueError(F"current_file_name {current_file_name} current_file_name_public is  not bool")
 
     def bert_calculate_embedding(self,model_name,model_version,dict_document):
         self.valid_model_name_and_version(model_name,model_version)
         self.valid_infer_document(dict_document)
         bert_embedding_tool = BertEmbedding()
-        id_to_infer_result = dict()
-        for current_id, current_text in dict_document.items():
-            id_to_infer_result[current_id] = bert_embedding_tool.calculate_embedding(current_text)      
-        return id_to_infer_result 
+        if model_version == "v1":
+            return bert_embedding_tool.calculate_batch_document_embeddings(dict_document)
+        elif model_version == "v2":
+            result_dict = dict()
+            for current_entry_id,current_document  in dict_document.items():
+                result_dict[current_entry_id] = bert_embedding_tool.calculate_document_embeddings_with_split_document(current_document)
+            return result_dict
         
     def __validate_model_management_file(self,path):
         if isinstance(path,str) is False:
             raise ValueError(f"path {path} is not str")
         if os.path.exists(path) is False:
             raise ValueError(f"model management file {path} is not exist")
         model_management_dict = self.__common_tool.read_json(path)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.25/setup.py` & `bytetrade-recommend-model-sdk-0.0.26/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.25",
+    version="0.0.26",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3"
```

