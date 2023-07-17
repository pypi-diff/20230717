# Comparing `tmp/molgraph-0.5.4.tar.gz` & `tmp/molgraph-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.4.tar", last modified: Mon Jul 17 13:47:02 2023, max compression
+gzip compressed data, was "molgraph-0.5.5.tar", last modified: Mon Jul 17 15:21:04 2023, max compression
```

## Comparing `molgraph-0.5.4.tar` & `molgraph-0.5.5.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.4/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6765 2023-07-17 13:47:02.666568 molgraph-0.5.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     6045 2023-07-17 13:46:46.000000 molgraph-0.5.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.4/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.4/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.4/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.4/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.4/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.4/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.4/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.4/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.4/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.4/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.4/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.4/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16276 2023-07-17 07:54:08.000000 molgraph-0.5.4/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.4/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.4/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.4/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11154 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11974 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20628 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.4/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.4/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.4/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.4/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.4/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.4/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.4/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.4/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.4/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.4/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.4/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6765 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 13:47:02.666568 molgraph-0.5.4/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.4/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.5/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-17 15:21:04.196512 molgraph-0.5.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5998 2023-07-17 15:20:50.000000 molgraph-0.5.5/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.5/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.5/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.5/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.5/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.5/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.5/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.5/molgraph/chemistry/vis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/internal.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.5/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12927 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11735 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9923 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11863 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10845 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17229 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.5/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10192 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11264 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10555 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.5/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9981 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10871 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26003 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.5/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16323 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14494 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.5/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10772 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.5/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3455 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3031 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.5/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11065 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4593 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9737 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4258 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6688 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20500 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.5/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6405 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4687 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3332 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6274 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5369 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.5/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2449 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.5/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.5/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6987 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7101 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10961 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6905 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.5/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23586 2023-07-17 14:06:48.000000 molgraph-0.5.5/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13073 2023-07-17 14:06:52.000000 molgraph-0.5.5/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.5/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.5/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1877 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    51973 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3329 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 15:21:04.196512 molgraph-0.5.5/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1418 2023-07-17 15:20:50.000000 molgraph-0.5.5/setup.py
```

### Comparing `molgraph-0.5.4/LICENSE` & `molgraph-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/PKG-INFO` & `molgraph-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.4
+Version: 0.5.5
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -72,17 +72,16 @@
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
-    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **TensorFlow** (version >= 2.10.0 recommended)
     - **RDKit** (version >= 2022.3.3 recommended)
-    - **NumPy** (version >= 1.21.2 recommended)
     - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
```

### Comparing `molgraph-0.5.4/README.md` & `molgraph-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,16 @@
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
-    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **TensorFlow** (version >= 2.10.0 recommended)
     - **RDKit** (version >= 2022.3.3 recommended)
-    - **NumPy** (version >= 1.21.2 recommended)
     - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
```

### Comparing `molgraph-0.5.4/molgraph/_filter_warnings.py` & `molgraph-0.5.5/molgraph/_filter_warnings.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,19 @@
         'Encoding a StructuredValue with type '
         'molgraph.tensors.graph_tensor.GraphTensorSpec; '
         'loading this StructuredValue will require that this '
         'type be imported and registered.*'
     )
 )
 
+filterwarnings('ignore',
+    message='Converting sparse IndexedSlices.*' +
+            'to a dense Tensor of unknown shape. ' +
+            'This may consume a large amount of memory.')
+
 absl.logging.set_verbosity(absl.logging.ERROR)
 
 #logging.getLogger('tensorflow').setLevel(logging.ERROR)
 logging.basicConfig(level=logging.INFO, format='%(message)s')
 
 def ignore_gradient_warning(record):
     # If e.g. `update_edge_features` is passed to the last GAT layer, edge
```

### Comparing `molgraph-0.5.4/molgraph/applications/graph_transformer.py` & `molgraph-0.5.5/molgraph/applications/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/__init__.py` & `molgraph-0.5.5/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.5/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.5/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.5/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.5/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.5/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.5/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/encoders.py` & `molgraph-0.5.5/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/features.py` & `molgraph-0.5.5/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.5/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/ops.py` & `molgraph-0.5.5/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/chemistry/vis.py` & `molgraph-0.5.5/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/layers/__init__.py` & `molgraph-0.5.5/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from keras import constraints
 
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers.attentional.gat_conv import GATConv
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class AttentiveFPConv(GATConv):
 
     '''Node message passing step ("Atom embedding") of AttentiveFP.
 
     `AttentiveFPConv` inherits from `GATConv` and adds a GRU update. Also
     performs a initial linear transformation on node features if needed or desired.
```

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/gat_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from keras import constraints
 from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops 
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GATConv(gnn_layer.GNNLayer):
 
     '''Multi-head graph attention layer (GAT).
 
     The implementation is based on Velickovic et al. (2018) [#]_ and
     Dwivedi et al. (2022) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from keras import constraints
 from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GatedGCNConv(gnn_layer.GNNLayer):
 
     '''Gated graph convolutional layer (GatedGCN).
 
     Implementation is based on Dwivedi et al. (2022) [#]_, Bresson et al. (2019) [#]_,
     Joshi et al. (2019) [#]_, and Bresson et al. (2018) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/gatv2_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from keras import constraints
 from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GATv2Conv(gnn_layer.GNNLayer):
 
     '''Multi-head graph attention (v2) layer (GATv2).
 
     The implementation is based on Brody et al. (2021) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/gmm_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from keras import constraints
 from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GMMConv(gnn_layer.GNNLayer):
 
     '''Multi-head graph gaussian mixture layer (MoNet)
 
     Implementation is based on Dwivedi et al. (2022) [#]_ and 
     Monti et al. (2016) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.5/molgraph/layers/attentional/gt_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 from keras import activations
 from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
+
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GTConv(gnn_layer.GNNLayer):
 
     '''Graph transformer layer
 
     Implementation is based on Dwivedi et al. (2021) [#]_.
 
     Alias: ``GraphTransformerConv``
@@ -129,15 +132,14 @@
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
         **kwargs: Valid (optional) keyword arguments are:
 
             *   `name` (str): Name of the layer instance.
-            *   `name` (str): Name of the layer instance.
             *   `update_step` (tf.keras.layers.Layer): Applies post-processing 
                 step on the output (produced by `_call`). If passed, 
                 `normalization`, `residual`, `activation` and `dropout` 
                 parameters will be ignored. If None, a default post-processing 
                 step will be used (taking into consideration the aforementioned 
                 parameters). Default to None.
             *   `use_edge_features`: Whether or not to use edge features. 
@@ -174,32 +176,35 @@
         bias_constraint: Optional[constraints.Constraint] = None,
         **kwargs
     ):
         kwargs['update_edge_features'] = (
             kwargs.get('update_edge_features', True) and 
             kwargs.get('use_edge_features', True)
         )
-
-        super().__init__(
-            units=units,
-            update_step=_FeedForwardNetwork(
+        update_step = kwargs.pop(
+            'update_step',
+            _FeedForwardNetwork(
                 units=units,
                 normalization=normalization,
                 activation=activation,
                 residual=residual,
                 dropout=dropout,
                 use_bias=use_bias,
                 kernel_initializer=kernel_initializer,
                 bias_initializer=bias_initializer,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
                 activity_regularizer=activity_regularizer,
                 kernel_constraint=kernel_constraint,
                 bias_constraint=bias_constraint,
-            ),
+            )
+        )
+        super().__init__(
+            units=units,
+            update_step=update_step,
             residual=residual,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
@@ -282,14 +287,15 @@
             'merge_mode': self.merge_mode,
             'self_projection': self.apply_self_projection,
         }
         base_config.update(config)
         return base_config
 
 
+@register_keras_serializable(package='molgraph')
 class _FeedForwardNetwork(layers.Layer):
 
     'Feed-forward network (FFN) of the graph transformer layer.'
 
     def __init__(
         self, 
         units: Optional[int] = None,
```

### Comparing `molgraph-0.5.4/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.5/molgraph/layers/convolutional/gcn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from keras import regularizers
 from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GCNConv(gnn_layer.GNNLayer):
 
     """Graph convolutional layer (GCN).
 
     Implementation is based on Kipf et al. (2017) [#]_, Dwivedi et al. (2022) [#]_,
     and, for RGCN, Schlichtkrull et al. (2017) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.5/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from keras import regularizers
 from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GCNIIConv(gnn_layer.GNNLayer):
 
     '''Graph convolutional 'via Initial residual and Identity mapping' layer (GCNII).
 
     Implementation is based on Chen et al. (2020) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.5/molgraph/layers/convolutional/gin_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 from keras import activations
 from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
+
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GINConv(gnn_layer.GNNLayer):
 
     '''Graph isomorphism convolution layer (GIN).
 
     Implementation based on Dwivedi et al. (2022) [#]_, Xu et al. (2019) [#]_, 
     and Hu et al. (2020) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.5/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from keras import activations
 from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GraphSageConv(gnn_layer.GNNLayer):
 
     '''Graph sage convolution layer (GraphSage)
 
     Implementation is based on Hamilton et al. (2018) [#]_ and
     Dwivedi et al. (2022) [#]_.
```

### Comparing `molgraph-0.5.4/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.5/molgraph/layers/geometric/dtnn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from keras import regularizers
 from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 from molgraph.layers.geometric import radial_basis
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class DTNNConv(gnn_layer.GNNLayer):
 
     """Deep Tensor Neural Network (DTNN).
 
     Implementation is based on Schütt et al. (2017a) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.5/molgraph/layers/geometric/gcf_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 import numpy as np
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 from molgraph.layers.geometric import radial_basis
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GCFConv(gnn_layer.GNNLayer):
 
     """(Graph) continuous filter convolution layer ((G)CFConv).
 
     Implementation is based on Schütt et al. (2017b) [#]_.
 
     Operates on 3D molecular graphs (encoding distance geometry).
```

### Comparing `molgraph-0.5.4/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.5/molgraph/layers/geometric/radial_basis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+
+@register_keras_serializable(package='molgraph')
 class RadialBasis(keras.layers.Layer):
 
     def __init__(
         self,
         distance_min: float = -1.0,
         distance_max: float = 18.0,
         distance_granularity: float = 0.1,
```

### Comparing `molgraph-0.5.4/molgraph/layers/gnn_layer.py` & `molgraph-0.5.5/molgraph/layers/gnn_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 
 from warnings import warn
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 from typing import List
-from typing import Tuple
 from typing import Type
-from typing import TypeVar
+
+from molgraph.internal import register_keras_serializable 
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
-from molgraph.layers import gnn_ops
-
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GNNLayer(layers.Layer, metaclass=abc.ABCMeta):
 
     '''Base layer for the built-in GNN layers. 
     
     Can also be used to create new GNN layers.
     
     **Example usage:**
@@ -508,14 +506,17 @@
                 layer instance. The config is usually obtained from 
                 ``get_config()`` of another layer instance (of the same class).
         
         Returns:
             A layer instance.
         '''
         graph_tensor_spec = config.pop('graph_tensor_spec', None)
+        update_step = config.pop('update_step')
+        config['update_step'] = (
+            None if update_step is None else layers.deserialize(update_step))
         layer = cls(**config)
         if graph_tensor_spec is None:
             warn(
                 (
                  'A GraphTensorSpec could not be obtained from the config, '
                  'indicating that the layer from which the config was '
                  'previously obtained was not yet built. Proceeding to '
```

### Comparing `molgraph-0.5.4/molgraph/layers/gnn_ops.py` & `molgraph-0.5.5/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.5/molgraph/layers/message_passing/edge_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 from typing import Type
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeConv(tf.keras.layers.Layer):
 
     '''Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#]_ like models.
 
     **Important:**
 
     As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
```

### Comparing `molgraph-0.5.4/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.5/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 import math
 
 from typing import Optional
 from typing import Callable
 from typing import Union
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class MPNNConv(gnn_layer.GNNLayer):
 
     """Message passing neural network layer (MPNN)
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to Gilmer
     et al. this implementation does not use weight tying by default; for neither the 
     message function nor the update function. Furthermore, instead of the GRU-based
```

### Comparing `molgraph-0.5.4/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.5/molgraph/layers/positional_encoding/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from keras import constraints
 from keras import activations
 
 from typing import Union
 from typing import Callable
 from typing import Optional
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class LaplacianPositionalEncoding(layers.Layer):
 
     '''Laplacian positional encoding.
 
     Implementation based on Dwivedi et al. (2021) [#]_ and Belkin et al. (2003) [#]_.
 
     **Example:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.5/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class DotProductIncident(keras.layers.Layer):
     '''Performs dot product on the incident node features.
 
     Useful for e.g., edge and link classification.
 
     **Example:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.5/molgraph/layers/postprocessing/extract_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class ExtractField(keras.layers.Layer):
     '''Extract specific field of ``GraphTensor``.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
```

### Comparing `molgraph-0.5.4/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.5/molgraph/layers/postprocessing/gather_incident.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GatherIncident(keras.layers.Layer):
     '''Gathers incident node features.
 
     Useful for e.g., downstream edge and link classification.
 
     **Example:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/center_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 from tensorflow import keras
 from keras import layers
 
 import numpy as np
 
 from typing import Optional
 
-from molgraph.tensors.graph_tensor import GraphTensor
-
-try:
-    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
-except AttributeError:
-    PreprocessingLayer = layers.PreprocessingLayer
+from molgraph.internal import register_keras_serializable 
+from molgraph.internal import PreprocessingLayer
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class CenterScaling(PreprocessingLayer):
 
     '''Centering.
 
     Specify, as keyword argument only,
     ``CenterScaling(feature='node_feature')`` to perform center scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
@@ -316,20 +313,20 @@
             'mean': _listify_tensors(self.mean),
             'feature': self.feature,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeCenterScaling(CenterScaling):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeCenterScaling(CenterScaling):
     feature = 'edge_feature'
 
 
 def _listify_tensors(x):
     if tf.is_tensor(x):
         x = x.numpy()
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeDropout(keras.layers.Layer):
     '''Randomly dropping nodes from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -74,15 +76,15 @@
 
     def get_config(self):
         config = {'rate': self.rate,}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeDropout(NodeDropout):
     '''Randomly dropping edges from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 from keras import regularizers
 from keras import constraints
 
 from typing import Optional
 from typing import Union
 from typing import List
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EmbeddingLookup(layers.StringLookup):
 
     '''A loookup layer and embedding layer in combination.
 
     Specify, as keyword argument only,
     ``EmbeddingLookup(feature='node_feature', ...)`` to perform embedding lookup
     on the ``node_feature`` component of the ``GraphTensor``, or,
@@ -242,15 +244,15 @@
                 self.embeddings_regularizer),
             'embeddings_constraint': constraints.serialize(
                 self.embeddings_constraint),
         })
         return base_config
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeEmbeddingLookup(EmbeddingLookup):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeEmbeddingLookup(EmbeddingLookup):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/masking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class FeatureMasking(keras.layers.Layer):
     '''Randomly masking node or edge features from the graph.
 
     Important: Requires node (or edge) features to be tokenized. I.e., requires 
     the `GraphTensor` instance to be produced from `molgraph.chemistry.Tokenizer` 
     instead of `molgraph.chemistry.Tokenizer`.
 
@@ -112,15 +114,15 @@
             'rate': self.rate, 
             'mask_token': self.mask_token
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeFeatureMasking(FeatureMasking):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeFeatureMasking(FeatureMasking):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 
 import numpy as np
 
 from typing import Tuple
 from typing import Optional
 from typing import Tuple
 
+from molgraph.internal import register_keras_serializable 
+from molgraph.internal import PreprocessingLayer
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
-try:
-    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
-except AttributeError:
-    PreprocessingLayer = layers.PreprocessingLayer
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class MinMaxScaling(PreprocessingLayer):
 
     '''Min-max scaling between a specified range.
 
     Specify, as keyword argument only,
     ``MinMaxScaling(feature='node_feature')`` to perform min-max scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
@@ -324,20 +323,20 @@
         if self.variance_threshold is not None:
             shape = input_spec.shape[:-1]
             shape += (len(self.keep),)
             return tf.TensorSpec(shape, dtype=tf.float32)
         return input_spec
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeMinMaxScaling(MinMaxScaling):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeMinMaxScaling(MinMaxScaling):
     feature = 'edge_feature'
 
 
 def _listify_tensors(x):
     if tf.is_tensor(x):
         x = x.numpy()
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from tensorflow import keras
 from keras import layers
 from keras import initializers
 from keras import regularizers
 from keras import constraints
 from keras import activations
 
+from molgraph.internal import register_keras_serializable 
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class FeatureProjection(layers.Layer):
 
     '''Feature projection via dense layer.
 
     Specify, as keyword argument only,
     ``FeatureProjection(feature='node_feature')`` to perform a projection
     of the ``node_feature`` component of the ``GraphTensor``, or,
@@ -154,15 +155,15 @@
             'kernel_constraint': constraints.serialize(self.kernel_constraint),
             'bias_constraint': constraints.serialize(self.bias_constraint),
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeFeatureProjection(FeatureProjection):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeFeatureProjection(FeatureProjection):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.4/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.5/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 from keras import initializers
 
 import numpy as np
 
 from typing import Optional
 from typing import Union
 
-from molgraph.tensors.graph_tensor import GraphTensor
-
-try:
-    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
-except AttributeError:
-    PreprocessingLayer = layers.PreprocessingLayer
+from molgraph.internal import register_keras_serializable 
+from molgraph.internal import PreprocessingLayer
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class StandardScaling(PreprocessingLayer):
 
     '''Standard scaling, via centering and standardization.
 
     Specify, as keyword argument only,
     ``StandardScaling(feature='node_feature')`` to perform standard scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
@@ -391,15 +388,15 @@
             'variance': _listify_tensors(self.variance),
             'feature': self.feature,
             'variance_threshold': self.variance_threshold}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class VarianceThreshold(StandardScaling):
 
     '''Variance thresholding.
 
     Uses the ``StandardScaling`` layer but ignores the normalization when
     calling the layer.
 
@@ -563,30 +560,30 @@
 
         if self.variance_threshold is not None:
             feature = tf.gather(feature, self.keep, axis=gather_axis)
 
         return data.update({self.feature: feature})
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeStandardScaling(StandardScaling):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeStandardScaling(StandardScaling):
     feature = 'edge_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeVarianceThreshold(VarianceThreshold):
     feature = 'node_feature'
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class EdgeVarianceThreshold(VarianceThreshold):
     feature = 'edge_feature'
 
 
 def _listify_tensors(x):
     if tf.is_tensor(x):
         x = x.numpy()
```

### Comparing `molgraph-0.5.4/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.5/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 from typing import Tuple
 from typing import TypeVar
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.layers.attentional.gat_conv import GATConv
-from molgraph.tensors.graph_tensor import GraphTensor
 
-Config = TypeVar('Config', bound=dict)
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class AttentiveFPReadout(tf.keras.layers.Layer):
 
     '''Readout step ("Molecule embedding") of AttentiveFP.
 
     For a complete implementation of AttentiveFP, add a number of `AttentiveFPConv` 
     steps before `AttentiveFPReadout` (see below).
 
@@ -118,15 +119,15 @@
                 tensor=tensor.node_feature, 
                 indices=virtual_node_indices[:, tf.newaxis], 
                 updates=virtual_node_state)
             tensor = tensor.update({'node_feature': node_feature_updated})
         
         return self.final_node_projection(virtual_node_state)
 
-    def get_config(self) -> Config:
+    def get_config(self) -> dict:
         config = super().get_config()
         config.update({
             'steps': self.steps, 
             'message_step': tf.keras.layers.serialize(self.message_step),
             'update_step': tf.keras.layers.serialize(self.update_step),
             'final_node_projection': tf.keras.layers.serialize(
                 self.final_node_projection)
```

### Comparing `molgraph-0.5.4/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.5/molgraph/layers/readout/node_readout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NodeReadout(keras.layers.Layer):
 
     '''Aggregates edge states to associated nodes.
 
     **Examples:**
 
     >>> graph_tensor = molgraph.GraphTensor(
```

### Comparing `molgraph-0.5.4/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.5/molgraph/layers/readout/segment_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 
-from molgraph.tensors.graph_tensor import GraphTensor
+from molgraph.internal import register_keras_serializable 
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class SegmentPoolingReadout(layers.Layer):
 
     '''Segmentation pooling for graph readout.
 
     Alias: ``Readout``
 
     **Example:**
```

### Comparing `molgraph-0.5.4/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.5/molgraph/layers/readout/set_gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 
 from typing import Tuple
 
-from molgraph.tensors.graph_tensor import GraphTensor
+from molgraph.internal import register_keras_serializable 
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class SetGatherReadout(layers.Layer):
 
     '''Set-to-set layer for graph readout.
 
     Implementation based on Gilmer et al. (2017) [#]_ and Vinyals et al. (2016) [#]_.
 
     **Example:**
@@ -127,15 +128,15 @@
         config = {
             'steps': self.steps,
         }
         base_config.update(config)
         return base_config
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NoInputLSTMCell(layers.Layer):
 
     'Custom LSTM Cell that takes no input'
 
     def build(self, input_shape):
         memory_state_dim = input_shape[0][-1]
         carry_state_dim = input_shape[1][-1]
```

### Comparing `molgraph-0.5.4/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.5/molgraph/layers/readout/transformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 from keras import activations
 
-from typing import Tuple
 from typing import Union
 from typing import Callable
 
-from molgraph.tensors.graph_tensor import GraphTensor
+from molgraph.internal import register_keras_serializable 
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class TransformerEncoderReadout(layers.Layer):
 
     '''Transformer encoder layer for graph readout.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
```

### Comparing `molgraph-0.5.4/molgraph/losses/link_losses.py` & `molgraph-0.5.5/molgraph/losses/link_losses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
 
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+
+@register_keras_serializable(package='molgraph.losses')
 class LinkBinaryCrossentropy(keras.losses.BinaryCrossentropy):
 
     def __init__(
         self,
         from_logits=True,
         label_smoothing=0.,
         axis=-1,
@@ -29,15 +31,15 @@
         y_pred = tf.concat([
             tf.ones_like(positive_score), tf.zeros_like(negative_score)
         ], axis=0)
         return super().call(y_pred, y_true)
 
 
 # TODO: Make it work for len(y_true) != len(y_pred)
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveMarginLoss(keras.losses.Loss):
 
     def __init__(
         self,
         margin=1.,
         reduction=keras.losses.Reduction.AUTO,
         name='link_contrastive_margin_loss',
@@ -51,15 +53,15 @@
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'margin': self.margin})
         return base_config
 
 
 # TODO: Make it work for len(y_true) != len(y_pred)
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveBinaryCrossentropy(keras.losses.Loss):
 
     def __init__(
         self,
         reduction=keras.losses.Reduction.AUTO,
         name='link_contrastive_bce_loss',
     ):
```

### Comparing `molgraph-0.5.4/molgraph/losses/masked_losses.py` & `molgraph-0.5.5/molgraph/losses/masked_losses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 
+from molgraph.internal import register_keras_serializable 
+
 
 class MaskedLoss(keras.losses.Loss):
 
     'Base class for masked losses.'
 
     def __init__(
         self,
@@ -49,15 +51,15 @@
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'reduction': self._reduction})
         return base_config
 
 
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class MaskedBinaryCrossentropy(MaskedLoss):
     
     '''Masked binary crossentropy loss. 
     
     Useful for multi-label classification with missing labels.
     '''
 
@@ -102,15 +104,15 @@
             'gamma': self._gamma,
             'from_logits': self._from_logits,
             'label_smoothing': self._label_smoothing,
         })
         return base_config
 
 
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class MaskedHuber(MaskedLoss):
 
     '''Masked huber loss. 
     
     Useful for multi-label regression with missing labels.
     '''
 
@@ -142,29 +144,29 @@
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'delta': self._delta})
         return base_config
 
 
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class MaskedMeanSquaredError(MaskedLoss):
 
     '''Masked mean squared error loss. 
     
     Useful for multi-label regression with missing labels.
     '''
 
     def call(self, y_true: tf.Tensor, y_pred: tf.Tensor) -> tf.Tensor:
         y_pred = tf.convert_to_tensor(y_pred)
         y_true = tf.cast(y_true, y_pred.dtype)
         return tf.math.squared_difference(y_pred, y_true)
 
 
-@keras.saving.register_keras_serializable(package='molgraph.losses')
+@register_keras_serializable(package='molgraph.losses')
 class MaskedMeanAbsoluteError(MaskedLoss):
 
     '''Masked mean absolute error loss. 
     
     Useful for multi-label regression with missing labels.
     '''
```

### Comparing `molgraph-0.5.4/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.5/molgraph/metrics/masked_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.metrics.mean_relative_error import MeanRelativeError
 
 
-@keras.saving.register_keras_serializable(package='molgraph.metrics')
+@register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanSquaredError(keras.metrics.MeanSquaredError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.saving.register_keras_serializable(package='molgraph.metrics')
+@register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanAbsoluteError(keras.metrics.MeanAbsoluteError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.saving.register_keras_serializable(package='molgraph.metrics')
+@register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanRelativeError(MeanRelativeError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.saving.register_keras_serializable(package='molgraph.metrics')
+@register_keras_serializable(package='molgraph.metrics')
 class MaskedRootMeanSquaredError(keras.metrics.RootMeanSquaredError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
```

### Comparing `molgraph-0.5.4/molgraph/models/__init__.py` & `molgraph-0.5.5/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/models/dgin.py` & `molgraph-0.5.5/molgraph/models/dgin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import tensorflow as tf
 from tensorflow import keras
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.message_passing.edge_conv import EdgeConv
 from molgraph.layers.convolutional.gin_conv import GINConv
 from molgraph.layers.readout.node_readout import NodeReadout
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class DGIN(keras.layers.Layer):
 
     '''Directed graph isomorphism network (DGIN).
 
     Implementation based on Wieder et al. (2021) [#]_. 
     
     **Important:**
```

### Comparing `molgraph-0.5.4/molgraph/models/dmpnn.py` & `molgraph-0.5.5/molgraph/models/dmpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import tensorflow as tf
 from tensorflow import keras
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.message_passing.edge_conv import EdgeConv
 from molgraph.layers.message_passing.mpnn_conv import MPNNConv
 from molgraph.layers.readout.node_readout import NodeReadout
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class DMPNN(keras.layers.Layer):
 
     '''Directed message passing neural network (DMPNN).
 
     Implementation based on Wieder et al. (2021) [#]_, though adding several
     `MPNNConv` layers for the node message passing (similar to how DGIN adds 
     several `GINConv` layers for the node message passsing).
```

### Comparing `molgraph-0.5.4/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.5/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.5/molgraph/models/interpretability/saliency.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 from typing import Optional
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-NOT_IMPLEMENTED_ERROR_MESSAGE = (
-    "{} only makes predictions (call model.predict instead)")
-
-
 def automatically_infer_input_signature(func):
     def call(
         self: 'SaliencyMapping', 
         x: GraphTensor, 
         y: Optional[tf.Tensor] = None
     ) -> Union[tf.Tensor, tf.RaggedTensor]:
         if not self._built:
```

### Comparing `molgraph-0.5.4/molgraph/models/mpnn.py` & `molgraph-0.5.5/molgraph/models/mpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 from typing import Tuple
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.message_passing.mpnn_conv import message_step
 
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class MPNN(keras.layers.Layer):
 
     '''Message passing neural network (MPNN) with weight tying.
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to
     ``MPNNConv``, which performs a single step of message passing, ``MPNN``
     performs n-steps of message passing. Furthermore, the weights are shared
```

### Comparing `molgraph-0.5.4/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.5/molgraph/models/pretraining/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 
 from typing import Optional
 from typing import Any
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
+
 from molgraph.layers.postprocessing.dot_product_incident import DotProductIncident
+
 from molgraph.losses.link_losses import LinkBinaryCrossentropy
 
     
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GraphAutoEncoder(keras.Model):
     '''Graph AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
         encoder (tf.keras.layers.Layer):
             The encoder part of the autoencoder. The encoder could be
             any of the graph neural neural network layers provided by
@@ -300,15 +304,15 @@
             `GraphTensor` as well as decoded `GraphTensor`s.
         '''
         return super().predict(
             x=x, batch_size=batch_size, *args, **kwargs)
 
       
 # TODO: instead of beta_initial/end/incr, pass a scheduler?
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class GraphVariationalAutoEncoder(GraphAutoEncoder):
     '''Graph Variational AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
         encoder (tf.keras.layers.Layer):
             The encoder part of the autoencoder. The encoder could be
             any of the graph neural neural network layers provided by
@@ -507,15 +511,15 @@
         config = super().get_config()
         config.update({
             'beta_initial': self.beta_initial,
             'beta_end': self.beta_end,
             'beta_incr': self.beta_incr
         })
 
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NaiveNegativeGraphSampler(layers.Layer):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     It is a "naive" implementation as it simply just shuffles `edge_dst` of
     the `GraphTensor` instance, without considering that the resulting
     `edge_dst` and `edge_src` pair could be a positive (correct) edge.
@@ -544,15 +548,15 @@
         return tensor.__class__(**data)
     
     def get_config(self):
         config = super().get_config()
         config.update({'k': self.k})
         return config
     
-@keras.saving.register_keras_serializable(package='molgraph')
+@register_keras_serializable(package='molgraph')
 class NegativeGraphSampler(NaiveNegativeGraphSampler):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     This is a "non-naive" implementation as it makes sure that the original
     (positive) edges do not exist in the set of negative edges.
```

### Comparing `molgraph-0.5.4/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.5/molgraph/models/pretraining/masked_modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import keras
 from keras import layers
 
 from typing import Optional
 from typing import List
 
+from molgraph.internal import register_keras_serializable 
+
 from molgraph.tensors.graph_tensor import GraphTensor
 
 from molgraph.layers.preprocessing.masking import FeatureMasking
 from molgraph.layers.preprocessing.embedding_lookup import EmbeddingLookup
 from molgraph.layers.postprocessing.gather_incident import GatherIncident
```

### Comparing `molgraph-0.5.4/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.5/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.4/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.5/molgraph/tensors/graph_keras_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-try:
-    from keras.engine import keras_tensor
-except ImportError:
-    from keras.src.engine import keras_tensor
-
-try:
-    from keras.layers import core
-except ImportError:
-    from keras.src.layers import core
+from molgraph.internal import keras_core 
+from molgraph.internal import keras_tensor
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 class GraphKerasTensor(keras_tensor.KerasTensor):
 
     @property
@@ -32,21 +25,21 @@
 for o in tensor_graph_operators:
     GraphKerasTensor._overload_operator(GraphTensor, o)
 
 tensor_graph_properties = [
     '_data', '_spec',
 ]
 for p in tensor_graph_properties:
-    core._delegate_property(GraphKerasTensor, p)
+    keras_core._delegate_property(GraphKerasTensor, p)
 
 tensor_graph_methods = [
     'update', 'remove', 'merge', 'separate',
 ]
 for m in tensor_graph_methods:
-    core._delegate_method(GraphKerasTensor, m)
+    keras_core._delegate_method(GraphKerasTensor, m)
 
 
 # from tensorflow.python.util import dispatch
 #
 # class TFClassMethodDispatcher(dispatch.OpDispatcher):
 #     """This class is defined as it could not be imported from keras.layers.core;
 #     reference:
```

### Comparing `molgraph-0.5.4/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.5/molgraph/tensors/graph_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import tensorflow as tf
 
 from tensorflow.python.framework import composite_tensor
 from tensorflow.python.framework import type_spec
 
-try:
-    from tensorflow.python.framework import type_spec_registry
-except ImportError:
-    type_spec_registry = None
-
 import numpy as np
 
 from typing import Optional
 from typing import Mapping
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Any
 from typing import Type
 
-from molgraph.layers import gnn_ops
+from molgraph.internal import type_spec_registry
 
+from molgraph.layers import gnn_ops
 
-type_spec_registry = (
-    type_spec_registry.register if type_spec_registry is not None 
-    else type_spec.register
-)
 
 _allowable_input_types = (
     tf.Tensor,
     tf.RaggedTensor,
     np.ndarray,
     list,
     tuple
```

### Comparing `molgraph-0.5.4/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.5/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.4
+Version: 0.5.5
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -72,17 +72,16 @@
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
-    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **TensorFlow** (version >= 2.10.0 recommended)
     - **RDKit** (version >= 2022.3.3 recommended)
-    - **NumPy** (version >= 1.21.2 recommended)
     - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
```

### Comparing `molgraph-0.5.4/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.5/molgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 molgraph/__init__.py
 molgraph/_filter_warnings.py
 molgraph/_version.py
+molgraph/internal.py
 molgraph.egg-info/PKG-INFO
 molgraph.egg-info/SOURCES.txt
 molgraph.egg-info/dependency_links.txt
 molgraph.egg-info/requires.txt
 molgraph.egg-info/top_level.txt
 molgraph/applications/__init__.py
 molgraph/applications/graph_transformer.py
```

### Comparing `molgraph-0.5.4/setup.py` & `molgraph-0.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,15 @@
   from _version import __version__ as version
   return version
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = [
-    "tensorflow>=2.7.0",
-    "numpy>=1.21.2",
+    "tensorflow>=2.10.0",
     "rdkit>=2022.3.3",
     "pandas>=1.0.3",
     "ipython==8.12.0",
 ]
 
 setuptools.setup(
     name='molgraph',
```

